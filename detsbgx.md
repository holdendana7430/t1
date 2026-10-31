代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://cx.9csxet.cn

TS:   s.split(",")
来源：http://fk.panjiajie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://kg.jctech888.com.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jo.shxzskj.cn

Ruby: s.split(",");  s.split
来源：http://rx.shtwfgs.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ni.lnxyls.cn

[E08] 数组按分隔符合并
来源：http://sy.panjiajie.cn

Py:   ",".join(items)
来源：http://bw.bjjhwx.cn

PHP:  implode(",", $items);
来源：http://sy.shxzukj.cn

JS:   items.join(",")
来源：http://yy.haigaiapp.cn

TS:   items.join(",")
来源：http://vh.wgjwhj.cn

Java: String.join(",", items)
来源：http://ux.521024.cn

Go:   strings.Join(items, ",")
来源：http://ut.shtwfgs.cn

Ruby: items.join(",")
来源：http://fp.szxytkj.cn

C#:   string.Join(",", items)
来源：http://fd.huanxung.cn

[E09] 去除所有空白字符
来源：http://bt.huixiangedu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ww.nszjky.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yh.chemitech.net.cn

JS:   s.replace(/\s+/g, "")
来源：http://cn.huixiangedu.cn

TS:   s.replace(/\s+/g, "")
来源：http://od.bjjhwx.cn

Java: s.replaceAll("\\s+", "")
来源：http://rc.shxzskj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://iq.jianghongdianzi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ce.haigaiapp.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tc.szsharing.cn

[E10] 左侧补零 / 定长填充
来源：http://so.huanxung.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jz.hahajie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jg.hahajie.cn

JS:   "7".padStart(3, "0")
来源：http://xo.asd995.cn

TS:   "7".padStart(3, "0")
来源：http://ri.szsharing.cn

Java: String.format("%03d", 7)
来源：http://cn.nszjky.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://an.hnjuh.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rd.shtwfgs.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tq.szxytkj.cn

[E11] 反转字符串
来源：http://ew.yuntaijiaju.cn

Py:   s[::-1]
来源：http://ix.chemitech.net.cn

PHP:  strrev($s);
来源：http://wf.nicolike.cn

JS:   [...s].reverse().join("")
来源：http://ll.chemitech.net.cn

TS:   [...s].reverse().join("")
来源：http://lb.bjjhwx.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://pg.nicolike.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://tt.huanxung.cn

Ruby: s.reverse
来源：http://go.bookmarksfly.cn

C#:   new string(s.Reverse().ToArray())
来源：http://id.huixiangedu.cn

[E12] 统计某字符出现次数
来源：http://yh.bookmarksfly.cn

Py:   s.count("a")
来源：http://ne.lnxyls.cn

PHP:  substr_count($s, "a");
来源：http://uj.jianghongdianzi.cn

JS:   s.split("a").length - 1
来源：http://kp.hahajie.cn

TS:   s.split("a").length - 1
来源：http://uz.nicolike.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jg.haigaiapp.cn

Go:   strings.Count(s, "a")
来源：http://bb.jianghongdianzi.cn

Ruby: s.count("a")
来源：http://ve.gzmigu.cn

C#:   s.Count(c => c == 'a')
来源：http://jp.szxytkj.cn

[E13] 逐字符遍历
来源：http://le.lnxyls.cn

Py:   for ch in s: print(ch)
来源：http://bp.jctech888.com.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://la.chemitech.net.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://rs.huixinmuqiang.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://me.bjjhwx.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sa.newstarts.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pj.shtwfgs.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ls.panjiajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://st.bjjhwx.cn

[E14] URL 编码与 Base64
来源：http://fj.colortex.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mf.hahajie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://xz.nszjky.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://sy.hahajie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bj.bookmarksfly.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ly.wgjwhj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rz.panjiajie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qd.haigaiapp.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ix.haigaiapp.cn

[E15] HTML 转义 / 反转义
来源：http://hv.huixinmuqiang.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://pz.jianghongdianzi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wh.hahajie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bn.nicolike.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://fj.lnxyls.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ya.colortex.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pi.bjjhwx.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tv.huixiangedu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rv.shxzskj.cn

[E16] 数字千分位
来源：http://we.szxytkj.cn

Py:   f"{1234567:,}"
来源：http://kz.colortex.cn

PHP:  number_format(1234567);
来源：http://ht.hahajie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://wj.szsharing.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ql.shtwfgs.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zv.shxzskj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rk.hahajie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nn.szxytkj.cn

C#:   1234567.ToString("N0")
来源：http://af.colortex.cn

[E17] 首字母大写
来源：http://ks.szxytkj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://iv.shxzskj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://be.chemitech.net.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nv.bjjhwx.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://if.nszjky.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bx.szxytkj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sh.panjiajie.cn

Ruby: s.capitalize
来源：http://sw.jianghongdianzi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gy.hahajie.cn

[E18] 模板占位符替换
来源：http://kn.521024.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bo.jctech888.com.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pe.newstarts.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://lj.jctech888.com.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://fo.nszjky.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hl.panjiajie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xe.jctech888.com.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jf.jctech888.com.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hp.colortex.cn

[E19] 多行文本按行拆分
来源：http://mf.bookmarksfly.cn

Py:   s.splitlines()
来源：http://ek.jctech888.com.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ft.szsharing.cn

JS:   s.split(/\r?\n/)
来源：http://sg.jctech888.com.cn

TS:   s.split(/\r?\n/)
来源：http://id.9csxet.cn

Java: s.lines().toList()
来源：http://tz.asd995.cn

Go:   strings.Split(s, "\n")
来源：http://al.bjjhwx.cn

Ruby: s.lines
来源：http://ym.colortex.cn

C#:   s.Split('\n')
来源：http://gp.yuntaijiaju.cn

[E20] 判断字符串是否为空
来源：http://gt.yuntaijiaju.cn

Py:   if not s:
来源：http://xf.huixinmuqiang.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jv.asd995.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vr.szxytkj.cn

TS:   if (s === "") {}
来源：http://mq.huixiangedu.cn

Java: if (s.isEmpty()) {}
来源：http://sp.bookmarksfly.cn

Go:   if s == "" {}
来源：http://zw.asd995.cn

Ruby: if s.empty?
来源：http://ak.bookmarksfly.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ps.panjiajie.cn

[E21] 超长截断加省略号
来源：http://ui.huanxung.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wj.hahajie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ry.huixiangedu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nq.gzmigu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sl.nszjky.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vy.chemitech.net.cn

Go:   // 按 rune 判断长度后截断
来源：http://uq.muxihuayi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zq.huanxung.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://da.huanxung.cn

[E22] 字节长度与字符长度
来源：http://dl.colortex.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lm.yuntaijiaju.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yf.nicolike.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hj.asd995.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bm.huixinmuqiang.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gh.bjjhwx.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bu.lnxyls.cn

Ruby: s.bytesize;  s.length
来源：http://jp.shxzukj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kz.szsharing.cn

================================================================================
来源：http://sg.newstarts.cn

F. 文件与目录
来源：http://xk.shtwfgs.cn

================================================================================
来源：http://ub.huanxung.cn

[F01] 读取整个文件
来源：http://cy.muxihuayi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kd.yuexingan06.cn

PHP:  file_get_contents("a.txt");
来源：http://gx.gzmigu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wb.haigaiapp.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sp.szsharing.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fp.haigaiapp.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://am.newstarts.cn

Ruby: File.read("a.txt")
来源：http://re.hnjuh.cn

C#:   File.ReadAllText("a.txt");
来源：http://wn.haigaiapp.cn

[F02] 逐行读取文件
来源：http://ph.shxzukj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cr.jctech888.com.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nq.9csxet.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ai.521024.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://id.huixiangedu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fr.bookmarksfly.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mq.yuntaijiaju.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wn.gzmigu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sy.hahajie.cn

[F03] 写入文件（覆盖）
来源：http://ct.jianghongdianzi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gt.9csxet.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://av.huixinmuqiang.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gh.chemitech.net.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://od.nszjky.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ex.9csxet.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ao.yuntaijiaju.cn

Ruby: File.write("a.txt", "hi")
来源：http://ai.huixiangedu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zn.szxytkj.cn

[F04] 追加写入文件
来源：http://le.hnjuh.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ba.jianghongdianzi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ht.asd995.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mp.shxzukj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nt.bookmarksfly.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bc.huixiangedu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://me.szxytkj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://em.bjjhwx.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cs.szsharing.cn

[F05] 判断文件或目录是否存在
来源：http://xi.521024.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pr.shxzukj.cn

PHP:  file_exists("a.txt");
来源：http://ut.9csxet.cn

JS:   fs.existsSync("a.txt")
来源：http://vj.lnxyls.cn

TS:   fs.existsSync("a.txt")
来源：http://lc.gzmigu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://na.huanxung.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://iw.huanxung.cn

Ruby: File.exist?("a.txt")
来源：http://qf.szxytkj.cn

C#:   File.Exists("a.txt")
来源：http://qf.jianghongdianzi.cn

[F06] 删除文件
来源：http://ui.huixinmuqiang.cn

Py:   os.remove("a.txt")
来源：http://hx.huixiangedu.cn

PHP:  unlink("a.txt");
来源：http://ld.hnjuh.cn

JS:   fs.unlinkSync("a.txt")
来源：http://sx.gzmigu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://zh.bjjhwx.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qe.szxytkj.cn

Go:   os.Remove("a.txt")
来源：http://ec.panjiajie.cn

Ruby: File.delete("a.txt")
来源：http://qu.newstarts.cn

C#:   File.Delete("a.txt");
来源：http://ga.huixinmuqiang.cn

[F07] 创建目录（含多级）
来源：http://vm.yuexingan06.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qn.lnxyls.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ce.jctech888.com.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dt.521024.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tz.jctech888.com.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://da.nszjky.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://du.szxytkj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://us.newstarts.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://iv.gzmigu.cn

[F08] 遍历目录
来源：http://se.asd995.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://hi.521024.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cb.lnxyls.cn

JS:   fs.readdirSync("dir")
来源：http://bp.huanxung.cn

TS:   fs.readdirSync("dir")
来源：http://rq.9csxet.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rt.colortex.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://iq.bookmarksfly.cn

Ruby: Dir.children("dir")
来源：http://xd.szxytkj.cn

C#:   Directory.GetFiles("dir")
来源：http://ua.panjiajie.cn

[F09] 获取文件大小
来源：http://jg.shtwfgs.cn

Py:   os.path.getsize("a.txt")
来源：http://vd.gzmigu.cn

PHP:  filesize("a.txt");
来源：http://ta.chemitech.net.cn

JS:   fs.statSync("a.txt").size
来源：http://vs.shxzskj.cn

TS:   fs.statSync("a.txt").size
来源：http://dc.newstarts.cn

Java: Files.size(Path.of("a.txt"))
来源：http://za.huixiangedu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cq.gzmigu.cn

Ruby: File.size("a.txt")
来源：http://bk.lnxyls.cn

C#:   new FileInfo("a.txt").Length
来源：http://ud.huixinmuqiang.cn

[F10] 取文件扩展名 / 文件名
来源：http://hi.huixiangedu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wc.newstarts.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qy.panjiajie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gz.shtwfgs.cn

TS:   path.extname("a.txt")
来源：http://ay.yuntaijiaju.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dv.huanxung.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mi.panjiajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ya.521024.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ne.newstarts.cn

[F11] 复制与移动文件
来源：http://xv.9csxet.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ia.9csxet.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ao.szxytkj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mr.huanxung.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hb.newstarts.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://af.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vz.yuexingan06.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ap.jctech888.com.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zy.hnjuh.cn

[F12] CSV 读写
来源：http://tx.szxytkj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hn.nicolike.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://af.bjjhwx.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xw.yuntaijiaju.cn

TS:   // 同上
来源：http://yv.9csxet.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://db.shtwfgs.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zp.521024.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tu.nszjky.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qq.hahajie.cn

================================================================================
来源：http://ma.huanxung.cn

G. 面向对象
来源：http://nj.lnxyls.cn

================================================================================
来源：http://le.gzmigu.cn

[G01] 定义类
来源：http://ko.yuntaijiaju.cn

Py:   class User: pass
来源：http://wg.asd995.cn

PHP:  class User {}
来源：http://qf.jianghongdianzi.cn

JS:   class User {}
来源：http://rr.521024.cn

TS:   class User { name: string = ""; }
来源：http://wo.szxytkj.cn

Java: class User {}
来源：http://fp.hnjuh.cn

Go:   type User struct { Name string }
来源：http://pq.yuntaijiaju.cn

Ruby: class User; end
来源：http://xk.bookmarksfly.cn

C#:   class User {}
来源：http://vj.chemitech.net.cn

[G02] 构造函数
来源：http://mk.shtwfgs.cn

Py:   def __init__(self, name): self.name = name
来源：http://ce.bjjhwx.cn

PHP:  public function __construct(public string $name) {}
来源：http://je.asd995.cn

JS:   constructor(name) { this.name = name; }
来源：http://oe.lnxyls.cn

TS:   constructor(public name: string) {}
来源：http://vk.jianghongdianzi.cn

Java: User(String name) { this.name = name; }
来源：http://nw.asd995.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gi.yuexingan06.cn

Ruby: def initialize(name); @name = name; end
来源：http://gg.yuexingan06.cn

C#:   public User(string name) { Name = name; }
来源：http://zp.huixiangedu.cn

[G03] 实例属性
来源：http://vb.panjiajie.cn

Py:   self.name = "x"
来源：http://le.huixiangedu.cn

PHP:  public string $name = "x";
来源：http://cg.huanxung.cn

JS:   this.name = "x";
来源：http://mm.huixinmuqiang.cn

TS:   name: string = "x";
来源：http://vx.9csxet.cn

Java: private String name;
来源：http://ih.wgjwhj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://am.wgjwhj.cn

Ruby: @name = "x"
来源：http://bl.colortex.cn

C#:   public string Name { get; set; } = "x";
来源：http://aq.jctech888.com.cn

[G04] 定义方法
来源：http://hx.yuexingan06.cn

Py:   def greet(self): return self.name
来源：http://qa.521024.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://vg.szxytkj.cn

JS:   greet() { return this.name; }
来源：http://vy.shtwfgs.cn

TS:   greet(): string { return this.name; }
来源：http://vs.colortex.cn

Java: String greet() { return name; }
来源：http://to.wgjwhj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://pf.nicolike.cn

Ruby: def greet; @name; end
来源：http://ly.9csxet.cn

C#:   public string Greet() => Name;
来源：http://fs.shtwfgs.cn

[G05] 继承
来源：http://in.szxytkj.cn

Py:   class Admin(User): pass
来源：http://sd.huixinmuqiang.cn

PHP:  class Admin extends User {}
来源：http://ul.asd995.cn

JS:   class Admin extends User {}
来源：http://rr.huixiangedu.cn

TS:   class Admin extends User {}
来源：http://tt.huixinmuqiang.cn

Java: class Admin extends User {}
来源：http://bx.jctech888.com.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xn.wgjwhj.cn

Ruby: class Admin < User; end
来源：http://wb.huixinmuqiang.cn

C#:   class Admin : User {}
来源：http://tu.wgjwhj.cn


<!-- 参考信息 -->