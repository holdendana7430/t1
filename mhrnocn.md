代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://tc.jctech888.com.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://py.haigaiapp.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vd.haigaiapp.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ez.nszjky.cn

C#:   s.Replace("a", "b")
来源：http://uf.gzmigu.cn

[E07] 按分隔符拆分
来源：http://xn.panjiajie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://an.huanxung.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://av.huixiangedu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://zm.521024.cn

TS:   s.split(",")
来源：http://nz.newstarts.cn

Java: s.split(",");  s.split("\\s+")
来源：http://lq.hnjuh.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qu.gzmigu.cn

Ruby: s.split(",");  s.split
来源：http://yl.wgjwhj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qx.jianghongdianzi.cn

[E08] 数组按分隔符合并
来源：http://ko.521024.cn

Py:   ",".join(items)
来源：http://ex.nszjky.cn

PHP:  implode(",", $items);
来源：http://jw.muxihuayi.cn

JS:   items.join(",")
来源：http://xv.shxzskj.cn

TS:   items.join(",")
来源：http://ad.nicolike.cn

Java: String.join(",", items)
来源：http://gn.nicolike.cn

Go:   strings.Join(items, ",")
来源：http://ds.szxytkj.cn

Ruby: items.join(",")
来源：http://gg.colortex.cn

C#:   string.Join(",", items)
来源：http://cs.wgjwhj.cn

[E09] 去除所有空白字符
来源：http://jx.nicolike.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://co.hahajie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kf.asd995.cn

JS:   s.replace(/\s+/g, "")
来源：http://oi.nicolike.cn

TS:   s.replace(/\s+/g, "")
来源：http://sn.shxzukj.cn

Java: s.replaceAll("\\s+", "")
来源：http://ho.muxihuayi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ab.asd995.cn

Ruby: s.gsub(/\s+/, "")
来源：http://th.chemitech.net.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xy.bjjhwx.cn

[E10] 左侧补零 / 定长填充
来源：http://fk.huixinmuqiang.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cw.jctech888.com.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cc.521024.cn

JS:   "7".padStart(3, "0")
来源：http://xk.huanxung.cn

TS:   "7".padStart(3, "0")
来源：http://vw.521024.cn

Java: String.format("%03d", 7)
来源：http://av.nicolike.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ef.muxihuayi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qy.jctech888.com.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pq.hnjuh.cn

[E11] 反转字符串
来源：http://my.lnxyls.cn

Py:   s[::-1]
来源：http://ux.szsharing.cn

PHP:  strrev($s);
来源：http://zd.yuexingan06.cn

JS:   [...s].reverse().join("")
来源：http://qo.huixinmuqiang.cn

TS:   [...s].reverse().join("")
来源：http://mw.szxytkj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://mk.jctech888.com.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://yn.jianghongdianzi.cn

Ruby: s.reverse
来源：http://nn.muxihuayi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://yi.hnjuh.cn

[E12] 统计某字符出现次数
来源：http://fq.nicolike.cn

Py:   s.count("a")
来源：http://qr.gzmigu.cn

PHP:  substr_count($s, "a");
来源：http://qp.jianghongdianzi.cn

JS:   s.split("a").length - 1
来源：http://fb.shxzskj.cn

TS:   s.split("a").length - 1
来源：http://hg.panjiajie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fm.yuexingan06.cn

Go:   strings.Count(s, "a")
来源：http://at.9csxet.cn

Ruby: s.count("a")
来源：http://pn.lnxyls.cn

C#:   s.Count(c => c == 'a')
来源：http://so.yuexingan06.cn

[E13] 逐字符遍历
来源：http://ro.lnxyls.cn

Py:   for ch in s: print(ch)
来源：http://ao.wgjwhj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ac.bookmarksfly.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ba.shxzskj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://db.yuexingan06.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lv.bjjhwx.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rx.gzmigu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ko.szsharing.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://eh.nszjky.cn

[E14] URL 编码与 Base64
来源：http://uj.nszjky.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hs.nszjky.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://fb.panjiajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xl.panjiajie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mj.szxytkj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gj.huixinmuqiang.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ur.huixiangedu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fj.newstarts.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sv.lnxyls.cn

[E15] HTML 转义 / 反转义
来源：http://bg.huixinmuqiang.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://zr.jctech888.com.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ml.shtwfgs.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://os.yuntaijiaju.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://pq.huixinmuqiang.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kd.huixiangedu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xe.shtwfgs.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bc.jianghongdianzi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qx.colortex.cn

[E16] 数字千分位
来源：http://vm.bjjhwx.cn

Py:   f"{1234567:,}"
来源：http://qv.hahajie.cn

PHP:  number_format(1234567);
来源：http://js.bookmarksfly.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://al.muxihuayi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://yx.muxihuayi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ed.huixiangedu.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rr.shxzskj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mp.gzmigu.cn

C#:   1234567.ToString("N0")
来源：http://lu.newstarts.cn

[E17] 首字母大写
来源：http://gy.asd995.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nj.gzmigu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ga.yuntaijiaju.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://eq.nicolike.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cr.asd995.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gt.9csxet.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wd.huixinmuqiang.cn

Ruby: s.capitalize
来源：http://jm.haigaiapp.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://eh.huanxung.cn

[E18] 模板占位符替换
来源：http://xc.jctech888.com.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sp.szxytkj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lc.lnxyls.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://wh.chemitech.net.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://mh.colortex.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bv.huanxung.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wq.yuntaijiaju.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://oi.szxytkj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ax.shtwfgs.cn

[E19] 多行文本按行拆分
来源：http://qx.9csxet.cn

Py:   s.splitlines()
来源：http://pq.szsharing.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ht.shxzukj.cn

JS:   s.split(/\r?\n/)
来源：http://sh.shtwfgs.cn

TS:   s.split(/\r?\n/)
来源：http://tj.haigaiapp.cn

Java: s.lines().toList()
来源：http://mt.shxzskj.cn

Go:   strings.Split(s, "\n")
来源：http://fr.huixiangedu.cn

Ruby: s.lines
来源：http://hc.huixinmuqiang.cn

C#:   s.Split('\n')
来源：http://cp.wgjwhj.cn

[E20] 判断字符串是否为空
来源：http://qf.chemitech.net.cn

Py:   if not s:
来源：http://yy.huanxung.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://oa.szsharing.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fh.colortex.cn

TS:   if (s === "") {}
来源：http://zd.shxzukj.cn

Java: if (s.isEmpty()) {}
来源：http://oq.muxihuayi.cn

Go:   if s == "" {}
来源：http://av.shxzskj.cn

Ruby: if s.empty?
来源：http://hl.shxzskj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://in.asd995.cn

[E21] 超长截断加省略号
来源：http://cz.szsharing.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ak.chemitech.net.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ei.newstarts.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yz.gzmigu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yu.nicolike.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dc.lnxyls.cn

Go:   // 按 rune 判断长度后截断
来源：http://fr.nicolike.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hp.bookmarksfly.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pt.shxzukj.cn

[E22] 字节长度与字符长度
来源：http://de.szsharing.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bn.bookmarksfly.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wn.szsharing.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://af.jctech888.com.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mo.haigaiapp.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://db.wgjwhj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://so.haigaiapp.cn

Ruby: s.bytesize;  s.length
来源：http://ps.gzmigu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mk.jianghongdianzi.cn

================================================================================
来源：http://dt.haigaiapp.cn

F. 文件与目录
来源：http://bc.shxzskj.cn

================================================================================
来源：http://pz.shxzukj.cn

[F01] 读取整个文件
来源：http://hg.bookmarksfly.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fl.nicolike.cn

PHP:  file_get_contents("a.txt");
来源：http://dr.shxzskj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rj.521024.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gu.nicolike.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vo.9csxet.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://va.wgjwhj.cn

Ruby: File.read("a.txt")
来源：http://qv.muxihuayi.cn

C#:   File.ReadAllText("a.txt");
来源：http://rg.muxihuayi.cn

[F02] 逐行读取文件
来源：http://ce.newstarts.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://eq.huixiangedu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://an.haigaiapp.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yj.bookmarksfly.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://si.chemitech.net.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wh.chemitech.net.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vd.jianghongdianzi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hc.yuexingan06.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://al.huanxung.cn

[F03] 写入文件（覆盖）
来源：http://lh.huixinmuqiang.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ig.9csxet.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vy.chemitech.net.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zc.hahajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dk.hnjuh.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dl.shxzukj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pa.asd995.cn

Ruby: File.write("a.txt", "hi")
来源：http://lj.muxihuayi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yg.shtwfgs.cn

[F04] 追加写入文件
来源：http://dz.shtwfgs.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yy.bjjhwx.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ky.gzmigu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yz.asd995.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ck.szsharing.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ms.hahajie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ek.nicolike.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fr.huixiangedu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zq.haigaiapp.cn

[F05] 判断文件或目录是否存在
来源：http://on.bookmarksfly.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gv.jianghongdianzi.cn

PHP:  file_exists("a.txt");
来源：http://wx.huixiangedu.cn

JS:   fs.existsSync("a.txt")
来源：http://li.jctech888.com.cn

TS:   fs.existsSync("a.txt")
来源：http://tk.521024.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ch.colortex.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lw.yuexingan06.cn

Ruby: File.exist?("a.txt")
来源：http://ip.bookmarksfly.cn

C#:   File.Exists("a.txt")
来源：http://sb.huanxung.cn

[F06] 删除文件
来源：http://zx.yuntaijiaju.cn

Py:   os.remove("a.txt")
来源：http://ob.nszjky.cn

PHP:  unlink("a.txt");
来源：http://mj.shtwfgs.cn

JS:   fs.unlinkSync("a.txt")
来源：http://gf.szsharing.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vc.hnjuh.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ob.shtwfgs.cn

Go:   os.Remove("a.txt")
来源：http://py.panjiajie.cn

Ruby: File.delete("a.txt")
来源：http://ao.asd995.cn

C#:   File.Delete("a.txt");
来源：http://yb.shxzukj.cn

[F07] 创建目录（含多级）
来源：http://aw.szsharing.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rj.newstarts.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nt.lnxyls.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iz.wgjwhj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ea.haigaiapp.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wc.shxzukj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mh.gzmigu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ba.bookmarksfly.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://do.wgjwhj.cn

[F08] 遍历目录
来源：http://qw.haigaiapp.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://tl.chemitech.net.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mm.asd995.cn

JS:   fs.readdirSync("dir")
来源：http://yy.shtwfgs.cn

TS:   fs.readdirSync("dir")
来源：http://kd.wgjwhj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lv.szxytkj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://xq.haigaiapp.cn

Ruby: Dir.children("dir")
来源：http://kh.shxzskj.cn

C#:   Directory.GetFiles("dir")
来源：http://ta.huixiangedu.cn

[F09] 获取文件大小
来源：http://rb.szsharing.cn

Py:   os.path.getsize("a.txt")
来源：http://uc.shtwfgs.cn

PHP:  filesize("a.txt");
来源：http://ay.521024.cn

JS:   fs.statSync("a.txt").size
来源：http://ry.bookmarksfly.cn

TS:   fs.statSync("a.txt").size
来源：http://im.bjjhwx.cn

Java: Files.size(Path.of("a.txt"))
来源：http://os.shxzskj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qd.jctech888.com.cn

Ruby: File.size("a.txt")
来源：http://vn.shxzukj.cn

C#:   new FileInfo("a.txt").Length
来源：http://ix.9csxet.cn

[F10] 取文件扩展名 / 文件名
来源：http://lb.muxihuayi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rj.shxzukj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hc.panjiajie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ql.hahajie.cn

TS:   path.extname("a.txt")
来源：http://vq.shxzukj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zz.muxihuayi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zk.hahajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nk.hahajie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vb.9csxet.cn

[F11] 复制与移动文件
来源：http://im.bookmarksfly.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zb.gzmigu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://io.jctech888.com.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ln.huixiangedu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lg.panjiajie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ul.huanxung.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ni.haigaiapp.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hi.lnxyls.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gt.huixinmuqiang.cn

[F12] CSV 读写
来源：http://ij.521024.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ir.jctech888.com.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://is.nszjky.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xw.bjjhwx.cn

TS:   // 同上
来源：http://eo.asd995.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kf.nicolike.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cm.huanxung.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wp.shxzukj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://vw.bookmarksfly.cn

================================================================================
来源：http://xg.huixiangedu.cn

G. 面向对象
来源：http://ld.bjjhwx.cn

================================================================================
来源：http://ez.panjiajie.cn

[G01] 定义类
来源：http://im.huixinmuqiang.cn

Py:   class User: pass
来源：http://jr.shxzskj.cn

PHP:  class User {}
来源：http://wa.jianghongdianzi.cn

JS:   class User {}
来源：http://ac.yuexingan06.cn

TS:   class User { name: string = ""; }
来源：http://vq.jianghongdianzi.cn

Java: class User {}
来源：http://uk.hahajie.cn

Go:   type User struct { Name string }
来源：http://np.jctech888.com.cn

Ruby: class User; end
来源：http://gm.haigaiapp.cn

C#:   class User {}
来源：http://mc.jianghongdianzi.cn

[G02] 构造函数
来源：http://ai.shxzukj.cn

Py:   def __init__(self, name): self.name = name
来源：http://xj.bjjhwx.cn

PHP:  public function __construct(public string $name) {}
来源：http://kp.colortex.cn

JS:   constructor(name) { this.name = name; }
来源：http://tx.bookmarksfly.cn

TS:   constructor(public name: string) {}
来源：http://lp.yuexingan06.cn

Java: User(String name) { this.name = name; }
来源：http://pa.colortex.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pl.huanxung.cn

Ruby: def initialize(name); @name = name; end
来源：http://fs.hnjuh.cn

C#:   public User(string name) { Name = name; }
来源：http://em.yuntaijiaju.cn

[G03] 实例属性
来源：http://yd.lnxyls.cn

Py:   self.name = "x"
来源：http://gh.shxzukj.cn

PHP:  public string $name = "x";
来源：http://cq.nicolike.cn

JS:   this.name = "x";
来源：http://on.colortex.cn

TS:   name: string = "x";
来源：http://vo.shtwfgs.cn

Java: private String name;
来源：http://iy.newstarts.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://py.colortex.cn

Ruby: @name = "x"
来源：http://oe.gzmigu.cn

C#:   public string Name { get; set; } = "x";
来源：http://ut.chemitech.net.cn

[G04] 定义方法
来源：http://de.asd995.cn

Py:   def greet(self): return self.name
来源：http://xx.hnjuh.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://gn.chemitech.net.cn

JS:   greet() { return this.name; }
来源：http://ga.bjjhwx.cn

TS:   greet(): string { return this.name; }
来源：http://uk.szsharing.cn

Java: String greet() { return name; }
来源：http://nt.szxytkj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://oj.huixinmuqiang.cn

Ruby: def greet; @name; end
来源：http://xx.bjjhwx.cn

C#:   public string Greet() => Name;
来源：http://bj.jctech888.com.cn

[G05] 继承
来源：http://ye.panjiajie.cn


<!-- 参考信息 -->