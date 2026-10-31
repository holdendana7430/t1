代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://mg.bjjhwx.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sl.haigaiapp.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://eu.jctech888.com.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zg.521024.cn

C#:   s.Replace("a", "b")
来源：http://lp.colortex.cn

[E07] 按分隔符拆分
来源：http://ql.jianghongdianzi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://aq.yuexingan06.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fb.gzmigu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://nw.panjiajie.cn

TS:   s.split(",")
来源：http://tg.chemitech.net.cn

Java: s.split(",");  s.split("\\s+")
来源：http://os.hnjuh.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://me.jctech888.com.cn

Ruby: s.split(",");  s.split
来源：http://pc.yuntaijiaju.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zi.jctech888.com.cn

[E08] 数组按分隔符合并
来源：http://gn.panjiajie.cn

Py:   ",".join(items)
来源：http://hw.nszjky.cn

PHP:  implode(",", $items);
来源：http://zc.colortex.cn

JS:   items.join(",")
来源：http://qx.asd995.cn

TS:   items.join(",")
来源：http://zv.lnxyls.cn

Java: String.join(",", items)
来源：http://ne.asd995.cn

Go:   strings.Join(items, ",")
来源：http://qo.wgjwhj.cn

Ruby: items.join(",")
来源：http://qm.nszjky.cn

C#:   string.Join(",", items)
来源：http://rx.bookmarksfly.cn

[E09] 去除所有空白字符
来源：http://ac.newstarts.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tt.bjjhwx.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://am.huixiangedu.cn

JS:   s.replace(/\s+/g, "")
来源：http://ad.jctech888.com.cn

TS:   s.replace(/\s+/g, "")
来源：http://dr.huanxung.cn

Java: s.replaceAll("\\s+", "")
来源：http://um.jianghongdianzi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://mz.nicolike.cn

Ruby: s.gsub(/\s+/, "")
来源：http://od.panjiajie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fj.yuntaijiaju.cn

[E10] 左侧补零 / 定长填充
来源：http://fm.panjiajie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ap.gzmigu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zm.bjjhwx.cn

JS:   "7".padStart(3, "0")
来源：http://nu.muxihuayi.cn

TS:   "7".padStart(3, "0")
来源：http://le.bookmarksfly.cn

Java: String.format("%03d", 7)
来源：http://xh.jctech888.com.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xj.muxihuayi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zz.panjiajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ra.szxytkj.cn

[E11] 反转字符串
来源：http://gp.colortex.cn

Py:   s[::-1]
来源：http://yi.yuexingan06.cn

PHP:  strrev($s);
来源：http://gg.haigaiapp.cn

JS:   [...s].reverse().join("")
来源：http://sx.shxzukj.cn

TS:   [...s].reverse().join("")
来源：http://vs.hnjuh.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://mj.huanxung.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://rv.shxzukj.cn

Ruby: s.reverse
来源：http://fw.9csxet.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ga.9csxet.cn

[E12] 统计某字符出现次数
来源：http://kv.hahajie.cn

Py:   s.count("a")
来源：http://fv.521024.cn

PHP:  substr_count($s, "a");
来源：http://pe.jctech888.com.cn

JS:   s.split("a").length - 1
来源：http://bx.panjiajie.cn

TS:   s.split("a").length - 1
来源：http://sa.shxzukj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dc.shxzukj.cn

Go:   strings.Count(s, "a")
来源：http://gc.szxytkj.cn

Ruby: s.count("a")
来源：http://cc.lnxyls.cn

C#:   s.Count(c => c == 'a')
来源：http://sx.panjiajie.cn

[E13] 逐字符遍历
来源：http://ir.huanxung.cn

Py:   for ch in s: print(ch)
来源：http://bn.jianghongdianzi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jn.shxzskj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://da.bookmarksfly.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://oq.colortex.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fg.szxytkj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://og.hahajie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://yk.gzmigu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://av.yuntaijiaju.cn

[E14] URL 编码与 Base64
来源：http://zr.shxzskj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ud.newstarts.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://sp.9csxet.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://sx.nicolike.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://if.shxzukj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uw.muxihuayi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mj.521024.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://if.yuntaijiaju.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://up.muxihuayi.cn

[E15] HTML 转义 / 反转义
来源：http://eg.chemitech.net.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://us.yuntaijiaju.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vu.yuntaijiaju.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ur.huanxung.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://hj.jctech888.com.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qq.yuexingan06.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://lu.muxihuayi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wu.szxytkj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bl.asd995.cn

[E16] 数字千分位
来源：http://bw.jianghongdianzi.cn

Py:   f"{1234567:,}"
来源：http://lo.hahajie.cn

PHP:  number_format(1234567);
来源：http://bc.huanxung.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://dp.yuntaijiaju.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://qd.newstarts.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mp.nszjky.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yd.huixiangedu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pa.shtwfgs.cn

C#:   1234567.ToString("N0")
来源：http://xk.9csxet.cn

[E17] 首字母大写
来源：http://ad.asd995.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kn.jctech888.com.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ss.muxihuayi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bs.nszjky.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ck.haigaiapp.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kp.gzmigu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://md.wgjwhj.cn

Ruby: s.capitalize
来源：http://vm.nszjky.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qu.shtwfgs.cn

[E18] 模板占位符替换
来源：http://ab.shxzukj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://oi.bjjhwx.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xi.chemitech.net.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://gx.chemitech.net.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://yu.szsharing.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://yj.panjiajie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mh.shxzukj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://sm.colortex.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vl.jianghongdianzi.cn

[E19] 多行文本按行拆分
来源：http://kp.gzmigu.cn

Py:   s.splitlines()
来源：http://bo.521024.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ww.asd995.cn

JS:   s.split(/\r?\n/)
来源：http://np.lnxyls.cn

TS:   s.split(/\r?\n/)
来源：http://oy.yuntaijiaju.cn

Java: s.lines().toList()
来源：http://vf.chemitech.net.cn

Go:   strings.Split(s, "\n")
来源：http://rx.haigaiapp.cn

Ruby: s.lines
来源：http://qy.jctech888.com.cn

C#:   s.Split('\n')
来源：http://yy.hnjuh.cn

[E20] 判断字符串是否为空
来源：http://of.yuntaijiaju.cn

Py:   if not s:
来源：http://iy.jctech888.com.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nw.huanxung.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ps.bookmarksfly.cn

TS:   if (s === "") {}
来源：http://ia.wgjwhj.cn

Java: if (s.isEmpty()) {}
来源：http://kq.bjjhwx.cn

Go:   if s == "" {}
来源：http://qb.521024.cn

Ruby: if s.empty?
来源：http://fp.jianghongdianzi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xi.hnjuh.cn

[E21] 超长截断加省略号
来源：http://gu.bjjhwx.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yg.lnxyls.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ul.szxytkj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mm.hahajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xq.chemitech.net.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kp.521024.cn

Go:   // 按 rune 判断长度后截断
来源：http://di.asd995.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cc.asd995.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kf.lnxyls.cn

[E22] 字节长度与字符长度
来源：http://bb.muxihuayi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://iq.bjjhwx.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hh.9csxet.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ma.hahajie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://de.haigaiapp.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cf.wgjwhj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bm.newstarts.cn

Ruby: s.bytesize;  s.length
来源：http://av.lnxyls.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sm.haigaiapp.cn

================================================================================
来源：http://vb.panjiajie.cn

F. 文件与目录
来源：http://dj.shxzukj.cn

================================================================================
来源：http://qc.huixiangedu.cn

[F01] 读取整个文件
来源：http://gz.shxzukj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gn.chemitech.net.cn

PHP:  file_get_contents("a.txt");
来源：http://hi.yuntaijiaju.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cm.hahajie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zz.shtwfgs.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://qf.panjiajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jc.colortex.cn

Ruby: File.read("a.txt")
来源：http://pb.shxzukj.cn

C#:   File.ReadAllText("a.txt");
来源：http://oq.hnjuh.cn

[F02] 逐行读取文件
来源：http://wj.panjiajie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rx.panjiajie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cq.panjiajie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ac.panjiajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cg.shtwfgs.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pc.nszjky.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ch.huanxung.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ui.shxzukj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ac.hahajie.cn

[F03] 写入文件（覆盖）
来源：http://mb.9csxet.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xs.asd995.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://pe.bookmarksfly.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fw.chemitech.net.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tp.huanxung.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tw.szxytkj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kr.lnxyls.cn

Ruby: File.write("a.txt", "hi")
来源：http://ru.nszjky.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jc.jianghongdianzi.cn

[F04] 追加写入文件
来源：http://pt.lnxyls.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lo.colortex.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zr.lnxyls.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ok.lnxyls.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lx.szxytkj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fn.9csxet.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vk.asd995.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://sk.9csxet.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://oo.yuntaijiaju.cn

[F05] 判断文件或目录是否存在
来源：http://fe.bjjhwx.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pu.panjiajie.cn

PHP:  file_exists("a.txt");
来源：http://un.9csxet.cn

JS:   fs.existsSync("a.txt")
来源：http://fg.shxzukj.cn

TS:   fs.existsSync("a.txt")
来源：http://dc.muxihuayi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://yb.9csxet.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://uo.nszjky.cn

Ruby: File.exist?("a.txt")
来源：http://of.jianghongdianzi.cn

C#:   File.Exists("a.txt")
来源：http://gp.nszjky.cn

[F06] 删除文件
来源：http://gj.chemitech.net.cn

Py:   os.remove("a.txt")
来源：http://sv.bjjhwx.cn

PHP:  unlink("a.txt");
来源：http://of.lnxyls.cn

JS:   fs.unlinkSync("a.txt")
来源：http://cj.shtwfgs.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ib.huixiangedu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://na.nszjky.cn

Go:   os.Remove("a.txt")
来源：http://tg.huanxung.cn

Ruby: File.delete("a.txt")
来源：http://jy.bookmarksfly.cn

C#:   File.Delete("a.txt");
来源：http://sx.bookmarksfly.cn

[F07] 创建目录（含多级）
来源：http://jt.bjjhwx.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xz.hahajie.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://in.asd995.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ft.newstarts.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tl.nszjky.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vy.jianghongdianzi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tj.newstarts.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cu.chemitech.net.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mo.huanxung.cn

[F08] 遍历目录
来源：http://kx.shtwfgs.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ws.huanxung.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qt.nicolike.cn

JS:   fs.readdirSync("dir")
来源：http://qx.colortex.cn

TS:   fs.readdirSync("dir")
来源：http://wm.huixinmuqiang.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://aw.shxzukj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://kg.huanxung.cn

Ruby: Dir.children("dir")
来源：http://mv.newstarts.cn

C#:   Directory.GetFiles("dir")
来源：http://mm.chemitech.net.cn

[F09] 获取文件大小
来源：http://qs.szxytkj.cn

Py:   os.path.getsize("a.txt")
来源：http://ef.9csxet.cn

PHP:  filesize("a.txt");
来源：http://cd.hnjuh.cn

JS:   fs.statSync("a.txt").size
来源：http://qm.nicolike.cn

TS:   fs.statSync("a.txt").size
来源：http://lt.newstarts.cn

Java: Files.size(Path.of("a.txt"))
来源：http://dq.nszjky.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mm.lnxyls.cn

Ruby: File.size("a.txt")
来源：http://jq.nszjky.cn

C#:   new FileInfo("a.txt").Length
来源：http://ej.jctech888.com.cn

[F10] 取文件扩展名 / 文件名
来源：http://fd.9csxet.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kr.yuntaijiaju.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nt.bjjhwx.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://no.shxzskj.cn

TS:   path.extname("a.txt")
来源：http://gc.muxihuayi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vh.shtwfgs.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ud.szsharing.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xf.muxihuayi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qe.gzmigu.cn

[F11] 复制与移动文件
来源：http://xu.huixinmuqiang.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://eh.huixinmuqiang.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ee.huanxung.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gf.nszjky.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pc.bookmarksfly.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://va.colortex.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mr.chemitech.net.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jv.szsharing.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bd.shxzskj.cn

[F12] CSV 读写
来源：http://oy.newstarts.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://uk.nicolike.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yx.szxytkj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vg.yuexingan06.cn

TS:   // 同上
来源：http://ml.bookmarksfly.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gv.huanxung.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pl.huixinmuqiang.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vq.huixinmuqiang.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://sr.lnxyls.cn

================================================================================
来源：http://fw.shxzskj.cn

G. 面向对象
来源：http://or.nicolike.cn

================================================================================
来源：http://we.nszjky.cn

[G01] 定义类
来源：http://cg.bookmarksfly.cn

Py:   class User: pass
来源：http://lz.haigaiapp.cn

PHP:  class User {}
来源：http://ln.szxytkj.cn

JS:   class User {}
来源：http://pv.nicolike.cn

TS:   class User { name: string = ""; }
来源：http://fc.bjjhwx.cn

Java: class User {}
来源：http://eq.szxytkj.cn

Go:   type User struct { Name string }
来源：http://xm.shtwfgs.cn

Ruby: class User; end
来源：http://or.muxihuayi.cn

C#:   class User {}
来源：http://ib.huixiangedu.cn

[G02] 构造函数
来源：http://ts.gzmigu.cn

Py:   def __init__(self, name): self.name = name
来源：http://za.huanxung.cn

PHP:  public function __construct(public string $name) {}
来源：http://so.muxihuayi.cn

JS:   constructor(name) { this.name = name; }
来源：http://sv.newstarts.cn

TS:   constructor(public name: string) {}
来源：http://zz.newstarts.cn

Java: User(String name) { this.name = name; }
来源：http://zk.nszjky.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ty.wgjwhj.cn

Ruby: def initialize(name); @name = name; end
来源：http://is.newstarts.cn

C#:   public User(string name) { Name = name; }
来源：http://cz.nszjky.cn

[G03] 实例属性
来源：http://df.szxytkj.cn

Py:   self.name = "x"
来源：http://nb.huixinmuqiang.cn

PHP:  public string $name = "x";
来源：http://xr.huanxung.cn

JS:   this.name = "x";
来源：http://th.muxihuayi.cn

TS:   name: string = "x";
来源：http://sc.yuexingan06.cn

Java: private String name;
来源：http://se.yuexingan06.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vp.bookmarksfly.cn

Ruby: @name = "x"
来源：http://wv.hnjuh.cn

C#:   public string Name { get; set; } = "x";
来源：http://oj.haigaiapp.cn

[G04] 定义方法
来源：http://jb.yuexingan06.cn

Py:   def greet(self): return self.name
来源：http://zw.huixinmuqiang.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ei.lnxyls.cn

JS:   greet() { return this.name; }
来源：http://kr.jctech888.com.cn

TS:   greet(): string { return this.name; }
来源：http://lb.lnxyls.cn

Java: String greet() { return name; }
来源：http://ff.hahajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://yc.521024.cn

Ruby: def greet; @name; end
来源：http://ph.wgjwhj.cn

C#:   public string Greet() => Name;
来源：http://nj.9csxet.cn

[G05] 继承
来源：http://oj.lnxyls.cn


<!-- 参考信息 -->