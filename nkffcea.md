代发 wailian999

C#:   s.Replace("a", "b")
来源：http://qj.szxytkj.cn

[E07] 按分隔符拆分
来源：http://rx.jianghongdianzi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mh.yuexingan06.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ea.hahajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://wz.colortex.cn

TS:   s.split(",")
来源：http://hk.shtwfgs.cn

Java: s.split(",");  s.split("\\s+")
来源：http://tx.muxihuayi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://od.chemitech.net.cn

Ruby: s.split(",");  s.split
来源：http://kb.yuntaijiaju.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mn.yuntaijiaju.cn

[E08] 数组按分隔符合并
来源：http://ms.shxzskj.cn

Py:   ",".join(items)
来源：http://zn.521024.cn

PHP:  implode(",", $items);
来源：http://lr.wgjwhj.cn

JS:   items.join(",")
来源：http://uf.szxytkj.cn

TS:   items.join(",")
来源：http://xi.yuntaijiaju.cn

Java: String.join(",", items)
来源：http://kr.asd995.cn

Go:   strings.Join(items, ",")
来源：http://hx.nszjky.cn

Ruby: items.join(",")
来源：http://uq.muxihuayi.cn

C#:   string.Join(",", items)
来源：http://lv.huixiangedu.cn

[E09] 去除所有空白字符
来源：http://hz.shxzskj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fn.huanxung.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fi.shtwfgs.cn

JS:   s.replace(/\s+/g, "")
来源：http://jy.szxytkj.cn

TS:   s.replace(/\s+/g, "")
来源：http://el.yuntaijiaju.cn

Java: s.replaceAll("\\s+", "")
来源：http://em.9csxet.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://wm.lnxyls.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ur.panjiajie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qc.haigaiapp.cn

[E10] 左侧补零 / 定长填充
来源：http://pf.haigaiapp.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lh.shxzukj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wv.muxihuayi.cn

JS:   "7".padStart(3, "0")
来源：http://sg.colortex.cn

TS:   "7".padStart(3, "0")
来源：http://qw.huanxung.cn

Java: String.format("%03d", 7)
来源：http://fg.yuntaijiaju.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://zq.huanxung.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vh.szsharing.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fe.9csxet.cn

[E11] 反转字符串
来源：http://en.nicolike.cn

Py:   s[::-1]
来源：http://ei.bjjhwx.cn

PHP:  strrev($s);
来源：http://ds.hnjuh.cn

JS:   [...s].reverse().join("")
来源：http://rb.huixinmuqiang.cn

TS:   [...s].reverse().join("")
来源：http://tr.nicolike.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ed.jianghongdianzi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://iu.asd995.cn

Ruby: s.reverse
来源：http://bg.panjiajie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://mg.yuexingan06.cn

[E12] 统计某字符出现次数
来源：http://il.shxzukj.cn

Py:   s.count("a")
来源：http://ly.hahajie.cn

PHP:  substr_count($s, "a");
来源：http://dt.chemitech.net.cn

JS:   s.split("a").length - 1
来源：http://gg.yuexingan06.cn

TS:   s.split("a").length - 1
来源：http://es.huanxung.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pk.szsharing.cn

Go:   strings.Count(s, "a")
来源：http://lc.shxzskj.cn

Ruby: s.count("a")
来源：http://wm.bjjhwx.cn

C#:   s.Count(c => c == 'a')
来源：http://fu.jctech888.com.cn

[E13] 逐字符遍历
来源：http://uf.hnjuh.cn

Py:   for ch in s: print(ch)
来源：http://kh.colortex.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tf.huanxung.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://gf.newstarts.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qz.jctech888.com.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tt.bookmarksfly.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://py.shxzukj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rw.colortex.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dc.lnxyls.cn

[E14] URL 编码与 Base64
来源：http://vg.szsharing.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://on.jctech888.com.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://pq.bjjhwx.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nb.shxzskj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://iu.shxzukj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pn.wgjwhj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nw.shxzukj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tu.huixinmuqiang.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bv.shtwfgs.cn

[E15] HTML 转义 / 反转义
来源：http://la.huixinmuqiang.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xr.wgjwhj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://eb.shxzukj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wl.hnjuh.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ij.yuntaijiaju.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rs.shxzukj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ny.jctech888.com.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ay.newstarts.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ze.shxzukj.cn

[E16] 数字千分位
来源：http://jb.panjiajie.cn

Py:   f"{1234567:,}"
来源：http://mr.colortex.cn

PHP:  number_format(1234567);
来源：http://ry.nszjky.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://qa.shtwfgs.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://uf.chemitech.net.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xl.newstarts.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yn.muxihuayi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://br.huixiangedu.cn

C#:   1234567.ToString("N0")
来源：http://se.muxihuayi.cn

[E17] 首字母大写
来源：http://lt.shtwfgs.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xa.szsharing.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://md.shxzskj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qg.hnjuh.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://eh.szsharing.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cj.newstarts.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qh.shtwfgs.cn

Ruby: s.capitalize
来源：http://ws.shxzskj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ez.hnjuh.cn

[E18] 模板占位符替换
来源：http://kb.jctech888.com.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hn.panjiajie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gl.asd995.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ay.nicolike.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://pv.muxihuayi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xo.wgjwhj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fe.panjiajie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xc.panjiajie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://op.nszjky.cn

[E19] 多行文本按行拆分
来源：http://nl.shtwfgs.cn

Py:   s.splitlines()
来源：http://yd.panjiajie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cb.shxzskj.cn

JS:   s.split(/\r?\n/)
来源：http://gc.yuexingan06.cn

TS:   s.split(/\r?\n/)
来源：http://ry.nszjky.cn

Java: s.lines().toList()
来源：http://ss.jianghongdianzi.cn

Go:   strings.Split(s, "\n")
来源：http://oc.hahajie.cn

Ruby: s.lines
来源：http://kg.huixiangedu.cn

C#:   s.Split('\n')
来源：http://ir.panjiajie.cn

[E20] 判断字符串是否为空
来源：http://xx.huixiangedu.cn

Py:   if not s:
来源：http://wr.wgjwhj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lz.gzmigu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mx.9csxet.cn

TS:   if (s === "") {}
来源：http://rw.panjiajie.cn

Java: if (s.isEmpty()) {}
来源：http://pb.newstarts.cn

Go:   if s == "" {}
来源：http://yi.nszjky.cn

Ruby: if s.empty?
来源：http://gq.shxzskj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bn.bjjhwx.cn

[E21] 超长截断加省略号
来源：http://yc.asd995.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yy.huixinmuqiang.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://aq.wgjwhj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ez.shxzukj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ra.nicolike.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ua.asd995.cn

Go:   // 按 rune 判断长度后截断
来源：http://ix.bookmarksfly.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pk.nszjky.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cx.521024.cn

[E22] 字节长度与字符长度
来源：http://wv.yuntaijiaju.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ej.jctech888.com.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ue.9csxet.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ev.nicolike.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ej.jianghongdianzi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xq.hahajie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rr.bjjhwx.cn

Ruby: s.bytesize;  s.length
来源：http://wt.chemitech.net.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://eq.hnjuh.cn

================================================================================
来源：http://qd.jctech888.com.cn

F. 文件与目录
来源：http://xm.szxytkj.cn

================================================================================
来源：http://zp.colortex.cn

[F01] 读取整个文件
来源：http://gu.huixiangedu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zu.hahajie.cn

PHP:  file_get_contents("a.txt");
来源：http://el.yuexingan06.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://da.yuntaijiaju.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ij.nszjky.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://bp.nszjky.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qk.yuntaijiaju.cn

Ruby: File.read("a.txt")
来源：http://cv.nicolike.cn

C#:   File.ReadAllText("a.txt");
来源：http://uj.szsharing.cn

[F02] 逐行读取文件
来源：http://jh.shxzukj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uz.huanxung.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://eg.colortex.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jy.bjjhwx.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ta.huanxung.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://al.huixinmuqiang.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nf.yuexingan06.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vz.muxihuayi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bu.yuexingan06.cn

[F03] 写入文件（覆盖）
来源：http://zk.shxzukj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pt.gzmigu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://pd.bjjhwx.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://be.panjiajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mm.panjiajie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://iz.bookmarksfly.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gk.lnxyls.cn

Ruby: File.write("a.txt", "hi")
来源：http://lc.lnxyls.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yd.jianghongdianzi.cn

[F04] 追加写入文件
来源：http://mo.szxytkj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hi.bjjhwx.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hc.jctech888.com.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nd.bjjhwx.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ty.shtwfgs.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gu.bjjhwx.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ti.huixiangedu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xr.nicolike.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://am.chemitech.net.cn

[F05] 判断文件或目录是否存在
来源：http://fh.chemitech.net.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ru.wgjwhj.cn

PHP:  file_exists("a.txt");
来源：http://wr.yuntaijiaju.cn

JS:   fs.existsSync("a.txt")
来源：http://mf.yuexingan06.cn

TS:   fs.existsSync("a.txt")
来源：http://lc.huixinmuqiang.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://zm.lnxyls.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ke.colortex.cn

Ruby: File.exist?("a.txt")
来源：http://dv.yuexingan06.cn

C#:   File.Exists("a.txt")
来源：http://zm.gzmigu.cn

[F06] 删除文件
来源：http://ra.muxihuayi.cn

Py:   os.remove("a.txt")
来源：http://gl.chemitech.net.cn

PHP:  unlink("a.txt");
来源：http://qg.shxzukj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://iu.gzmigu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://wd.hahajie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xa.hahajie.cn

Go:   os.Remove("a.txt")
来源：http://ku.lnxyls.cn

Ruby: File.delete("a.txt")
来源：http://xk.colortex.cn

C#:   File.Delete("a.txt");
来源：http://bm.asd995.cn

[F07] 创建目录（含多级）
来源：http://fv.muxihuayi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hq.muxihuayi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tj.chemitech.net.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hq.shxzskj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mw.gzmigu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zu.bjjhwx.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ue.nicolike.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wp.shtwfgs.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rj.hahajie.cn

[F08] 遍历目录
来源：http://qv.newstarts.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://lf.muxihuayi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nn.hahajie.cn

JS:   fs.readdirSync("dir")
来源：http://zf.muxihuayi.cn

TS:   fs.readdirSync("dir")
来源：http://kk.shxzukj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wx.newstarts.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ks.yuntaijiaju.cn

Ruby: Dir.children("dir")
来源：http://xz.9csxet.cn

C#:   Directory.GetFiles("dir")
来源：http://jz.521024.cn

[F09] 获取文件大小
来源：http://wl.shxzskj.cn

Py:   os.path.getsize("a.txt")
来源：http://yl.wgjwhj.cn

PHP:  filesize("a.txt");
来源：http://lp.haigaiapp.cn

JS:   fs.statSync("a.txt").size
来源：http://en.newstarts.cn

TS:   fs.statSync("a.txt").size
来源：http://lj.newstarts.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ao.nicolike.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nb.9csxet.cn

Ruby: File.size("a.txt")
来源：http://ov.szsharing.cn

C#:   new FileInfo("a.txt").Length
来源：http://qk.jianghongdianzi.cn

[F10] 取文件扩展名 / 文件名
来源：http://uo.huanxung.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vw.huixinmuqiang.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://in.bookmarksfly.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fr.9csxet.cn

TS:   path.extname("a.txt")
来源：http://qw.muxihuayi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://az.shxzskj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xy.bookmarksfly.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://if.newstarts.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://so.bookmarksfly.cn

[F11] 复制与移动文件
来源：http://mx.nszjky.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xc.huanxung.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lw.shxzukj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ew.shtwfgs.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wj.hnjuh.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://td.gzmigu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://aj.szxytkj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kj.hahajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ib.haigaiapp.cn

[F12] CSV 读写
来源：http://hu.haigaiapp.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://eo.9csxet.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xu.szsharing.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qv.muxihuayi.cn

TS:   // 同上
来源：http://ne.szxytkj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cu.shtwfgs.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kq.huixinmuqiang.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nw.521024.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://cs.huixinmuqiang.cn

================================================================================
来源：http://yi.bookmarksfly.cn

G. 面向对象
来源：http://ej.shxzskj.cn

================================================================================
来源：http://ed.szsharing.cn

[G01] 定义类
来源：http://us.huixiangedu.cn

Py:   class User: pass
来源：http://in.521024.cn

PHP:  class User {}
来源：http://mp.gzmigu.cn

JS:   class User {}
来源：http://to.chemitech.net.cn

TS:   class User { name: string = ""; }
来源：http://jc.huanxung.cn

Java: class User {}
来源：http://ms.huixinmuqiang.cn

Go:   type User struct { Name string }
来源：http://oa.lnxyls.cn

Ruby: class User; end
来源：http://hp.huixinmuqiang.cn

C#:   class User {}
来源：http://ae.jctech888.com.cn

[G02] 构造函数
来源：http://dw.wgjwhj.cn

Py:   def __init__(self, name): self.name = name
来源：http://ox.huixiangedu.cn

PHP:  public function __construct(public string $name) {}
来源：http://kr.lnxyls.cn

JS:   constructor(name) { this.name = name; }
来源：http://mt.haigaiapp.cn

TS:   constructor(public name: string) {}
来源：http://gw.521024.cn

Java: User(String name) { this.name = name; }
来源：http://xe.yuexingan06.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ea.yuexingan06.cn

Ruby: def initialize(name); @name = name; end
来源：http://cl.nicolike.cn

C#:   public User(string name) { Name = name; }
来源：http://pf.muxihuayi.cn

[G03] 实例属性
来源：http://xb.szxytkj.cn

Py:   self.name = "x"
来源：http://ft.lnxyls.cn

PHP:  public string $name = "x";
来源：http://ex.nicolike.cn

JS:   this.name = "x";
来源：http://mv.newstarts.cn

TS:   name: string = "x";
来源：http://mm.521024.cn

Java: private String name;
来源：http://iw.jctech888.com.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vb.szsharing.cn

Ruby: @name = "x"
来源：http://pv.haigaiapp.cn

C#:   public string Name { get; set; } = "x";
来源：http://mp.yuexingan06.cn

[G04] 定义方法
来源：http://wb.asd995.cn

Py:   def greet(self): return self.name
来源：http://ww.hnjuh.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://jg.nszjky.cn

JS:   greet() { return this.name; }
来源：http://vj.nicolike.cn

TS:   greet(): string { return this.name; }
来源：http://ox.colortex.cn

Java: String greet() { return name; }
来源：http://id.shxzskj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://kl.muxihuayi.cn

Ruby: def greet; @name; end
来源：http://vv.chemitech.net.cn

C#:   public string Greet() => Name;
来源：http://qs.lnxyls.cn

[G05] 继承
来源：http://yq.szsharing.cn

Py:   class Admin(User): pass
来源：http://en.colortex.cn

PHP:  class Admin extends User {}
来源：http://at.muxihuayi.cn

JS:   class Admin extends User {}
来源：http://ai.hnjuh.cn

TS:   class Admin extends User {}
来源：http://nl.panjiajie.cn


<!-- 参考信息 -->