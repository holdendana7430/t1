代发 wailian999

[E06] 替换子串
来源：http://kc.lnxyls.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ml.shxzukj.cn

PHP:  str_replace("a", "b", $s);
来源：http://xo.yuexingan06.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bi.nicolike.cn

TS:   s.replaceAll("a", "b")
来源：http://at.521024.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sy.nicolike.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rb.shxzskj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ve.huixinmuqiang.cn

C#:   s.Replace("a", "b")
来源：http://vp.chemitech.net.cn

[E07] 按分隔符拆分
来源：http://rx.muxihuayi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qy.bjjhwx.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mu.gzmigu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://vk.521024.cn

TS:   s.split(",")
来源：http://eu.jianghongdianzi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://tw.huixiangedu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ue.lnxyls.cn

Ruby: s.split(",");  s.split
来源：http://nr.nszjky.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bx.9csxet.cn

[E08] 数组按分隔符合并
来源：http://ar.jianghongdianzi.cn

Py:   ",".join(items)
来源：http://xs.szsharing.cn

PHP:  implode(",", $items);
来源：http://np.jianghongdianzi.cn

JS:   items.join(",")
来源：http://pw.chemitech.net.cn

TS:   items.join(",")
来源：http://gz.panjiajie.cn

Java: String.join(",", items)
来源：http://ul.jianghongdianzi.cn

Go:   strings.Join(items, ",")
来源：http://fx.9csxet.cn

Ruby: items.join(",")
来源：http://xo.hahajie.cn

C#:   string.Join(",", items)
来源：http://uo.colortex.cn

[E09] 去除所有空白字符
来源：http://ob.hahajie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bj.wgjwhj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://go.chemitech.net.cn

JS:   s.replace(/\s+/g, "")
来源：http://kn.panjiajie.cn

TS:   s.replace(/\s+/g, "")
来源：http://ix.chemitech.net.cn

Java: s.replaceAll("\\s+", "")
来源：http://ag.haigaiapp.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://cu.szsharing.cn

Ruby: s.gsub(/\s+/, "")
来源：http://lz.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ys.hahajie.cn

[E10] 左侧补零 / 定长填充
来源：http://dr.panjiajie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ej.asd995.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://re.521024.cn

JS:   "7".padStart(3, "0")
来源：http://ew.asd995.cn

TS:   "7".padStart(3, "0")
来源：http://iu.shtwfgs.cn

Java: String.format("%03d", 7)
来源：http://tf.jianghongdianzi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://en.nicolike.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dp.newstarts.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://si.shxzukj.cn

[E11] 反转字符串
来源：http://cq.hnjuh.cn

Py:   s[::-1]
来源：http://us.9csxet.cn

PHP:  strrev($s);
来源：http://vm.bookmarksfly.cn

JS:   [...s].reverse().join("")
来源：http://uh.szsharing.cn

TS:   [...s].reverse().join("")
来源：http://pa.521024.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://su.shtwfgs.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ph.huixinmuqiang.cn

Ruby: s.reverse
来源：http://ag.shxzukj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://re.shtwfgs.cn

[E12] 统计某字符出现次数
来源：http://iq.huixiangedu.cn

Py:   s.count("a")
来源：http://wx.huixinmuqiang.cn

PHP:  substr_count($s, "a");
来源：http://lg.nicolike.cn

JS:   s.split("a").length - 1
来源：http://xf.shxzskj.cn

TS:   s.split("a").length - 1
来源：http://ov.jctech888.com.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gy.bookmarksfly.cn

Go:   strings.Count(s, "a")
来源：http://me.521024.cn

Ruby: s.count("a")
来源：http://pa.jctech888.com.cn

C#:   s.Count(c => c == 'a')
来源：http://la.muxihuayi.cn

[E13] 逐字符遍历
来源：http://jj.hahajie.cn

Py:   for ch in s: print(ch)
来源：http://cb.shxzukj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gz.asd995.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://bu.colortex.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://jc.521024.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yj.chemitech.net.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mv.asd995.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://cf.colortex.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ib.chemitech.net.cn

[E14] URL 编码与 Base64
来源：http://lj.asd995.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ej.yuntaijiaju.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ye.szsharing.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mj.bjjhwx.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://oz.yuntaijiaju.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pe.bookmarksfly.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yw.huixiangedu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vx.hnjuh.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sf.haigaiapp.cn

[E15] HTML 转义 / 反转义
来源：http://wc.521024.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://qg.colortex.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ek.nszjky.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wx.haigaiapp.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://lc.huixinmuqiang.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cz.shxzskj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ex.nszjky.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://if.newstarts.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://il.gzmigu.cn

[E16] 数字千分位
来源：http://yj.huixiangedu.cn

Py:   f"{1234567:,}"
来源：http://py.muxihuayi.cn

PHP:  number_format(1234567);
来源：http://xu.521024.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://hs.jianghongdianzi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://nz.nicolike.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vq.nicolike.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pm.nszjky.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ed.szxytkj.cn

C#:   1234567.ToString("N0")
来源：http://cs.shtwfgs.cn

[E17] 首字母大写
来源：http://bf.wgjwhj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qx.lnxyls.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://iv.huanxung.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xz.huixinmuqiang.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zh.huixiangedu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vg.huanxung.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ii.yuntaijiaju.cn

Ruby: s.capitalize
来源：http://pz.huanxung.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://aj.bjjhwx.cn

[E18] 模板占位符替换
来源：http://wx.huixinmuqiang.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hi.asd995.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dg.nicolike.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://jv.wgjwhj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://sk.huanxung.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rg.jianghongdianzi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ug.521024.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://im.huixiangedu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ba.jctech888.com.cn

[E19] 多行文本按行拆分
来源：http://oz.jianghongdianzi.cn

Py:   s.splitlines()
来源：http://uv.jianghongdianzi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jd.huixinmuqiang.cn

JS:   s.split(/\r?\n/)
来源：http://wy.bookmarksfly.cn

TS:   s.split(/\r?\n/)
来源：http://fx.szsharing.cn

Java: s.lines().toList()
来源：http://zr.shxzskj.cn

Go:   strings.Split(s, "\n")
来源：http://qp.bjjhwx.cn

Ruby: s.lines
来源：http://mo.yuntaijiaju.cn

C#:   s.Split('\n')
来源：http://fl.huanxung.cn

[E20] 判断字符串是否为空
来源：http://dz.gzmigu.cn

Py:   if not s:
来源：http://hh.panjiajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cl.yuexingan06.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://uw.wgjwhj.cn

TS:   if (s === "") {}
来源：http://si.nicolike.cn

Java: if (s.isEmpty()) {}
来源：http://bk.bookmarksfly.cn

Go:   if s == "" {}
来源：http://pc.shtwfgs.cn

Ruby: if s.empty?
来源：http://kc.9csxet.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gc.hnjuh.cn

[E21] 超长截断加省略号
来源：http://ot.nszjky.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ed.asd995.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ii.newstarts.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qa.nicolike.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sv.lnxyls.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ek.haigaiapp.cn

Go:   // 按 rune 判断长度后截断
来源：http://va.shtwfgs.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zw.colortex.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ly.hahajie.cn

[E22] 字节长度与字符长度
来源：http://xi.hahajie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kj.lnxyls.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hu.bjjhwx.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hu.bjjhwx.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gv.muxihuayi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kc.9csxet.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pm.shtwfgs.cn

Ruby: s.bytesize;  s.length
来源：http://vp.wgjwhj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kw.asd995.cn

================================================================================
来源：http://ty.shxzukj.cn

F. 文件与目录
来源：http://ki.gzmigu.cn

================================================================================
来源：http://kn.nicolike.cn

[F01] 读取整个文件
来源：http://wj.nszjky.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://us.yuexingan06.cn

PHP:  file_get_contents("a.txt");
来源：http://br.shxzskj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dq.szsharing.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://uy.jctech888.com.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fp.szsharing.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xu.asd995.cn

Ruby: File.read("a.txt")
来源：http://ti.szxytkj.cn

C#:   File.ReadAllText("a.txt");
来源：http://eq.nicolike.cn

[F02] 逐行读取文件
来源：http://mz.yuntaijiaju.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hs.shxzskj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sg.colortex.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ol.jianghongdianzi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ti.nszjky.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://me.521024.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://il.haigaiapp.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hq.szxytkj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xi.yuexingan06.cn

[F03] 写入文件（覆盖）
来源：http://bm.bjjhwx.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fc.jctech888.com.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://dq.shxzskj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kc.hahajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ut.jctech888.com.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jg.huixiangedu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wp.colortex.cn

Ruby: File.write("a.txt", "hi")
来源：http://sf.jctech888.com.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yo.szxytkj.cn

[F04] 追加写入文件
来源：http://yz.muxihuayi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vv.jianghongdianzi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fr.jctech888.com.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oq.yuexingan06.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jv.lnxyls.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://oo.bjjhwx.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://md.huanxung.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xt.bjjhwx.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hb.newstarts.cn

[F05] 判断文件或目录是否存在
来源：http://xm.yuexingan06.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://sy.szsharing.cn

PHP:  file_exists("a.txt");
来源：http://ys.bookmarksfly.cn

JS:   fs.existsSync("a.txt")
来源：http://sg.huanxung.cn

TS:   fs.existsSync("a.txt")
来源：http://fl.jctech888.com.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://lu.shxzukj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yw.bookmarksfly.cn

Ruby: File.exist?("a.txt")
来源：http://nb.lnxyls.cn

C#:   File.Exists("a.txt")
来源：http://qv.lnxyls.cn

[F06] 删除文件
来源：http://sc.jctech888.com.cn

Py:   os.remove("a.txt")
来源：http://ze.bjjhwx.cn

PHP:  unlink("a.txt");
来源：http://fk.szxytkj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://gs.521024.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ba.nicolike.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sk.panjiajie.cn

Go:   os.Remove("a.txt")
来源：http://wv.newstarts.cn

Ruby: File.delete("a.txt")
来源：http://kh.521024.cn

C#:   File.Delete("a.txt");
来源：http://bx.jianghongdianzi.cn

[F07] 创建目录（含多级）
来源：http://ux.panjiajie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://et.shxzukj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zb.shtwfgs.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pm.chemitech.net.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tz.bookmarksfly.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ol.huanxung.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xw.bookmarksfly.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bt.9csxet.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://st.asd995.cn

[F08] 遍历目录
来源：http://jq.hahajie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://br.9csxet.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ht.shtwfgs.cn

JS:   fs.readdirSync("dir")
来源：http://cp.panjiajie.cn

TS:   fs.readdirSync("dir")
来源：http://ud.asd995.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zv.yuexingan06.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://yb.9csxet.cn

Ruby: Dir.children("dir")
来源：http://hc.nszjky.cn

C#:   Directory.GetFiles("dir")
来源：http://aa.colortex.cn

[F09] 获取文件大小
来源：http://nr.colortex.cn

Py:   os.path.getsize("a.txt")
来源：http://mz.szsharing.cn

PHP:  filesize("a.txt");
来源：http://nz.hnjuh.cn

JS:   fs.statSync("a.txt").size
来源：http://bc.bookmarksfly.cn

TS:   fs.statSync("a.txt").size
来源：http://va.shxzukj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://pg.hnjuh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://uy.hahajie.cn

Ruby: File.size("a.txt")
来源：http://zi.jianghongdianzi.cn

C#:   new FileInfo("a.txt").Length
来源：http://di.jctech888.com.cn

[F10] 取文件扩展名 / 文件名
来源：http://vm.shxzukj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tl.asd995.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kk.newstarts.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://di.huixinmuqiang.cn

TS:   path.extname("a.txt")
来源：http://wr.nszjky.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ap.gzmigu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pe.shxzukj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://er.nicolike.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mq.haigaiapp.cn

[F11] 复制与移动文件
来源：http://ur.9csxet.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ls.haigaiapp.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ba.newstarts.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yi.521024.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bu.newstarts.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cr.gzmigu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rq.yuexingan06.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tg.shxzskj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lc.asd995.cn

[F12] CSV 读写
来源：http://hv.colortex.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mv.hahajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ny.jianghongdianzi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dx.haigaiapp.cn

TS:   // 同上
来源：http://iq.9csxet.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ag.hnjuh.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sv.gzmigu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xz.yuexingan06.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ey.wgjwhj.cn

================================================================================
来源：http://ta.newstarts.cn

G. 面向对象
来源：http://rc.panjiajie.cn

================================================================================
来源：http://ay.wgjwhj.cn

[G01] 定义类
来源：http://ip.huixiangedu.cn

Py:   class User: pass
来源：http://nh.hnjuh.cn

PHP:  class User {}
来源：http://ur.shtwfgs.cn

JS:   class User {}
来源：http://wh.szxytkj.cn

TS:   class User { name: string = ""; }
来源：http://ob.muxihuayi.cn

Java: class User {}
来源：http://kn.hahajie.cn

Go:   type User struct { Name string }
来源：http://cl.chemitech.net.cn

Ruby: class User; end
来源：http://nv.shxzskj.cn

C#:   class User {}
来源：http://fw.yuexingan06.cn

[G02] 构造函数
来源：http://qi.hnjuh.cn

Py:   def __init__(self, name): self.name = name
来源：http://yj.colortex.cn

PHP:  public function __construct(public string $name) {}
来源：http://ed.huixinmuqiang.cn

JS:   constructor(name) { this.name = name; }
来源：http://vh.521024.cn

TS:   constructor(public name: string) {}
来源：http://qe.9csxet.cn

Java: User(String name) { this.name = name; }
来源：http://ir.muxihuayi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ol.gzmigu.cn

Ruby: def initialize(name); @name = name; end
来源：http://re.shxzukj.cn

C#:   public User(string name) { Name = name; }
来源：http://rf.lnxyls.cn

[G03] 实例属性
来源：http://kp.bookmarksfly.cn

Py:   self.name = "x"
来源：http://jn.chemitech.net.cn

PHP:  public string $name = "x";
来源：http://qb.wgjwhj.cn

JS:   this.name = "x";
来源：http://tp.szsharing.cn

TS:   name: string = "x";
来源：http://sp.hahajie.cn

Java: private String name;
来源：http://bw.shxzukj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ap.huixinmuqiang.cn

Ruby: @name = "x"
来源：http://hy.hahajie.cn

C#:   public string Name { get; set; } = "x";
来源：http://en.9csxet.cn

[G04] 定义方法
来源：http://dz.muxihuayi.cn

Py:   def greet(self): return self.name
来源：http://rk.haigaiapp.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://tv.panjiajie.cn

JS:   greet() { return this.name; }
来源：http://ys.huanxung.cn

TS:   greet(): string { return this.name; }
来源：http://ji.asd995.cn

Java: String greet() { return name; }
来源：http://sd.bookmarksfly.cn


<!-- 参考信息 -->