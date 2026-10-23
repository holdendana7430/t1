代发 wailian999

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3epeeevdm.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ebrblgnx.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3wwoocfry.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3pomvuqev.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3sguspjid.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3cxlfxhgj.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3tuefccec.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3sjtoisal.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3okdgsilt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3wjtkwcyn.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3kvgybvkl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3nfzhvbfy.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3qrgfvqje.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3grziycsa.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3srnuowlh.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3fijypnyb.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3eojwlrce.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3sufohpfo.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3whxtcrkn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ikxcbsph.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ilfvlawn.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3emrgtwuz.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3podsmvkp.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fqnzxuid.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tezmnivy.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wnaplkxz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mmagztcp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3uwkgdcuv.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3isvtgghk.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3juftvfda.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3wupdlvtk.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3nljugbjh.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3zboadfoc.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3pnlipezj.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3kzlxenkq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3viucoejd.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3yggyfijf.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mudnzytd.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3nvqplveb.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xqekrydy.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3ffbmwtfb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3xbvsrzxr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3pzkitbzq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3pmitagtr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zgondcbl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3lweizmpc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3ybtbpyut.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3dvcoeheo.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3rbxoyvie.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3ymkzecjx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3vedjbxze.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3hsqsngwk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3btybqfvl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3fucpazrx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3ikraqlif.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3tyzwkwih.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3bjnjkiqx.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3rdxctpvp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gbylofxs.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3zzninpyo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3tffykzyj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3spdapedn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3sphiahrc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hrytevkc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yzdidgmm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3emwwhfux.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3jhvwyuon.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3rozemrhu.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3trqphkiw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3pbnsgxaz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3crzyfmdx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3zmeorfjs.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3hjwvazrq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3hvutndnv.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3mmrsvyfo.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3bjfkmbyj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3hnfdthbd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3czfytsba.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ngywxhjy.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tbogguir.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3glujodlz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3bvmovwfg.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3qserpocl.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3xgzhddhb.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3odidcenj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3oxpazeio.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3kbczzmdg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vbrnoeqd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jmnsguig.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ivbouprx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3uapipuwt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3jjaipzhv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3gqxvqxsn.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3zyyvolbk.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3vvijivgt.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ywyncltv.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3fbhzbaos.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ufwzuzfo.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3pebnxczj.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dqysbbmg.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3rsebigwz.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3iiuejelx.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3bbjyogon.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3gjsscqci.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3ztlocpjl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hivkaaqa.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3pwhdfveg.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3nyejhskn.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3lyssxeyx.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3zmrhucnu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hzjbubtj.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3nfkknywi.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3olbcopzg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3gdpdabiq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3sxmvwwjz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xqwxmfzu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3diqdbees.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3uugjpqrv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3klaxpwrc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vjgrwlhx.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3kfnteqjx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wpzsjdvi.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3mjctnkdu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3mdeoaeno.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gibxpmiu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3wdjpeqcm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3jmejmcig.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3kccocxbf.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3jjtdtdep.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ewwnybjm.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3aesopbma.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lmuscedw.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ocuvganr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3xvncthjx.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3slcqtsoa.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3nbdvljyr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3oedmxojz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3pkwobzyu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3lfmucwed.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fugpcjdb.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3znuyqlqv.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3aiffqutd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3xgvsbokk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3ookxvtcz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3iscnonww.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zslgfksn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ekvyrrwp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3siraocyd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3qetusndw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3itxqynad.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3dzaztzju.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3jypzvzuo.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3xjzcqgsv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ltaxjsyz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3xcosshaf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3gzqmonhe.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3izcukaht.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3rfhkpreb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3slpztvxt.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3noyqlbvq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ertqevpd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3oacsjdgv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ssrjdgxd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3adkuqgtq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3wdxrgcyy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3xiwedvnu.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3zfhjbync.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3kgaxycyh.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3pwhujrur.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3nfnoligd.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vxzccoeq.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ltlpzbeh.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wlnehyxf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3luzfxihh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3vpuzcowq.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mgsrmikc.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rmylmost.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3hptuzmfw.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bewsacys.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hzovcutt.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hdvhaayu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3csorzxlb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3kkweyghj.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dgopxxci.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pqajndcg.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fjrsrfpo.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3knsoedhx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zfyhkpit.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3zjdgbwhs.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3jabfhvbp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3anqgguun.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3pxvlksld.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3kjspgjmt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3yrgsfwdu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3kikevosu.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3podgvbow.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3xqgqusha.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3ighsfyul.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fcbzxqou.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ejngzuer.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3lzasjluk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3brlersau.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3jxdvxbuf.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3ftjsvuhz.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3gsfuiszc.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nzsfxdcw.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cqqftlgf.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3qhifutja.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3awebcbhj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ycmovkzp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3tformnpu.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vcazxnpc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3ctlvgudd.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3mnvabowk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xdyeaisz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vzqnlkau.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ctqikfes.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rwhybiix.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3oxxjxwfe.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pyglupta.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gydnlemk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3djgivjus.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3cezuqdgt.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ilmcarbd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3qywbqddz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zzqeddux.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dohzdoiq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3mmiblkrs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3mrcfwitw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vfidahna.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3nhknrlml.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3usmfsnad.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3vukxvfwm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3gzaaaczy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3uuofdogb.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3jgksfgxo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3vqndlckn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3uxyeqlez.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3lajliiyb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3opjlaief.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mhuavvog.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3nqwezzjq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3afaliufp.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3awxyboxf.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3ykdfrmot.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3svxpshms.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3evhdwvhc.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3zueghbrz.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mfcigfpu.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3tgoyfioz.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3awwefjhz.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3iowbjjdh.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3ueigqbgj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3pwzyecdh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3isqptotg.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3dgwhvcdr.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3nljjtrdz.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3cmejkmer.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3htydxmlv.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3maxhpjfv.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oiaaccqd.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3nwmhopiy.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3tfuxffnq.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xwltvgbt.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3vtrzoqgm.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3qivqlntn.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3smbfclza.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3pycuyxfg.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3obqfrxka.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3dqsjxtqy.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3mzdgjfkx.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3eciujsxk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3hldgtvaa.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3gkaudnug.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ddhbpggb.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rjleneca.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3mlfjeefb.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3lohoswbt.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ilbijdnb.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3flvptmna.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3cklstizp.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3msowucog.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3lczvsukt.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3gahgfchs.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bujnjzlo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3ekqzfqfz.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3mapkakqt.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fohpncmk.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3cfphtpqa.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3yhvzrais.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3nsrifiez.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwjzyonw.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3dmklnwsl.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3pvyjmonv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3viouklgn.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3hkzteyvr.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3mgvmhgir.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3ncujlgts.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3hzqkdybc.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bbabewsg.html


<!-- 参考信息 -->