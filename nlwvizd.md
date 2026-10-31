代发 wailian999

C#:   s.Replace("a", "b")
来源：http://iw.gzmigu.cn

[E07] 按分隔符拆分
来源：http://bt.asd995.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ix.hahajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tn.szsharing.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://sl.shtwfgs.cn

TS:   s.split(",")
来源：http://my.muxihuayi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://sa.521024.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xa.521024.cn

Ruby: s.split(",");  s.split
来源：http://xv.colortex.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gk.bjjhwx.cn

[E08] 数组按分隔符合并
来源：http://sp.muxihuayi.cn

Py:   ",".join(items)
来源：http://ll.szxytkj.cn

PHP:  implode(",", $items);
来源：http://kx.bookmarksfly.cn

JS:   items.join(",")
来源：http://jl.jctech888.com.cn

TS:   items.join(",")
来源：http://cw.hnjuh.cn

Java: String.join(",", items)
来源：http://tk.wgjwhj.cn

Go:   strings.Join(items, ",")
来源：http://vs.yuntaijiaju.cn

Ruby: items.join(",")
来源：http://dc.jctech888.com.cn

C#:   string.Join(",", items)
来源：http://om.huixiangedu.cn

[E09] 去除所有空白字符
来源：http://jz.yuntaijiaju.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dp.panjiajie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://km.hnjuh.cn

JS:   s.replace(/\s+/g, "")
来源：http://lu.newstarts.cn

TS:   s.replace(/\s+/g, "")
来源：http://fu.shxzskj.cn

Java: s.replaceAll("\\s+", "")
来源：http://nk.huixiangedu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://rj.jctech888.com.cn

Ruby: s.gsub(/\s+/, "")
来源：http://mb.nicolike.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qp.lnxyls.cn

[E10] 左侧补零 / 定长填充
来源：http://pm.huixinmuqiang.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dl.haigaiapp.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vk.521024.cn

JS:   "7".padStart(3, "0")
来源：http://sg.haigaiapp.cn

TS:   "7".padStart(3, "0")
来源：http://rg.nszjky.cn

Java: String.format("%03d", 7)
来源：http://ig.shxzskj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://jl.huixinmuqiang.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jr.szxytkj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gw.shxzukj.cn

[E11] 反转字符串
来源：http://fj.9csxet.cn

Py:   s[::-1]
来源：http://rd.muxihuayi.cn

PHP:  strrev($s);
来源：http://wh.yuexingan06.cn

JS:   [...s].reverse().join("")
来源：http://qz.jctech888.com.cn

TS:   [...s].reverse().join("")
来源：http://te.jianghongdianzi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://to.chemitech.net.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ik.jianghongdianzi.cn

Ruby: s.reverse
来源：http://ci.wgjwhj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://oh.hnjuh.cn

[E12] 统计某字符出现次数
来源：http://md.chemitech.net.cn

Py:   s.count("a")
来源：http://el.huixiangedu.cn

PHP:  substr_count($s, "a");
来源：http://el.haigaiapp.cn

JS:   s.split("a").length - 1
来源：http://ye.nszjky.cn

TS:   s.split("a").length - 1
来源：http://fg.9csxet.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ye.huixiangedu.cn

Go:   strings.Count(s, "a")
来源：http://mc.nszjky.cn

Ruby: s.count("a")
来源：http://pb.huixiangedu.cn

C#:   s.Count(c => c == 'a')
来源：http://ez.gzmigu.cn

[E13] 逐字符遍历
来源：http://uc.asd995.cn

Py:   for ch in s: print(ch)
来源：http://dn.huanxung.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://do.colortex.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://jq.bookmarksfly.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bw.gzmigu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gd.muxihuayi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ux.hahajie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://kz.shxzukj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jq.szsharing.cn

[E14] URL 编码与 Base64
来源：http://kb.jctech888.com.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://id.shtwfgs.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://rk.9csxet.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nc.newstarts.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pl.gzmigu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bv.panjiajie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qs.asd995.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zi.colortex.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fb.shxzukj.cn

[E15] HTML 转义 / 反转义
来源：http://fo.newstarts.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://hj.nszjky.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ev.nicolike.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mq.panjiajie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://qb.nszjky.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bc.gzmigu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://eu.hnjuh.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://az.haigaiapp.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gg.haigaiapp.cn

[E16] 数字千分位
来源：http://dv.asd995.cn

Py:   f"{1234567:,}"
来源：http://sg.nszjky.cn

PHP:  number_format(1234567);
来源：http://zj.jianghongdianzi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ob.szxytkj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://nc.gzmigu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nk.yuexingan06.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vf.huixinmuqiang.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tw.hahajie.cn

C#:   1234567.ToString("N0")
来源：http://xc.gzmigu.cn

[E17] 首字母大写
来源：http://gn.jianghongdianzi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rc.shxzukj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ey.yuntaijiaju.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://eb.nszjky.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://eg.colortex.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://df.shxzukj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pl.shtwfgs.cn

Ruby: s.capitalize
来源：http://ix.asd995.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pv.jctech888.com.cn

[E18] 模板占位符替换
来源：http://rc.huixiangedu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uc.asd995.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tz.jctech888.com.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://jf.huixiangedu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://hr.panjiajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ql.bjjhwx.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pu.hnjuh.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tm.gzmigu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yw.newstarts.cn

[E19] 多行文本按行拆分
来源：http://md.huanxung.cn

Py:   s.splitlines()
来源：http://ux.hnjuh.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qt.bookmarksfly.cn

JS:   s.split(/\r?\n/)
来源：http://ay.shxzskj.cn

TS:   s.split(/\r?\n/)
来源：http://be.huixiangedu.cn

Java: s.lines().toList()
来源：http://io.jctech888.com.cn

Go:   strings.Split(s, "\n")
来源：http://ay.colortex.cn

Ruby: s.lines
来源：http://mb.yuntaijiaju.cn

C#:   s.Split('\n')
来源：http://dp.bjjhwx.cn

[E20] 判断字符串是否为空
来源：http://dm.shxzukj.cn

Py:   if not s:
来源：http://ng.asd995.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rx.bookmarksfly.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tu.nszjky.cn

TS:   if (s === "") {}
来源：http://zh.9csxet.cn

Java: if (s.isEmpty()) {}
来源：http://jo.chemitech.net.cn

Go:   if s == "" {}
来源：http://rt.szxytkj.cn

Ruby: if s.empty?
来源：http://tm.panjiajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nr.hnjuh.cn

[E21] 超长截断加省略号
来源：http://in.yuntaijiaju.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ws.shxzskj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vc.yuntaijiaju.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pz.wgjwhj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ua.wgjwhj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ib.szxytkj.cn

Go:   // 按 rune 判断长度后截断
来源：http://db.shxzskj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ym.newstarts.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gi.huixiangedu.cn

[E22] 字节长度与字符长度
来源：http://tx.wgjwhj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fp.shxzskj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hq.nszjky.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bj.haigaiapp.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dz.bookmarksfly.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://en.asd995.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nr.gzmigu.cn

Ruby: s.bytesize;  s.length
来源：http://ex.shxzukj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gc.huixinmuqiang.cn

================================================================================
来源：http://bb.nicolike.cn

F. 文件与目录
来源：http://dq.szxytkj.cn

================================================================================
来源：http://wo.yuntaijiaju.cn

[F01] 读取整个文件
来源：http://ch.nicolike.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fg.huixiangedu.cn

PHP:  file_get_contents("a.txt");
来源：http://nh.521024.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ne.9csxet.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ez.szxytkj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vo.shxzskj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://iz.nszjky.cn

Ruby: File.read("a.txt")
来源：http://bs.huanxung.cn

C#:   File.ReadAllText("a.txt");
来源：http://us.nszjky.cn

[F02] 逐行读取文件
来源：http://ly.jctech888.com.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gi.szxytkj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ld.huanxung.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fm.colortex.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yf.asd995.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jn.shxzukj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mn.panjiajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://is.newstarts.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nm.chemitech.net.cn

[F03] 写入文件（覆盖）
来源：http://qe.bjjhwx.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ka.colortex.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://nc.nicolike.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kp.shxzskj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pd.shtwfgs.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wz.huixiangedu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ze.521024.cn

Ruby: File.write("a.txt", "hi")
来源：http://xx.nszjky.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zs.muxihuayi.cn

[F04] 追加写入文件
来源：http://kd.hnjuh.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ov.huanxung.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gw.szxytkj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hk.huixinmuqiang.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://td.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tx.shxzukj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bw.nicolike.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gg.colortex.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hj.yuntaijiaju.cn

[F05] 判断文件或目录是否存在
来源：http://gd.haigaiapp.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ko.nicolike.cn

PHP:  file_exists("a.txt");
来源：http://ru.haigaiapp.cn

JS:   fs.existsSync("a.txt")
来源：http://cz.newstarts.cn

TS:   fs.existsSync("a.txt")
来源：http://vm.nicolike.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://fw.huixinmuqiang.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://iw.newstarts.cn

Ruby: File.exist?("a.txt")
来源：http://xd.nicolike.cn

C#:   File.Exists("a.txt")
来源：http://ll.szxytkj.cn

[F06] 删除文件
来源：http://ju.szxytkj.cn

Py:   os.remove("a.txt")
来源：http://oj.hnjuh.cn

PHP:  unlink("a.txt");
来源：http://vs.gzmigu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://bj.wgjwhj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://zd.lnxyls.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wy.wgjwhj.cn

Go:   os.Remove("a.txt")
来源：http://qh.shxzukj.cn

Ruby: File.delete("a.txt")
来源：http://kc.bookmarksfly.cn

C#:   File.Delete("a.txt");
来源：http://pu.jctech888.com.cn

[F07] 创建目录（含多级）
来源：http://mz.bookmarksfly.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sb.521024.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ce.chemitech.net.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tz.szxytkj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yc.jianghongdianzi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lb.colortex.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lm.szxytkj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yl.huanxung.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dc.shxzukj.cn

[F08] 遍历目录
来源：http://yp.jctech888.com.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://kb.szxytkj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fl.shtwfgs.cn

JS:   fs.readdirSync("dir")
来源：http://cn.521024.cn

TS:   fs.readdirSync("dir")
来源：http://jz.shxzukj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vw.wgjwhj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://qe.huixinmuqiang.cn

Ruby: Dir.children("dir")
来源：http://lq.yuexingan06.cn

C#:   Directory.GetFiles("dir")
来源：http://cl.shtwfgs.cn

[F09] 获取文件大小
来源：http://yu.hnjuh.cn

Py:   os.path.getsize("a.txt")
来源：http://eb.chemitech.net.cn

PHP:  filesize("a.txt");
来源：http://fm.521024.cn

JS:   fs.statSync("a.txt").size
来源：http://lk.bjjhwx.cn

TS:   fs.statSync("a.txt").size
来源：http://uk.wgjwhj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mf.jctech888.com.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wv.jianghongdianzi.cn

Ruby: File.size("a.txt")
来源：http://hd.muxihuayi.cn

C#:   new FileInfo("a.txt").Length
来源：http://pp.panjiajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://qh.muxihuayi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nq.szxytkj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bl.hnjuh.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qy.shxzukj.cn

TS:   path.extname("a.txt")
来源：http://zc.yuntaijiaju.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zn.shxzukj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zx.gzmigu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qo.panjiajie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ep.bookmarksfly.cn

[F11] 复制与移动文件
来源：http://xa.haigaiapp.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ey.huixinmuqiang.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ws.asd995.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://aj.asd995.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cu.9csxet.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://le.huixiangedu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rk.panjiajie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fv.9csxet.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://oi.shxzskj.cn

[F12] CSV 读写
来源：http://jf.chemitech.net.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xu.bjjhwx.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ej.shxzskj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zn.jctech888.com.cn

TS:   // 同上
来源：http://zi.chemitech.net.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bp.chemitech.net.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://en.jctech888.com.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ki.yuntaijiaju.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://is.shtwfgs.cn

================================================================================
来源：http://zy.haigaiapp.cn

G. 面向对象
来源：http://xn.colortex.cn

================================================================================
来源：http://nn.lnxyls.cn

[G01] 定义类
来源：http://pc.asd995.cn

Py:   class User: pass
来源：http://ra.lnxyls.cn

PHP:  class User {}
来源：http://ui.panjiajie.cn

JS:   class User {}
来源：http://jy.szsharing.cn

TS:   class User { name: string = ""; }
来源：http://wq.shxzskj.cn

Java: class User {}
来源：http://dp.szsharing.cn

Go:   type User struct { Name string }
来源：http://vp.yuntaijiaju.cn

Ruby: class User; end
来源：http://yo.nicolike.cn

C#:   class User {}
来源：http://rg.colortex.cn

[G02] 构造函数
来源：http://sm.hnjuh.cn

Py:   def __init__(self, name): self.name = name
来源：http://oa.nicolike.cn

PHP:  public function __construct(public string $name) {}
来源：http://ij.chemitech.net.cn

JS:   constructor(name) { this.name = name; }
来源：http://mt.huixinmuqiang.cn

TS:   constructor(public name: string) {}
来源：http://qk.colortex.cn

Java: User(String name) { this.name = name; }
来源：http://pb.wgjwhj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xf.nszjky.cn

Ruby: def initialize(name); @name = name; end
来源：http://pg.szsharing.cn

C#:   public User(string name) { Name = name; }
来源：http://fn.panjiajie.cn

[G03] 实例属性
来源：http://kh.521024.cn

Py:   self.name = "x"
来源：http://iz.gzmigu.cn

PHP:  public string $name = "x";
来源：http://rn.jianghongdianzi.cn

JS:   this.name = "x";
来源：http://oe.shtwfgs.cn

TS:   name: string = "x";
来源：http://cv.nszjky.cn

Java: private String name;
来源：http://rp.bjjhwx.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nd.szxytkj.cn

Ruby: @name = "x"
来源：http://pf.hahajie.cn

C#:   public string Name { get; set; } = "x";
来源：http://ct.shxzskj.cn

[G04] 定义方法
来源：http://fe.hnjuh.cn

Py:   def greet(self): return self.name
来源：http://ct.szsharing.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://kt.huanxung.cn

JS:   greet() { return this.name; }
来源：http://te.szxytkj.cn

TS:   greet(): string { return this.name; }
来源：http://gk.jctech888.com.cn

Java: String greet() { return name; }
来源：http://ds.bjjhwx.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://lr.521024.cn

Ruby: def greet; @name; end
来源：http://pa.shxzukj.cn

C#:   public string Greet() => Name;
来源：http://ds.yuexingan06.cn

[G05] 继承
来源：http://pq.bjjhwx.cn

Py:   class Admin(User): pass
来源：http://im.huanxung.cn

PHP:  class Admin extends User {}
来源：http://br.huixinmuqiang.cn

JS:   class Admin extends User {}
来源：http://da.haigaiapp.cn

TS:   class Admin extends User {}
来源：http://ez.szsharing.cn


<!-- 参考信息 -->