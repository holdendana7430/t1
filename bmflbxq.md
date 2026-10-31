代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://ub.yuntaijiaju.cn

TS:   s.split(",")
来源：http://vs.wgjwhj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://sn.9csxet.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://td.asd995.cn

Ruby: s.split(",");  s.split
来源：http://ui.jianghongdianzi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://if.wgjwhj.cn

[E08] 数组按分隔符合并
来源：http://su.jctech888.com.cn

Py:   ",".join(items)
来源：http://oe.szxytkj.cn

PHP:  implode(",", $items);
来源：http://du.szsharing.cn

JS:   items.join(",")
来源：http://hr.panjiajie.cn

TS:   items.join(",")
来源：http://uh.yuntaijiaju.cn

Java: String.join(",", items)
来源：http://vw.wgjwhj.cn

Go:   strings.Join(items, ",")
来源：http://vu.colortex.cn

Ruby: items.join(",")
来源：http://pt.newstarts.cn

C#:   string.Join(",", items)
来源：http://px.shxzukj.cn

[E09] 去除所有空白字符
来源：http://tu.lnxyls.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kx.jctech888.com.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://th.hnjuh.cn

JS:   s.replace(/\s+/g, "")
来源：http://wc.bookmarksfly.cn

TS:   s.replace(/\s+/g, "")
来源：http://zb.shxzukj.cn

Java: s.replaceAll("\\s+", "")
来源：http://di.gzmigu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://yy.wgjwhj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://oq.nicolike.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nh.gzmigu.cn

[E10] 左侧补零 / 定长填充
来源：http://di.szsharing.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lz.yuexingan06.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dw.nicolike.cn

JS:   "7".padStart(3, "0")
来源：http://mr.lnxyls.cn

TS:   "7".padStart(3, "0")
来源：http://et.asd995.cn

Java: String.format("%03d", 7)
来源：http://bj.haigaiapp.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ed.shtwfgs.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sk.nszjky.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cz.szxytkj.cn

[E11] 反转字符串
来源：http://si.jianghongdianzi.cn

Py:   s[::-1]
来源：http://if.nicolike.cn

PHP:  strrev($s);
来源：http://na.haigaiapp.cn

JS:   [...s].reverse().join("")
来源：http://pf.shxzskj.cn

TS:   [...s].reverse().join("")
来源：http://sh.muxihuayi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ma.gzmigu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://vk.szsharing.cn

Ruby: s.reverse
来源：http://pv.hnjuh.cn

C#:   new string(s.Reverse().ToArray())
来源：http://oi.shxzukj.cn

[E12] 统计某字符出现次数
来源：http://qv.chemitech.net.cn

Py:   s.count("a")
来源：http://ew.bookmarksfly.cn

PHP:  substr_count($s, "a");
来源：http://ly.chemitech.net.cn

JS:   s.split("a").length - 1
来源：http://ht.gzmigu.cn

TS:   s.split("a").length - 1
来源：http://wc.huixinmuqiang.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zt.bjjhwx.cn

Go:   strings.Count(s, "a")
来源：http://ew.huixiangedu.cn

Ruby: s.count("a")
来源：http://cf.bookmarksfly.cn

C#:   s.Count(c => c == 'a')
来源：http://by.chemitech.net.cn

[E13] 逐字符遍历
来源：http://fo.nszjky.cn

Py:   for ch in s: print(ch)
来源：http://iy.szsharing.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vs.hnjuh.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://mv.gzmigu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://hx.newstarts.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://er.shxzskj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ma.huanxung.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://jt.jianghongdianzi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://oy.panjiajie.cn

[E14] URL 编码与 Base64
来源：http://mq.jctech888.com.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zv.muxihuayi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bp.nicolike.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rw.shtwfgs.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ju.bookmarksfly.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lq.nicolike.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://po.bookmarksfly.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yf.shxzukj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://oh.huixiangedu.cn

[E15] HTML 转义 / 反转义
来源：http://gx.chemitech.net.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xn.huixiangedu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bm.nicolike.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bw.521024.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://zi.yuexingan06.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xf.nszjky.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qx.yuexingan06.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yw.asd995.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ze.shxzukj.cn

[E16] 数字千分位
来源：http://bi.newstarts.cn

Py:   f"{1234567:,}"
来源：http://yj.hahajie.cn

PHP:  number_format(1234567);
来源：http://ca.szxytkj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mj.huanxung.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://tw.panjiajie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sy.gzmigu.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pm.asd995.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://sy.jianghongdianzi.cn

C#:   1234567.ToString("N0")
来源：http://cc.yuntaijiaju.cn

[E17] 首字母大写
来源：http://ti.hahajie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fc.hahajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://lj.szxytkj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zb.yuntaijiaju.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ed.haigaiapp.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://go.jianghongdianzi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qq.shxzskj.cn

Ruby: s.capitalize
来源：http://pf.asd995.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xq.shxzskj.cn

[E18] 模板占位符替换
来源：http://iz.hahajie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tf.panjiajie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cg.hnjuh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://wk.gzmigu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://yb.yuntaijiaju.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nh.huixinmuqiang.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://po.haigaiapp.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dd.huixinmuqiang.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ho.newstarts.cn

[E19] 多行文本按行拆分
来源：http://jw.shtwfgs.cn

Py:   s.splitlines()
来源：http://ct.bjjhwx.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vr.hahajie.cn

JS:   s.split(/\r?\n/)
来源：http://ly.jianghongdianzi.cn

TS:   s.split(/\r?\n/)
来源：http://kg.huixinmuqiang.cn

Java: s.lines().toList()
来源：http://hx.szsharing.cn

Go:   strings.Split(s, "\n")
来源：http://du.hnjuh.cn

Ruby: s.lines
来源：http://dn.bjjhwx.cn

C#:   s.Split('\n')
来源：http://og.muxihuayi.cn

[E20] 判断字符串是否为空
来源：http://hk.hahajie.cn

Py:   if not s:
来源：http://wc.huanxung.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://us.chemitech.net.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cf.jianghongdianzi.cn

TS:   if (s === "") {}
来源：http://wk.huanxung.cn

Java: if (s.isEmpty()) {}
来源：http://kg.gzmigu.cn

Go:   if s == "" {}
来源：http://fx.colortex.cn

Ruby: if s.empty?
来源：http://xr.szsharing.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pn.nicolike.cn

[E21] 超长截断加省略号
来源：http://su.asd995.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ew.shxzskj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://we.nicolike.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yl.bookmarksfly.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xm.jctech888.com.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jt.bookmarksfly.cn

Go:   // 按 rune 判断长度后截断
来源：http://xg.szsharing.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dg.huixinmuqiang.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nj.panjiajie.cn

[E22] 字节长度与字符长度
来源：http://ft.muxihuayi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jb.521024.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rl.haigaiapp.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lh.yuexingan06.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mq.lnxyls.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://um.nszjky.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xx.jctech888.com.cn

Ruby: s.bytesize;  s.length
来源：http://mb.haigaiapp.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bx.bjjhwx.cn

================================================================================
来源：http://yg.hahajie.cn

F. 文件与目录
来源：http://im.lnxyls.cn

================================================================================
来源：http://hx.colortex.cn

[F01] 读取整个文件
来源：http://mk.nszjky.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tg.hnjuh.cn

PHP:  file_get_contents("a.txt");
来源：http://gd.szsharing.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rn.haigaiapp.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://om.bjjhwx.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hr.huixiangedu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wy.shtwfgs.cn

Ruby: File.read("a.txt")
来源：http://nu.shxzskj.cn

C#:   File.ReadAllText("a.txt");
来源：http://qs.szxytkj.cn

[F02] 逐行读取文件
来源：http://zj.szsharing.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tq.haigaiapp.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pz.panjiajie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rb.newstarts.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oc.wgjwhj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vd.shxzskj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cp.hahajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pq.asd995.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bu.bookmarksfly.cn

[F03] 写入文件（覆盖）
来源：http://of.huixiangedu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wj.bjjhwx.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ts.newstarts.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wt.panjiajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hl.szsharing.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rm.shtwfgs.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hg.9csxet.cn

Ruby: File.write("a.txt", "hi")
来源：http://ln.nicolike.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bz.panjiajie.cn

[F04] 追加写入文件
来源：http://si.lnxyls.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ps.huixiangedu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://sa.asd995.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cd.521024.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gy.szxytkj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tj.hnjuh.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ma.szxytkj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hi.colortex.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qr.nszjky.cn

[F05] 判断文件或目录是否存在
来源：http://gc.shxzukj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://sv.asd995.cn

PHP:  file_exists("a.txt");
来源：http://jf.9csxet.cn

JS:   fs.existsSync("a.txt")
来源：http://yc.newstarts.cn

TS:   fs.existsSync("a.txt")
来源：http://vn.yuntaijiaju.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://lx.huanxung.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://uc.shxzukj.cn

Ruby: File.exist?("a.txt")
来源：http://gy.shxzskj.cn

C#:   File.Exists("a.txt")
来源：http://es.shxzskj.cn

[F06] 删除文件
来源：http://ep.521024.cn

Py:   os.remove("a.txt")
来源：http://lb.muxihuayi.cn

PHP:  unlink("a.txt");
来源：http://ug.huixinmuqiang.cn

JS:   fs.unlinkSync("a.txt")
来源：http://za.bjjhwx.cn

TS:   fs.unlinkSync("a.txt")
来源：http://qi.9csxet.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fg.hnjuh.cn

Go:   os.Remove("a.txt")
来源：http://kq.muxihuayi.cn

Ruby: File.delete("a.txt")
来源：http://ha.newstarts.cn

C#:   File.Delete("a.txt");
来源：http://jk.nszjky.cn

[F07] 创建目录（含多级）
来源：http://ww.wgjwhj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://av.chemitech.net.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wl.shtwfgs.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zw.huanxung.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://du.yuntaijiaju.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vq.bookmarksfly.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ur.haigaiapp.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ah.panjiajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bz.szsharing.cn

[F08] 遍历目录
来源：http://sv.lnxyls.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://mr.wgjwhj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sp.muxihuayi.cn

JS:   fs.readdirSync("dir")
来源：http://ml.shxzukj.cn

TS:   fs.readdirSync("dir")
来源：http://qy.shtwfgs.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hj.yuexingan06.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://na.bjjhwx.cn

Ruby: Dir.children("dir")
来源：http://if.lnxyls.cn

C#:   Directory.GetFiles("dir")
来源：http://hu.wgjwhj.cn

[F09] 获取文件大小
来源：http://oj.nszjky.cn

Py:   os.path.getsize("a.txt")
来源：http://rv.lnxyls.cn

PHP:  filesize("a.txt");
来源：http://hv.panjiajie.cn

JS:   fs.statSync("a.txt").size
来源：http://ua.bjjhwx.cn

TS:   fs.statSync("a.txt").size
来源：http://am.yuexingan06.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mc.huanxung.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pm.yuntaijiaju.cn

Ruby: File.size("a.txt")
来源：http://xu.shxzskj.cn

C#:   new FileInfo("a.txt").Length
来源：http://qv.gzmigu.cn

[F10] 取文件扩展名 / 文件名
来源：http://sr.jianghongdianzi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pb.nszjky.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zn.haigaiapp.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jw.newstarts.cn

TS:   path.extname("a.txt")
来源：http://co.panjiajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://np.bjjhwx.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ow.shxzukj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://da.huixinmuqiang.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jo.nicolike.cn

[F11] 复制与移动文件
来源：http://ht.jctech888.com.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://iw.hnjuh.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jg.newstarts.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tk.9csxet.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ru.jctech888.com.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ss.yuexingan06.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tn.521024.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://aj.nicolike.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lf.panjiajie.cn

[F12] CSV 读写
来源：http://ud.nicolike.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.521024.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ij.shtwfgs.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ui.haigaiapp.cn

TS:   // 同上
来源：http://wm.panjiajie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://oe.bookmarksfly.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fz.szsharing.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nr.521024.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://rf.panjiajie.cn

================================================================================
来源：http://lk.chemitech.net.cn

G. 面向对象
来源：http://iz.haigaiapp.cn

================================================================================
来源：http://od.huixiangedu.cn

[G01] 定义类
来源：http://dh.nicolike.cn

Py:   class User: pass
来源：http://bc.szxytkj.cn

PHP:  class User {}
来源：http://yx.szsharing.cn

JS:   class User {}
来源：http://mh.yuntaijiaju.cn

TS:   class User { name: string = ""; }
来源：http://bi.haigaiapp.cn

Java: class User {}
来源：http://pc.hnjuh.cn

Go:   type User struct { Name string }
来源：http://jt.nicolike.cn

Ruby: class User; end
来源：http://ck.muxihuayi.cn

C#:   class User {}
来源：http://cr.shxzskj.cn

[G02] 构造函数
来源：http://xs.szsharing.cn

Py:   def __init__(self, name): self.name = name
来源：http://kz.bookmarksfly.cn

PHP:  public function __construct(public string $name) {}
来源：http://sr.asd995.cn

JS:   constructor(name) { this.name = name; }
来源：http://rn.hahajie.cn

TS:   constructor(public name: string) {}
来源：http://fm.nszjky.cn

Java: User(String name) { this.name = name; }
来源：http://yw.521024.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://av.shxzskj.cn

Ruby: def initialize(name); @name = name; end
来源：http://hr.jianghongdianzi.cn

C#:   public User(string name) { Name = name; }
来源：http://db.hahajie.cn

[G03] 实例属性
来源：http://eo.gzmigu.cn

Py:   self.name = "x"
来源：http://ii.shxzskj.cn

PHP:  public string $name = "x";
来源：http://ct.szxytkj.cn

JS:   this.name = "x";
来源：http://ll.nicolike.cn

TS:   name: string = "x";
来源：http://hh.521024.cn

Java: private String name;
来源：http://lr.521024.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ra.bookmarksfly.cn

Ruby: @name = "x"
来源：http://iw.lnxyls.cn

C#:   public string Name { get; set; } = "x";
来源：http://ij.nszjky.cn

[G04] 定义方法
来源：http://pi.huixiangedu.cn

Py:   def greet(self): return self.name
来源：http://cq.chemitech.net.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ca.lnxyls.cn

JS:   greet() { return this.name; }
来源：http://at.nicolike.cn

TS:   greet(): string { return this.name; }
来源：http://fi.yuexingan06.cn

Java: String greet() { return name; }
来源：http://vg.huixinmuqiang.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://jw.jianghongdianzi.cn

Ruby: def greet; @name; end
来源：http://wu.jctech888.com.cn

C#:   public string Greet() => Name;
来源：http://pf.newstarts.cn

[G05] 继承
来源：http://gx.jianghongdianzi.cn

Py:   class Admin(User): pass
来源：http://np.shtwfgs.cn

PHP:  class Admin extends User {}
来源：http://dh.huixiangedu.cn

JS:   class Admin extends User {}
来源：http://ze.shtwfgs.cn

TS:   class Admin extends User {}
来源：http://rf.jctech888.com.cn

Java: class Admin extends User {}
来源：http://tc.huanxung.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ug.wgjwhj.cn

Ruby: class Admin < User; end
来源：http://kr.lnxyls.cn

C#:   class Admin : User {}
来源：http://wg.haigaiapp.cn


<!-- 参考信息 -->