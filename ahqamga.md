代发 wailian999

C#:   s.Replace("a", "b")
来源：http://of.muxihuayi.cn

[E07] 按分隔符拆分
来源：http://xd.huixiangedu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://oi.newstarts.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rc.colortex.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://fd.gzmigu.cn

TS:   s.split(",")
来源：http://mg.shtwfgs.cn

Java: s.split(",");  s.split("\\s+")
来源：http://lj.shtwfgs.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ai.yuntaijiaju.cn

Ruby: s.split(",");  s.split
来源：http://yl.nszjky.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xa.jianghongdianzi.cn

[E08] 数组按分隔符合并
来源：http://hm.szsharing.cn

Py:   ",".join(items)
来源：http://io.huixiangedu.cn

PHP:  implode(",", $items);
来源：http://tp.szsharing.cn

JS:   items.join(",")
来源：http://wj.gzmigu.cn

TS:   items.join(",")
来源：http://wd.shxzukj.cn

Java: String.join(",", items)
来源：http://ny.asd995.cn

Go:   strings.Join(items, ",")
来源：http://kw.jianghongdianzi.cn

Ruby: items.join(",")
来源：http://ij.yuexingan06.cn

C#:   string.Join(",", items)
来源：http://sk.nszjky.cn

[E09] 去除所有空白字符
来源：http://zr.huixiangedu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ga.panjiajie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vw.colortex.cn

JS:   s.replace(/\s+/g, "")
来源：http://da.shxzskj.cn

TS:   s.replace(/\s+/g, "")
来源：http://hf.shxzskj.cn

Java: s.replaceAll("\\s+", "")
来源：http://lb.panjiajie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://hs.yuexingan06.cn

Ruby: s.gsub(/\s+/, "")
来源：http://gr.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ho.huanxung.cn

[E10] 左侧补零 / 定长填充
来源：http://er.muxihuayi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zs.huixiangedu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ts.panjiajie.cn

JS:   "7".padStart(3, "0")
来源：http://bw.newstarts.cn

TS:   "7".padStart(3, "0")
来源：http://td.shtwfgs.cn

Java: String.format("%03d", 7)
来源：http://xd.szxytkj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://hw.bookmarksfly.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tx.chemitech.net.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ik.shxzukj.cn

[E11] 反转字符串
来源：http://ml.huanxung.cn

Py:   s[::-1]
来源：http://ej.huixiangedu.cn

PHP:  strrev($s);
来源：http://tx.yuexingan06.cn

JS:   [...s].reverse().join("")
来源：http://vp.jctech888.com.cn

TS:   [...s].reverse().join("")
来源：http://zm.nszjky.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ft.shxzskj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://yh.521024.cn

Ruby: s.reverse
来源：http://od.hnjuh.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ua.haigaiapp.cn

[E12] 统计某字符出现次数
来源：http://pd.shxzskj.cn

Py:   s.count("a")
来源：http://os.hnjuh.cn

PHP:  substr_count($s, "a");
来源：http://ab.wgjwhj.cn

JS:   s.split("a").length - 1
来源：http://rg.yuntaijiaju.cn

TS:   s.split("a").length - 1
来源：http://yu.yuntaijiaju.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jp.panjiajie.cn

Go:   strings.Count(s, "a")
来源：http://cv.szxytkj.cn

Ruby: s.count("a")
来源：http://om.asd995.cn

C#:   s.Count(c => c == 'a')
来源：http://mc.yuexingan06.cn

[E13] 逐字符遍历
来源：http://vh.colortex.cn

Py:   for ch in s: print(ch)
来源：http://ol.huanxung.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sh.jianghongdianzi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ls.jianghongdianzi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qz.huixinmuqiang.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ei.shtwfgs.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qn.yuexingan06.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://hb.shxzukj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://un.hnjuh.cn

[E14] URL 编码与 Base64
来源：http://mz.lnxyls.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hh.nicolike.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://wq.chemitech.net.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://av.bookmarksfly.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jg.chemitech.net.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dw.asd995.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qv.gzmigu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fk.jianghongdianzi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zv.9csxet.cn

[E15] HTML 转义 / 反转义
来源：http://fb.wgjwhj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://dn.bookmarksfly.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dz.521024.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ig.huanxung.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://bu.jianghongdianzi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qo.lnxyls.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://og.wgjwhj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vq.huanxung.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://db.9csxet.cn

[E16] 数字千分位
来源：http://jz.gzmigu.cn

Py:   f"{1234567:,}"
来源：http://cj.521024.cn

PHP:  number_format(1234567);
来源：http://hs.huanxung.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gz.jctech888.com.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://tw.huanxung.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ib.bookmarksfly.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qk.colortex.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pn.shxzskj.cn

C#:   1234567.ToString("N0")
来源：http://vh.gzmigu.cn

[E17] 首字母大写
来源：http://rd.nszjky.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gl.gzmigu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://mc.szxytkj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ou.jctech888.com.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://go.yuexingan06.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ij.haigaiapp.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lq.lnxyls.cn

Ruby: s.capitalize
来源：http://ah.panjiajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rg.wgjwhj.cn

[E18] 模板占位符替换
来源：http://yw.521024.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lf.yuntaijiaju.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://um.muxihuayi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://nm.gzmigu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://rv.haigaiapp.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bz.jctech888.com.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://em.bookmarksfly.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fn.wgjwhj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gx.shxzskj.cn

[E19] 多行文本按行拆分
来源：http://ek.bjjhwx.cn

Py:   s.splitlines()
来源：http://zp.shxzukj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gv.521024.cn

JS:   s.split(/\r?\n/)
来源：http://my.lnxyls.cn

TS:   s.split(/\r?\n/)
来源：http://ns.521024.cn

Java: s.lines().toList()
来源：http://tk.huanxung.cn

Go:   strings.Split(s, "\n")
来源：http://wo.newstarts.cn

Ruby: s.lines
来源：http://ba.szxytkj.cn

C#:   s.Split('\n')
来源：http://cg.hahajie.cn

[E20] 判断字符串是否为空
来源：http://xc.yuexingan06.cn

Py:   if not s:
来源：http://gf.huixiangedu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bj.lnxyls.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ng.wgjwhj.cn

TS:   if (s === "") {}
来源：http://ya.nicolike.cn

Java: if (s.isEmpty()) {}
来源：http://bx.newstarts.cn

Go:   if s == "" {}
来源：http://py.gzmigu.cn

Ruby: if s.empty?
来源：http://ti.huixiangedu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://oi.newstarts.cn

[E21] 超长截断加省略号
来源：http://dl.bookmarksfly.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ux.shtwfgs.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hu.yuexingan06.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://he.shxzukj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kx.lnxyls.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://aw.huanxung.cn

Go:   // 按 rune 判断长度后截断
来源：http://bd.gzmigu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ry.huixinmuqiang.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ql.nszjky.cn

[E22] 字节长度与字符长度
来源：http://jc.hnjuh.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rn.shxzukj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bj.szsharing.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hd.huixinmuqiang.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bn.gzmigu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sw.hahajie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jm.nicolike.cn

Ruby: s.bytesize;  s.length
来源：http://wy.hnjuh.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zf.muxihuayi.cn

================================================================================
来源：http://zm.panjiajie.cn

F. 文件与目录
来源：http://qt.9csxet.cn

================================================================================
来源：http://pu.jianghongdianzi.cn

[F01] 读取整个文件
来源：http://rm.nicolike.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xa.huixiangedu.cn

PHP:  file_get_contents("a.txt");
来源：http://mz.szsharing.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yp.jianghongdianzi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zr.chemitech.net.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://gc.521024.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ox.shxzukj.cn

Ruby: File.read("a.txt")
来源：http://zi.panjiajie.cn

C#:   File.ReadAllText("a.txt");
来源：http://ep.muxihuayi.cn

[F02] 逐行读取文件
来源：http://gs.hahajie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ef.jctech888.com.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ek.chemitech.net.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://om.huixiangedu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ys.nszjky.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rh.panjiajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://br.wgjwhj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://eh.nszjky.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cn.huixiangedu.cn

[F03] 写入文件（覆盖）
来源：http://gh.haigaiapp.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rz.bjjhwx.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://uj.newstarts.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ly.nicolike.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dy.szsharing.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dx.panjiajie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fl.huanxung.cn

Ruby: File.write("a.txt", "hi")
来源：http://mn.wgjwhj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kd.shxzukj.cn

[F04] 追加写入文件
来源：http://tl.colortex.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fc.hnjuh.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ew.lnxyls.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uz.nicolike.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eb.bjjhwx.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pm.521024.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qb.lnxyls.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ea.colortex.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://eh.yuexingan06.cn

[F05] 判断文件或目录是否存在
来源：http://fh.huixinmuqiang.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rs.jianghongdianzi.cn

PHP:  file_exists("a.txt");
来源：http://os.yuexingan06.cn

JS:   fs.existsSync("a.txt")
来源：http://nl.huixiangedu.cn

TS:   fs.existsSync("a.txt")
来源：http://ob.huixinmuqiang.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://yz.gzmigu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sj.9csxet.cn

Ruby: File.exist?("a.txt")
来源：http://fe.huanxung.cn

C#:   File.Exists("a.txt")
来源：http://wv.szxytkj.cn

[F06] 删除文件
来源：http://oa.hahajie.cn

Py:   os.remove("a.txt")
来源：http://iv.muxihuayi.cn

PHP:  unlink("a.txt");
来源：http://yr.yuexingan06.cn

JS:   fs.unlinkSync("a.txt")
来源：http://hk.newstarts.cn

TS:   fs.unlinkSync("a.txt")
来源：http://lx.nszjky.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://iq.lnxyls.cn

Go:   os.Remove("a.txt")
来源：http://fn.nszjky.cn

Ruby: File.delete("a.txt")
来源：http://us.yuexingan06.cn

C#:   File.Delete("a.txt");
来源：http://mb.jianghongdianzi.cn

[F07] 创建目录（含多级）
来源：http://la.gzmigu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xp.szsharing.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ys.huixiangedu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hc.asd995.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tr.wgjwhj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pe.wgjwhj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ly.bjjhwx.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://an.hahajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lz.bookmarksfly.cn

[F08] 遍历目录
来源：http://tg.hnjuh.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://cc.newstarts.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sm.gzmigu.cn

JS:   fs.readdirSync("dir")
来源：http://yd.521024.cn

TS:   fs.readdirSync("dir")
来源：http://li.jctech888.com.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qb.lnxyls.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://hf.jianghongdianzi.cn

Ruby: Dir.children("dir")
来源：http://xo.wgjwhj.cn

C#:   Directory.GetFiles("dir")
来源：http://az.muxihuayi.cn

[F09] 获取文件大小
来源：http://kn.asd995.cn

Py:   os.path.getsize("a.txt")
来源：http://lm.shxzukj.cn

PHP:  filesize("a.txt");
来源：http://cn.chemitech.net.cn

JS:   fs.statSync("a.txt").size
来源：http://dq.bjjhwx.cn

TS:   fs.statSync("a.txt").size
来源：http://rt.chemitech.net.cn

Java: Files.size(Path.of("a.txt"))
来源：http://df.haigaiapp.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fx.haigaiapp.cn

Ruby: File.size("a.txt")
来源：http://mx.colortex.cn

C#:   new FileInfo("a.txt").Length
来源：http://qt.shxzskj.cn

[F10] 取文件扩展名 / 文件名
来源：http://av.gzmigu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rp.nicolike.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ot.yuntaijiaju.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ff.colortex.cn

TS:   path.extname("a.txt")
来源：http://wj.muxihuayi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yj.szxytkj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hj.hahajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xx.huanxung.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xw.shxzskj.cn

[F11] 复制与移动文件
来源：http://vv.9csxet.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://iz.szsharing.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xq.bjjhwx.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dh.muxihuayi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qt.muxihuayi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wk.colortex.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zh.jianghongdianzi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fq.huanxung.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ii.hnjuh.cn

[F12] CSV 读写
来源：http://bj.9csxet.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ka.szxytkj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vz.huixinmuqiang.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xv.yuexingan06.cn

TS:   // 同上
来源：http://fq.bookmarksfly.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lq.shxzukj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://oi.bookmarksfly.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ui.bjjhwx.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://mb.colortex.cn

================================================================================
来源：http://sl.jianghongdianzi.cn

G. 面向对象
来源：http://mv.wgjwhj.cn

================================================================================
来源：http://jd.hahajie.cn

[G01] 定义类
来源：http://tl.huixinmuqiang.cn

Py:   class User: pass
来源：http://xe.yuntaijiaju.cn

PHP:  class User {}
来源：http://fl.szxytkj.cn

JS:   class User {}
来源：http://ac.jctech888.com.cn

TS:   class User { name: string = ""; }
来源：http://tg.521024.cn

Java: class User {}
来源：http://nl.nszjky.cn

Go:   type User struct { Name string }
来源：http://qs.szxytkj.cn

Ruby: class User; end
来源：http://ma.muxihuayi.cn

C#:   class User {}
来源：http://zb.lnxyls.cn

[G02] 构造函数
来源：http://mq.wgjwhj.cn

Py:   def __init__(self, name): self.name = name
来源：http://ck.lnxyls.cn

PHP:  public function __construct(public string $name) {}
来源：http://zg.shxzskj.cn

JS:   constructor(name) { this.name = name; }
来源：http://wq.haigaiapp.cn

TS:   constructor(public name: string) {}
来源：http://km.yuntaijiaju.cn

Java: User(String name) { this.name = name; }
来源：http://cb.szsharing.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vf.szsharing.cn

Ruby: def initialize(name); @name = name; end
来源：http://gr.chemitech.net.cn

C#:   public User(string name) { Name = name; }
来源：http://fx.9csxet.cn

[G03] 实例属性
来源：http://gt.521024.cn

Py:   self.name = "x"
来源：http://rn.szxytkj.cn

PHP:  public string $name = "x";
来源：http://ed.521024.cn

JS:   this.name = "x";
来源：http://dc.chemitech.net.cn

TS:   name: string = "x";
来源：http://zv.yuntaijiaju.cn

Java: private String name;
来源：http://xy.panjiajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://by.huanxung.cn

Ruby: @name = "x"
来源：http://vj.yuexingan06.cn

C#:   public string Name { get; set; } = "x";
来源：http://xt.wgjwhj.cn

[G04] 定义方法
来源：http://xb.yuntaijiaju.cn

Py:   def greet(self): return self.name
来源：http://vj.shxzukj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://tp.shtwfgs.cn

JS:   greet() { return this.name; }
来源：http://yf.asd995.cn

TS:   greet(): string { return this.name; }
来源：http://to.wgjwhj.cn

Java: String greet() { return name; }
来源：http://yf.newstarts.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://lb.asd995.cn

Ruby: def greet; @name; end
来源：http://ay.asd995.cn

C#:   public string Greet() => Name;
来源：http://ap.chemitech.net.cn

[G05] 继承
来源：http://yr.nszjky.cn

Py:   class Admin(User): pass
来源：http://nn.huixiangedu.cn

PHP:  class Admin extends User {}
来源：http://lm.shxzukj.cn

JS:   class Admin extends User {}
来源：http://up.huanxung.cn

TS:   class Admin extends User {}
来源：http://jp.huanxung.cn


<!-- 参考信息 -->