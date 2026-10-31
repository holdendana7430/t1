代发 wailian999

[E06] 替换子串
来源：http://cn.shxzukj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jg.nicolike.cn

PHP:  str_replace("a", "b", $s);
来源：http://pq.nszjky.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lb.shxzskj.cn

TS:   s.replaceAll("a", "b")
来源：http://ob.haigaiapp.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xd.wgjwhj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://iv.bookmarksfly.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zc.newstarts.cn

C#:   s.Replace("a", "b")
来源：http://ml.shxzskj.cn

[E07] 按分隔符拆分
来源：http://oq.huanxung.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://av.asd995.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jh.haigaiapp.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://cx.9csxet.cn

TS:   s.split(",")
来源：http://kg.shxzskj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://vp.colortex.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://td.yuexingan06.cn

Ruby: s.split(",");  s.split
来源：http://xv.lnxyls.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jv.shxzukj.cn

[E08] 数组按分隔符合并
来源：http://ca.panjiajie.cn

Py:   ",".join(items)
来源：http://kh.haigaiapp.cn

PHP:  implode(",", $items);
来源：http://an.huixinmuqiang.cn

JS:   items.join(",")
来源：http://ch.hahajie.cn

TS:   items.join(",")
来源：http://gk.hnjuh.cn

Java: String.join(",", items)
来源：http://wt.szsharing.cn

Go:   strings.Join(items, ",")
来源：http://bg.huixinmuqiang.cn

Ruby: items.join(",")
来源：http://sn.yuntaijiaju.cn

C#:   string.Join(",", items)
来源：http://hp.yuexingan06.cn

[E09] 去除所有空白字符
来源：http://wm.szsharing.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gy.yuntaijiaju.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qa.lnxyls.cn

JS:   s.replace(/\s+/g, "")
来源：http://cw.shxzskj.cn

TS:   s.replace(/\s+/g, "")
来源：http://kp.shxzukj.cn

Java: s.replaceAll("\\s+", "")
来源：http://ja.huixinmuqiang.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ei.szsharing.cn

Ruby: s.gsub(/\s+/, "")
来源：http://eo.nicolike.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qy.chemitech.net.cn

[E10] 左侧补零 / 定长填充
来源：http://tt.asd995.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ny.szxytkj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://os.yuntaijiaju.cn

JS:   "7".padStart(3, "0")
来源：http://zz.yuexingan06.cn

TS:   "7".padStart(3, "0")
来源：http://gk.nszjky.cn

Java: String.format("%03d", 7)
来源：http://tm.nszjky.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://co.haigaiapp.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vp.nszjky.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vd.newstarts.cn

[E11] 反转字符串
来源：http://vi.szsharing.cn

Py:   s[::-1]
来源：http://ge.jianghongdianzi.cn

PHP:  strrev($s);
来源：http://tw.hahajie.cn

JS:   [...s].reverse().join("")
来源：http://dh.asd995.cn

TS:   [...s].reverse().join("")
来源：http://pa.muxihuayi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://od.szxytkj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://xc.hnjuh.cn

Ruby: s.reverse
来源：http://bp.asd995.cn

C#:   new string(s.Reverse().ToArray())
来源：http://hj.nicolike.cn

[E12] 统计某字符出现次数
来源：http://dd.bookmarksfly.cn

Py:   s.count("a")
来源：http://nd.muxihuayi.cn

PHP:  substr_count($s, "a");
来源：http://uk.newstarts.cn

JS:   s.split("a").length - 1
来源：http://cd.yuntaijiaju.cn

TS:   s.split("a").length - 1
来源：http://iv.9csxet.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://io.521024.cn

Go:   strings.Count(s, "a")
来源：http://jr.jctech888.com.cn

Ruby: s.count("a")
来源：http://kq.szxytkj.cn

C#:   s.Count(c => c == 'a')
来源：http://ea.newstarts.cn

[E13] 逐字符遍历
来源：http://rc.bookmarksfly.cn

Py:   for ch in s: print(ch)
来源：http://qj.lnxyls.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mi.panjiajie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://hg.nszjky.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://yg.haigaiapp.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qz.haigaiapp.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ay.huixinmuqiang.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rg.shxzskj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://io.asd995.cn

[E14] URL 编码与 Base64
来源：http://hy.nicolike.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jm.haigaiapp.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://is.wgjwhj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ro.bjjhwx.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sj.shxzukj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qv.gzmigu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qk.panjiajie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dn.huixinmuqiang.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ij.haigaiapp.cn

[E15] HTML 转义 / 反转义
来源：http://ai.lnxyls.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://sp.lnxyls.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jb.bjjhwx.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://li.huixinmuqiang.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://qz.bookmarksfly.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ms.lnxyls.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uk.shxzskj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tl.bookmarksfly.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dy.hahajie.cn

[E16] 数字千分位
来源：http://jk.nszjky.cn

Py:   f"{1234567:,}"
来源：http://hc.szsharing.cn

PHP:  number_format(1234567);
来源：http://tg.jctech888.com.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://xh.shxzskj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://yi.szxytkj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lx.lnxyls.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mb.asd995.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://if.jianghongdianzi.cn

C#:   1234567.ToString("N0")
来源：http://aw.yuntaijiaju.cn

[E17] 首字母大写
来源：http://yi.panjiajie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ig.newstarts.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://pv.colortex.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://db.shxzukj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jo.szsharing.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bv.newstarts.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gq.huanxung.cn

Ruby: s.capitalize
来源：http://ap.bjjhwx.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qb.shtwfgs.cn

[E18] 模板占位符替换
来源：http://tl.yuntaijiaju.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dq.lnxyls.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mz.asd995.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://dc.521024.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://el.yuexingan06.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://oh.hahajie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kc.521024.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hg.huixiangedu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.bjjhwx.cn

[E19] 多行文本按行拆分
来源：http://ax.lnxyls.cn

Py:   s.splitlines()
来源：http://xo.newstarts.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hy.jianghongdianzi.cn

JS:   s.split(/\r?\n/)
来源：http://ym.panjiajie.cn

TS:   s.split(/\r?\n/)
来源：http://is.hahajie.cn

Java: s.lines().toList()
来源：http://kl.nszjky.cn

Go:   strings.Split(s, "\n")
来源：http://qa.gzmigu.cn

Ruby: s.lines
来源：http://sc.asd995.cn

C#:   s.Split('\n')
来源：http://um.wgjwhj.cn

[E20] 判断字符串是否为空
来源：http://fr.asd995.cn

Py:   if not s:
来源：http://hh.521024.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vz.yuntaijiaju.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rw.asd995.cn

TS:   if (s === "") {}
来源：http://bz.muxihuayi.cn

Java: if (s.isEmpty()) {}
来源：http://jl.panjiajie.cn

Go:   if s == "" {}
来源：http://vy.chemitech.net.cn

Ruby: if s.empty?
来源：http://lc.jctech888.com.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ot.shtwfgs.cn

[E21] 超长截断加省略号
来源：http://zw.bjjhwx.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://et.bookmarksfly.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://es.jianghongdianzi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://na.wgjwhj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rs.newstarts.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yr.nszjky.cn

Go:   // 按 rune 判断长度后截断
来源：http://tq.huixiangedu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hv.wgjwhj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://oc.wgjwhj.cn

[E22] 字节长度与字符长度
来源：http://dw.shxzskj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wg.jianghongdianzi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tl.muxihuayi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kx.hnjuh.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zc.newstarts.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zg.muxihuayi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cb.szsharing.cn

Ruby: s.bytesize;  s.length
来源：http://pc.yuexingan06.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ym.huanxung.cn

================================================================================
来源：http://rq.gzmigu.cn

F. 文件与目录
来源：http://ag.yuexingan06.cn

================================================================================
来源：http://cr.szsharing.cn

[F01] 读取整个文件
来源：http://dp.jianghongdianzi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kf.bjjhwx.cn

PHP:  file_get_contents("a.txt");
来源：http://rq.szxytkj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kx.jctech888.com.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mt.szsharing.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://po.huixiangedu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cv.huanxung.cn

Ruby: File.read("a.txt")
来源：http://wm.huanxung.cn

C#:   File.ReadAllText("a.txt");
来源：http://pl.colortex.cn

[F02] 逐行读取文件
来源：http://nm.shtwfgs.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ov.huixinmuqiang.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fy.bjjhwx.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qg.shxzukj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ih.shxzukj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wo.nszjky.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hv.newstarts.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://me.gzmigu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rc.muxihuayi.cn

[F03] 写入文件（覆盖）
来源：http://ni.panjiajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ze.521024.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://wm.shtwfgs.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gf.huixiangedu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oy.haigaiapp.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://st.hnjuh.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kk.521024.cn

Ruby: File.write("a.txt", "hi")
来源：http://bj.hnjuh.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://av.hahajie.cn

[F04] 追加写入文件
来源：http://zk.bookmarksfly.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pj.bjjhwx.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://op.wgjwhj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zv.hnjuh.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qu.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sa.yuntaijiaju.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wh.jctech888.com.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ph.jianghongdianzi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bp.hnjuh.cn

[F05] 判断文件或目录是否存在
来源：http://km.521024.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://uz.shxzukj.cn

PHP:  file_exists("a.txt");
来源：http://vf.haigaiapp.cn

JS:   fs.existsSync("a.txt")
来源：http://na.shtwfgs.cn

TS:   fs.existsSync("a.txt")
来源：http://mx.chemitech.net.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://cc.shxzskj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://az.huanxung.cn

Ruby: File.exist?("a.txt")
来源：http://ll.shxzukj.cn

C#:   File.Exists("a.txt")
来源：http://ez.huixinmuqiang.cn

[F06] 删除文件
来源：http://xu.yuexingan06.cn

Py:   os.remove("a.txt")
来源：http://jg.huanxung.cn

PHP:  unlink("a.txt");
来源：http://kh.muxihuayi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ly.hahajie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ur.haigaiapp.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sg.nicolike.cn

Go:   os.Remove("a.txt")
来源：http://oo.shxzskj.cn

Ruby: File.delete("a.txt")
来源：http://py.hnjuh.cn

C#:   File.Delete("a.txt");
来源：http://us.nszjky.cn

[F07] 创建目录（含多级）
来源：http://sn.shtwfgs.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rz.haigaiapp.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cw.panjiajie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xa.wgjwhj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ct.hnjuh.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pl.gzmigu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nd.panjiajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gn.jctech888.com.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kv.huixiangedu.cn

[F08] 遍历目录
来源：http://my.panjiajie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://el.lnxyls.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fw.huixinmuqiang.cn

JS:   fs.readdirSync("dir")
来源：http://fi.gzmigu.cn

TS:   fs.readdirSync("dir")
来源：http://ae.gzmigu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ww.muxihuayi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fo.shxzskj.cn

Ruby: Dir.children("dir")
来源：http://jg.hnjuh.cn

C#:   Directory.GetFiles("dir")
来源：http://uy.9csxet.cn

[F09] 获取文件大小
来源：http://ll.bookmarksfly.cn

Py:   os.path.getsize("a.txt")
来源：http://th.haigaiapp.cn

PHP:  filesize("a.txt");
来源：http://hn.chemitech.net.cn

JS:   fs.statSync("a.txt").size
来源：http://tq.yuntaijiaju.cn

TS:   fs.statSync("a.txt").size
来源：http://jo.nszjky.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hc.hnjuh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hu.yuexingan06.cn

Ruby: File.size("a.txt")
来源：http://ar.wgjwhj.cn

C#:   new FileInfo("a.txt").Length
来源：http://zl.haigaiapp.cn

[F10] 取文件扩展名 / 文件名
来源：http://pp.haigaiapp.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xt.huixiangedu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://np.huixinmuqiang.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nk.jianghongdianzi.cn

TS:   path.extname("a.txt")
来源：http://kf.shtwfgs.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ni.bookmarksfly.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://oj.jianghongdianzi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xo.huanxung.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vh.lnxyls.cn

[F11] 复制与移动文件
来源：http://rp.yuntaijiaju.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nb.colortex.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://iv.shtwfgs.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bu.shxzskj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qu.chemitech.net.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tm.521024.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hq.muxihuayi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pm.asd995.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zl.newstarts.cn

[F12] CSV 读写
来源：http://lv.lnxyls.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nf.huixinmuqiang.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dp.bookmarksfly.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fv.hnjuh.cn

TS:   // 同上
来源：http://bv.yuexingan06.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ux.nszjky.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yq.wgjwhj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bw.521024.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://zb.szsharing.cn

================================================================================
来源：http://xd.hahajie.cn

G. 面向对象
来源：http://cf.bjjhwx.cn

================================================================================
来源：http://cw.jianghongdianzi.cn

[G01] 定义类
来源：http://gj.huixinmuqiang.cn

Py:   class User: pass
来源：http://xb.nicolike.cn

PHP:  class User {}
来源：http://xn.newstarts.cn

JS:   class User {}
来源：http://hp.wgjwhj.cn

TS:   class User { name: string = ""; }
来源：http://sl.haigaiapp.cn

Java: class User {}
来源：http://mp.hnjuh.cn

Go:   type User struct { Name string }
来源：http://zo.haigaiapp.cn

Ruby: class User; end
来源：http://on.gzmigu.cn

C#:   class User {}
来源：http://bd.haigaiapp.cn

[G02] 构造函数
来源：http://rv.nszjky.cn

Py:   def __init__(self, name): self.name = name
来源：http://gf.huixiangedu.cn

PHP:  public function __construct(public string $name) {}
来源：http://rw.colortex.cn

JS:   constructor(name) { this.name = name; }
来源：http://vq.521024.cn

TS:   constructor(public name: string) {}
来源：http://ul.huixinmuqiang.cn

Java: User(String name) { this.name = name; }
来源：http://wh.shtwfgs.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vq.shtwfgs.cn

Ruby: def initialize(name); @name = name; end
来源：http://ia.huanxung.cn

C#:   public User(string name) { Name = name; }
来源：http://xy.hahajie.cn

[G03] 实例属性
来源：http://tw.jctech888.com.cn

Py:   self.name = "x"
来源：http://lh.bjjhwx.cn

PHP:  public string $name = "x";
来源：http://ll.jianghongdianzi.cn

JS:   this.name = "x";
来源：http://nm.nszjky.cn

TS:   name: string = "x";
来源：http://tb.szxytkj.cn

Java: private String name;
来源：http://bg.huanxung.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jn.asd995.cn

Ruby: @name = "x"
来源：http://wl.hahajie.cn

C#:   public string Name { get; set; } = "x";
来源：http://an.haigaiapp.cn

[G04] 定义方法
来源：http://mh.hahajie.cn

Py:   def greet(self): return self.name
来源：http://hx.hahajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://up.shxzukj.cn

JS:   greet() { return this.name; }
来源：http://yf.newstarts.cn

TS:   greet(): string { return this.name; }
来源：http://mi.jianghongdianzi.cn

Java: String greet() { return name; }
来源：http://id.shtwfgs.cn


<!-- 参考信息 -->