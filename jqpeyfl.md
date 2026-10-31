代发 wailian999

[E06] 替换子串
来源：http://wy.chemitech.net.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ze.nszjky.cn

PHP:  str_replace("a", "b", $s);
来源：http://by.shxzskj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wn.yuntaijiaju.cn

TS:   s.replaceAll("a", "b")
来源：http://ef.9csxet.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qs.shxzskj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vb.521024.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ea.jctech888.com.cn

C#:   s.Replace("a", "b")
来源：http://ip.jianghongdianzi.cn

[E07] 按分隔符拆分
来源：http://ml.colortex.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cw.wgjwhj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://is.huanxung.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://xd.gzmigu.cn

TS:   s.split(",")
来源：http://hl.gzmigu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://sb.hnjuh.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ga.bookmarksfly.cn

Ruby: s.split(",");  s.split
来源：http://fu.newstarts.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://oe.bjjhwx.cn

[E08] 数组按分隔符合并
来源：http://jr.yuexingan06.cn

Py:   ",".join(items)
来源：http://jz.yuntaijiaju.cn

PHP:  implode(",", $items);
来源：http://pd.asd995.cn

JS:   items.join(",")
来源：http://ix.gzmigu.cn

TS:   items.join(",")
来源：http://wt.panjiajie.cn

Java: String.join(",", items)
来源：http://xb.bjjhwx.cn

Go:   strings.Join(items, ",")
来源：http://wf.newstarts.cn

Ruby: items.join(",")
来源：http://rt.bjjhwx.cn

C#:   string.Join(",", items)
来源：http://jm.huanxung.cn

[E09] 去除所有空白字符
来源：http://oc.hahajie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://yq.shxzukj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cm.chemitech.net.cn

JS:   s.replace(/\s+/g, "")
来源：http://ad.shxzskj.cn

TS:   s.replace(/\s+/g, "")
来源：http://zk.shxzskj.cn

Java: s.replaceAll("\\s+", "")
来源：http://ay.jctech888.com.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://xm.shxzukj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xk.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kd.wgjwhj.cn

[E10] 左侧补零 / 定长填充
来源：http://md.bjjhwx.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ya.shtwfgs.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ln.yuntaijiaju.cn

JS:   "7".padStart(3, "0")
来源：http://bm.521024.cn

TS:   "7".padStart(3, "0")
来源：http://jg.huixiangedu.cn

Java: String.format("%03d", 7)
来源：http://mh.wgjwhj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ev.521024.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://oe.asd995.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ks.shxzukj.cn

[E11] 反转字符串
来源：http://gw.haigaiapp.cn

Py:   s[::-1]
来源：http://vs.bjjhwx.cn

PHP:  strrev($s);
来源：http://xa.shxzskj.cn

JS:   [...s].reverse().join("")
来源：http://uz.muxihuayi.cn

TS:   [...s].reverse().join("")
来源：http://wa.hnjuh.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ld.nicolike.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://xi.nszjky.cn

Ruby: s.reverse
来源：http://ln.521024.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ol.lnxyls.cn

[E12] 统计某字符出现次数
来源：http://ym.bjjhwx.cn

Py:   s.count("a")
来源：http://dn.asd995.cn

PHP:  substr_count($s, "a");
来源：http://bf.muxihuayi.cn

JS:   s.split("a").length - 1
来源：http://qu.nszjky.cn

TS:   s.split("a").length - 1
来源：http://bs.nszjky.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kt.huixinmuqiang.cn

Go:   strings.Count(s, "a")
来源：http://gv.yuexingan06.cn

Ruby: s.count("a")
来源：http://ek.hnjuh.cn

C#:   s.Count(c => c == 'a')
来源：http://ae.521024.cn

[E13] 逐字符遍历
来源：http://xg.yuntaijiaju.cn

Py:   for ch in s: print(ch)
来源：http://yw.huixinmuqiang.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://uz.hahajie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://yx.newstarts.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ru.521024.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://go.521024.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lw.bookmarksfly.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://mp.lnxyls.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://sk.shxzskj.cn

[E14] URL 编码与 Base64
来源：http://hk.jctech888.com.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rh.huixiangedu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://yf.yuntaijiaju.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ul.huanxung.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yo.panjiajie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mq.lnxyls.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ov.colortex.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qc.asd995.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yt.hahajie.cn

[E15] HTML 转义 / 反转义
来源：http://dy.shtwfgs.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xw.asd995.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ao.jianghongdianzi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bi.huixiangedu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://yg.szxytkj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ju.asd995.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ul.colortex.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qk.wgjwhj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qn.wgjwhj.cn

[E16] 数字千分位
来源：http://yv.bjjhwx.cn

Py:   f"{1234567:,}"
来源：http://wg.bjjhwx.cn

PHP:  number_format(1234567);
来源：http://pu.asd995.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://hs.jianghongdianzi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://qn.panjiajie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vx.shxzskj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lc.bjjhwx.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dl.nszjky.cn

C#:   1234567.ToString("N0")
来源：http://zz.panjiajie.cn

[E17] 首字母大写
来源：http://ur.9csxet.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wh.jianghongdianzi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://uf.bookmarksfly.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kz.shxzskj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://no.lnxyls.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://le.yuntaijiaju.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lr.lnxyls.cn

Ruby: s.capitalize
来源：http://mw.shxzskj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rm.yuexingan06.cn

[E18] 模板占位符替换
来源：http://pp.huanxung.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gq.hahajie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jx.hnjuh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://lq.newstarts.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ns.521024.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gr.haigaiapp.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://or.yuntaijiaju.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://em.gzmigu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kt.colortex.cn

[E19] 多行文本按行拆分
来源：http://gt.colortex.cn

Py:   s.splitlines()
来源：http://wl.chemitech.net.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wk.huixiangedu.cn

JS:   s.split(/\r?\n/)
来源：http://ah.hahajie.cn

TS:   s.split(/\r?\n/)
来源：http://vo.bookmarksfly.cn

Java: s.lines().toList()
来源：http://vz.yuexingan06.cn

Go:   strings.Split(s, "\n")
来源：http://fm.asd995.cn

Ruby: s.lines
来源：http://gr.newstarts.cn

C#:   s.Split('\n')
来源：http://nn.yuexingan06.cn

[E20] 判断字符串是否为空
来源：http://by.huixinmuqiang.cn

Py:   if not s:
来源：http://pf.shxzskj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zh.gzmigu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ra.9csxet.cn

TS:   if (s === "") {}
来源：http://za.muxihuayi.cn

Java: if (s.isEmpty()) {}
来源：http://ef.nicolike.cn

Go:   if s == "" {}
来源：http://km.newstarts.cn

Ruby: if s.empty?
来源：http://fz.chemitech.net.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bj.nszjky.cn

[E21] 超长截断加省略号
来源：http://fm.lnxyls.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://by.shtwfgs.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cg.asd995.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sv.lnxyls.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bv.colortex.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ro.yuexingan06.cn

Go:   // 按 rune 判断长度后截断
来源：http://er.9csxet.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lo.huixinmuqiang.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tf.jianghongdianzi.cn

[E22] 字节长度与字符长度
来源：http://kc.szsharing.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nt.jctech888.com.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ra.lnxyls.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cr.hahajie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dh.hahajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sy.nicolike.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xf.yuexingan06.cn

Ruby: s.bytesize;  s.length
来源：http://jk.yuntaijiaju.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vb.huanxung.cn

================================================================================
来源：http://pr.szxytkj.cn

F. 文件与目录
来源：http://el.haigaiapp.cn

================================================================================
来源：http://dn.jianghongdianzi.cn

[F01] 读取整个文件
来源：http://ee.asd995.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hf.huixiangedu.cn

PHP:  file_get_contents("a.txt");
来源：http://xu.asd995.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mt.hnjuh.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pe.jctech888.com.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ok.wgjwhj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vg.chemitech.net.cn

Ruby: File.read("a.txt")
来源：http://em.nszjky.cn

C#:   File.ReadAllText("a.txt");
来源：http://uj.haigaiapp.cn

[F02] 逐行读取文件
来源：http://ns.hnjuh.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://eq.panjiajie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://re.shxzukj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://le.shxzukj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fl.yuexingan06.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ka.521024.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ov.9csxet.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ds.szxytkj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://na.chemitech.net.cn

[F03] 写入文件（覆盖）
来源：http://mx.bookmarksfly.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ku.nszjky.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://im.521024.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kv.jianghongdianzi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tc.panjiajie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qe.asd995.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cb.szsharing.cn

Ruby: File.write("a.txt", "hi")
来源：http://lb.asd995.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xu.bjjhwx.cn

[F04] 追加写入文件
来源：http://jr.shtwfgs.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://du.hnjuh.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ni.shxzskj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ih.muxihuayi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yc.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mg.wgjwhj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ra.bookmarksfly.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fm.521024.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jt.muxihuayi.cn

[F05] 判断文件或目录是否存在
来源：http://gp.9csxet.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yd.shxzukj.cn

PHP:  file_exists("a.txt");
来源：http://zn.haigaiapp.cn

JS:   fs.existsSync("a.txt")
来源：http://mu.bookmarksfly.cn

TS:   fs.existsSync("a.txt")
来源：http://ln.yuntaijiaju.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qm.hnjuh.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pb.shxzukj.cn

Ruby: File.exist?("a.txt")
来源：http://pv.muxihuayi.cn

C#:   File.Exists("a.txt")
来源：http://hu.bookmarksfly.cn

[F06] 删除文件
来源：http://se.yuntaijiaju.cn

Py:   os.remove("a.txt")
来源：http://qf.wgjwhj.cn

PHP:  unlink("a.txt");
来源：http://sc.huixinmuqiang.cn

JS:   fs.unlinkSync("a.txt")
来源：http://nk.lnxyls.cn

TS:   fs.unlinkSync("a.txt")
来源：http://tz.hahajie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fp.nszjky.cn

Go:   os.Remove("a.txt")
来源：http://op.jctech888.com.cn

Ruby: File.delete("a.txt")
来源：http://uo.wgjwhj.cn

C#:   File.Delete("a.txt");
来源：http://nj.shxzukj.cn

[F07] 创建目录（含多级）
来源：http://pr.jianghongdianzi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ij.9csxet.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ck.bookmarksfly.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lp.huixinmuqiang.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xe.colortex.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zi.huixinmuqiang.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nm.newstarts.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://sr.shxzskj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ex.gzmigu.cn

[F08] 遍历目录
来源：http://uq.asd995.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://pj.bjjhwx.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xi.huixinmuqiang.cn

JS:   fs.readdirSync("dir")
来源：http://kg.huanxung.cn

TS:   fs.readdirSync("dir")
来源：http://vo.szsharing.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mp.colortex.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://az.yuexingan06.cn

Ruby: Dir.children("dir")
来源：http://vf.hnjuh.cn

C#:   Directory.GetFiles("dir")
来源：http://hr.shtwfgs.cn

[F09] 获取文件大小
来源：http://jf.muxihuayi.cn

Py:   os.path.getsize("a.txt")
来源：http://fn.huanxung.cn

PHP:  filesize("a.txt");
来源：http://hp.shxzukj.cn

JS:   fs.statSync("a.txt").size
来源：http://ox.newstarts.cn

TS:   fs.statSync("a.txt").size
来源：http://ze.haigaiapp.cn

Java: Files.size(Path.of("a.txt"))
来源：http://rl.wgjwhj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fu.szsharing.cn

Ruby: File.size("a.txt")
来源：http://kg.shxzukj.cn

C#:   new FileInfo("a.txt").Length
来源：http://vw.jianghongdianzi.cn

[F10] 取文件扩展名 / 文件名
来源：http://lt.shxzskj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vv.lnxyls.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cm.newstarts.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ou.chemitech.net.cn

TS:   path.extname("a.txt")
来源：http://cq.521024.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gg.hahajie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dv.nicolike.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wp.huanxung.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xk.panjiajie.cn

[F11] 复制与移动文件
来源：http://vy.wgjwhj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cl.shxzukj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cf.shtwfgs.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nu.shtwfgs.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://be.wgjwhj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gx.9csxet.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dp.asd995.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xl.nicolike.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ki.jianghongdianzi.cn

[F12] CSV 读写
来源：http://fv.bookmarksfly.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lr.nszjky.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lu.huixinmuqiang.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kl.yuntaijiaju.cn

TS:   // 同上
来源：http://bh.nicolike.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vl.yuexingan06.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zg.jianghongdianzi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ab.521024.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ts.nszjky.cn

================================================================================
来源：http://zw.shtwfgs.cn

G. 面向对象
来源：http://ki.wgjwhj.cn

================================================================================
来源：http://ds.huixiangedu.cn

[G01] 定义类
来源：http://jk.huanxung.cn

Py:   class User: pass
来源：http://qs.yuntaijiaju.cn

PHP:  class User {}
来源：http://rf.lnxyls.cn

JS:   class User {}
来源：http://ad.asd995.cn

TS:   class User { name: string = ""; }
来源：http://nw.shtwfgs.cn

Java: class User {}
来源：http://bs.yuexingan06.cn

Go:   type User struct { Name string }
来源：http://cq.hnjuh.cn

Ruby: class User; end
来源：http://sg.muxihuayi.cn

C#:   class User {}
来源：http://iu.huixiangedu.cn

[G02] 构造函数
来源：http://zl.wgjwhj.cn

Py:   def __init__(self, name): self.name = name
来源：http://gk.asd995.cn

PHP:  public function __construct(public string $name) {}
来源：http://br.panjiajie.cn

JS:   constructor(name) { this.name = name; }
来源：http://nq.newstarts.cn

TS:   constructor(public name: string) {}
来源：http://an.haigaiapp.cn

Java: User(String name) { this.name = name; }
来源：http://tr.9csxet.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://er.szxytkj.cn

Ruby: def initialize(name); @name = name; end
来源：http://gp.jianghongdianzi.cn

C#:   public User(string name) { Name = name; }
来源：http://ut.shxzskj.cn

[G03] 实例属性
来源：http://fy.panjiajie.cn

Py:   self.name = "x"
来源：http://my.haigaiapp.cn

PHP:  public string $name = "x";
来源：http://hm.nicolike.cn

JS:   this.name = "x";
来源：http://hz.9csxet.cn

TS:   name: string = "x";
来源：http://uj.panjiajie.cn

Java: private String name;
来源：http://yn.yuexingan06.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ve.huanxung.cn

Ruby: @name = "x"
来源：http://ew.gzmigu.cn

C#:   public string Name { get; set; } = "x";
来源：http://hs.asd995.cn

[G04] 定义方法
来源：http://tk.521024.cn

Py:   def greet(self): return self.name
来源：http://hx.haigaiapp.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ij.lnxyls.cn

JS:   greet() { return this.name; }
来源：http://iz.lnxyls.cn

TS:   greet(): string { return this.name; }
来源：http://be.muxihuayi.cn

Java: String greet() { return name; }
来源：http://fq.hnjuh.cn


<!-- 参考信息 -->