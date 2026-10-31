代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://rx.521024.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jd.nszjky.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kk.521024.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hh.bjjhwx.cn

C#:   s.Replace("a", "b")
来源：http://rr.szxytkj.cn

[E07] 按分隔符拆分
来源：http://br.chemitech.net.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://te.szsharing.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kw.gzmigu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://un.huixinmuqiang.cn

TS:   s.split(",")
来源：http://ud.nicolike.cn

Java: s.split(",");  s.split("\\s+")
来源：http://pc.chemitech.net.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jd.shxzukj.cn

Ruby: s.split(",");  s.split
来源：http://cs.9csxet.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://or.shxzskj.cn

[E08] 数组按分隔符合并
来源：http://jf.hnjuh.cn

Py:   ",".join(items)
来源：http://vq.szsharing.cn

PHP:  implode(",", $items);
来源：http://oa.wgjwhj.cn

JS:   items.join(",")
来源：http://jc.colortex.cn

TS:   items.join(",")
来源：http://za.szxytkj.cn

Java: String.join(",", items)
来源：http://so.muxihuayi.cn

Go:   strings.Join(items, ",")
来源：http://ha.521024.cn

Ruby: items.join(",")
来源：http://om.bookmarksfly.cn

C#:   string.Join(",", items)
来源：http://cy.huixinmuqiang.cn

[E09] 去除所有空白字符
来源：http://sa.szxytkj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zq.shxzskj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ti.lnxyls.cn

JS:   s.replace(/\s+/g, "")
来源：http://dj.521024.cn

TS:   s.replace(/\s+/g, "")
来源：http://ci.muxihuayi.cn

Java: s.replaceAll("\\s+", "")
来源：http://dr.panjiajie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://jg.yuexingan06.cn

Ruby: s.gsub(/\s+/, "")
来源：http://mm.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dg.chemitech.net.cn

[E10] 左侧补零 / 定长填充
来源：http://ah.muxihuayi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://px.9csxet.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vw.shxzskj.cn

JS:   "7".padStart(3, "0")
来源：http://lq.huanxung.cn

TS:   "7".padStart(3, "0")
来源：http://sd.jianghongdianzi.cn

Java: String.format("%03d", 7)
来源：http://pm.shxzskj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://hq.shxzukj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yq.newstarts.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rt.huanxung.cn

[E11] 反转字符串
来源：http://wo.9csxet.cn

Py:   s[::-1]
来源：http://tf.haigaiapp.cn

PHP:  strrev($s);
来源：http://fv.panjiajie.cn

JS:   [...s].reverse().join("")
来源：http://ip.huanxung.cn

TS:   [...s].reverse().join("")
来源：http://bx.wgjwhj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://cy.colortex.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://tk.gzmigu.cn

Ruby: s.reverse
来源：http://ag.gzmigu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://fy.shxzukj.cn

[E12] 统计某字符出现次数
来源：http://yi.colortex.cn

Py:   s.count("a")
来源：http://ke.jctech888.com.cn

PHP:  substr_count($s, "a");
来源：http://aj.muxihuayi.cn

JS:   s.split("a").length - 1
来源：http://nc.panjiajie.cn

TS:   s.split("a").length - 1
来源：http://ln.asd995.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jk.szsharing.cn

Go:   strings.Count(s, "a")
来源：http://ld.shxzukj.cn

Ruby: s.count("a")
来源：http://qr.shxzukj.cn

C#:   s.Count(c => c == 'a')
来源：http://hf.asd995.cn

[E13] 逐字符遍历
来源：http://qw.szsharing.cn

Py:   for ch in s: print(ch)
来源：http://tm.gzmigu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xg.newstarts.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://js.9csxet.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://cu.haigaiapp.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lm.huixinmuqiang.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jk.huanxung.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vh.muxihuayi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://uq.asd995.cn

[E14] URL 编码与 Base64
来源：http://wf.jctech888.com.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://we.panjiajie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://cd.huixinmuqiang.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hb.nicolike.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zt.nszjky.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://sf.9csxet.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fi.szsharing.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hl.muxihuayi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ox.shtwfgs.cn

[E15] HTML 转义 / 反转义
来源：http://ls.asd995.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://yl.bookmarksfly.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jc.chemitech.net.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cx.9csxet.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ov.jianghongdianzi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wq.huanxung.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ud.chemitech.net.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ul.shtwfgs.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mp.hnjuh.cn

[E16] 数字千分位
来源：http://xx.colortex.cn

Py:   f"{1234567:,}"
来源：http://lm.lnxyls.cn

PHP:  number_format(1234567);
来源：http://sr.gzmigu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://re.shxzukj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://rm.jianghongdianzi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fy.nicolike.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ej.lnxyls.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ay.shxzskj.cn

C#:   1234567.ToString("N0")
来源：http://gp.asd995.cn

[E17] 首字母大写
来源：http://oi.jctech888.com.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vm.hahajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ap.shxzukj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iq.gzmigu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mm.nicolike.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rh.hahajie.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ke.9csxet.cn

Ruby: s.capitalize
来源：http://sr.lnxyls.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cs.szsharing.cn

[E18] 模板占位符替换
来源：http://kr.asd995.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://oo.colortex.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wm.szsharing.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://wg.chemitech.net.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://an.gzmigu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kp.hahajie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kp.colortex.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://af.haigaiapp.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hq.9csxet.cn

[E19] 多行文本按行拆分
来源：http://nv.hnjuh.cn

Py:   s.splitlines()
来源：http://mp.nicolike.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lg.huixinmuqiang.cn

JS:   s.split(/\r?\n/)
来源：http://zd.chemitech.net.cn

TS:   s.split(/\r?\n/)
来源：http://lm.hnjuh.cn

Java: s.lines().toList()
来源：http://or.yuntaijiaju.cn

Go:   strings.Split(s, "\n")
来源：http://kv.nszjky.cn

Ruby: s.lines
来源：http://ts.huixinmuqiang.cn

C#:   s.Split('\n')
来源：http://jc.nicolike.cn

[E20] 判断字符串是否为空
来源：http://qj.asd995.cn

Py:   if not s:
来源：http://xv.wgjwhj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rv.panjiajie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qi.yuntaijiaju.cn

TS:   if (s === "") {}
来源：http://cl.muxihuayi.cn

Java: if (s.isEmpty()) {}
来源：http://xh.shxzskj.cn

Go:   if s == "" {}
来源：http://bz.newstarts.cn

Ruby: if s.empty?
来源：http://lr.yuntaijiaju.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xp.szxytkj.cn

[E21] 超长截断加省略号
来源：http://qz.shxzukj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ld.panjiajie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://aa.lnxyls.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iw.bjjhwx.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nk.lnxyls.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xa.panjiajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://ft.muxihuayi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tx.huanxung.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wh.szxytkj.cn

[E22] 字节长度与字符长度
来源：http://sm.szsharing.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kh.jctech888.com.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qt.wgjwhj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zw.huixiangedu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zq.nszjky.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dd.9csxet.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tb.muxihuayi.cn

Ruby: s.bytesize;  s.length
来源：http://lu.huixinmuqiang.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ob.yuexingan06.cn

================================================================================
来源：http://lm.521024.cn

F. 文件与目录
来源：http://vm.gzmigu.cn

================================================================================
来源：http://hy.chemitech.net.cn

[F01] 读取整个文件
来源：http://qz.szxytkj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yz.colortex.cn

PHP:  file_get_contents("a.txt");
来源：http://qp.newstarts.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rl.jianghongdianzi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://by.szsharing.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fm.szxytkj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://eh.haigaiapp.cn

Ruby: File.read("a.txt")
来源：http://my.huanxung.cn

C#:   File.ReadAllText("a.txt");
来源：http://uz.lnxyls.cn

[F02] 逐行读取文件
来源：http://ir.newstarts.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ds.bookmarksfly.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vs.jctech888.com.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wg.hnjuh.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yn.shxzukj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ae.szsharing.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ks.szxytkj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cb.chemitech.net.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://om.panjiajie.cn

[F03] 写入文件（覆盖）
来源：http://yz.colortex.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://op.bjjhwx.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://qj.huixiangedu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ec.9csxet.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ru.huixiangedu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xn.colortex.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qz.huixiangedu.cn

Ruby: File.write("a.txt", "hi")
来源：http://rh.huixiangedu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hl.jianghongdianzi.cn

[F04] 追加写入文件
来源：http://we.shtwfgs.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xr.shxzukj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://my.wgjwhj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://om.bjjhwx.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vn.shxzukj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://om.lnxyls.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rr.huixinmuqiang.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://at.huanxung.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://np.hahajie.cn

[F05] 判断文件或目录是否存在
来源：http://tm.huixiangedu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dv.wgjwhj.cn

PHP:  file_exists("a.txt");
来源：http://ap.gzmigu.cn

JS:   fs.existsSync("a.txt")
来源：http://be.panjiajie.cn

TS:   fs.existsSync("a.txt")
来源：http://du.panjiajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://fk.huixinmuqiang.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zp.szsharing.cn

Ruby: File.exist?("a.txt")
来源：http://ih.jianghongdianzi.cn

C#:   File.Exists("a.txt")
来源：http://kz.gzmigu.cn

[F06] 删除文件
来源：http://nr.bjjhwx.cn

Py:   os.remove("a.txt")
来源：http://qn.nicolike.cn

PHP:  unlink("a.txt");
来源：http://sy.bjjhwx.cn

JS:   fs.unlinkSync("a.txt")
来源：http://of.szsharing.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vn.lnxyls.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yo.szsharing.cn

Go:   os.Remove("a.txt")
来源：http://rg.muxihuayi.cn

Ruby: File.delete("a.txt")
来源：http://ih.szsharing.cn

C#:   File.Delete("a.txt");
来源：http://hg.wgjwhj.cn

[F07] 创建目录（含多级）
来源：http://vw.asd995.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hg.bookmarksfly.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ar.wgjwhj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ug.asd995.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sx.bjjhwx.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://iu.shtwfgs.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ly.chemitech.net.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jq.jctech888.com.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tl.shxzskj.cn

[F08] 遍历目录
来源：http://kq.muxihuayi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://mp.chemitech.net.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cw.yuexingan06.cn

JS:   fs.readdirSync("dir")
来源：http://co.521024.cn

TS:   fs.readdirSync("dir")
来源：http://dd.szxytkj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ww.shxzskj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ei.shtwfgs.cn

Ruby: Dir.children("dir")
来源：http://el.shxzukj.cn

C#:   Directory.GetFiles("dir")
来源：http://pe.gzmigu.cn

[F09] 获取文件大小
来源：http://ac.jctech888.com.cn

Py:   os.path.getsize("a.txt")
来源：http://so.jctech888.com.cn

PHP:  filesize("a.txt");
来源：http://fv.szxytkj.cn

JS:   fs.statSync("a.txt").size
来源：http://bh.bookmarksfly.cn

TS:   fs.statSync("a.txt").size
来源：http://kv.gzmigu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://sz.yuntaijiaju.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://sh.wgjwhj.cn

Ruby: File.size("a.txt")
来源：http://aa.colortex.cn

C#:   new FileInfo("a.txt").Length
来源：http://uw.jctech888.com.cn

[F10] 取文件扩展名 / 文件名
来源：http://tn.hahajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ol.newstarts.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yf.yuexingan06.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://eh.haigaiapp.cn

TS:   path.extname("a.txt")
来源：http://gs.yuexingan06.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qz.shtwfgs.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rc.haigaiapp.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gx.shxzukj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gp.gzmigu.cn

[F11] 复制与移动文件
来源：http://ut.bjjhwx.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://sr.nicolike.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mj.hnjuh.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zc.hahajie.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sf.shtwfgs.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cc.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://il.nicolike.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://uz.colortex.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ks.colortex.cn

[F12] CSV 读写
来源：http://yl.jianghongdianzi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fn.chemitech.net.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xz.9csxet.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yk.gzmigu.cn

TS:   // 同上
来源：http://ot.bjjhwx.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qc.nszjky.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bd.chemitech.net.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ru.gzmigu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://zn.panjiajie.cn

================================================================================
来源：http://cv.szxytkj.cn

G. 面向对象
来源：http://eg.521024.cn

================================================================================
来源：http://ew.szxytkj.cn

[G01] 定义类
来源：http://dy.bookmarksfly.cn

Py:   class User: pass
来源：http://av.9csxet.cn

PHP:  class User {}
来源：http://zd.bookmarksfly.cn

JS:   class User {}
来源：http://jn.yuntaijiaju.cn

TS:   class User { name: string = ""; }
来源：http://pe.hnjuh.cn

Java: class User {}
来源：http://ny.hnjuh.cn

Go:   type User struct { Name string }
来源：http://yo.muxihuayi.cn

Ruby: class User; end
来源：http://an.szxytkj.cn

C#:   class User {}
来源：http://bb.chemitech.net.cn

[G02] 构造函数
来源：http://zn.haigaiapp.cn

Py:   def __init__(self, name): self.name = name
来源：http://er.chemitech.net.cn

PHP:  public function __construct(public string $name) {}
来源：http://tv.9csxet.cn

JS:   constructor(name) { this.name = name; }
来源：http://yk.9csxet.cn

TS:   constructor(public name: string) {}
来源：http://ie.huanxung.cn

Java: User(String name) { this.name = name; }
来源：http://xe.shtwfgs.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wq.hnjuh.cn

Ruby: def initialize(name); @name = name; end
来源：http://tk.panjiajie.cn

C#:   public User(string name) { Name = name; }
来源：http://wv.shxzukj.cn

[G03] 实例属性
来源：http://de.gzmigu.cn

Py:   self.name = "x"
来源：http://lx.szxytkj.cn

PHP:  public string $name = "x";
来源：http://dn.bookmarksfly.cn

JS:   this.name = "x";
来源：http://am.huixiangedu.cn

TS:   name: string = "x";
来源：http://ae.yuntaijiaju.cn

Java: private String name;
来源：http://tr.bookmarksfly.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pj.nicolike.cn

Ruby: @name = "x"
来源：http://fi.hahajie.cn

C#:   public string Name { get; set; } = "x";
来源：http://mo.521024.cn

[G04] 定义方法
来源：http://pk.szxytkj.cn

Py:   def greet(self): return self.name
来源：http://gw.jianghongdianzi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://vo.bjjhwx.cn

JS:   greet() { return this.name; }
来源：http://aq.yuntaijiaju.cn

TS:   greet(): string { return this.name; }
来源：http://bn.chemitech.net.cn

Java: String greet() { return name; }
来源：http://ky.muxihuayi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qv.shtwfgs.cn

Ruby: def greet; @name; end
来源：http://gu.521024.cn

C#:   public string Greet() => Name;
来源：http://tb.lnxyls.cn

[G05] 继承
来源：http://go.wgjwhj.cn


<!-- 参考信息 -->