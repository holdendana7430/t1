代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://hg.hahajie.cn

TS:   s.split(",")
来源：http://wt.hahajie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://pm.nicolike.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dk.yuntaijiaju.cn

Ruby: s.split(",");  s.split
来源：http://xo.huixinmuqiang.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wt.szsharing.cn

[E08] 数组按分隔符合并
来源：http://vz.yuntaijiaju.cn

Py:   ",".join(items)
来源：http://jb.bookmarksfly.cn

PHP:  implode(",", $items);
来源：http://qj.521024.cn

JS:   items.join(",")
来源：http://nk.chemitech.net.cn

TS:   items.join(",")
来源：http://af.yuexingan06.cn

Java: String.join(",", items)
来源：http://av.9csxet.cn

Go:   strings.Join(items, ",")
来源：http://cy.lnxyls.cn

Ruby: items.join(",")
来源：http://fz.jianghongdianzi.cn

C#:   string.Join(",", items)
来源：http://ma.bjjhwx.cn

[E09] 去除所有空白字符
来源：http://xm.yuntaijiaju.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fc.nszjky.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://di.hahajie.cn

JS:   s.replace(/\s+/g, "")
来源：http://bg.haigaiapp.cn

TS:   s.replace(/\s+/g, "")
来源：http://ul.szsharing.cn

Java: s.replaceAll("\\s+", "")
来源：http://ji.yuexingan06.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ip.521024.cn

Ruby: s.gsub(/\s+/, "")
来源：http://yn.bjjhwx.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xk.nszjky.cn

[E10] 左侧补零 / 定长填充
来源：http://zr.newstarts.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ag.jianghongdianzi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hc.nszjky.cn

JS:   "7".padStart(3, "0")
来源：http://qq.shtwfgs.cn

TS:   "7".padStart(3, "0")
来源：http://kg.huixiangedu.cn

Java: String.format("%03d", 7)
来源：http://oa.bookmarksfly.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://hr.gzmigu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gx.shxzskj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bp.wgjwhj.cn

[E11] 反转字符串
来源：http://jd.huanxung.cn

Py:   s[::-1]
来源：http://sf.nszjky.cn

PHP:  strrev($s);
来源：http://tt.jctech888.com.cn

JS:   [...s].reverse().join("")
来源：http://gi.bookmarksfly.cn

TS:   [...s].reverse().join("")
来源：http://bx.szsharing.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://mr.huanxung.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zl.chemitech.net.cn

Ruby: s.reverse
来源：http://aw.jianghongdianzi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ow.colortex.cn

[E12] 统计某字符出现次数
来源：http://fk.shxzukj.cn

Py:   s.count("a")
来源：http://os.9csxet.cn

PHP:  substr_count($s, "a");
来源：http://wc.lnxyls.cn

JS:   s.split("a").length - 1
来源：http://zt.haigaiapp.cn

TS:   s.split("a").length - 1
来源：http://in.shxzskj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://is.wgjwhj.cn

Go:   strings.Count(s, "a")
来源：http://zi.shxzskj.cn

Ruby: s.count("a")
来源：http://gl.lnxyls.cn

C#:   s.Count(c => c == 'a')
来源：http://zk.wgjwhj.cn

[E13] 逐字符遍历
来源：http://bi.nicolike.cn

Py:   for ch in s: print(ch)
来源：http://ay.muxihuayi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gb.szxytkj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://jl.nszjky.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wr.szxytkj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wm.shtwfgs.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hl.wgjwhj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://nd.muxihuayi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://by.huixinmuqiang.cn

[E14] URL 编码与 Base64
来源：http://ik.gzmigu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qc.szsharing.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://nf.huixinmuqiang.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wd.asd995.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hm.bookmarksfly.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yi.jctech888.com.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bf.nszjky.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zp.shxzukj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tv.yuexingan06.cn

[E15] HTML 转义 / 反转义
来源：http://eh.shxzukj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://nb.jctech888.com.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cn.wgjwhj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bz.newstarts.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ea.haigaiapp.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lt.bjjhwx.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hb.shxzukj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://th.hahajie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.yuntaijiaju.cn

[E16] 数字千分位
来源：http://is.haigaiapp.cn

Py:   f"{1234567:,}"
来源：http://bh.wgjwhj.cn

PHP:  number_format(1234567);
来源：http://yc.shtwfgs.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://hf.bookmarksfly.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ua.hnjuh.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vz.shtwfgs.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pw.bookmarksfly.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ug.hnjuh.cn

C#:   1234567.ToString("N0")
来源：http://pc.panjiajie.cn

[E17] 首字母大写
来源：http://tk.shxzukj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ve.lnxyls.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://wr.chemitech.net.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ij.huixinmuqiang.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ju.nicolike.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dh.wgjwhj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://za.jctech888.com.cn

Ruby: s.capitalize
来源：http://ud.9csxet.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://df.colortex.cn

[E18] 模板占位符替换
来源：http://kk.newstarts.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://or.yuexingan06.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://aq.huanxung.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ev.chemitech.net.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://si.bookmarksfly.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zz.szsharing.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fa.yuexingan06.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://oj.jctech888.com.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mv.9csxet.cn

[E19] 多行文本按行拆分
来源：http://hh.bookmarksfly.cn

Py:   s.splitlines()
来源：http://hz.szsharing.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fg.colortex.cn

JS:   s.split(/\r?\n/)
来源：http://em.hahajie.cn

TS:   s.split(/\r?\n/)
来源：http://ol.jctech888.com.cn

Java: s.lines().toList()
来源：http://nc.chemitech.net.cn

Go:   strings.Split(s, "\n")
来源：http://dn.bookmarksfly.cn

Ruby: s.lines
来源：http://ik.jianghongdianzi.cn

C#:   s.Split('\n')
来源：http://ae.nszjky.cn

[E20] 判断字符串是否为空
来源：http://kg.newstarts.cn

Py:   if not s:
来源：http://zg.nicolike.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://az.yuntaijiaju.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cy.haigaiapp.cn

TS:   if (s === "") {}
来源：http://il.nicolike.cn

Java: if (s.isEmpty()) {}
来源：http://ng.bookmarksfly.cn

Go:   if s == "" {}
来源：http://kq.gzmigu.cn

Ruby: if s.empty?
来源：http://do.jctech888.com.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dw.colortex.cn

[E21] 超长截断加省略号
来源：http://le.wgjwhj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lt.shxzukj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xc.chemitech.net.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tr.szsharing.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tc.haigaiapp.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rg.szsharing.cn

Go:   // 按 rune 判断长度后截断
来源：http://my.shxzukj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tp.huixiangedu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vp.huixiangedu.cn

[E22] 字节长度与字符长度
来源：http://bn.hahajie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ve.haigaiapp.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dy.szxytkj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://eo.hnjuh.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wn.hahajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pj.shxzukj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qi.nicolike.cn

Ruby: s.bytesize;  s.length
来源：http://vq.shtwfgs.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ap.yuexingan06.cn

================================================================================
来源：http://et.haigaiapp.cn

F. 文件与目录
来源：http://ml.wgjwhj.cn

================================================================================
来源：http://hx.shxzskj.cn

[F01] 读取整个文件
来源：http://rj.hahajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fb.shxzukj.cn

PHP:  file_get_contents("a.txt");
来源：http://fl.521024.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sk.huanxung.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ux.huixiangedu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ss.yuntaijiaju.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sf.yuntaijiaju.cn

Ruby: File.read("a.txt")
来源：http://hn.huixinmuqiang.cn

C#:   File.ReadAllText("a.txt");
来源：http://si.jianghongdianzi.cn

[F02] 逐行读取文件
来源：http://qk.szxytkj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vg.yuntaijiaju.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mi.hahajie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hf.hnjuh.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zz.bjjhwx.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lr.yuntaijiaju.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ea.huixinmuqiang.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gy.shxzukj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://if.lnxyls.cn

[F03] 写入文件（覆盖）
来源：http://pk.wgjwhj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://br.yuexingan06.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://eo.huanxung.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gb.panjiajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ys.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gh.jianghongdianzi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fw.nicolike.cn

Ruby: File.write("a.txt", "hi")
来源：http://qa.shtwfgs.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kk.yuexingan06.cn

[F04] 追加写入文件
来源：http://vk.yuntaijiaju.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bb.9csxet.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cd.hahajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yn.newstarts.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nv.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nq.wgjwhj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dt.huanxung.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vp.nszjky.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gp.huanxung.cn

[F05] 判断文件或目录是否存在
来源：http://cf.chemitech.net.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ad.shxzukj.cn

PHP:  file_exists("a.txt");
来源：http://lp.jianghongdianzi.cn

JS:   fs.existsSync("a.txt")
来源：http://ky.bjjhwx.cn

TS:   fs.existsSync("a.txt")
来源：http://yf.asd995.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://eu.jianghongdianzi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xk.lnxyls.cn

Ruby: File.exist?("a.txt")
来源：http://hy.shxzskj.cn

C#:   File.Exists("a.txt")
来源：http://kr.hahajie.cn

[F06] 删除文件
来源：http://aq.colortex.cn

Py:   os.remove("a.txt")
来源：http://jd.panjiajie.cn

PHP:  unlink("a.txt");
来源：http://ub.9csxet.cn

JS:   fs.unlinkSync("a.txt")
来源：http://of.jianghongdianzi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://co.muxihuayi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cy.jianghongdianzi.cn

Go:   os.Remove("a.txt")
来源：http://yc.521024.cn

Ruby: File.delete("a.txt")
来源：http://ov.bookmarksfly.cn

C#:   File.Delete("a.txt");
来源：http://gu.gzmigu.cn

[F07] 创建目录（含多级）
来源：http://yw.shxzskj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://up.haigaiapp.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zu.huixiangedu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fx.lnxyls.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pl.hnjuh.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jz.muxihuayi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gz.colortex.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dm.gzmigu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ln.muxihuayi.cn

[F08] 遍历目录
来源：http://lo.panjiajie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zy.huixinmuqiang.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qy.wgjwhj.cn

JS:   fs.readdirSync("dir")
来源：http://of.szxytkj.cn

TS:   fs.readdirSync("dir")
来源：http://un.shxzskj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://re.wgjwhj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://gb.huanxung.cn

Ruby: Dir.children("dir")
来源：http://yi.9csxet.cn

C#:   Directory.GetFiles("dir")
来源：http://sc.huanxung.cn

[F09] 获取文件大小
来源：http://in.jctech888.com.cn

Py:   os.path.getsize("a.txt")
来源：http://xd.9csxet.cn

PHP:  filesize("a.txt");
来源：http://al.521024.cn

JS:   fs.statSync("a.txt").size
来源：http://os.huixinmuqiang.cn

TS:   fs.statSync("a.txt").size
来源：http://ir.shxzukj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://vn.hnjuh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lz.yuexingan06.cn

Ruby: File.size("a.txt")
来源：http://rm.wgjwhj.cn

C#:   new FileInfo("a.txt").Length
来源：http://rq.yuexingan06.cn

[F10] 取文件扩展名 / 文件名
来源：http://bp.nszjky.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://es.gzmigu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ru.huanxung.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://oe.bookmarksfly.cn

TS:   path.extname("a.txt")
来源：http://vc.yuexingan06.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bg.yuntaijiaju.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qm.shxzskj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gn.wgjwhj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://aa.hnjuh.cn

[F11] 复制与移动文件
来源：http://fj.shxzskj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dx.szsharing.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fd.hahajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://el.wgjwhj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bt.chemitech.net.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ms.newstarts.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fk.colortex.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ny.szxytkj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://va.colortex.cn

[F12] CSV 读写
来源：http://cq.newstarts.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hs.nszjky.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zg.521024.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://sd.shxzukj.cn

TS:   // 同上
来源：http://vf.521024.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ql.szxytkj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pv.shxzskj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xz.panjiajie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://vx.jctech888.com.cn

================================================================================
来源：http://cz.gzmigu.cn

G. 面向对象
来源：http://sz.shxzukj.cn

================================================================================
来源：http://ht.yuexingan06.cn

[G01] 定义类
来源：http://xe.shxzukj.cn

Py:   class User: pass
来源：http://xb.chemitech.net.cn

PHP:  class User {}
来源：http://mh.jctech888.com.cn

JS:   class User {}
来源：http://wx.panjiajie.cn

TS:   class User { name: string = ""; }
来源：http://ao.bjjhwx.cn

Java: class User {}
来源：http://qm.haigaiapp.cn

Go:   type User struct { Name string }
来源：http://py.panjiajie.cn

Ruby: class User; end
来源：http://ph.yuntaijiaju.cn

C#:   class User {}
来源：http://ak.bookmarksfly.cn

[G02] 构造函数
来源：http://cd.shxzskj.cn

Py:   def __init__(self, name): self.name = name
来源：http://kg.asd995.cn

PHP:  public function __construct(public string $name) {}
来源：http://re.shtwfgs.cn

JS:   constructor(name) { this.name = name; }
来源：http://vl.hnjuh.cn

TS:   constructor(public name: string) {}
来源：http://ps.yuexingan06.cn

Java: User(String name) { this.name = name; }
来源：http://es.gzmigu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://os.huixinmuqiang.cn

Ruby: def initialize(name); @name = name; end
来源：http://vq.szxytkj.cn

C#:   public User(string name) { Name = name; }
来源：http://jh.newstarts.cn

[G03] 实例属性
来源：http://zl.shxzukj.cn

Py:   self.name = "x"
来源：http://ss.yuexingan06.cn

PHP:  public string $name = "x";
来源：http://gt.bookmarksfly.cn

JS:   this.name = "x";
来源：http://jk.huixinmuqiang.cn

TS:   name: string = "x";
来源：http://fz.yuntaijiaju.cn

Java: private String name;
来源：http://am.panjiajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xz.521024.cn

Ruby: @name = "x"
来源：http://lc.nicolike.cn

C#:   public string Name { get; set; } = "x";
来源：http://ko.bookmarksfly.cn

[G04] 定义方法
来源：http://bj.nicolike.cn

Py:   def greet(self): return self.name
来源：http://qe.colortex.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://sf.asd995.cn

JS:   greet() { return this.name; }
来源：http://qn.shxzskj.cn

TS:   greet(): string { return this.name; }
来源：http://sd.wgjwhj.cn

Java: String greet() { return name; }
来源：http://zw.9csxet.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://wu.colortex.cn

Ruby: def greet; @name; end
来源：http://jn.colortex.cn

C#:   public string Greet() => Name;
来源：http://ry.szxytkj.cn

[G05] 继承
来源：http://hs.szxytkj.cn

Py:   class Admin(User): pass
来源：http://kn.9csxet.cn

PHP:  class Admin extends User {}
来源：http://oo.shxzskj.cn

JS:   class Admin extends User {}
来源：http://xm.jctech888.com.cn

TS:   class Admin extends User {}
来源：http://dd.bjjhwx.cn

Java: class Admin extends User {}
来源：http://xn.huixinmuqiang.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ch.jctech888.com.cn

Ruby: class Admin < User; end
来源：http://ok.haigaiapp.cn

C#:   class Admin : User {}
来源：http://fe.gzmigu.cn


<!-- 参考信息 -->