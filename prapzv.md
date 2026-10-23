代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3mtpwkaye.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3yebsnlhf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3jwypdkei.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xgzaivtp.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3oeemcwqr.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3uoygsarl.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3dvpsikag.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3qvimtyie.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3vsqvfbqz.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3ekmsivks.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3tqxtlcqf.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3bqvddxlb.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3afgrgbmd.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mmyzgeru.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wgnoehqd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3bjainojg.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ywszhivn.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3revlvojl.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3fgctggmr.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3avisvbfr.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3igudntcj.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3lbovdgir.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3jodggapb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3dvjcxzqf.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3zwbitxgc.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3izeniuer.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3hzfiueyj.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3dumcplnp.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3hfpnqjjl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3mkpncxde.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zowkdypk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3oijvcpps.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3nkvdkhrm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3whzywrhu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3lfifajnd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3gbecvrhr.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3awrnuyeo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3hyqooiux.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3ijhmonef.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3nwvkdaly.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ytukqjxr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3psbdubxp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3jboezzrp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3xjbcpxpv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3runhhviw.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3ejduxxxo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yhkvixxh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pfqxghxy.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gmmkswwd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ivigbohe.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3umxjumbe.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jtjmkmak.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3cztffgro.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3uyyxfgwf.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3tivpzpwf.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3nspouugo.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3dffzseai.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3igtneoip.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3guoxbdvk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3meeeectr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3sivgrmpg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dybzzuxy.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3syvsyuvl.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3mtlwbeey.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3mjkokfoj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3fdjrhudb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uqvlbmmj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3anqgxixb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3requuafu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3pzshixom.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3rokplezd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3xzylssdq.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3uvaazbqb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3ouzsxirp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3jbxmcwtz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3mrehaezp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qyymfbyo.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qnzxpvdk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3tlxmohcb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ofnymycr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3uxyhhhhv.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3zjgkcorn.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3fwetftek.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qwuhynzu.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3mnmwjbnn.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3vtddtmgm.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3djgilwpa.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3abfyubmn.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3oksrssmb.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3qmcnqzgv.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3ghixjzqm.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3uhxknurc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3xejolcap.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3cwevdscu.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3vsxsrmuh.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xdjpkjvg.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3xawnhsir.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3hqzjmfyh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3wgxkeqag.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3kdqwdrwv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3trmtdxcb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3lmdtsmdk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fhwugpxe.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3eqbupokv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dipoolqt.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3xjbtjrau.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hzusbhfy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wjunbfyq.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3ouvudavc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3qjhczluh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3zheizxaz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3cxpaiywg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3qfhgsgmk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3imdsnmad.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3rufhklmd.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3aptwbmyl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3tvloftxn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dseqmywr.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3khjqsguo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3btwidhgg.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3czstbzxe.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3fhrasyfp.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3igbaxmhe.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3jdodcrzp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3uvdcfoaz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3fpbbtahp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3ipqclord.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jlggcsgf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3miepslil.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3ofgzkeab.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3rzscatux.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3oetksjcl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ljxfonlp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3uqazrxuk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3rlulkbtm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3ucddkenx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3eccicbat.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3ihtxvffv.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3lcqczdlc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3mzqmlucw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3agyfsizv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3xekngtyt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3hqltszln.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3rphzxzqq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3lmfdonrc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3cqnktomp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3hfmeyvrk.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3glhkxdif.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3bsnxbzlz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3cikibuqu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rrbfwceg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nfpeorql.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3axkqmxsz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3cvqygcni.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3qzgyuxbl.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3darwzvpr.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3jgaqcpln.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3yqqowzcf.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3spfhgmuh.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qnizkjyx.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dkpaopmq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3cnqpdkqx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3gjqdsgri.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fpfsllkc.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hqnzrwlw.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3skrstwrp.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ykizffsq.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yckeqvdc.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xxpuupvi.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jnxglwpu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3gqeibijc.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xjensciw.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zrfamvtf.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kobpkwxk.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3tqvmykju.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3yftppcuj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3nrlnhpbu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3tsfpuvya.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3mjaxxohy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3fznsjsqs.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3buqamaol.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3fyozczhz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3ykheaqgx.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3clfxxmxe.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3ntmtamte.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3gaxqaqea.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vitpsepx.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3zlhojfvt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3uhsbvwcq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3veiofvpo.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dzdwutnr.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3nnyebdfh.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3yhkixwij.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ayywxcjk.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3odzrmrhu.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3indtmudx.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3oumvvmgp.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rfdojqxk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3qvbjrjrd.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hkxfbdrm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3vxlazsvw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3grzlftoq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mtbshzjp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pltuyjhv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dnreywce.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xaujddlr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3vfpzlbgy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3avqfyhgb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yiupqqrp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jonmjaai.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3vbjnovap.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kjcrrcvc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hzleoajh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wswbhfjj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wccslcur.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3glgrlbme.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3fncxezms.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3cmpiwmta.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3iqhnnifu.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3rfofqjcq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3qvqhadnd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3tnncfanj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3qfuwbaqd.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3lviklceh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3ttzbzkrk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3omhkddmm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3mjlhgyxx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3qhhmnjyd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tqegcowm.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3ituipluc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lptxnkpf.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3rfpuwdgd.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3onbhxajs.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3yjnwqivr.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fexsqiux.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3oawwvmiy.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ubrpizxv.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3gzoypjul.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3djaahtwf.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3anrzzpia.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3xmwpkbbe.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3vqxsgqbq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3feyitqwy.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3axqvystm.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3wmoygkyk.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3qnkmksde.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3qdvakndx.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3xibsbfjs.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3qjmwnvpj.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3axcxeipw.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3qclalaox.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3roktqcwv.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3qjxgyqyh.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3gbogabct.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3zolvggka.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3pjqxhxkj.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3nlrieiba.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3hspebymb.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3ywwzywjr.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3sdwvavhi.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3remxgelt.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3awrmbrco.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3oaciubfc.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yeeuuwju.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3medzqrkk.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3fnjxxpxp.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3lepxkmjh.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3zchxzcgy.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3iqzbfbhb.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ewzeegvr.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3trjrcznf.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xyagmcra.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ymysfyfr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3smsbehmh.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3ubrvnnqd.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3zhbgejpx.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3qwjsawce.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3jgqyvhsx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3kfuqflev.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3obxvfoyv.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3hegswmqv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3iaglsrmn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3pszrpiga.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3eyvcpzug.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3ebtedgnt.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3egtetlxq.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3gzzokdtq.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dzcyqbbn.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3emjhbdjp.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3icmnvnpm.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3nxuwsukr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3gyqxontf.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3hskbtzwi.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pxccjfkg.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3bgavpmcx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3yqskgzsu.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3ivnrykjl.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3gpvgpyfd.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3qgofehqc.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3wfjnfrmr.html


<!-- 参考信息 -->