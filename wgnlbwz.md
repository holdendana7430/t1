代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ed.nszjky.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dn.yuntaijiaju.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ey.newstarts.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gr.huixinmuqiang.cn

[E06] 替换子串
来源：http://ys.hnjuh.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mx.huanxung.cn

PHP:  str_replace("a", "b", $s);
来源：http://lj.szsharing.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://py.bookmarksfly.cn

TS:   s.replaceAll("a", "b")
来源：http://hl.newstarts.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ak.szsharing.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://or.newstarts.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fc.shxzukj.cn

C#:   s.Replace("a", "b")
来源：http://qj.shxzukj.cn

[E07] 按分隔符拆分
来源：http://iy.shtwfgs.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tf.yuntaijiaju.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://uu.yuexingan06.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://sl.bjjhwx.cn

TS:   s.split(",")
来源：http://by.szsharing.cn

Java: s.split(",");  s.split("\\s+")
来源：http://pw.hahajie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ab.haigaiapp.cn

Ruby: s.split(",");  s.split
来源：http://az.hnjuh.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://we.jctech888.com.cn

[E08] 数组按分隔符合并
来源：http://mn.gzmigu.cn

Py:   ",".join(items)
来源：http://pk.hnjuh.cn

PHP:  implode(",", $items);
来源：http://jr.huixinmuqiang.cn

JS:   items.join(",")
来源：http://cb.huixinmuqiang.cn

TS:   items.join(",")
来源：http://sw.szxytkj.cn

Java: String.join(",", items)
来源：http://kj.jianghongdianzi.cn

Go:   strings.Join(items, ",")
来源：http://xs.lnxyls.cn

Ruby: items.join(",")
来源：http://gc.hahajie.cn

C#:   string.Join(",", items)
来源：http://mh.yuntaijiaju.cn

[E09] 去除所有空白字符
来源：http://vi.bjjhwx.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ny.jianghongdianzi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ut.szxytkj.cn

JS:   s.replace(/\s+/g, "")
来源：http://kj.nicolike.cn

TS:   s.replace(/\s+/g, "")
来源：http://rd.lnxyls.cn

Java: s.replaceAll("\\s+", "")
来源：http://fj.nicolike.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://mz.panjiajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ou.yuexingan06.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fb.bjjhwx.cn

[E10] 左侧补零 / 定长填充
来源：http://wh.szsharing.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://sl.nicolike.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ak.bjjhwx.cn

JS:   "7".padStart(3, "0")
来源：http://dj.9csxet.cn

TS:   "7".padStart(3, "0")
来源：http://ke.huixiangedu.cn

Java: String.format("%03d", 7)
来源：http://et.nszjky.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ug.bookmarksfly.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qd.shxzskj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bi.shxzukj.cn

[E11] 反转字符串
来源：http://qx.nszjky.cn

Py:   s[::-1]
来源：http://dx.hnjuh.cn

PHP:  strrev($s);
来源：http://qc.shxzukj.cn

JS:   [...s].reverse().join("")
来源：http://ew.521024.cn

TS:   [...s].reverse().join("")
来源：http://xg.huixinmuqiang.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ep.gzmigu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://cp.newstarts.cn

Ruby: s.reverse
来源：http://gj.muxihuayi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://rq.wgjwhj.cn

[E12] 统计某字符出现次数
来源：http://ag.haigaiapp.cn

Py:   s.count("a")
来源：http://lb.asd995.cn

PHP:  substr_count($s, "a");
来源：http://kv.521024.cn

JS:   s.split("a").length - 1
来源：http://wv.shxzukj.cn

TS:   s.split("a").length - 1
来源：http://gl.shtwfgs.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kh.lnxyls.cn

Go:   strings.Count(s, "a")
来源：http://ua.bjjhwx.cn

Ruby: s.count("a")
来源：http://em.asd995.cn

C#:   s.Count(c => c == 'a')
来源：http://mh.hahajie.cn

[E13] 逐字符遍历
来源：http://ca.shxzskj.cn

Py:   for ch in s: print(ch)
来源：http://ce.lnxyls.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fg.nicolike.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://nr.wgjwhj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://nt.521024.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://en.521024.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vs.shtwfgs.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://hs.muxihuayi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://co.haigaiapp.cn

[E14] URL 编码与 Base64
来源：http://bu.yuexingan06.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ex.panjiajie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://eg.panjiajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ck.hahajie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yw.bookmarksfly.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bd.szsharing.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://js.hnjuh.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://di.lnxyls.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gs.panjiajie.cn

[E15] HTML 转义 / 反转义
来源：http://hk.huanxung.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://cg.521024.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xn.colortex.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cb.panjiajie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://dl.shxzskj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ed.bjjhwx.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sn.newstarts.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yn.hahajie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://df.bjjhwx.cn

[E16] 数字千分位
来源：http://zf.szxytkj.cn

Py:   f"{1234567:,}"
来源：http://xo.jianghongdianzi.cn

PHP:  number_format(1234567);
来源：http://aq.muxihuayi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://rm.haigaiapp.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ze.shxzskj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nk.hahajie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rv.huixiangedu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://eq.chemitech.net.cn

C#:   1234567.ToString("N0")
来源：http://lb.haigaiapp.cn

[E17] 首字母大写
来源：http://et.huixiangedu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jc.wgjwhj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://gv.shxzskj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uk.szsharing.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mt.shtwfgs.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://js.muxihuayi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vd.asd995.cn

Ruby: s.capitalize
来源：http://mn.jianghongdianzi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jj.lnxyls.cn

[E18] 模板占位符替换
来源：http://dy.colortex.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ss.szsharing.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mk.huixiangedu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://kk.nszjky.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://bh.yuntaijiaju.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hs.lnxyls.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zb.huanxung.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://em.521024.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ep.huixiangedu.cn

[E19] 多行文本按行拆分
来源：http://ny.hahajie.cn

Py:   s.splitlines()
来源：http://jn.yuexingan06.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ac.haigaiapp.cn

JS:   s.split(/\r?\n/)
来源：http://cs.nszjky.cn

TS:   s.split(/\r?\n/)
来源：http://oa.chemitech.net.cn

Java: s.lines().toList()
来源：http://ap.gzmigu.cn

Go:   strings.Split(s, "\n")
来源：http://ci.bjjhwx.cn

Ruby: s.lines
来源：http://lw.chemitech.net.cn

C#:   s.Split('\n')
来源：http://pt.bjjhwx.cn

[E20] 判断字符串是否为空
来源：http://ll.shtwfgs.cn

Py:   if not s:
来源：http://at.shxzukj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nc.muxihuayi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://oq.panjiajie.cn

TS:   if (s === "") {}
来源：http://ks.asd995.cn

Java: if (s.isEmpty()) {}
来源：http://gb.shxzukj.cn

Go:   if s == "" {}
来源：http://uo.hahajie.cn

Ruby: if s.empty?
来源：http://gt.huanxung.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yi.colortex.cn

[E21] 超长截断加省略号
来源：http://kg.hahajie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ed.lnxyls.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rd.colortex.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cx.nicolike.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ga.hnjuh.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wf.huanxung.cn

Go:   // 按 rune 判断长度后截断
来源：http://jt.huixinmuqiang.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yq.gzmigu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://va.bookmarksfly.cn

[E22] 字节长度与字符长度
来源：http://to.yuntaijiaju.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fr.bjjhwx.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://db.shtwfgs.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pc.bjjhwx.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yj.asd995.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qg.colortex.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hu.colortex.cn

Ruby: s.bytesize;  s.length
来源：http://tp.shxzukj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ei.shxzskj.cn

================================================================================
来源：http://yj.lnxyls.cn

F. 文件与目录
来源：http://dm.huixinmuqiang.cn

================================================================================
来源：http://cg.yuexingan06.cn

[F01] 读取整个文件
来源：http://ef.nszjky.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rb.hahajie.cn

PHP:  file_get_contents("a.txt");
来源：http://ev.huanxung.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ge.nicolike.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qw.jianghongdianzi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rk.bjjhwx.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zb.szsharing.cn

Ruby: File.read("a.txt")
来源：http://ov.szxytkj.cn

C#:   File.ReadAllText("a.txt");
来源：http://zf.asd995.cn

[F02] 逐行读取文件
来源：http://nc.yuexingan06.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uq.szsharing.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nv.newstarts.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yy.wgjwhj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zl.yuntaijiaju.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wp.asd995.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qj.nicolike.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://at.jianghongdianzi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ve.wgjwhj.cn

[F03] 写入文件（覆盖）
来源：http://tk.wgjwhj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://oo.jctech888.com.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://rm.jctech888.com.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ox.nszjky.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hw.shtwfgs.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://he.szsharing.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mi.panjiajie.cn

Ruby: File.write("a.txt", "hi")
来源：http://im.colortex.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ah.jianghongdianzi.cn

[F04] 追加写入文件
来源：http://nn.yuexingan06.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tl.jctech888.com.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rk.hahajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gt.shxzukj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ik.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vo.huixinmuqiang.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wu.huixiangedu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lp.huanxung.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ge.shxzukj.cn

[F05] 判断文件或目录是否存在
来源：http://ta.bjjhwx.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yx.yuexingan06.cn

PHP:  file_exists("a.txt");
来源：http://qz.chemitech.net.cn

JS:   fs.existsSync("a.txt")
来源：http://lz.gzmigu.cn

TS:   fs.existsSync("a.txt")
来源：http://pm.nszjky.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vd.9csxet.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ua.shxzukj.cn

Ruby: File.exist?("a.txt")
来源：http://lk.jianghongdianzi.cn

C#:   File.Exists("a.txt")
来源：http://te.hahajie.cn

[F06] 删除文件
来源：http://qi.9csxet.cn

Py:   os.remove("a.txt")
来源：http://uy.haigaiapp.cn

PHP:  unlink("a.txt");
来源：http://nt.haigaiapp.cn

JS:   fs.unlinkSync("a.txt")
来源：http://wc.yuntaijiaju.cn

TS:   fs.unlinkSync("a.txt")
来源：http://jh.huixiangedu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vz.yuntaijiaju.cn

Go:   os.Remove("a.txt")
来源：http://jw.hnjuh.cn

Ruby: File.delete("a.txt")
来源：http://yy.colortex.cn

C#:   File.Delete("a.txt");
来源：http://ko.lnxyls.cn

[F07] 创建目录（含多级）
来源：http://nw.szxytkj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://iy.asd995.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pc.shxzskj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bp.szxytkj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yb.hnjuh.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://so.hahajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fh.chemitech.net.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jj.bookmarksfly.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xb.shxzskj.cn

[F08] 遍历目录
来源：http://km.szxytkj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ss.newstarts.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ku.huanxung.cn

JS:   fs.readdirSync("dir")
来源：http://ct.jctech888.com.cn

TS:   fs.readdirSync("dir")
来源：http://vg.hnjuh.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lv.haigaiapp.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fg.shxzukj.cn

Ruby: Dir.children("dir")
来源：http://bd.huixiangedu.cn

C#:   Directory.GetFiles("dir")
来源：http://jq.wgjwhj.cn

[F09] 获取文件大小
来源：http://jn.yuntaijiaju.cn

Py:   os.path.getsize("a.txt")
来源：http://re.hnjuh.cn

PHP:  filesize("a.txt");
来源：http://fw.jctech888.com.cn

JS:   fs.statSync("a.txt").size
来源：http://eo.shtwfgs.cn

TS:   fs.statSync("a.txt").size
来源：http://ca.muxihuayi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://rv.huixiangedu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nf.huixinmuqiang.cn

Ruby: File.size("a.txt")
来源：http://rf.bjjhwx.cn

C#:   new FileInfo("a.txt").Length
来源：http://qy.shxzukj.cn

[F10] 取文件扩展名 / 文件名
来源：http://ad.shxzskj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://yt.jianghongdianzi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://km.colortex.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://uf.huanxung.cn

TS:   path.extname("a.txt")
来源：http://es.bjjhwx.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ke.asd995.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vr.chemitech.net.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://uh.lnxyls.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bc.chemitech.net.cn

[F11] 复制与移动文件
来源：http://yl.9csxet.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vt.colortex.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xu.chemitech.net.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tc.9csxet.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ay.huanxung.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pw.yuexingan06.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bn.wgjwhj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gu.asd995.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://li.chemitech.net.cn

[F12] CSV 读写
来源：http://jp.chemitech.net.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://is.hnjuh.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yd.jianghongdianzi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yb.bjjhwx.cn

TS:   // 同上
来源：http://mz.nicolike.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yn.colortex.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xz.szsharing.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mq.hahajie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://kf.huixiangedu.cn

================================================================================
来源：http://tn.bookmarksfly.cn

G. 面向对象
来源：http://vu.colortex.cn

================================================================================
来源：http://ba.szxytkj.cn

[G01] 定义类
来源：http://jv.shxzskj.cn

Py:   class User: pass
来源：http://sw.jianghongdianzi.cn

PHP:  class User {}
来源：http://fl.shxzskj.cn

JS:   class User {}
来源：http://of.chemitech.net.cn

TS:   class User { name: string = ""; }
来源：http://oa.yuntaijiaju.cn

Java: class User {}
来源：http://nl.shxzukj.cn

Go:   type User struct { Name string }
来源：http://fu.yuntaijiaju.cn

Ruby: class User; end
来源：http://gv.jianghongdianzi.cn

C#:   class User {}
来源：http://ss.nszjky.cn

[G02] 构造函数
来源：http://es.bookmarksfly.cn

Py:   def __init__(self, name): self.name = name
来源：http://et.jianghongdianzi.cn

PHP:  public function __construct(public string $name) {}
来源：http://ks.jianghongdianzi.cn

JS:   constructor(name) { this.name = name; }
来源：http://ho.muxihuayi.cn

TS:   constructor(public name: string) {}
来源：http://mk.hahajie.cn

Java: User(String name) { this.name = name; }
来源：http://kf.nicolike.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fz.bjjhwx.cn

Ruby: def initialize(name); @name = name; end
来源：http://vg.huanxung.cn

C#:   public User(string name) { Name = name; }
来源：http://yw.shxzukj.cn

[G03] 实例属性
来源：http://nn.chemitech.net.cn

Py:   self.name = "x"
来源：http://sn.huanxung.cn

PHP:  public string $name = "x";
来源：http://kq.shxzukj.cn

JS:   this.name = "x";
来源：http://ny.haigaiapp.cn

TS:   name: string = "x";
来源：http://os.9csxet.cn

Java: private String name;
来源：http://dm.huixinmuqiang.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zr.lnxyls.cn

Ruby: @name = "x"
来源：http://sh.chemitech.net.cn

C#:   public string Name { get; set; } = "x";
来源：http://tu.hahajie.cn

[G04] 定义方法
来源：http://zz.wgjwhj.cn

Py:   def greet(self): return self.name
来源：http://pj.colortex.cn


<!-- 参考信息 -->