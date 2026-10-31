代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ts.asd995.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xs.haigaiapp.cn

JS:   s.replace(/\s+/g, "")
来源：http://hx.colortex.cn

TS:   s.replace(/\s+/g, "")
来源：http://dz.gzmigu.cn

Java: s.replaceAll("\\s+", "")
来源：http://oq.huixiangedu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://lo.shxzskj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://gx.shxzukj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ax.huixiangedu.cn

[E10] 左侧补零 / 定长填充
来源：http://dt.lnxyls.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://as.asd995.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hw.521024.cn

JS:   "7".padStart(3, "0")
来源：http://ob.asd995.cn

TS:   "7".padStart(3, "0")
来源：http://nt.jianghongdianzi.cn

Java: String.format("%03d", 7)
来源：http://sf.colortex.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://fx.nicolike.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://uk.shxzukj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hx.gzmigu.cn

[E11] 反转字符串
来源：http://ir.asd995.cn

Py:   s[::-1]
来源：http://oq.hahajie.cn

PHP:  strrev($s);
来源：http://db.haigaiapp.cn

JS:   [...s].reverse().join("")
来源：http://nv.9csxet.cn

TS:   [...s].reverse().join("")
来源：http://jv.colortex.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://kw.nszjky.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://rz.jctech888.com.cn

Ruby: s.reverse
来源：http://ds.bjjhwx.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ya.shxzukj.cn

[E12] 统计某字符出现次数
来源：http://yp.nicolike.cn

Py:   s.count("a")
来源：http://hy.jctech888.com.cn

PHP:  substr_count($s, "a");
来源：http://qq.jianghongdianzi.cn

JS:   s.split("a").length - 1
来源：http://as.shxzskj.cn

TS:   s.split("a").length - 1
来源：http://tc.hahajie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mt.nszjky.cn

Go:   strings.Count(s, "a")
来源：http://ax.szxytkj.cn

Ruby: s.count("a")
来源：http://hk.jctech888.com.cn

C#:   s.Count(c => c == 'a')
来源：http://uq.hahajie.cn

[E13] 逐字符遍历
来源：http://gu.nszjky.cn

Py:   for ch in s: print(ch)
来源：http://in.newstarts.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vq.bjjhwx.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://fd.yuexingan06.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://mi.gzmigu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cp.huixiangedu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ql.521024.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://qy.hahajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xd.huixiangedu.cn

[E14] URL 编码与 Base64
来源：http://fg.521024.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mc.bookmarksfly.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ow.gzmigu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dm.huixiangedu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://in.panjiajie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ci.asd995.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cu.szsharing.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gs.shxzskj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gk.gzmigu.cn

[E15] HTML 转义 / 反转义
来源：http://rw.huanxung.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://in.chemitech.net.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jn.9csxet.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pf.yuexingan06.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://le.gzmigu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ya.nicolike.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mw.yuexingan06.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gn.bjjhwx.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ue.shtwfgs.cn

[E16] 数字千分位
来源：http://fl.haigaiapp.cn

Py:   f"{1234567:,}"
来源：http://re.9csxet.cn

PHP:  number_format(1234567);
来源：http://uf.hahajie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gv.muxihuayi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wa.lnxyls.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sr.gzmigu.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dd.bjjhwx.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bs.szxytkj.cn

C#:   1234567.ToString("N0")
来源：http://st.bjjhwx.cn

[E17] 首字母大写
来源：http://af.9csxet.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mv.huixiangedu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xv.huanxung.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zw.szsharing.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kq.hnjuh.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://yl.shtwfgs.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vi.521024.cn

Ruby: s.capitalize
来源：http://cw.9csxet.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rl.bookmarksfly.cn

[E18] 模板占位符替换
来源：http://ma.shtwfgs.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cw.yuntaijiaju.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jm.gzmigu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://dz.jianghongdianzi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ci.shxzukj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xv.newstarts.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yn.shtwfgs.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hq.yuexingan06.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://od.newstarts.cn

[E19] 多行文本按行拆分
来源：http://kx.jianghongdianzi.cn

Py:   s.splitlines()
来源：http://jp.bookmarksfly.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rk.wgjwhj.cn

JS:   s.split(/\r?\n/)
来源：http://jd.huanxung.cn

TS:   s.split(/\r?\n/)
来源：http://nt.nicolike.cn

Java: s.lines().toList()
来源：http://ao.wgjwhj.cn

Go:   strings.Split(s, "\n")
来源：http://gz.shxzukj.cn

Ruby: s.lines
来源：http://gr.colortex.cn

C#:   s.Split('\n')
来源：http://rq.shxzukj.cn

[E20] 判断字符串是否为空
来源：http://tc.huixiangedu.cn

Py:   if not s:
来源：http://wv.huixinmuqiang.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xy.bjjhwx.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wi.yuexingan06.cn

TS:   if (s === "") {}
来源：http://qs.jctech888.com.cn

Java: if (s.isEmpty()) {}
来源：http://wz.huixinmuqiang.cn

Go:   if s == "" {}
来源：http://rl.panjiajie.cn

Ruby: if s.empty?
来源：http://hh.gzmigu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vv.asd995.cn

[E21] 超长截断加省略号
来源：http://ci.hahajie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pc.bookmarksfly.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pg.yuexingan06.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hh.yuntaijiaju.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oo.jctech888.com.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mv.jctech888.com.cn

Go:   // 按 rune 判断长度后截断
来源：http://zc.bookmarksfly.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nz.hahajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wf.chemitech.net.cn

[E22] 字节长度与字符长度
来源：http://nl.yuexingan06.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gg.panjiajie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ra.szsharing.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ac.huixiangedu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ft.yuexingan06.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hq.chemitech.net.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dw.shtwfgs.cn

Ruby: s.bytesize;  s.length
来源：http://eg.panjiajie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xg.panjiajie.cn

================================================================================
来源：http://od.nszjky.cn

F. 文件与目录
来源：http://ho.muxihuayi.cn

================================================================================
来源：http://zp.newstarts.cn

[F01] 读取整个文件
来源：http://hb.huixiangedu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xl.hahajie.cn

PHP:  file_get_contents("a.txt");
来源：http://at.521024.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qn.bookmarksfly.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ku.521024.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ku.hnjuh.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dz.szxytkj.cn

Ruby: File.read("a.txt")
来源：http://rt.muxihuayi.cn

C#:   File.ReadAllText("a.txt");
来源：http://mm.hahajie.cn

[F02] 逐行读取文件
来源：http://qc.haigaiapp.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://od.newstarts.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ix.hahajie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nn.nszjky.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ow.asd995.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://do.asd995.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ac.wgjwhj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kk.huixinmuqiang.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mg.chemitech.net.cn

[F03] 写入文件（覆盖）
来源：http://sg.asd995.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gl.jctech888.com.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://lg.nicolike.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dq.bjjhwx.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iy.yuexingan06.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ge.newstarts.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nw.panjiajie.cn

Ruby: File.write("a.txt", "hi")
来源：http://au.jctech888.com.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ch.shtwfgs.cn

[F04] 追加写入文件
来源：http://zs.9csxet.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ih.colortex.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ti.huanxung.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ud.asd995.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://co.jianghongdianzi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mm.nszjky.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lb.shxzskj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pf.521024.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mf.shtwfgs.cn

[F05] 判断文件或目录是否存在
来源：http://ym.gzmigu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://us.jctech888.com.cn

PHP:  file_exists("a.txt");
来源：http://fe.yuntaijiaju.cn

JS:   fs.existsSync("a.txt")
来源：http://rp.chemitech.net.cn

TS:   fs.existsSync("a.txt")
来源：http://rm.hahajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qq.chemitech.net.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fx.yuntaijiaju.cn

Ruby: File.exist?("a.txt")
来源：http://pa.huanxung.cn

C#:   File.Exists("a.txt")
来源：http://sh.asd995.cn

[F06] 删除文件
来源：http://th.huixiangedu.cn

Py:   os.remove("a.txt")
来源：http://if.gzmigu.cn

PHP:  unlink("a.txt");
来源：http://fv.nicolike.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ef.szsharing.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ex.shxzukj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gl.yuntaijiaju.cn

Go:   os.Remove("a.txt")
来源：http://at.huixiangedu.cn

Ruby: File.delete("a.txt")
来源：http://ak.shtwfgs.cn

C#:   File.Delete("a.txt");
来源：http://ad.newstarts.cn

[F07] 创建目录（含多级）
来源：http://ep.9csxet.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vm.huixiangedu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://aq.hnjuh.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xy.nszjky.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jd.szsharing.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gj.nicolike.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://al.shxzukj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ns.shxzukj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ol.jctech888.com.cn

[F08] 遍历目录
来源：http://kh.shxzukj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://en.lnxyls.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wv.bookmarksfly.cn

JS:   fs.readdirSync("dir")
来源：http://ja.muxihuayi.cn

TS:   fs.readdirSync("dir")
来源：http://tr.yuexingan06.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ts.huanxung.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ya.yuexingan06.cn

Ruby: Dir.children("dir")
来源：http://gb.jctech888.com.cn

C#:   Directory.GetFiles("dir")
来源：http://se.huixinmuqiang.cn

[F09] 获取文件大小
来源：http://cz.panjiajie.cn

Py:   os.path.getsize("a.txt")
来源：http://zp.muxihuayi.cn

PHP:  filesize("a.txt");
来源：http://ts.9csxet.cn

JS:   fs.statSync("a.txt").size
来源：http://ou.muxihuayi.cn

TS:   fs.statSync("a.txt").size
来源：http://ct.chemitech.net.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ym.shxzukj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fi.9csxet.cn

Ruby: File.size("a.txt")
来源：http://uc.szsharing.cn

C#:   new FileInfo("a.txt").Length
来源：http://mb.gzmigu.cn

[F10] 取文件扩展名 / 文件名
来源：http://tu.szxytkj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ab.huixiangedu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qm.shxzukj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://oz.szsharing.cn

TS:   path.extname("a.txt")
来源：http://ua.jianghongdianzi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zp.shxzskj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vw.shtwfgs.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tx.szxytkj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://za.colortex.cn

[F11] 复制与移动文件
来源：http://yi.newstarts.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://df.gzmigu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ae.huanxung.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pz.jianghongdianzi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://my.jianghongdianzi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uv.9csxet.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ns.chemitech.net.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hq.521024.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ma.chemitech.net.cn

[F12] CSV 读写
来源：http://lp.lnxyls.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://la.huixinmuqiang.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ed.chemitech.net.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dd.gzmigu.cn

TS:   // 同上
来源：http://jp.bookmarksfly.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ie.shxzskj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mc.jctech888.com.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qz.shxzskj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ed.hnjuh.cn

================================================================================
来源：http://ww.jianghongdianzi.cn

G. 面向对象
来源：http://fl.newstarts.cn

================================================================================
来源：http://bu.shxzukj.cn

[G01] 定义类
来源：http://wo.huixiangedu.cn

Py:   class User: pass
来源：http://uw.shtwfgs.cn

PHP:  class User {}
来源：http://fd.huixiangedu.cn

JS:   class User {}
来源：http://ii.yuntaijiaju.cn

TS:   class User { name: string = ""; }
来源：http://od.shtwfgs.cn

Java: class User {}
来源：http://pa.panjiajie.cn

Go:   type User struct { Name string }
来源：http://qc.hahajie.cn

Ruby: class User; end
来源：http://wu.jctech888.com.cn

C#:   class User {}
来源：http://cu.chemitech.net.cn

[G02] 构造函数
来源：http://kb.newstarts.cn

Py:   def __init__(self, name): self.name = name
来源：http://iw.huanxung.cn

PHP:  public function __construct(public string $name) {}
来源：http://fa.chemitech.net.cn

JS:   constructor(name) { this.name = name; }
来源：http://pg.521024.cn

TS:   constructor(public name: string) {}
来源：http://od.huixiangedu.cn

Java: User(String name) { this.name = name; }
来源：http://tm.gzmigu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dx.shxzskj.cn

Ruby: def initialize(name); @name = name; end
来源：http://cf.haigaiapp.cn

C#:   public User(string name) { Name = name; }
来源：http://yp.nicolike.cn

[G03] 实例属性
来源：http://zx.chemitech.net.cn

Py:   self.name = "x"
来源：http://gu.wgjwhj.cn

PHP:  public string $name = "x";
来源：http://wc.haigaiapp.cn

JS:   this.name = "x";
来源：http://il.shtwfgs.cn

TS:   name: string = "x";
来源：http://tl.newstarts.cn

Java: private String name;
来源：http://al.newstarts.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nk.huixiangedu.cn

Ruby: @name = "x"
来源：http://cz.colortex.cn

C#:   public string Name { get; set; } = "x";
来源：http://gx.panjiajie.cn

[G04] 定义方法
来源：http://fl.lnxyls.cn

Py:   def greet(self): return self.name
来源：http://gq.asd995.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://is.shtwfgs.cn

JS:   greet() { return this.name; }
来源：http://wj.hahajie.cn

TS:   greet(): string { return this.name; }
来源：http://in.jctech888.com.cn

Java: String greet() { return name; }
来源：http://sa.hnjuh.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://bn.haigaiapp.cn

Ruby: def greet; @name; end
来源：http://zr.nszjky.cn

C#:   public string Greet() => Name;
来源：http://jo.huixinmuqiang.cn

[G05] 继承
来源：http://ls.huixinmuqiang.cn

Py:   class Admin(User): pass
来源：http://jo.huixinmuqiang.cn

PHP:  class Admin extends User {}
来源：http://hs.huanxung.cn

JS:   class Admin extends User {}
来源：http://ti.haigaiapp.cn

TS:   class Admin extends User {}
来源：http://eu.haigaiapp.cn

Java: class Admin extends User {}
来源：http://ae.shtwfgs.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yq.szxytkj.cn

Ruby: class Admin < User; end
来源：http://be.bookmarksfly.cn

C#:   class Admin : User {}
来源：http://bc.bjjhwx.cn

[G06] 重写方法
来源：http://mx.colortex.cn

Py:   def greet(self): return "admin"
来源：http://ux.shxzskj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://qz.shtwfgs.cn

JS:   greet() { return "admin"; }
来源：http://xa.bjjhwx.cn

TS:   greet(): string { return "admin"; }
来源：http://an.huixinmuqiang.cn

Java: @Override String greet() { return "admin"; }
来源：http://gu.nicolike.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gw.huanxung.cn

Ruby: def greet; "admin"; end
来源：http://id.newstarts.cn

C#:   public override string Greet() => "admin";
来源：http://ee.yuexingan06.cn

[G07] 调用父类方法
来源：http://ru.yuexingan06.cn

Py:   super().greet()
来源：http://wx.bookmarksfly.cn

PHP:  parent::greet();
来源：http://da.hahajie.cn

JS:   super.greet();
来源：http://my.panjiajie.cn

TS:   super.greet();
来源：http://rl.lnxyls.cn

Java: super.greet();
来源：http://hq.lnxyls.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://an.521024.cn


<!-- 参考信息 -->