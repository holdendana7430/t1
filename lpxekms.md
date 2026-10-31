代发 wailian999

C#:   s.Replace("a", "b")
来源：http://vn.521024.cn

[E07] 按分隔符拆分
来源：http://lt.bookmarksfly.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xw.yuexingan06.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ru.lnxyls.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://od.chemitech.net.cn

TS:   s.split(",")
来源：http://om.panjiajie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://hi.lnxyls.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lp.lnxyls.cn

Ruby: s.split(",");  s.split
来源：http://tp.huixiangedu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ft.nicolike.cn

[E08] 数组按分隔符合并
来源：http://ql.lnxyls.cn

Py:   ",".join(items)
来源：http://at.szxytkj.cn

PHP:  implode(",", $items);
来源：http://lc.muxihuayi.cn

JS:   items.join(",")
来源：http://kb.nszjky.cn

TS:   items.join(",")
来源：http://zu.521024.cn

Java: String.join(",", items)
来源：http://fj.hahajie.cn

Go:   strings.Join(items, ",")
来源：http://ij.jctech888.com.cn

Ruby: items.join(",")
来源：http://lr.gzmigu.cn

C#:   string.Join(",", items)
来源：http://po.shtwfgs.cn

[E09] 去除所有空白字符
来源：http://ut.521024.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zp.wgjwhj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hy.haigaiapp.cn

JS:   s.replace(/\s+/g, "")
来源：http://bc.shtwfgs.cn

TS:   s.replace(/\s+/g, "")
来源：http://qv.colortex.cn

Java: s.replaceAll("\\s+", "")
来源：http://qb.muxihuayi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://bg.yuexingan06.cn

Ruby: s.gsub(/\s+/, "")
来源：http://af.gzmigu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yx.hnjuh.cn

[E10] 左侧补零 / 定长填充
来源：http://uq.huixinmuqiang.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qg.haigaiapp.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kv.jctech888.com.cn

JS:   "7".padStart(3, "0")
来源：http://ea.bookmarksfly.cn

TS:   "7".padStart(3, "0")
来源：http://ls.panjiajie.cn

Java: String.format("%03d", 7)
来源：http://ri.newstarts.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://bs.lnxyls.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kv.szsharing.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ev.nicolike.cn

[E11] 反转字符串
来源：http://da.bjjhwx.cn

Py:   s[::-1]
来源：http://wb.shxzskj.cn

PHP:  strrev($s);
来源：http://zh.yuntaijiaju.cn

JS:   [...s].reverse().join("")
来源：http://qx.haigaiapp.cn

TS:   [...s].reverse().join("")
来源：http://az.huanxung.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zp.9csxet.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ma.521024.cn

Ruby: s.reverse
来源：http://oy.colortex.cn

C#:   new string(s.Reverse().ToArray())
来源：http://su.hahajie.cn

[E12] 统计某字符出现次数
来源：http://ju.gzmigu.cn

Py:   s.count("a")
来源：http://pz.szxytkj.cn

PHP:  substr_count($s, "a");
来源：http://ma.lnxyls.cn

JS:   s.split("a").length - 1
来源：http://oo.hahajie.cn

TS:   s.split("a").length - 1
来源：http://dq.colortex.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yp.jianghongdianzi.cn

Go:   strings.Count(s, "a")
来源：http://ch.jctech888.com.cn

Ruby: s.count("a")
来源：http://yq.bookmarksfly.cn

C#:   s.Count(c => c == 'a')
来源：http://ta.huixinmuqiang.cn

[E13] 逐字符遍历
来源：http://ug.chemitech.net.cn

Py:   for ch in s: print(ch)
来源：http://oq.huixinmuqiang.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://il.muxihuayi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://fe.panjiajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://hi.gzmigu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://th.bookmarksfly.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tb.wgjwhj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://sq.yuexingan06.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jh.asd995.cn

[E14] URL 编码与 Base64
来源：http://zt.shxzukj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gx.wgjwhj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://jt.nicolike.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bv.panjiajie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://al.9csxet.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uf.nszjky.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fi.wgjwhj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wt.huixinmuqiang.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tf.szxytkj.cn

[E15] HTML 转义 / 反转义
来源：http://an.521024.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://wb.newstarts.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ot.jctech888.com.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mf.hnjuh.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://rz.shxzukj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jr.hahajie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pj.yuntaijiaju.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wt.lnxyls.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://oe.bjjhwx.cn

[E16] 数字千分位
来源：http://ct.szsharing.cn

Py:   f"{1234567:,}"
来源：http://hz.newstarts.cn

PHP:  number_format(1234567);
来源：http://ri.hahajie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://pl.szsharing.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ry.lnxyls.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ne.szsharing.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ho.huixiangedu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://is.521024.cn

C#:   1234567.ToString("N0")
来源：http://uf.huanxung.cn

[E17] 首字母大写
来源：http://pb.hahajie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://my.colortex.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://rv.bjjhwx.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fn.muxihuayi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kl.shtwfgs.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://og.hahajie.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ri.chemitech.net.cn

Ruby: s.capitalize
来源：http://ae.szsharing.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pq.hahajie.cn

[E18] 模板占位符替换
来源：http://ax.huixiangedu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lf.bookmarksfly.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yn.huixinmuqiang.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://pb.shxzskj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://rt.shtwfgs.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vv.szsharing.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nz.haigaiapp.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gg.9csxet.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ru.bookmarksfly.cn

[E19] 多行文本按行拆分
来源：http://vn.jctech888.com.cn

Py:   s.splitlines()
来源：http://oj.asd995.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nv.newstarts.cn

JS:   s.split(/\r?\n/)
来源：http://ju.colortex.cn

TS:   s.split(/\r?\n/)
来源：http://rr.bjjhwx.cn

Java: s.lines().toList()
来源：http://ml.nicolike.cn

Go:   strings.Split(s, "\n")
来源：http://zu.hnjuh.cn

Ruby: s.lines
来源：http://rg.shtwfgs.cn

C#:   s.Split('\n')
来源：http://db.hahajie.cn

[E20] 判断字符串是否为空
来源：http://ye.lnxyls.cn

Py:   if not s:
来源：http://om.9csxet.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ot.gzmigu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cv.haigaiapp.cn

TS:   if (s === "") {}
来源：http://ng.jctech888.com.cn

Java: if (s.isEmpty()) {}
来源：http://ad.shtwfgs.cn

Go:   if s == "" {}
来源：http://ta.lnxyls.cn

Ruby: if s.empty?
来源：http://ek.huanxung.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tt.jctech888.com.cn

[E21] 超长截断加省略号
来源：http://bp.shtwfgs.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bo.jctech888.com.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gb.yuntaijiaju.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gj.bjjhwx.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vz.521024.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tr.lnxyls.cn

Go:   // 按 rune 判断长度后截断
来源：http://xg.muxihuayi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ei.hnjuh.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gv.colortex.cn

[E22] 字节长度与字符长度
来源：http://gm.huanxung.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ep.shxzukj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ag.haigaiapp.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vc.wgjwhj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zk.bjjhwx.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fs.9csxet.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vw.shtwfgs.cn

Ruby: s.bytesize;  s.length
来源：http://pd.nicolike.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rv.lnxyls.cn

================================================================================
来源：http://tp.hnjuh.cn

F. 文件与目录
来源：http://ki.jctech888.com.cn

================================================================================
来源：http://fl.szxytkj.cn

[F01] 读取整个文件
来源：http://ww.521024.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ht.bjjhwx.cn

PHP:  file_get_contents("a.txt");
来源：http://bt.9csxet.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://et.521024.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ty.colortex.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://lv.panjiajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ns.szsharing.cn

Ruby: File.read("a.txt")
来源：http://xm.521024.cn

C#:   File.ReadAllText("a.txt");
来源：http://bx.yuntaijiaju.cn

[F02] 逐行读取文件
来源：http://hb.huixiangedu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mh.shxzukj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lb.muxihuayi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cg.colortex.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wa.shtwfgs.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kr.huixinmuqiang.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gu.chemitech.net.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ps.9csxet.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jh.huixiangedu.cn

[F03] 写入文件（覆盖）
来源：http://ki.yuntaijiaju.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ry.wgjwhj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://is.newstarts.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iu.shtwfgs.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zj.szxytkj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mv.colortex.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fi.9csxet.cn

Ruby: File.write("a.txt", "hi")
来源：http://or.shxzskj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zd.chemitech.net.cn

[F04] 追加写入文件
来源：http://dl.shxzukj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pc.bookmarksfly.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tk.asd995.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ti.huixiangedu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vm.colortex.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zm.szsharing.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ez.huixinmuqiang.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ab.asd995.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ix.shxzskj.cn

[F05] 判断文件或目录是否存在
来源：http://ek.szxytkj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vy.yuntaijiaju.cn

PHP:  file_exists("a.txt");
来源：http://gy.yuexingan06.cn

JS:   fs.existsSync("a.txt")
来源：http://vq.huixinmuqiang.cn

TS:   fs.existsSync("a.txt")
来源：http://eb.panjiajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ey.shtwfgs.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zd.huixiangedu.cn

Ruby: File.exist?("a.txt")
来源：http://dw.lnxyls.cn

C#:   File.Exists("a.txt")
来源：http://au.colortex.cn

[F06] 删除文件
来源：http://eu.521024.cn

Py:   os.remove("a.txt")
来源：http://dd.haigaiapp.cn

PHP:  unlink("a.txt");
来源：http://fo.lnxyls.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vf.shtwfgs.cn

TS:   fs.unlinkSync("a.txt")
来源：http://lz.shxzskj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vd.huixiangedu.cn

Go:   os.Remove("a.txt")
来源：http://go.nszjky.cn

Ruby: File.delete("a.txt")
来源：http://ce.szxytkj.cn

C#:   File.Delete("a.txt");
来源：http://ci.lnxyls.cn

[F07] 创建目录（含多级）
来源：http://ia.nicolike.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ei.nicolike.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zc.haigaiapp.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ie.9csxet.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jz.szxytkj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fv.muxihuayi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://od.521024.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://be.panjiajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://yr.huixinmuqiang.cn

[F08] 遍历目录
来源：http://hr.shtwfgs.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://jm.chemitech.net.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://st.huixiangedu.cn

JS:   fs.readdirSync("dir")
来源：http://ey.gzmigu.cn

TS:   fs.readdirSync("dir")
来源：http://cn.bjjhwx.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ia.szsharing.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://tr.gzmigu.cn

Ruby: Dir.children("dir")
来源：http://rx.jianghongdianzi.cn

C#:   Directory.GetFiles("dir")
来源：http://as.muxihuayi.cn

[F09] 获取文件大小
来源：http://hj.521024.cn

Py:   os.path.getsize("a.txt")
来源：http://wk.gzmigu.cn

PHP:  filesize("a.txt");
来源：http://ht.521024.cn

JS:   fs.statSync("a.txt").size
来源：http://nr.bookmarksfly.cn

TS:   fs.statSync("a.txt").size
来源：http://ue.szsharing.cn

Java: Files.size(Path.of("a.txt"))
来源：http://bp.shxzukj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zk.gzmigu.cn

Ruby: File.size("a.txt")
来源：http://bc.shxzskj.cn

C#:   new FileInfo("a.txt").Length
来源：http://iz.chemitech.net.cn

[F10] 取文件扩展名 / 文件名
来源：http://df.hnjuh.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jw.muxihuayi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rk.gzmigu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://et.shxzukj.cn

TS:   path.extname("a.txt")
来源：http://ox.huanxung.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ef.asd995.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mq.colortex.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jj.shtwfgs.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://aa.panjiajie.cn

[F11] 复制与移动文件
来源：http://bn.shtwfgs.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xl.521024.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bb.yuntaijiaju.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vc.shxzukj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ls.shtwfgs.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ag.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kr.shxzukj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lm.nicolike.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cz.asd995.cn

[F12] CSV 读写
来源：http://gk.haigaiapp.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://us.hnjuh.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ht.jianghongdianzi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qj.jctech888.com.cn

TS:   // 同上
来源：http://bn.lnxyls.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ni.bjjhwx.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zb.yuexingan06.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://th.chemitech.net.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://yq.szxytkj.cn

================================================================================
来源：http://xg.huanxung.cn

G. 面向对象
来源：http://ju.gzmigu.cn

================================================================================
来源：http://cl.wgjwhj.cn

[G01] 定义类
来源：http://kj.hahajie.cn

Py:   class User: pass
来源：http://mb.lnxyls.cn

PHP:  class User {}
来源：http://hr.newstarts.cn

JS:   class User {}
来源：http://fw.shxzukj.cn

TS:   class User { name: string = ""; }
来源：http://xv.hahajie.cn

Java: class User {}
来源：http://aa.newstarts.cn

Go:   type User struct { Name string }
来源：http://kx.521024.cn

Ruby: class User; end
来源：http://fl.shxzskj.cn

C#:   class User {}
来源：http://fx.shtwfgs.cn

[G02] 构造函数
来源：http://fx.hahajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://ks.wgjwhj.cn

PHP:  public function __construct(public string $name) {}
来源：http://lj.bookmarksfly.cn

JS:   constructor(name) { this.name = name; }
来源：http://xo.asd995.cn

TS:   constructor(public name: string) {}
来源：http://pc.szsharing.cn

Java: User(String name) { this.name = name; }
来源：http://na.nszjky.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nd.huanxung.cn

Ruby: def initialize(name); @name = name; end
来源：http://ct.yuexingan06.cn

C#:   public User(string name) { Name = name; }
来源：http://yp.muxihuayi.cn

[G03] 实例属性
来源：http://za.wgjwhj.cn

Py:   self.name = "x"
来源：http://zx.shtwfgs.cn

PHP:  public string $name = "x";
来源：http://vc.gzmigu.cn

JS:   this.name = "x";
来源：http://ak.panjiajie.cn

TS:   name: string = "x";
来源：http://lt.bookmarksfly.cn

Java: private String name;
来源：http://gj.huixinmuqiang.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://du.huixinmuqiang.cn

Ruby: @name = "x"
来源：http://il.bookmarksfly.cn

C#:   public string Name { get; set; } = "x";
来源：http://dc.szxytkj.cn

[G04] 定义方法
来源：http://kn.nicolike.cn

Py:   def greet(self): return self.name
来源：http://jy.asd995.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://hw.szxytkj.cn

JS:   greet() { return this.name; }
来源：http://yr.muxihuayi.cn

TS:   greet(): string { return this.name; }
来源：http://yj.yuntaijiaju.cn

Java: String greet() { return name; }
来源：http://rp.haigaiapp.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://eh.newstarts.cn

Ruby: def greet; @name; end
来源：http://jc.shxzukj.cn

C#:   public string Greet() => Name;
来源：http://rn.bookmarksfly.cn

[G05] 继承
来源：http://tt.newstarts.cn

Py:   class Admin(User): pass
来源：http://eq.newstarts.cn

PHP:  class Admin extends User {}
来源：http://lb.521024.cn

JS:   class Admin extends User {}
来源：http://pk.huixinmuqiang.cn

TS:   class Admin extends User {}
来源：http://ix.bookmarksfly.cn


<!-- 参考信息 -->