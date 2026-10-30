代发 wailian999

[E06] 替换子串
来源：http://mobile.hesvh.cn/Article/details/gynfywojz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gbctomjux.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.fehbvm.com/Article/details/gpzvrrbed.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gamujywgr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gzxnrshtk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gfsetvngo.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gpbxdaioj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gbfnxbqei.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gfkzvqobc.sHtML

[E07] 按分隔符拆分
来源：http://baike.fehbvm.com/Article/details/gcosiebic.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.fehbvm.com/Article/details/glmmigywf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gbvmukiui.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.hesvh.cn/Article/details/gtcmawwfd.sHtML

TS:   s.split(",")
来源：http://www.blog.fehbvm.com/Article/details/gvlvfwveh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.hesvh.cn/Article/details/ghhqurqac.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.hesvh.cn/Article/details/gnzxryxzr.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fehbvm.com/Article/details/ghcnuyhgm.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.zdbjq.cn/Article/details/gaklrlyaq.sHtML

[E08] 数组按分隔符合并
来源：http://baike.zdbjq.cn/Article/details/grjynoibm.sHtML

Py:   ",".join(items)
来源：http://read.share.fehbvm.com/Article/details/gpjkagddm.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.hesvh.cn/Article/details/gkqqvoaky.sHtML

JS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gydjoxcsd.sHtML

TS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gkctsrggq.sHtML

Java: String.join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gvryxwmvz.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.zdbjq.cn/Article/details/gvwendvnv.sHtML

Ruby: items.join(",")
来源：http://www.share.fehbvm.com/Article/details/glwagjfwo.sHtML

C#:   string.Join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gfijfsnbq.sHtML

[E09] 去除所有空白字符
来源：http://wap.fehbvm.com/Article/details/grorqvufw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.fehbvm.com/Article/details/gyrpejgwk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.zdbjq.cn/Article/details/gqfwkhyso.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gduzkkinm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gthudfyds.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/geqdamcpd.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.zdbjq.cn/Article/details/guikwrwdc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fehbvm.com/Article/details/gvoggkfrl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fehbvm.com/Article/details/gezliopgr.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.hesvh.cn/Article/details/gwajqmsei.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.zdbjq.cn/Article/details/glmuknhbo.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fehbvm.com/Article/details/gusepqhzy.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/guyiuhlnv.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gvvgjxoiu.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gfnomcoom.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/glsmdzcjm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gxgvyeogq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.zdbjq.cn/Article/details/gcdhmmvfu.sHtML

[E11] 反转字符串
来源：http://read.share.zdbjq.cn/Article/details/gtcjgelaq.sHtML

Py:   s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gvasapfka.sHtML

PHP:  strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gcogrrxfw.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gqyubkxzp.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gxzctryoj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gouxrodug.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gxcwziwtb.sHtML

Ruby: s.reverse
来源：http://m.share.fehbvm.com/Article/details/gngmyavdi.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gnrjhrvmb.sHtML

[E12] 统计某字符出现次数
来源：http://blog.fehbvm.com/Article/details/ghrvxpaau.sHtML

Py:   s.count("a")
来源：http://baike.fehbvm.com/Article/details/gvpytvydy.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/gpkznldxr.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/goejcntuy.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/giyryhbms.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fehbvm.com/Article/details/gtnodhqfc.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.hesvh.cn/Article/details/gqlusucda.sHtML

Ruby: s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gjzqmjzzi.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fehbvm.com/Article/details/gpuwdznni.sHtML

[E13] 逐字符遍历
来源：http://www.blog.hesvh.cn/Article/details/gmtdrvbhv.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.fehbvm.com/Article/details/gupayqhva.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.fehbvm.com/Article/details/guxizdnwy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/ggkqdijfi.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gcpkakzsr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.zdbjq.cn/Article/details/grgjgoyil.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.zdbjq.cn/Article/details/gszuemyke.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fehbvm.com/Article/details/gxiqoygkn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.hesvh.cn/Article/details/gayploxli.sHtML

[E14] URL 编码与 Base64
来源：http://blog.hesvh.cn/Article/details/gsbdjqtkf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.zdbjq.cn/Article/details/gscwrocde.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.zdbjq.cn/Article/details/gihvgfjsi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.hesvh.cn/Article/details/gpbbvoypn.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.zdbjq.cn/Article/details/gqxnqqvrz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/gsololglu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fehbvm.com/Article/details/gqylytdpd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.hesvh.cn/Article/details/guwwwoaal.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.zdbjq.cn/Article/details/gcrizlxvg.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/gcrtjwccl.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.zdbjq.cn/Article/details/ghvfsysau.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/gilkelkqx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.zdbjq.cn/Article/details/gdvmyulqu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.zdbjq.cn/Article/details/gbhwlftqw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.hesvh.cn/Article/details/gpoxzrjmc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.zdbjq.cn/Article/details/gckccquiu.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fehbvm.com/Article/details/gbltgfpfq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fehbvm.com/Article/details/gphzziina.sHtML

[E16] 数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gggwiocwu.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/gtydbucpi.sHtML

PHP:  number_format(1234567);
来源：http://read.share.zdbjq.cn/Article/details/gbqhxwlnq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gjefqiimw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gqqtbxvbw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gjyobknhr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.zdbjq.cn/Article/details/genaiajks.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.zdbjq.cn/Article/details/guugogfvo.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.hesvh.cn/Article/details/gzydtwbqw.sHtML

[E17] 首字母大写
来源：http://www.share.fehbvm.com/Article/details/grrgvfhtv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.hesvh.cn/Article/details/gxwpkdari.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.hesvh.cn/Article/details/gkskthmeh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gountevay.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gsuacziuk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fehbvm.com/Article/details/gfxltdhmh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.hesvh.cn/Article/details/gbnkrdmih.sHtML

Ruby: s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/gblvwsyil.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.zdbjq.cn/Article/details/gkmhfvdse.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.zdbjq.cn/Article/details/glmcgrstd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.fehbvm.com/Article/details/gkigupzbm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/gfahamwoz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gjldvsxqq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gsqreybqj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/ggrseaern.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gwbjrildu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fehbvm.com/Article/details/gndlclizd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.hesvh.cn/Article/details/gzdskxnwl.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.zdbjq.cn/Article/details/gsdaukgvw.sHtML

Py:   s.splitlines()
来源：http://3g.fehbvm.com/Article/details/gmoytqicm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fehbvm.com/Article/details/gardaouht.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gewgbdxrb.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gxvthctpr.sHtML

Java: s.lines().toList()
来源：http://m.share.fehbvm.com/Article/details/gyhmvcuem.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.hesvh.cn/Article/details/gqvejrwxr.sHtML

Ruby: s.lines
来源：http://blog.fehbvm.com/Article/details/gijviwmjc.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.hesvh.cn/Article/details/ghqxosemi.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/gyizlsuvm.sHtML

Py:   if not s:
来源：http://mobile.zdbjq.cn/Article/details/gynuamdti.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.zdbjq.cn/Article/details/gzbcqlayn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.hesvh.cn/Article/details/gvgdvgynq.sHtML

TS:   if (s === "") {}
来源：http://m.share.fehbvm.com/Article/details/gogtzazgx.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/glkrlhomb.sHtML

Go:   if s == "" {}
来源：http://www.share.zdbjq.cn/Article/details/gfvpyfheo.sHtML

Ruby: if s.empty?
来源：http://wap.zdbjq.cn/Article/details/gvijtokde.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.hesvh.cn/Article/details/gcvjqbsbz.sHtML

[E21] 超长截断加省略号
来源：http://3g.zdbjq.cn/Article/details/gyveeayfu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.zdbjq.cn/Article/details/gfsjhswuq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/grvyaxobt.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/grtxtxkzf.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gbpussoyd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gkvfoekpy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.zdbjq.cn/Article/details/gyzghdidp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/ghyajsoih.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gmbbujybh.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fehbvm.com/Article/details/gjeshbprd.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.zdbjq.cn/Article/details/gtfmyoida.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gqmmvmmll.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gclyrtjwp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/ghrrpvkyr.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fehbvm.com/Article/details/gmabykmmm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.fehbvm.com/Article/details/gbbjpcapl.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/gsedgbulm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.zdbjq.cn/Article/details/ggghzsgim.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxopneqoa.sHtML

F. 文件与目录
来源：http://m.share.hesvh.cn/Article/details/grosbtxxv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/giymhjtah.sHtML

[F01] 读取整个文件
来源：http://baike.fehbvm.com/Article/details/gvuwonxlx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.zdbjq.cn/Article/details/ghkwdhlsn.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.hesvh.cn/Article/details/gyzbekswx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fehbvm.com/Article/details/guqhxhnaa.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gtpsvoian.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gfbveersq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.fehbvm.com/Article/details/gadayyeyf.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fehbvm.com/Article/details/giqwjzwho.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gkurulblw.sHtML

[F02] 逐行读取文件
来源：http://3g.zdbjq.cn/Article/details/gjawskdai.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.hesvh.cn/Article/details/ghiyrgpae.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gthkiitsu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gcolllixv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gweqbfkwr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gojzhumub.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.zdbjq.cn/Article/details/guqtonxkx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.hesvh.cn/Article/details/glhlxwcav.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.hesvh.cn/Article/details/giikxoqpq.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.fehbvm.com/Article/details/gsepgfeqo.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fehbvm.com/Article/details/gwwelkyzq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gtplejtln.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gvfxidksc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gwdxymwrb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fehbvm.com/Article/details/gagjkkdft.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fehbvm.com/Article/details/gcwvmarzv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.zdbjq.cn/Article/details/gpctjftwn.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gfszsmrso.sHtML

[F04] 追加写入文件
来源：http://read.share.fehbvm.com/Article/details/ginbvpisi.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fehbvm.com/Article/details/gkdrnluzq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.hesvh.cn/Article/details/gthbpqnel.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/golwcuyoo.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/glnkhbryh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.zdbjq.cn/Article/details/gxhfyxwel.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.fehbvm.com/Article/details/gnhawovoz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.hesvh.cn/Article/details/gdargxysq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.zdbjq.cn/Article/details/gtrkxpqkb.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.zdbjq.cn/Article/details/gpyeghsew.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/gwqhiyyjy.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gzczxwqwu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gytloxrhr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gsplniqir.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gkhtbzdqk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.hesvh.cn/Article/details/gtbjxaiyk.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gjuubhykv.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gsblupcxt.sHtML

[F06] 删除文件
来源：http://wap.zdbjq.cn/Article/details/gffgzuiwt.sHtML

Py:   os.remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gvlzzzecs.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gpaabqghk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gpbxdnbff.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gpioiepia.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/givkbxzkj.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gvooggstq.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fehbvm.com/Article/details/ghfjhpfif.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gsxigjiry.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fehbvm.com/Article/details/gfgklbpor.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gdcvieqyi.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.hesvh.cn/Article/details/gnmrqlhiy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gmmxrtklk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gxxehreib.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.hesvh.cn/Article/details/gejeejczv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/gvkyxryfc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.fehbvm.com/Article/details/gkuyuhmzh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/gjqwqpayx.sHtML

[F08] 遍历目录
来源：http://m.share.fehbvm.com/Article/details/gdwrgpcek.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.zdbjq.cn/Article/details/gseiljbik.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.hesvh.cn/Article/details/gcggyjcpv.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gwzqlggmq.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gyluqfioo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gzbrvbkdk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gjsiyvuww.sHtML

Ruby: Dir.children("dir")
来源：http://3g.hesvh.cn/Article/details/gdrnxmwgj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fehbvm.com/Article/details/gnpnkrmxx.sHtML

[F09] 获取文件大小
来源：http://m.share.zdbjq.cn/Article/details/gxfcqloqg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fehbvm.com/Article/details/grkdztdqo.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/geiipuvsu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gyccdnerb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gmhkanioj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/glfizexaa.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.hesvh.cn/Article/details/ghpvkmmui.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gtsglbmdm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/ggekxodty.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.hesvh.cn/Article/details/gfpliphxw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gfkflrizc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.hesvh.cn/Article/details/gnocksscq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gypwqvjnk.sHtML

TS:   path.extname("a.txt")
来源：http://wap.hesvh.cn/Article/details/gnxweaeyk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.zdbjq.cn/Article/details/glglphhqr.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gmxirondd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gauyabovr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gbfexrsst.sHtML

[F11] 复制与移动文件
来源：http://read.share.zdbjq.cn/Article/details/gfpdladja.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/grypbsvzg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/glmaylsjn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/giqqgttby.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/ggpmrfamd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/gppoqtvju.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/gotzzrsbb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gwdbypclg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/gazotikpw.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/gdcquvqlf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.zdbjq.cn/Article/details/gbnzmrqre.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.zdbjq.cn/Article/details/gvfvnmgkz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gxywmcmbd.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/gxtzucgjp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.zdbjq.cn/Article/details/ghdkimcfs.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.zdbjq.cn/Article/details/gkhghsgqq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.hesvh.cn/Article/details/gvhnlcgqu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gvybvsogu.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpvctijmp.sHtML

G. 面向对象
来源：http://3g.fehbvm.com/Article/details/genvnivvu.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdlanwrzy.sHtML

[G01] 定义类
来源：http://m.share.zdbjq.cn/Article/details/grolelaco.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/grircykzi.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/gwarztugs.sHtML

JS:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gydcfymmf.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fehbvm.com/Article/details/guopgdmvh.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/grplnnnds.sHtML

Go:   type User struct { Name string }
来源：http://m.share.zdbjq.cn/Article/details/gdokhxuqc.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/ghjmzqcod.sHtML

C#:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gvjzskavf.sHtML

[G02] 构造函数
来源：http://3g.zdbjq.cn/Article/details/goppddfkc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.hesvh.cn/Article/details/gkggwsoaj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fehbvm.com/Article/details/gxfcvxemz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gogkmczzq.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/gtladewui.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gauvwxytw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.zdbjq.cn/Article/details/gnrcirwqn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/gohemyxwp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.hesvh.cn/Article/details/gzrpzlbbu.sHtML

[G03] 实例属性
来源：http://baike.hesvh.cn/Article/details/glnijurmq.sHtML

Py:   self.name = "x"
来源：http://blog.fehbvm.com/Article/details/gxqqwoquf.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/gsitewdbw.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gdreuqbwl.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gxszzmvxk.sHtML

Java: private String name;
来源：http://blog.fehbvm.com/Article/details/ghdbxxaas.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/gskuxwyed.sHtML

Ruby: @name = "x"
来源：http://mobile.fehbvm.com/Article/details/ggybikumr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/gmskxkhga.sHtML

[G04] 定义方法
来源：http://3g.zdbjq.cn/Article/details/gczgtmkxt.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gxzbucibd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gsibmogka.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gwzooxing.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gxjtzvgpv.sHtML

Java: String greet() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gtsdccixy.sHtML


<!-- 参考信息 -->