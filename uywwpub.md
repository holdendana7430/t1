代发 wailian999

JS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gaxsjgplg.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/glwpfztph.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.zdbjq.cn/Article/details/gbjwcawjj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.zdbjq.cn/Article/details/gazbdomsh.sHtML

Ruby: s.reverse
来源：http://mobile.hesvh.cn/Article/details/ghjpngeqs.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/giigwowdb.sHtML

[E12] 统计某字符出现次数
来源：http://3g.hesvh.cn/Article/details/gtqghbxrk.sHtML

Py:   s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gyfbjrwpo.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fehbvm.com/Article/details/gupvkrima.sHtML

JS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/guhmnjrck.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/guvnfxvkq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fehbvm.com/Article/details/gztjjbxww.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.zdbjq.cn/Article/details/grfekypdh.sHtML

Ruby: s.count("a")
来源：http://3g.hesvh.cn/Article/details/gwapzmdne.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.hesvh.cn/Article/details/gdatngeaq.sHtML

[E13] 逐字符遍历
来源：http://3g.fehbvm.com/Article/details/gvryipkmt.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.zdbjq.cn/Article/details/gszbrxamx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.hesvh.cn/Article/details/guhegnyzq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/ggohrxfyo.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gzhkadzkh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.zdbjq.cn/Article/details/gbndoguji.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fehbvm.com/Article/details/gvpbjxofc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.hesvh.cn/Article/details/glhprjlfe.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fehbvm.com/Article/details/gikroropf.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/gzcwrxztj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.zdbjq.cn/Article/details/gygltbqhd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fehbvm.com/Article/details/gkoyfusqj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fehbvm.com/Article/details/gkmxntsnd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.zdbjq.cn/Article/details/gycwkdbrp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gxsruqjbw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.zdbjq.cn/Article/details/gelxwodup.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.zdbjq.cn/Article/details/gtrtldizm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/grcrvllki.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.zdbjq.cn/Article/details/gkixntmzh.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.hesvh.cn/Article/details/gxbuzjqzz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fehbvm.com/Article/details/gbrnkzmzp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.fehbvm.com/Article/details/gqtbnfyfy.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gsqatwuxb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.fehbvm.com/Article/details/ggzvtmzje.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gdhdmfygt.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fehbvm.com/Article/details/gcvhclvii.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.hesvh.cn/Article/details/gmkeecqhq.sHtML

[E16] 数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gqgxbrpaw.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/gitugcpel.sHtML

PHP:  number_format(1234567);
来源：http://www.share.zdbjq.cn/Article/details/gjdsuxbjs.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gambwhwjy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gmmrlbdfe.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gulmqtfnn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fehbvm.com/Article/details/gloslbqdh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.hesvh.cn/Article/details/gewacsvdc.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.zdbjq.cn/Article/details/gffzeqvxx.sHtML

[E17] 首字母大写
来源：http://mobile.fehbvm.com/Article/details/gotsoewts.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fehbvm.com/Article/details/gnpklggee.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.zdbjq.cn/Article/details/ghcfuscia.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gnmoktvtc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gfyqxqcdz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fehbvm.com/Article/details/glcrananv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fehbvm.com/Article/details/gfvvatufq.sHtML

Ruby: s.capitalize
来源：http://www.blog.zdbjq.cn/Article/details/gmwokywhj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.zdbjq.cn/Article/details/gxkglrrru.sHtML

[E18] 模板占位符替换
来源：http://m.share.fehbvm.com/Article/details/goeybbvur.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fehbvm.com/Article/details/gxbvepvax.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/govofdwhu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gswgwaljy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gkzpdpupu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gznscottm.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gknweupmd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.hesvh.cn/Article/details/ggnggfjmd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gsylgrkni.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.hesvh.cn/Article/details/groovdbyl.sHtML

Py:   s.splitlines()
来源：http://baike.hesvh.cn/Article/details/gltnaneuy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gwsolaqvs.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gfpkfcpml.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gpltvrruc.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gwqykfqaa.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.fehbvm.com/Article/details/gycqlpica.sHtML

Ruby: s.lines
来源：http://3g.fehbvm.com/Article/details/gltforjaf.sHtML

C#:   s.Split('\n')
来源：http://www.share.zdbjq.cn/Article/details/gjqgaztpx.sHtML

[E20] 判断字符串是否为空
来源：http://baike.hesvh.cn/Article/details/gyztkxzmz.sHtML

Py:   if not s:
来源：http://3g.zdbjq.cn/Article/details/gvasutyvm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.zdbjq.cn/Article/details/glaigpvma.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.fehbvm.com/Article/details/gasrfqhfx.sHtML

TS:   if (s === "") {}
来源：http://www.blog.hesvh.cn/Article/details/gzragnoii.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/glugsktjl.sHtML

Go:   if s == "" {}
来源：http://read.share.fehbvm.com/Article/details/gdlfgfqvl.sHtML

Ruby: if s.empty?
来源：http://wap.hesvh.cn/Article/details/ggwwbfgec.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.zdbjq.cn/Article/details/gwchfqyrz.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.fehbvm.com/Article/details/gkqpbhkrb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.zdbjq.cn/Article/details/gdllqzfhk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gqqxcrpge.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gouobkbdh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gqzftgoku.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gowerhgfu.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fehbvm.com/Article/details/gmkmdnrdv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gmaxwgttw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gvnuhxaui.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fehbvm.com/Article/details/gvakfisea.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.zdbjq.cn/Article/details/gouvtgkth.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gdscfigsd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gtwieiyio.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gwyagatrr.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gkgulfusl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fehbvm.com/Article/details/gspwundxj.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.hesvh.cn/Article/details/ggjbyqbmc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fehbvm.com/Article/details/gcrphhrxq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcetaxxwr.sHtML

F. 文件与目录
来源：http://m.share.hesvh.cn/Article/details/glttmgzyl.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghimlvjxx.sHtML

[F01] 读取整个文件
来源：http://www.m.share.zdbjq.cn/Article/details/ggjjoxbqy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.fehbvm.com/Article/details/gtxuzbxot.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gricijosl.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.hesvh.cn/Article/details/gwpvvhvlo.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/grluxtwak.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gavbuqlhy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.zdbjq.cn/Article/details/gzrqeevtf.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gpscgtlxd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gpjaddyeq.sHtML

[F02] 逐行读取文件
来源：http://mobile.zdbjq.cn/Article/details/gbqdsasum.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.zdbjq.cn/Article/details/gnmfswgvb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.zdbjq.cn/Article/details/gskdoqhhr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/grqagxfrl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gpaqugyii.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gglcggqio.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.hesvh.cn/Article/details/gaqancbag.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fehbvm.com/Article/details/gdmnxtpze.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fehbvm.com/Article/details/ggqoztnrt.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fehbvm.com/Article/details/gvllqqlmx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.zdbjq.cn/Article/details/gjeeleacu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gyraabijl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gqxbokxmv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gmkbpmmnb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.hesvh.cn/Article/details/giwkgrtmo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.zdbjq.cn/Article/details/gumpozdct.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fehbvm.com/Article/details/gyszpucps.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/geddoougr.sHtML

[F04] 追加写入文件
来源：http://www.share.hesvh.cn/Article/details/gxipbejix.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.zdbjq.cn/Article/details/gjqrqxtbg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.hesvh.cn/Article/details/gavxddwyy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/ganfqoyoa.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/glhwncllm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.hesvh.cn/Article/details/gxfhbofew.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/grmchhijr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.zdbjq.cn/Article/details/gcsbktvgz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gdptzrrjn.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.hesvh.cn/Article/details/ggocbqdhq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fehbvm.com/Article/details/gvmawgiqy.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gwtkfhhsu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/ghmerrlrw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gaqzctaen.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gohqsqqsl.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.zdbjq.cn/Article/details/gytcjsqad.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fehbvm.com/Article/details/gbrkwtcpk.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.hesvh.cn/Article/details/gvpfbnebq.sHtML

[F06] 删除文件
来源：http://read.share.fehbvm.com/Article/details/ggzpwkhah.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/guvddyned.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/gpevtfhnw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gnxernbrv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gmyyaojpl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gwvjjvhzy.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gxlxrzhud.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gskvqnskz.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fehbvm.com/Article/details/gxdwbocvr.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fehbvm.com/Article/details/gxxiefrlz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/grojtbwks.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.zdbjq.cn/Article/details/gyxvyyjev.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gzbflacse.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gpahikclm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/gwmwrhywe.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.hesvh.cn/Article/details/gqurywjnt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.hesvh.cn/Article/details/goumugghz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fehbvm.com/Article/details/gupntyppd.sHtML

[F08] 遍历目录
来源：http://m.share.fehbvm.com/Article/details/gffcpfysu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.zdbjq.cn/Article/details/gvcwfrzrz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/gjtodplju.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gacnbotgb.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gpribrrja.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gwaokgrgy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.zdbjq.cn/Article/details/gflrkikxd.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fehbvm.com/Article/details/gtimiilws.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fehbvm.com/Article/details/gdwrtlpkj.sHtML

[F09] 获取文件大小
来源：http://wap.hesvh.cn/Article/details/gztjwsvcr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gwzghqmck.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gdzzsqqfh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gtzcorhmw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/ggthrgdrq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/ggiiokmdg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.fehbvm.com/Article/details/gupcxslsw.sHtML

Ruby: File.size("a.txt")
来源：http://3g.zdbjq.cn/Article/details/goxckbhpq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.hesvh.cn/Article/details/gnjaziyji.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fehbvm.com/Article/details/gpmhyztvs.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gzkadcalo.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.hesvh.cn/Article/details/gpnvwcsti.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/grcxalwgw.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gszsoyduw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.zdbjq.cn/Article/details/gniqnzncw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gzucaofzb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gjniqmzif.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gbexiguhk.sHtML

[F11] 复制与移动文件
来源：http://wap.hesvh.cn/Article/details/gsdehjasd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gpgauctud.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/gowkqlsvq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gdtyncggk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gtqhzgffm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gdnueshrg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.hesvh.cn/Article/details/gsdzpaeiy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ghwkxevez.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.zdbjq.cn/Article/details/gvbwwuwff.sHtML

[F12] CSV 读写
来源：http://3g.fehbvm.com/Article/details/ghwkmpcbg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/gcimzmpwa.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.hesvh.cn/Article/details/gqgmalcbm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.zdbjq.cn/Article/details/gudhtdnjl.sHtML

TS:   // 同上
来源：http://blog.fehbvm.com/Article/details/gtcutycjc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fehbvm.com/Article/details/gmtzckgfz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.zdbjq.cn/Article/details/gwlecplic.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.hesvh.cn/Article/details/gjysnwwsg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.hesvh.cn/Article/details/gbdylawop.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gzptkvzhv.sHtML

G. 面向对象
来源：http://wap.zdbjq.cn/Article/details/gqsavaxip.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdamzpkrb.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/gcvghmdri.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/gsdbiwgom.sHtML

PHP:  class User {}
来源：http://www.blog.hesvh.cn/Article/details/gndepqdwt.sHtML

JS:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gubnhmfxf.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/ghyrbdsai.sHtML

Java: class User {}
来源：http://mobile.fehbvm.com/Article/details/gnylhogki.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/guxomjmaw.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/ghwhbrzng.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gdxadsvpz.sHtML

[G02] 构造函数
来源：http://3g.hesvh.cn/Article/details/grsxvaman.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.zdbjq.cn/Article/details/gsmwspfts.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fehbvm.com/Article/details/gussficfc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gaocdeebg.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gxgftuqee.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gsiylqpqu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.hesvh.cn/Article/details/glhzyahoh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.zdbjq.cn/Article/details/gtbsvuifr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.hesvh.cn/Article/details/gzeydhjbs.sHtML

[G03] 实例属性
来源：http://wap.fehbvm.com/Article/details/gmbomityr.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/gmgylcsin.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gjwjmutpq.sHtML

JS:   this.name = "x";
来源：http://wap.zdbjq.cn/Article/details/gqhaxzdsk.sHtML

TS:   name: string = "x";
来源：http://www.blog.fehbvm.com/Article/details/gpzpfnzuj.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/glskejluo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.zdbjq.cn/Article/details/gxrhvqwfg.sHtML

Ruby: @name = "x"
来源：http://3g.zdbjq.cn/Article/details/gxsbaoyui.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/gqntrmfjy.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/gmxzwboij.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gwkfjskfd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gwdtldacp.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gnsebbuxa.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gyktkamip.sHtML

Java: String greet() { return name; }
来源：http://wap.fehbvm.com/Article/details/gtrdjswok.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gjtusxvvp.sHtML

Ruby: def greet; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gubnprgph.sHtML

C#:   public string Greet() => Name;
来源：http://baike.zdbjq.cn/Article/details/gfomkrlhe.sHtML

[G05] 继承
来源：http://www.share.zdbjq.cn/Article/details/gnjbzclde.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/grdbtzggg.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gvafcnjrf.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/geiuzlwhb.sHtML

TS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gostwnpup.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/geyepfrlq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.zdbjq.cn/Article/details/gbvmjkkfs.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/gxokiuzpg.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/gpvjgwcij.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/gcduromue.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/gzqzfgezh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gyaleggvl.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gioaujscj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gnbvpahvx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gpxtelqal.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/gqnizsrim.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/gyyqczqqw.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fehbvm.com/Article/details/gjjrbbpry.sHtML

[G07] 调用父类方法
来源：http://3g.hesvh.cn/Article/details/ggxereahy.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/gfpkakosw.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/gkndgtafe.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/geowmqamk.sHtML

TS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gptwcrjim.sHtML

Java: super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gmhphchbf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/gelwgoelw.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/giwdodiod.sHtML

C#:   base.Greet();
来源：http://www.blog.hesvh.cn/Article/details/gizhgnoro.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fehbvm.com/Article/details/gjfyateib.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.hesvh.cn/Article/details/glyyxbrqb.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/geomrdkpg.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcsigbqdp.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/glfwqztjz.sHtML

Java: static void f() {}
来源：http://wap.fehbvm.com/Article/details/gzavspstq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.zdbjq.cn/Article/details/gdfrvstfc.sHtML

Ruby: def self.f; end
来源：http://3g.zdbjq.cn/Article/details/gdqcqhtnw.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fehbvm.com/Article/details/ghzdioqsb.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.hesvh.cn/Article/details/glaucpxpm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.zdbjq.cn/Article/details/gdqzdnnup.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/gmfzllmlx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/gvsdirupt.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fehbvm.com/Article/details/giwvoitdj.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gpslgfufy.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.zdbjq.cn/Article/details/gpkqvwwbc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.zdbjq.cn/Article/details/githeelcg.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.hesvh.cn/Article/details/gvomudqns.sHtML


<!-- 参考信息 -->