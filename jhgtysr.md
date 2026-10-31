代发 wailian999

Ruby: s.split(",");  s.split
来源：http://wn.gzmigu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rr.wgjwhj.cn

[E08] 数组按分隔符合并
来源：http://us.jctech888.com.cn

Py:   ",".join(items)
来源：http://ug.9csxet.cn

PHP:  implode(",", $items);
来源：http://nn.colortex.cn

JS:   items.join(",")
来源：http://lp.jctech888.com.cn

TS:   items.join(",")
来源：http://kp.newstarts.cn

Java: String.join(",", items)
来源：http://dl.huixinmuqiang.cn

Go:   strings.Join(items, ",")
来源：http://uk.bjjhwx.cn

Ruby: items.join(",")
来源：http://qc.bjjhwx.cn

C#:   string.Join(",", items)
来源：http://tk.jianghongdianzi.cn

[E09] 去除所有空白字符
来源：http://pc.bookmarksfly.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pu.nszjky.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wc.colortex.cn

JS:   s.replace(/\s+/g, "")
来源：http://ve.nicolike.cn

TS:   s.replace(/\s+/g, "")
来源：http://nz.hahajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://wg.panjiajie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://jl.9csxet.cn

Ruby: s.gsub(/\s+/, "")
来源：http://vm.hahajie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ym.huanxung.cn

[E10] 左侧补零 / 定长填充
来源：http://az.muxihuayi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yq.yuexingan06.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zb.shtwfgs.cn

JS:   "7".padStart(3, "0")
来源：http://kk.shxzukj.cn

TS:   "7".padStart(3, "0")
来源：http://dl.huixiangedu.cn

Java: String.format("%03d", 7)
来源：http://fo.shxzukj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://bo.asd995.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://uy.jctech888.com.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kg.521024.cn

[E11] 反转字符串
来源：http://pf.huanxung.cn

Py:   s[::-1]
来源：http://rl.huanxung.cn

PHP:  strrev($s);
来源：http://bj.hahajie.cn

JS:   [...s].reverse().join("")
来源：http://gp.shtwfgs.cn

TS:   [...s].reverse().join("")
来源：http://jk.bjjhwx.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ug.jctech888.com.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://bb.shtwfgs.cn

Ruby: s.reverse
来源：http://yn.bjjhwx.cn

C#:   new string(s.Reverse().ToArray())
来源：http://fc.bjjhwx.cn

[E12] 统计某字符出现次数
来源：http://gn.newstarts.cn

Py:   s.count("a")
来源：http://kj.huixiangedu.cn

PHP:  substr_count($s, "a");
来源：http://vn.lnxyls.cn

JS:   s.split("a").length - 1
来源：http://kp.huixinmuqiang.cn

TS:   s.split("a").length - 1
来源：http://qq.yuexingan06.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ef.yuntaijiaju.cn

Go:   strings.Count(s, "a")
来源：http://kr.huanxung.cn

Ruby: s.count("a")
来源：http://fb.newstarts.cn

C#:   s.Count(c => c == 'a')
来源：http://zy.haigaiapp.cn

[E13] 逐字符遍历
来源：http://rv.wgjwhj.cn

Py:   for ch in s: print(ch)
来源：http://rw.chemitech.net.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zu.nszjky.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ou.hahajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://kd.521024.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rv.jianghongdianzi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ql.yuntaijiaju.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://wv.panjiajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://co.yuntaijiaju.cn

[E14] URL 编码与 Base64
来源：http://sg.chemitech.net.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ue.9csxet.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://im.nicolike.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nm.gzmigu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zx.lnxyls.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yd.yuexingan06.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ky.shxzukj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gi.asd995.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://uh.jctech888.com.cn

[E15] HTML 转义 / 反转义
来源：http://at.panjiajie.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ka.nicolike.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jy.lnxyls.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tg.muxihuayi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://gx.hahajie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wg.shxzukj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sx.jianghongdianzi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rq.9csxet.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ht.shtwfgs.cn

[E16] 数字千分位
来源：http://ba.shtwfgs.cn

Py:   f"{1234567:,}"
来源：http://pt.huixinmuqiang.cn

PHP:  number_format(1234567);
来源：http://gh.szsharing.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://hh.shtwfgs.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://um.jctech888.com.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ka.521024.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dk.szsharing.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ra.szsharing.cn

C#:   1234567.ToString("N0")
来源：http://bx.shxzukj.cn

[E17] 首字母大写
来源：http://uw.chemitech.net.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ji.haigaiapp.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ku.jianghongdianzi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nq.muxihuayi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vp.asd995.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nt.521024.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kv.szsharing.cn

Ruby: s.capitalize
来源：http://fb.huixiangedu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ks.haigaiapp.cn

[E18] 模板占位符替换
来源：http://yp.shxzukj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pw.nszjky.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://og.gzmigu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://wq.hahajie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://hk.colortex.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pf.521024.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mz.wgjwhj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ui.hnjuh.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qp.hahajie.cn

[E19] 多行文本按行拆分
来源：http://li.jctech888.com.cn

Py:   s.splitlines()
来源：http://gr.huixinmuqiang.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zk.wgjwhj.cn

JS:   s.split(/\r?\n/)
来源：http://jd.huanxung.cn

TS:   s.split(/\r?\n/)
来源：http://lr.haigaiapp.cn

Java: s.lines().toList()
来源：http://vk.chemitech.net.cn

Go:   strings.Split(s, "\n")
来源：http://fq.shtwfgs.cn

Ruby: s.lines
来源：http://rz.jctech888.com.cn

C#:   s.Split('\n')
来源：http://te.haigaiapp.cn

[E20] 判断字符串是否为空
来源：http://cl.haigaiapp.cn

Py:   if not s:
来源：http://ex.huixiangedu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bu.wgjwhj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kc.hnjuh.cn

TS:   if (s === "") {}
来源：http://pk.bookmarksfly.cn

Java: if (s.isEmpty()) {}
来源：http://xe.huixinmuqiang.cn

Go:   if s == "" {}
来源：http://wk.nicolike.cn

Ruby: if s.empty?
来源：http://zp.huanxung.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mr.yuntaijiaju.cn

[E21] 超长截断加省略号
来源：http://vg.lnxyls.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://md.gzmigu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://iy.bookmarksfly.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ek.yuexingan06.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vh.gzmigu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rv.lnxyls.cn

Go:   // 按 rune 判断长度后截断
来源：http://cc.yuexingan06.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://to.jctech888.com.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xs.521024.cn

[E22] 字节长度与字符长度
来源：http://ao.newstarts.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qq.haigaiapp.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sb.hahajie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gy.9csxet.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pm.huanxung.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hw.jctech888.com.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ms.wgjwhj.cn

Ruby: s.bytesize;  s.length
来源：http://xv.szxytkj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zi.szxytkj.cn

================================================================================
来源：http://hh.shxzskj.cn

F. 文件与目录
来源：http://rk.jianghongdianzi.cn

================================================================================
来源：http://yr.yuexingan06.cn

[F01] 读取整个文件
来源：http://um.panjiajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ni.szsharing.cn

PHP:  file_get_contents("a.txt");
来源：http://on.szxytkj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://eb.colortex.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hl.colortex.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://wg.jctech888.com.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ty.wgjwhj.cn

Ruby: File.read("a.txt")
来源：http://gv.hahajie.cn

C#:   File.ReadAllText("a.txt");
来源：http://vn.9csxet.cn

[F02] 逐行读取文件
来源：http://sg.shxzukj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dk.521024.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wc.colortex.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rz.nicolike.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jb.huixiangedu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jx.bookmarksfly.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ry.muxihuayi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://sa.bookmarksfly.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fu.jctech888.com.cn

[F03] 写入文件（覆盖）
来源：http://qy.panjiajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yk.szsharing.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://zn.newstarts.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qt.asd995.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dd.bjjhwx.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://se.nicolike.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zd.wgjwhj.cn

Ruby: File.write("a.txt", "hi")
来源：http://qp.nszjky.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yo.jctech888.com.cn

[F04] 追加写入文件
来源：http://gd.huanxung.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ir.9csxet.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vv.yuexingan06.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gg.lnxyls.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jq.yuntaijiaju.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ic.asd995.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qv.nicolike.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kt.haigaiapp.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mc.9csxet.cn

[F05] 判断文件或目录是否存在
来源：http://wl.szsharing.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gp.huixinmuqiang.cn

PHP:  file_exists("a.txt");
来源：http://uc.yuexingan06.cn

JS:   fs.existsSync("a.txt")
来源：http://zw.bookmarksfly.cn

TS:   fs.existsSync("a.txt")
来源：http://jh.szsharing.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://jj.521024.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://uu.jianghongdianzi.cn

Ruby: File.exist?("a.txt")
来源：http://op.yuntaijiaju.cn

C#:   File.Exists("a.txt")
来源：http://nn.newstarts.cn

[F06] 删除文件
来源：http://yr.bjjhwx.cn

Py:   os.remove("a.txt")
来源：http://xs.yuexingan06.cn

PHP:  unlink("a.txt");
来源：http://ql.9csxet.cn

JS:   fs.unlinkSync("a.txt")
来源：http://wq.hahajie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://wb.colortex.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://id.nicolike.cn

Go:   os.Remove("a.txt")
来源：http://rx.9csxet.cn

Ruby: File.delete("a.txt")
来源：http://da.shxzskj.cn

C#:   File.Delete("a.txt");
来源：http://fp.lnxyls.cn

[F07] 创建目录（含多级）
来源：http://ux.jianghongdianzi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xt.bookmarksfly.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gu.muxihuayi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cm.hahajie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kd.bookmarksfly.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jf.lnxyls.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wg.colortex.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gs.szxytkj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wl.gzmigu.cn

[F08] 遍历目录
来源：http://dc.haigaiapp.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://nj.huixiangedu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pm.asd995.cn

JS:   fs.readdirSync("dir")
来源：http://em.lnxyls.cn

TS:   fs.readdirSync("dir")
来源：http://up.shxzukj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vz.521024.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://sf.521024.cn

Ruby: Dir.children("dir")
来源：http://qr.haigaiapp.cn

C#:   Directory.GetFiles("dir")
来源：http://nq.shtwfgs.cn

[F09] 获取文件大小
来源：http://lb.jianghongdianzi.cn

Py:   os.path.getsize("a.txt")
来源：http://tg.huanxung.cn

PHP:  filesize("a.txt");
来源：http://an.huanxung.cn

JS:   fs.statSync("a.txt").size
来源：http://ad.yuntaijiaju.cn

TS:   fs.statSync("a.txt").size
来源：http://ds.jianghongdianzi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://nz.haigaiapp.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kj.shtwfgs.cn

Ruby: File.size("a.txt")
来源：http://yj.asd995.cn

C#:   new FileInfo("a.txt").Length
来源：http://lp.huixinmuqiang.cn

[F10] 取文件扩展名 / 文件名
来源：http://xn.hahajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.colortex.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hw.haigaiapp.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://px.szxytkj.cn

TS:   path.extname("a.txt")
来源：http://yt.9csxet.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jy.hahajie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lj.huanxung.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xk.lnxyls.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wa.521024.cn

[F11] 复制与移动文件
来源：http://rb.newstarts.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://oz.bjjhwx.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fo.yuntaijiaju.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ov.huixinmuqiang.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tu.bjjhwx.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lj.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://io.9csxet.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yw.asd995.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bw.huanxung.cn

[F12] CSV 读写
来源：http://we.panjiajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gz.asd995.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pm.hnjuh.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tt.szsharing.cn

TS:   // 同上
来源：http://ti.bookmarksfly.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gy.hnjuh.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vd.lnxyls.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ad.szxytkj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://cl.chemitech.net.cn

================================================================================
来源：http://me.gzmigu.cn

G. 面向对象
来源：http://ql.yuexingan06.cn

================================================================================
来源：http://cj.gzmigu.cn

[G01] 定义类
来源：http://nk.gzmigu.cn

Py:   class User: pass
来源：http://ni.colortex.cn

PHP:  class User {}
来源：http://kl.panjiajie.cn

JS:   class User {}
来源：http://mp.yuexingan06.cn

TS:   class User { name: string = ""; }
来源：http://ba.hahajie.cn

Java: class User {}
来源：http://df.szsharing.cn

Go:   type User struct { Name string }
来源：http://vu.gzmigu.cn

Ruby: class User; end
来源：http://jc.szsharing.cn

C#:   class User {}
来源：http://pw.hnjuh.cn

[G02] 构造函数
来源：http://ak.gzmigu.cn

Py:   def __init__(self, name): self.name = name
来源：http://pr.hahajie.cn

PHP:  public function __construct(public string $name) {}
来源：http://gd.lnxyls.cn

JS:   constructor(name) { this.name = name; }
来源：http://vp.newstarts.cn

TS:   constructor(public name: string) {}
来源：http://hv.bjjhwx.cn

Java: User(String name) { this.name = name; }
来源：http://or.asd995.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://au.huixinmuqiang.cn

Ruby: def initialize(name); @name = name; end
来源：http://sy.lnxyls.cn

C#:   public User(string name) { Name = name; }
来源：http://ti.gzmigu.cn

[G03] 实例属性
来源：http://nf.muxihuayi.cn

Py:   self.name = "x"
来源：http://lc.huixinmuqiang.cn

PHP:  public string $name = "x";
来源：http://bs.shxzskj.cn

JS:   this.name = "x";
来源：http://hg.shtwfgs.cn

TS:   name: string = "x";
来源：http://og.colortex.cn

Java: private String name;
来源：http://xu.shxzskj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cl.yuexingan06.cn

Ruby: @name = "x"
来源：http://rt.szxytkj.cn

C#:   public string Name { get; set; } = "x";
来源：http://av.nicolike.cn

[G04] 定义方法
来源：http://hg.newstarts.cn

Py:   def greet(self): return self.name
来源：http://bv.newstarts.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ys.lnxyls.cn

JS:   greet() { return this.name; }
来源：http://jv.bjjhwx.cn

TS:   greet(): string { return this.name; }
来源：http://xl.jianghongdianzi.cn

Java: String greet() { return name; }
来源：http://ms.521024.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://iz.nicolike.cn

Ruby: def greet; @name; end
来源：http://ff.nszjky.cn

C#:   public string Greet() => Name;
来源：http://tj.huanxung.cn

[G05] 继承
来源：http://zw.nszjky.cn

Py:   class Admin(User): pass
来源：http://do.nicolike.cn

PHP:  class Admin extends User {}
来源：http://hl.lnxyls.cn

JS:   class Admin extends User {}
来源：http://mg.shxzukj.cn

TS:   class Admin extends User {}
来源：http://gb.lnxyls.cn

Java: class Admin extends User {}
来源：http://ih.shtwfgs.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ca.newstarts.cn

Ruby: class Admin < User; end
来源：http://br.shxzukj.cn

C#:   class Admin : User {}
来源：http://kv.huixinmuqiang.cn

[G06] 重写方法
来源：http://ae.asd995.cn

Py:   def greet(self): return "admin"
来源：http://hw.jianghongdianzi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://nt.szxytkj.cn

JS:   greet() { return "admin"; }
来源：http://jy.shxzskj.cn


<!-- 参考信息 -->