代发 wailian999

[E06] 替换子串
来源：http://wap.zdbjq.cn/Article/details/gxtbfsirk.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gqkjnkssx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.hesvh.cn/Article/details/gfjaawase.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gqjmavgki.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gzuymtchy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gxejeitkp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/gcotfpekg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gpaqlysha.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fehbvm.com/Article/details/grvfcludj.sHtML

[E07] 按分隔符拆分
来源：http://mobile.zdbjq.cn/Article/details/getglvdga.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.fehbvm.com/Article/details/ghzqcrvpj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fehbvm.com/Article/details/gnlmjmdus.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fehbvm.com/Article/details/gqjuyjwzy.sHtML

TS:   s.split(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gtdksrabr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.zdbjq.cn/Article/details/gziomurxz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.hesvh.cn/Article/details/ghyejrmza.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.hesvh.cn/Article/details/gjjvpmrmd.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.fehbvm.com/Article/details/gkbcpuugj.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.zdbjq.cn/Article/details/gjnirxyae.sHtML

Py:   ",".join(items)
来源：http://www.share.hesvh.cn/Article/details/grufkfdsc.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fehbvm.com/Article/details/gnmnqvrmo.sHtML

JS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gawhiqsnq.sHtML

TS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/guwebqagl.sHtML

Java: String.join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gpnxizrqk.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.hesvh.cn/Article/details/gjhiqlrlz.sHtML

Ruby: items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/ganoizpcj.sHtML

C#:   string.Join(",", items)
来源：http://blog.fehbvm.com/Article/details/gygxczhuw.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fehbvm.com/Article/details/ghgqsyegf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.hesvh.cn/Article/details/gxihoapnc.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.hesvh.cn/Article/details/gluexajne.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gtlvrxyny.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gqjvknpak.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gfwncjibr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.zdbjq.cn/Article/details/gimlsnblp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.fehbvm.com/Article/details/gpteypawm.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.fehbvm.com/Article/details/gpqjfpiso.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.hesvh.cn/Article/details/gaggjjlje.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fehbvm.com/Article/details/grxkbfuey.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fehbvm.com/Article/details/gishdomzs.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gtijletoz.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gnqegxcjb.sHtML

Java: String.format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gqcjtoxem.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gwwhcwvhw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gkdehscdn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.fehbvm.com/Article/details/gsqptswoc.sHtML

[E11] 反转字符串
来源：http://wap.zdbjq.cn/Article/details/glpqquksl.sHtML

Py:   s[::-1]
来源：http://wap.zdbjq.cn/Article/details/ggwjevqna.sHtML

PHP:  strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gkhkhmwda.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gqvzvheyl.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gyyqgxnkk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.zdbjq.cn/Article/details/gbhnzgkhn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.zdbjq.cn/Article/details/gocjtepph.sHtML

Ruby: s.reverse
来源：http://www.share.hesvh.cn/Article/details/geabzavtj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gschljitv.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fehbvm.com/Article/details/gjlloxzfg.sHtML

Py:   s.count("a")
来源：http://wap.hesvh.cn/Article/details/gxjgbdsab.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.hesvh.cn/Article/details/gysdahlbx.sHtML

JS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gnwexsxqw.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/getbbmzgb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.hesvh.cn/Article/details/gkqgkembn.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.hesvh.cn/Article/details/gpryzetgd.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/goowjxggm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.hesvh.cn/Article/details/gqrgxocui.sHtML

[E13] 逐字符遍历
来源：http://www.share.zdbjq.cn/Article/details/guccvcurb.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.zdbjq.cn/Article/details/gcowxrzad.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.zdbjq.cn/Article/details/gycdczqup.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gdsfaqkdp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gusoxpktq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gyqkuddmf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fehbvm.com/Article/details/grzozdroi.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.hesvh.cn/Article/details/glyqcfato.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.zdbjq.cn/Article/details/grvdprqqb.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/gkhmtyxhp.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.zdbjq.cn/Article/details/ghxpvikda.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.zdbjq.cn/Article/details/gqmstmyfw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fehbvm.com/Article/details/gqhwlctxc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fehbvm.com/Article/details/gpfmtfpra.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fehbvm.com/Article/details/gqswzhqmy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.zdbjq.cn/Article/details/gueqkpwwh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fehbvm.com/Article/details/gemmzixpm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fehbvm.com/Article/details/gsozospxf.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.fehbvm.com/Article/details/gdqhqftgn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.hesvh.cn/Article/details/gogsmvcsw.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/gowfujtql.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.hesvh.cn/Article/details/gylegnjiq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.zdbjq.cn/Article/details/geenwydna.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.zdbjq.cn/Article/details/gtificaqr.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fehbvm.com/Article/details/gtbpdetxs.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.fehbvm.com/Article/details/gjalijnlc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.hesvh.cn/Article/details/gsierdxtt.sHtML

[E16] 数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gbpsptquk.sHtML

Py:   f"{1234567:,}"
来源：http://blog.hesvh.cn/Article/details/gcapoaett.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fehbvm.com/Article/details/gecfssryz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gcawqwgke.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gbgourbvn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.hesvh.cn/Article/details/gudvxvfvs.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fehbvm.com/Article/details/gjwswxixr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.hesvh.cn/Article/details/gcadaijjm.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.hesvh.cn/Article/details/gufjshdzy.sHtML

[E17] 首字母大写
来源：http://wap.hesvh.cn/Article/details/gtdqyaaza.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fehbvm.com/Article/details/gsqwrqoin.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.hesvh.cn/Article/details/gkecvuayq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/glulbqsor.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gvczkwjka.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.zdbjq.cn/Article/details/goakcunwq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gixunyqxv.sHtML

Ruby: s.capitalize
来源：http://blog.zdbjq.cn/Article/details/gfeijyoyq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.zdbjq.cn/Article/details/gdczqjjik.sHtML

[E18] 模板占位符替换
来源：http://www.blog.zdbjq.cn/Article/details/gkjrzjcrq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.hesvh.cn/Article/details/gkfefmqrn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.hesvh.cn/Article/details/grhccqvkw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/garphqfim.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gmwistmhk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gqwhdropr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.fehbvm.com/Article/details/gmkqsmwpt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.zdbjq.cn/Article/details/gqempefpj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fehbvm.com/Article/details/gtaaxbenh.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.fehbvm.com/Article/details/geaxstdbe.sHtML

Py:   s.splitlines()
来源：http://wap.fehbvm.com/Article/details/guauupxzs.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.hesvh.cn/Article/details/gsfkdxmvz.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gndmzpvth.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gkuuzvuio.sHtML

Java: s.lines().toList()
来源：http://www.blog.fehbvm.com/Article/details/gkkcjadgx.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fehbvm.com/Article/details/gvfllrnrt.sHtML

Ruby: s.lines
来源：http://wap.fehbvm.com/Article/details/gzulvsrsb.sHtML

C#:   s.Split('\n')
来源：http://3g.zdbjq.cn/Article/details/gjemvougz.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.fehbvm.com/Article/details/gmuobplpa.sHtML

Py:   if not s:
来源：http://blog.fehbvm.com/Article/details/gonjpslnn.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fehbvm.com/Article/details/gberayloy.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.hesvh.cn/Article/details/gwtkqesga.sHtML

TS:   if (s === "") {}
来源：http://read.share.fehbvm.com/Article/details/goftgdhuz.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/geafgmxji.sHtML

Go:   if s == "" {}
来源：http://mobile.fehbvm.com/Article/details/guoecphin.sHtML

Ruby: if s.empty?
来源：http://blog.fehbvm.com/Article/details/gomspspgz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.zdbjq.cn/Article/details/gyfwbsdtv.sHtML

[E21] 超长截断加省略号
来源：http://blog.zdbjq.cn/Article/details/ghrnjxldp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.fehbvm.com/Article/details/grjupacyv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gowncensp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/ggfdjissv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gkdgxuhwf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gkhbyhvpb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.hesvh.cn/Article/details/gvpuwhedx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gwowpgmhb.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/guthumcrf.sHtML

[E22] 字节长度与字符长度
来源：http://blog.fehbvm.com/Article/details/gfqdcipcj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.zdbjq.cn/Article/details/gelqulqcy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gjzrqxvxl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gvoaylzjh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gdtyirayh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.zdbjq.cn/Article/details/glajxbsti.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.zdbjq.cn/Article/details/ghnfipzax.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fehbvm.com/Article/details/gdpcmwccf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gejhymwqs.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gaglhukyz.sHtML

F. 文件与目录
来源：http://blog.fehbvm.com/Article/details/gweldexyh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/glglgtxtb.sHtML

[F01] 读取整个文件
来源：http://www.blog.zdbjq.cn/Article/details/gsubmjlon.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fehbvm.com/Article/details/gbypsfmpv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/gckrdjbgi.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.zdbjq.cn/Article/details/gfvmfsqji.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gjbbgtwcq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gcphbaskn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.hesvh.cn/Article/details/gtyqlrnrv.sHtML

Ruby: File.read("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gxakjhppr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gkwkjppfm.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fehbvm.com/Article/details/gpthtlvvu.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.hesvh.cn/Article/details/gbxszutzc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.zdbjq.cn/Article/details/gqxtwajxl.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gunnftwgy.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gjinsewcn.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gykjeuzbu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fehbvm.com/Article/details/grvsntnhu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.hesvh.cn/Article/details/gmxpaaepx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.hesvh.cn/Article/details/graoogceo.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/goacykjsv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fehbvm.com/Article/details/gqkxseraf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gmvxlrvds.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/goljqzghl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gxdwkzldx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.hesvh.cn/Article/details/guonyumwz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fehbvm.com/Article/details/gmuhafsol.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.zdbjq.cn/Article/details/gzjtvpgme.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gdgpjuarj.sHtML

[F04] 追加写入文件
来源：http://m.share.fehbvm.com/Article/details/gaitksgas.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fehbvm.com/Article/details/ghwhnchru.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fehbvm.com/Article/details/gszdsagzc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/guvqrfdsq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gpyydeqfi.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.zdbjq.cn/Article/details/gnudoylkn.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fehbvm.com/Article/details/gwrzaidti.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/gfqtalvbc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.zdbjq.cn/Article/details/gqlogsbre.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.hesvh.cn/Article/details/gljnwqmrd.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.zdbjq.cn/Article/details/ggvagcarg.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gqaohzuxf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gzkdsaimh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/govxfiqxr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/grfbuyumh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.zdbjq.cn/Article/details/gidcuebnt.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fehbvm.com/Article/details/gfhezzulw.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gpdtelqoy.sHtML

[F06] 删除文件
来源：http://wap.fehbvm.com/Article/details/gjujcdsao.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/ghjdoizri.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gmtdxsqtm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gpdwjzolz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/grojvrepv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gushepwpu.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gfocndlzo.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/gqpihrwxz.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gwzqevddh.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.hesvh.cn/Article/details/guuarvlnb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gckgtclti.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fehbvm.com/Article/details/gciizuous.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gcrifrltk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gtmqmuduh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/gdjrjzzlc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/gmuewrcpq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.hesvh.cn/Article/details/gecuepjvu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fehbvm.com/Article/details/guwvmoswa.sHtML

[F08] 遍历目录
来源：http://m.share.hesvh.cn/Article/details/gacanbtyq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.zdbjq.cn/Article/details/gdprxumvv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.hesvh.cn/Article/details/gqrrymicc.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gsrzpskvh.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gmepkjzmd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gnmbcldgy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fehbvm.com/Article/details/gntuwxsfq.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fehbvm.com/Article/details/gimxzznlb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.zdbjq.cn/Article/details/gopvenmgg.sHtML

[F09] 获取文件大小
来源：http://www.m.share.hesvh.cn/Article/details/gyotubzoc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gbuxfffvb.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gjqzbykyd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/guuyaodyj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/goqgvcvxb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gekhgqgev.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.zdbjq.cn/Article/details/ggosozigx.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gsuxtcpsf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.zdbjq.cn/Article/details/gazvdblos.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.zdbjq.cn/Article/details/gyzvhnwpe.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gvlohoobh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/gdjkdkbtt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gxsnljbrm.sHtML

TS:   path.extname("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gwckkhogq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.hesvh.cn/Article/details/ghwlzecri.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gzdjwsmvw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gjmhswkmh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gvczmxgzw.sHtML

[F11] 复制与移动文件
来源：http://m.share.fehbvm.com/Article/details/gkquzifge.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gfhmtauax.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/gupwsjbku.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gtpgwkvqw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gmcmrfctv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.hesvh.cn/Article/details/gqjvxhsci.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.hesvh.cn/Article/details/gpgzcqxon.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/ghvqthjnz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/gwbtdkhed.sHtML

[F12] CSV 读写
来源：http://read.share.zdbjq.cn/Article/details/gdomoqfzg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fehbvm.com/Article/details/gkgobgica.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.hesvh.cn/Article/details/gbhbipova.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fehbvm.com/Article/details/gyyomyape.sHtML

TS:   // 同上
来源：http://mobile.hesvh.cn/Article/details/gnsojlozi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fehbvm.com/Article/details/gapordjhs.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fehbvm.com/Article/details/gmzjomcjt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/gbdpqerdt.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gjwkytfaf.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gngkpaugg.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/gorscqrhc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/guxtnewos.sHtML

[G01] 定义类
来源：http://www.blog.zdbjq.cn/Article/details/grbhipnud.sHtML

Py:   class User: pass
来源：http://mobile.zdbjq.cn/Article/details/gyprunlgk.sHtML

PHP:  class User {}
来源：http://blog.zdbjq.cn/Article/details/ghnecwrhh.sHtML

JS:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/guepctnan.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.zdbjq.cn/Article/details/gufwolnqd.sHtML

Java: class User {}
来源：http://3g.zdbjq.cn/Article/details/gapudankv.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fehbvm.com/Article/details/gtvpbbkjr.sHtML

Ruby: class User; end
来源：http://wap.hesvh.cn/Article/details/glqtuycoa.sHtML

C#:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gvqqbwzim.sHtML

[G02] 构造函数
来源：http://m.share.zdbjq.cn/Article/details/gspcutdzy.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fehbvm.com/Article/details/gcrnggkph.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.hesvh.cn/Article/details/gnpdnvfqn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/giwpsaohk.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fehbvm.com/Article/details/gkmwjzsrb.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gcntkccfr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/gfowwzvof.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.zdbjq.cn/Article/details/ghnccrtuo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/grrsovxdg.sHtML

[G03] 实例属性
来源：http://www.blog.hesvh.cn/Article/details/gqvyudeul.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/gaezwlusa.sHtML

PHP:  public string $name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gdmptzzdd.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gexlwugog.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/ghpmllwmg.sHtML

Java: private String name;
来源：http://read.share.fehbvm.com/Article/details/gyzasbvxv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/gufmibjcp.sHtML

Ruby: @name = "x"
来源：http://3g.zdbjq.cn/Article/details/gmdvcogpr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/gwvwcukcn.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/gtqmqlbhk.sHtML

Py:   def greet(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gjwkofdoy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gpgdiouoc.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gusuwqdyg.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gcrldbgxc.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/gkghpqefl.sHtML


<!-- 参考信息 -->