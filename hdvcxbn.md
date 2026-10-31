代发 wailian999

PHP:  strpos($s, "x");
来源：http://jh.szxytkj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zh.shxzukj.cn

TS:   s.indexOf("x")
来源：http://sf.huixiangedu.cn

Java: s.indexOf("x")
来源：http://yw.panjiajie.cn

Go:   strings.Index(s, "x")
来源：http://bn.jctech888.com.cn

Ruby: s.index("x")
来源：http://zk.bookmarksfly.cn

C#:   s.IndexOf("x")
来源：http://de.jianghongdianzi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ss.521024.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uj.shxzskj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ge.yuntaijiaju.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pw.bjjhwx.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://tm.nicolike.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uj.szxytkj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mu.huixiangedu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pc.wgjwhj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://uu.jctech888.com.cn

[E06] 替换子串
来源：http://jd.huanxung.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://md.panjiajie.cn

PHP:  str_replace("a", "b", $s);
来源：http://df.huixiangedu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oo.newstarts.cn

TS:   s.replaceAll("a", "b")
来源：http://fg.jianghongdianzi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vm.nszjky.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zd.lnxyls.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hq.jctech888.com.cn

C#:   s.Replace("a", "b")
来源：http://ij.wgjwhj.cn

[E07] 按分隔符拆分
来源：http://yz.bookmarksfly.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zo.lnxyls.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ny.hahajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://my.szsharing.cn

TS:   s.split(",")
来源：http://ne.szsharing.cn

Java: s.split(",");  s.split("\\s+")
来源：http://er.huanxung.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jx.newstarts.cn

Ruby: s.split(",");  s.split
来源：http://gs.huanxung.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kz.shxzukj.cn

[E08] 数组按分隔符合并
来源：http://av.huanxung.cn

Py:   ",".join(items)
来源：http://gu.muxihuayi.cn

PHP:  implode(",", $items);
来源：http://py.huixiangedu.cn

JS:   items.join(",")
来源：http://bd.panjiajie.cn

TS:   items.join(",")
来源：http://iy.lnxyls.cn

Java: String.join(",", items)
来源：http://nj.huanxung.cn

Go:   strings.Join(items, ",")
来源：http://gm.jianghongdianzi.cn

Ruby: items.join(",")
来源：http://gy.panjiajie.cn

C#:   string.Join(",", items)
来源：http://bw.colortex.cn

[E09] 去除所有空白字符
来源：http://ci.9csxet.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ct.huixinmuqiang.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gh.hahajie.cn

JS:   s.replace(/\s+/g, "")
来源：http://ok.huixiangedu.cn

TS:   s.replace(/\s+/g, "")
来源：http://bp.asd995.cn

Java: s.replaceAll("\\s+", "")
来源：http://yg.nszjky.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://eo.haigaiapp.cn

Ruby: s.gsub(/\s+/, "")
来源：http://dz.panjiajie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://za.szxytkj.cn

[E10] 左侧补零 / 定长填充
来源：http://ns.lnxyls.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fo.asd995.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qv.huixiangedu.cn

JS:   "7".padStart(3, "0")
来源：http://fh.huanxung.cn

TS:   "7".padStart(3, "0")
来源：http://bi.asd995.cn

Java: String.format("%03d", 7)
来源：http://wb.asd995.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://kq.bjjhwx.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ya.yuntaijiaju.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nd.shxzukj.cn

[E11] 反转字符串
来源：http://br.yuexingan06.cn

Py:   s[::-1]
来源：http://zb.yuntaijiaju.cn

PHP:  strrev($s);
来源：http://od.jctech888.com.cn

JS:   [...s].reverse().join("")
来源：http://jn.bjjhwx.cn

TS:   [...s].reverse().join("")
来源：http://sy.nicolike.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://kh.shtwfgs.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://fo.gzmigu.cn

Ruby: s.reverse
来源：http://dz.bjjhwx.cn

C#:   new string(s.Reverse().ToArray())
来源：http://fq.hahajie.cn

[E12] 统计某字符出现次数
来源：http://tx.wgjwhj.cn

Py:   s.count("a")
来源：http://jm.9csxet.cn

PHP:  substr_count($s, "a");
来源：http://bw.huanxung.cn

JS:   s.split("a").length - 1
来源：http://bp.huixiangedu.cn

TS:   s.split("a").length - 1
来源：http://wg.521024.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ni.bookmarksfly.cn

Go:   strings.Count(s, "a")
来源：http://jl.9csxet.cn

Ruby: s.count("a")
来源：http://gf.haigaiapp.cn

C#:   s.Count(c => c == 'a')
来源：http://dt.hnjuh.cn

[E13] 逐字符遍历
来源：http://kc.lnxyls.cn

Py:   for ch in s: print(ch)
来源：http://uc.shxzskj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yn.huanxung.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://uj.9csxet.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ft.lnxyls.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://th.shtwfgs.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ed.bookmarksfly.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://yp.gzmigu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ln.asd995.cn

[E14] URL 编码与 Base64
来源：http://am.yuntaijiaju.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zt.huixinmuqiang.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://aw.nicolike.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tb.521024.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://af.huanxung.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dz.9csxet.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hb.wgjwhj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zm.jianghongdianzi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ku.chemitech.net.cn

[E15] HTML 转义 / 反转义
来源：http://sj.shxzskj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://di.521024.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qu.yuexingan06.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yy.huanxung.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wh.521024.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ya.szsharing.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bc.bookmarksfly.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wg.bjjhwx.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kd.szsharing.cn

[E16] 数字千分位
来源：http://zn.yuexingan06.cn

Py:   f"{1234567:,}"
来源：http://lp.shxzskj.cn

PHP:  number_format(1234567);
来源：http://xo.nicolike.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mj.shxzukj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://fr.shtwfgs.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://za.wgjwhj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zb.asd995.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://yf.nicolike.cn

C#:   1234567.ToString("N0")
来源：http://ks.bookmarksfly.cn

[E17] 首字母大写
来源：http://us.bookmarksfly.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lk.szsharing.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ln.gzmigu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lp.wgjwhj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vp.yuexingan06.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bq.yuexingan06.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://js.shxzukj.cn

Ruby: s.capitalize
来源：http://ow.chemitech.net.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zl.yuexingan06.cn

[E18] 模板占位符替换
来源：http://cz.jianghongdianzi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://op.lnxyls.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tf.asd995.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ad.jctech888.com.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://or.9csxet.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://an.shxzskj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://si.nicolike.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nq.bjjhwx.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ka.shxzskj.cn

[E19] 多行文本按行拆分
来源：http://vf.haigaiapp.cn

Py:   s.splitlines()
来源：http://ek.chemitech.net.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nh.shxzskj.cn

JS:   s.split(/\r?\n/)
来源：http://xp.huanxung.cn

TS:   s.split(/\r?\n/)
来源：http://yc.yuexingan06.cn

Java: s.lines().toList()
来源：http://ao.bjjhwx.cn

Go:   strings.Split(s, "\n")
来源：http://ks.nszjky.cn

Ruby: s.lines
来源：http://fh.yuntaijiaju.cn

C#:   s.Split('\n')
来源：http://td.nicolike.cn

[E20] 判断字符串是否为空
来源：http://as.lnxyls.cn

Py:   if not s:
来源：http://kk.szxytkj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ud.panjiajie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://oa.huanxung.cn

TS:   if (s === "") {}
来源：http://cf.gzmigu.cn

Java: if (s.isEmpty()) {}
来源：http://jh.bookmarksfly.cn

Go:   if s == "" {}
来源：http://tf.shxzskj.cn

Ruby: if s.empty?
来源：http://ll.shxzukj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vy.muxihuayi.cn

[E21] 超长截断加省略号
来源：http://gr.9csxet.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yf.wgjwhj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://si.bookmarksfly.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zs.colortex.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gr.muxihuayi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nk.hahajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://tf.yuexingan06.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cy.lnxyls.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rl.9csxet.cn

[E22] 字节长度与字符长度
来源：http://sx.nicolike.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vn.yuntaijiaju.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lj.nicolike.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mo.bjjhwx.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ai.panjiajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uz.huixiangedu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qe.yuntaijiaju.cn

Ruby: s.bytesize;  s.length
来源：http://ur.colortex.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ml.huixiangedu.cn

================================================================================
来源：http://tz.yuntaijiaju.cn

F. 文件与目录
来源：http://qw.shtwfgs.cn

================================================================================
来源：http://gc.panjiajie.cn

[F01] 读取整个文件
来源：http://eh.huixiangedu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://es.shxzukj.cn

PHP:  file_get_contents("a.txt");
来源：http://ao.huixinmuqiang.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yk.yuexingan06.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vx.shxzskj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://wa.nicolike.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hl.huanxung.cn

Ruby: File.read("a.txt")
来源：http://yp.haigaiapp.cn

C#:   File.ReadAllText("a.txt");
来源：http://ut.shtwfgs.cn

[F02] 逐行读取文件
来源：http://ti.nszjky.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tx.newstarts.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tx.huixiangedu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uo.hahajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ir.yuexingan06.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wm.panjiajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nu.521024.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gf.521024.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://iv.shxzskj.cn

[F03] 写入文件（覆盖）
来源：http://oz.jctech888.com.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://aa.huanxung.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://qp.jctech888.com.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pq.shtwfgs.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ly.yuntaijiaju.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ex.yuntaijiaju.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gw.huixiangedu.cn

Ruby: File.write("a.txt", "hi")
来源：http://gw.huixiangedu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rl.huanxung.cn

[F04] 追加写入文件
来源：http://le.nicolike.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bi.jctech888.com.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uz.bjjhwx.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://db.shxzskj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kg.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lc.wgjwhj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gx.jianghongdianzi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ny.panjiajie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xt.hahajie.cn

[F05] 判断文件或目录是否存在
来源：http://ph.shtwfgs.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yv.nszjky.cn

PHP:  file_exists("a.txt");
来源：http://az.yuntaijiaju.cn

JS:   fs.existsSync("a.txt")
来源：http://ua.jctech888.com.cn

TS:   fs.existsSync("a.txt")
来源：http://qj.haigaiapp.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://bz.9csxet.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fx.nicolike.cn

Ruby: File.exist?("a.txt")
来源：http://sn.szsharing.cn

C#:   File.Exists("a.txt")
来源：http://nu.jianghongdianzi.cn

[F06] 删除文件
来源：http://oy.szsharing.cn

Py:   os.remove("a.txt")
来源：http://or.shxzskj.cn

PHP:  unlink("a.txt");
来源：http://gk.panjiajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://zl.szxytkj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://bk.muxihuayi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tb.wgjwhj.cn

Go:   os.Remove("a.txt")
来源：http://gf.shxzskj.cn

Ruby: File.delete("a.txt")
来源：http://ek.chemitech.net.cn

C#:   File.Delete("a.txt");
来源：http://ww.gzmigu.cn

[F07] 创建目录（含多级）
来源：http://eu.521024.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wb.wgjwhj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://eg.9csxet.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://el.wgjwhj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cq.nszjky.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qz.panjiajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jh.wgjwhj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://es.chemitech.net.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kb.szxytkj.cn

[F08] 遍历目录
来源：http://oc.panjiajie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://qy.shxzukj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sy.jctech888.com.cn

JS:   fs.readdirSync("dir")
来源：http://yf.gzmigu.cn

TS:   fs.readdirSync("dir")
来源：http://cu.bookmarksfly.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bq.muxihuayi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ov.nszjky.cn

Ruby: Dir.children("dir")
来源：http://kw.shtwfgs.cn

C#:   Directory.GetFiles("dir")
来源：http://jk.lnxyls.cn

[F09] 获取文件大小
来源：http://tk.9csxet.cn

Py:   os.path.getsize("a.txt")
来源：http://so.asd995.cn

PHP:  filesize("a.txt");
来源：http://xs.colortex.cn

JS:   fs.statSync("a.txt").size
来源：http://ix.newstarts.cn

TS:   fs.statSync("a.txt").size
来源：http://ny.jctech888.com.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ks.jianghongdianzi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ug.jianghongdianzi.cn

Ruby: File.size("a.txt")
来源：http://wt.huixinmuqiang.cn

C#:   new FileInfo("a.txt").Length
来源：http://yb.jianghongdianzi.cn

[F10] 取文件扩展名 / 文件名
来源：http://vr.chemitech.net.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kx.asd995.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bo.jianghongdianzi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hq.hahajie.cn

TS:   path.extname("a.txt")
来源：http://eg.bjjhwx.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ly.chemitech.net.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://to.szxytkj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ts.lnxyls.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ev.bookmarksfly.cn

[F11] 复制与移动文件
来源：http://zv.shxzskj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ro.nszjky.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hy.wgjwhj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://im.wgjwhj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yy.shxzskj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ay.newstarts.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://it.nicolike.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mn.szsharing.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ae.521024.cn

[F12] CSV 读写
来源：http://ds.jianghongdianzi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://to.panjiajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kx.huanxung.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ra.hnjuh.cn

TS:   // 同上
来源：http://nd.hnjuh.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://sd.nicolike.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yv.jianghongdianzi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tc.huanxung.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gd.asd995.cn

================================================================================
来源：http://bz.colortex.cn

G. 面向对象
来源：http://vl.hahajie.cn

================================================================================
来源：http://ul.bjjhwx.cn

[G01] 定义类
来源：http://ua.nicolike.cn

Py:   class User: pass
来源：http://zl.huixiangedu.cn

PHP:  class User {}
来源：http://vl.nicolike.cn

JS:   class User {}
来源：http://wo.muxihuayi.cn

TS:   class User { name: string = ""; }
来源：http://jo.hnjuh.cn

Java: class User {}
来源：http://xx.gzmigu.cn

Go:   type User struct { Name string }
来源：http://tf.nszjky.cn

Ruby: class User; end
来源：http://bn.shxzukj.cn

C#:   class User {}
来源：http://tz.shtwfgs.cn

[G02] 构造函数
来源：http://pp.panjiajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://ko.yuntaijiaju.cn

PHP:  public function __construct(public string $name) {}
来源：http://ys.shxzukj.cn

JS:   constructor(name) { this.name = name; }
来源：http://jp.panjiajie.cn

TS:   constructor(public name: string) {}
来源：http://bi.lnxyls.cn

Java: User(String name) { this.name = name; }
来源：http://xr.huanxung.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ru.szxytkj.cn

Ruby: def initialize(name); @name = name; end
来源：http://zv.hahajie.cn


<!-- 参考信息 -->