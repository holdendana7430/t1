代发 wailian999

C#:   s.Replace("a", "b")
来源：http://jf.hnjuh.cn

[E07] 按分隔符拆分
来源：http://ra.shxzukj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yi.chemitech.net.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://sn.9csxet.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://tc.huixiangedu.cn

TS:   s.split(",")
来源：http://sh.colortex.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ar.wgjwhj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ve.colortex.cn

Ruby: s.split(",");  s.split
来源：http://ui.bookmarksfly.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://za.huixiangedu.cn

[E08] 数组按分隔符合并
来源：http://ia.nszjky.cn

Py:   ",".join(items)
来源：http://km.shxzukj.cn

PHP:  implode(",", $items);
来源：http://bc.huixinmuqiang.cn

JS:   items.join(",")
来源：http://rr.521024.cn

TS:   items.join(",")
来源：http://fy.huanxung.cn

Java: String.join(",", items)
来源：http://xs.chemitech.net.cn

Go:   strings.Join(items, ",")
来源：http://mb.chemitech.net.cn

Ruby: items.join(",")
来源：http://er.chemitech.net.cn

C#:   string.Join(",", items)
来源：http://de.bookmarksfly.cn

[E09] 去除所有空白字符
来源：http://zt.chemitech.net.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jl.shtwfgs.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xh.jctech888.com.cn

JS:   s.replace(/\s+/g, "")
来源：http://ft.hahajie.cn

TS:   s.replace(/\s+/g, "")
来源：http://fg.huixinmuqiang.cn

Java: s.replaceAll("\\s+", "")
来源：http://zq.wgjwhj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://pa.jianghongdianzi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://gk.panjiajie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xm.szsharing.cn

[E10] 左侧补零 / 定长填充
来源：http://nb.szxytkj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rs.yuntaijiaju.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cx.bookmarksfly.cn

JS:   "7".padStart(3, "0")
来源：http://qj.bookmarksfly.cn

TS:   "7".padStart(3, "0")
来源：http://ig.asd995.cn

Java: String.format("%03d", 7)
来源：http://vf.gzmigu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://fm.521024.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pi.nicolike.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nw.shxzskj.cn

[E11] 反转字符串
来源：http://yu.hnjuh.cn

Py:   s[::-1]
来源：http://jp.wgjwhj.cn

PHP:  strrev($s);
来源：http://tj.chemitech.net.cn

JS:   [...s].reverse().join("")
来源：http://ni.huanxung.cn

TS:   [...s].reverse().join("")
来源：http://wv.yuntaijiaju.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zz.nszjky.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ay.wgjwhj.cn

Ruby: s.reverse
来源：http://ay.gzmigu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://cp.gzmigu.cn

[E12] 统计某字符出现次数
来源：http://gy.huixiangedu.cn

Py:   s.count("a")
来源：http://af.hnjuh.cn

PHP:  substr_count($s, "a");
来源：http://hb.nicolike.cn

JS:   s.split("a").length - 1
来源：http://he.szsharing.cn

TS:   s.split("a").length - 1
来源：http://mw.lnxyls.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://si.haigaiapp.cn

Go:   strings.Count(s, "a")
来源：http://xm.huanxung.cn

Ruby: s.count("a")
来源：http://ex.shxzukj.cn

C#:   s.Count(c => c == 'a')
来源：http://jr.gzmigu.cn

[E13] 逐字符遍历
来源：http://ea.yuntaijiaju.cn

Py:   for ch in s: print(ch)
来源：http://jg.nszjky.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://uh.shtwfgs.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ri.nszjky.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wk.jianghongdianzi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vz.bjjhwx.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vz.jianghongdianzi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://fo.9csxet.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://sn.huixiangedu.cn

[E14] URL 编码与 Base64
来源：http://um.jctech888.com.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://aj.szxytkj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ts.bjjhwx.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cq.jianghongdianzi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mh.yuexingan06.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fm.huixiangedu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://uo.jctech888.com.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://aa.colortex.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bh.521024.cn

[E15] HTML 转义 / 反转义
来源：http://af.huanxung.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://vc.yuntaijiaju.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xs.hahajie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fx.colortex.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ol.huixinmuqiang.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hm.9csxet.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wb.521024.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tq.haigaiapp.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ks.9csxet.cn

[E16] 数字千分位
来源：http://xc.yuntaijiaju.cn

Py:   f"{1234567:,}"
来源：http://wk.yuexingan06.cn

PHP:  number_format(1234567);
来源：http://pu.haigaiapp.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mc.szsharing.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://hk.huixinmuqiang.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zh.nicolike.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lf.shxzskj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xc.shtwfgs.cn

C#:   1234567.ToString("N0")
来源：http://rb.nszjky.cn

[E17] 首字母大写
来源：http://gt.huixiangedu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vc.nicolike.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://yl.nicolike.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uz.bjjhwx.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tp.bjjhwx.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rb.chemitech.net.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ji.huixinmuqiang.cn

Ruby: s.capitalize
来源：http://ku.szsharing.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wd.newstarts.cn

[E18] 模板占位符替换
来源：http://ro.nicolike.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ql.bookmarksfly.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wq.jianghongdianzi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://tq.yuexingan06.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://uq.lnxyls.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ow.shxzskj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qj.lnxyls.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://sr.huixinmuqiang.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zd.chemitech.net.cn

[E19] 多行文本按行拆分
来源：http://xb.shxzskj.cn

Py:   s.splitlines()
来源：http://md.hahajie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xh.szsharing.cn

JS:   s.split(/\r?\n/)
来源：http://xe.521024.cn

TS:   s.split(/\r?\n/)
来源：http://fq.asd995.cn

Java: s.lines().toList()
来源：http://db.shxzukj.cn

Go:   strings.Split(s, "\n")
来源：http://il.huanxung.cn

Ruby: s.lines
来源：http://df.shxzukj.cn

C#:   s.Split('\n')
来源：http://fa.9csxet.cn

[E20] 判断字符串是否为空
来源：http://zm.huixinmuqiang.cn

Py:   if not s:
来源：http://jb.shtwfgs.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fw.huanxung.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mq.bjjhwx.cn

TS:   if (s === "") {}
来源：http://qc.shxzukj.cn

Java: if (s.isEmpty()) {}
来源：http://pe.muxihuayi.cn

Go:   if s == "" {}
来源：http://mu.jctech888.com.cn

Ruby: if s.empty?
来源：http://ut.bjjhwx.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vm.shxzskj.cn

[E21] 超长截断加省略号
来源：http://fu.9csxet.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zv.9csxet.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vy.bjjhwx.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hy.huanxung.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lr.huixinmuqiang.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://en.wgjwhj.cn

Go:   // 按 rune 判断长度后截断
来源：http://pk.huanxung.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ku.bjjhwx.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://oj.jctech888.com.cn

[E22] 字节长度与字符长度
来源：http://lg.521024.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pe.bjjhwx.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nw.gzmigu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pb.huanxung.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yt.szsharing.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zt.colortex.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://en.huixinmuqiang.cn

Ruby: s.bytesize;  s.length
来源：http://et.hahajie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ow.wgjwhj.cn

================================================================================
来源：http://gd.jianghongdianzi.cn

F. 文件与目录
来源：http://lf.lnxyls.cn

================================================================================
来源：http://bp.shtwfgs.cn

[F01] 读取整个文件
来源：http://sk.newstarts.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://sn.bjjhwx.cn

PHP:  file_get_contents("a.txt");
来源：http://gu.huixinmuqiang.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gt.9csxet.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hq.wgjwhj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ki.colortex.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wi.haigaiapp.cn

Ruby: File.read("a.txt")
来源：http://sv.yuexingan06.cn

C#:   File.ReadAllText("a.txt");
来源：http://pr.nszjky.cn

[F02] 逐行读取文件
来源：http://hw.huixinmuqiang.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fk.jctech888.com.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wb.chemitech.net.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jq.hahajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ti.hnjuh.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rv.yuntaijiaju.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bo.9csxet.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zt.gzmigu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pq.panjiajie.cn

[F03] 写入文件（覆盖）
来源：http://av.huixinmuqiang.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zv.huixinmuqiang.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://rl.shxzukj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nd.yuexingan06.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://np.yuexingan06.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fv.wgjwhj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wc.huixinmuqiang.cn

Ruby: File.write("a.txt", "hi")
来源：http://jy.shxzukj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dr.hahajie.cn

[F04] 追加写入文件
来源：http://im.huixiangedu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ky.shxzukj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tf.jianghongdianzi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://av.jianghongdianzi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://aq.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kz.huixiangedu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://so.huixinmuqiang.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qy.newstarts.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rx.shxzukj.cn

[F05] 判断文件或目录是否存在
来源：http://uz.9csxet.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ru.newstarts.cn

PHP:  file_exists("a.txt");
来源：http://mz.hnjuh.cn

JS:   fs.existsSync("a.txt")
来源：http://nw.haigaiapp.cn

TS:   fs.existsSync("a.txt")
来源：http://yq.bjjhwx.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://oh.9csxet.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ct.hahajie.cn

Ruby: File.exist?("a.txt")
来源：http://sm.chemitech.net.cn

C#:   File.Exists("a.txt")
来源：http://zy.szxytkj.cn

[F06] 删除文件
来源：http://cj.nszjky.cn

Py:   os.remove("a.txt")
来源：http://ta.bookmarksfly.cn

PHP:  unlink("a.txt");
来源：http://rw.yuexingan06.cn

JS:   fs.unlinkSync("a.txt")
来源：http://rd.panjiajie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ky.shxzskj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gg.shxzukj.cn

Go:   os.Remove("a.txt")
来源：http://fq.hahajie.cn

Ruby: File.delete("a.txt")
来源：http://mx.huixiangedu.cn

C#:   File.Delete("a.txt");
来源：http://wr.wgjwhj.cn

[F07] 创建目录（含多级）
来源：http://zg.jianghongdianzi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zi.jctech888.com.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cm.szxytkj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ao.haigaiapp.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fs.haigaiapp.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gr.shxzukj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ws.nszjky.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cw.lnxyls.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://or.wgjwhj.cn

[F08] 遍历目录
来源：http://qh.nicolike.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://uv.huanxung.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jo.521024.cn

JS:   fs.readdirSync("dir")
来源：http://od.jianghongdianzi.cn

TS:   fs.readdirSync("dir")
来源：http://lf.shxzukj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://if.nicolike.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://sa.haigaiapp.cn

Ruby: Dir.children("dir")
来源：http://pu.shtwfgs.cn

C#:   Directory.GetFiles("dir")
来源：http://ig.shtwfgs.cn

[F09] 获取文件大小
来源：http://tr.9csxet.cn

Py:   os.path.getsize("a.txt")
来源：http://bw.haigaiapp.cn

PHP:  filesize("a.txt");
来源：http://xs.szxytkj.cn

JS:   fs.statSync("a.txt").size
来源：http://hn.9csxet.cn

TS:   fs.statSync("a.txt").size
来源：http://ht.asd995.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zz.yuntaijiaju.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mk.asd995.cn

Ruby: File.size("a.txt")
来源：http://lg.muxihuayi.cn

C#:   new FileInfo("a.txt").Length
来源：http://pp.shtwfgs.cn

[F10] 取文件扩展名 / 文件名
来源：http://lu.shxzukj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nd.nicolike.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hh.jianghongdianzi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xk.newstarts.cn

TS:   path.extname("a.txt")
来源：http://hu.colortex.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ca.huanxung.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ro.nicolike.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nt.huixinmuqiang.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ce.yuexingan06.cn

[F11] 复制与移动文件
来源：http://ub.panjiajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cj.gzmigu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nc.yuntaijiaju.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ty.colortex.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://af.muxihuayi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://sg.shxzskj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ty.bjjhwx.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yp.chemitech.net.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xk.nicolike.cn

[F12] CSV 读写
来源：http://ue.gzmigu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rl.bookmarksfly.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pw.shxzukj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lu.huanxung.cn

TS:   // 同上
来源：http://wr.gzmigu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tg.bjjhwx.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ik.colortex.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dr.wgjwhj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://pi.shxzukj.cn

================================================================================
来源：http://mx.jctech888.com.cn

G. 面向对象
来源：http://vt.newstarts.cn

================================================================================
来源：http://cv.bookmarksfly.cn

[G01] 定义类
来源：http://mm.muxihuayi.cn

Py:   class User: pass
来源：http://cm.haigaiapp.cn

PHP:  class User {}
来源：http://cm.9csxet.cn

JS:   class User {}
来源：http://zi.bjjhwx.cn

TS:   class User { name: string = ""; }
来源：http://wo.shxzukj.cn

Java: class User {}
来源：http://zt.yuexingan06.cn

Go:   type User struct { Name string }
来源：http://km.bjjhwx.cn

Ruby: class User; end
来源：http://sj.huixinmuqiang.cn

C#:   class User {}
来源：http://sj.nicolike.cn

[G02] 构造函数
来源：http://ue.szsharing.cn

Py:   def __init__(self, name): self.name = name
来源：http://sq.gzmigu.cn

PHP:  public function __construct(public string $name) {}
来源：http://gl.shtwfgs.cn

JS:   constructor(name) { this.name = name; }
来源：http://yw.szsharing.cn

TS:   constructor(public name: string) {}
来源：http://lx.nszjky.cn

Java: User(String name) { this.name = name; }
来源：http://gu.huixinmuqiang.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gm.hahajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://rl.szsharing.cn

C#:   public User(string name) { Name = name; }
来源：http://fr.bjjhwx.cn

[G03] 实例属性
来源：http://ox.colortex.cn

Py:   self.name = "x"
来源：http://sb.szsharing.cn

PHP:  public string $name = "x";
来源：http://tk.wgjwhj.cn

JS:   this.name = "x";
来源：http://oy.huanxung.cn

TS:   name: string = "x";
来源：http://vx.huixinmuqiang.cn

Java: private String name;
来源：http://fa.bookmarksfly.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qo.haigaiapp.cn

Ruby: @name = "x"
来源：http://av.hahajie.cn

C#:   public string Name { get; set; } = "x";
来源：http://ce.gzmigu.cn

[G04] 定义方法
来源：http://bl.panjiajie.cn

Py:   def greet(self): return self.name
来源：http://dn.szxytkj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://er.bookmarksfly.cn

JS:   greet() { return this.name; }
来源：http://jv.panjiajie.cn

TS:   greet(): string { return this.name; }
来源：http://an.hahajie.cn

Java: String greet() { return name; }
来源：http://fg.shxzukj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://sm.asd995.cn

Ruby: def greet; @name; end
来源：http://ka.chemitech.net.cn

C#:   public string Greet() => Name;
来源：http://nn.szxytkj.cn

[G05] 继承
来源：http://mv.haigaiapp.cn

Py:   class Admin(User): pass
来源：http://tf.hahajie.cn

PHP:  class Admin extends User {}
来源：http://pn.jctech888.com.cn

JS:   class Admin extends User {}
来源：http://kb.huixinmuqiang.cn

TS:   class Admin extends User {}
来源：http://ky.yuntaijiaju.cn


<!-- 参考信息 -->