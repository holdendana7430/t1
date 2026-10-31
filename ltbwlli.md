代发 wailian999

Ruby: s.split(",");  s.split
来源：http://ma.muxihuayi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ai.521024.cn

[E08] 数组按分隔符合并
来源：http://sr.hnjuh.cn

Py:   ",".join(items)
来源：http://ky.gzmigu.cn

PHP:  implode(",", $items);
来源：http://dm.jianghongdianzi.cn

JS:   items.join(",")
来源：http://wl.szxytkj.cn

TS:   items.join(",")
来源：http://vu.huixiangedu.cn

Java: String.join(",", items)
来源：http://qr.colortex.cn

Go:   strings.Join(items, ",")
来源：http://no.huixiangedu.cn

Ruby: items.join(",")
来源：http://ha.hnjuh.cn

C#:   string.Join(",", items)
来源：http://gc.521024.cn

[E09] 去除所有空白字符
来源：http://ro.huixiangedu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mv.asd995.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jl.colortex.cn

JS:   s.replace(/\s+/g, "")
来源：http://nx.jctech888.com.cn

TS:   s.replace(/\s+/g, "")
来源：http://bh.panjiajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://ck.szsharing.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://jv.9csxet.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ni.szsharing.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zk.newstarts.cn

[E10] 左侧补零 / 定长填充
来源：http://lw.shxzukj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rv.huixinmuqiang.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ja.shxzukj.cn

JS:   "7".padStart(3, "0")
来源：http://zd.hnjuh.cn

TS:   "7".padStart(3, "0")
来源：http://pj.muxihuayi.cn

Java: String.format("%03d", 7)
来源：http://yb.newstarts.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://uj.nicolike.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://aw.szxytkj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gc.shxzukj.cn

[E11] 反转字符串
来源：http://ww.9csxet.cn

Py:   s[::-1]
来源：http://ua.shxzukj.cn

PHP:  strrev($s);
来源：http://gn.huanxung.cn

JS:   [...s].reverse().join("")
来源：http://if.nszjky.cn

TS:   [...s].reverse().join("")
来源：http://xo.wgjwhj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://kq.hahajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://cs.haigaiapp.cn

Ruby: s.reverse
来源：http://ht.9csxet.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ae.9csxet.cn

[E12] 统计某字符出现次数
来源：http://mt.huixinmuqiang.cn

Py:   s.count("a")
来源：http://va.nicolike.cn

PHP:  substr_count($s, "a");
来源：http://pn.muxihuayi.cn

JS:   s.split("a").length - 1
来源：http://cj.bookmarksfly.cn

TS:   s.split("a").length - 1
来源：http://cp.huixinmuqiang.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hy.lnxyls.cn

Go:   strings.Count(s, "a")
来源：http://ru.yuntaijiaju.cn

Ruby: s.count("a")
来源：http://yi.nicolike.cn

C#:   s.Count(c => c == 'a')
来源：http://dx.bjjhwx.cn

[E13] 逐字符遍历
来源：http://hh.yuexingan06.cn

Py:   for ch in s: print(ch)
来源：http://so.hahajie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qu.gzmigu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ks.huanxung.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://js.9csxet.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cv.521024.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://we.colortex.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://fi.bjjhwx.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dg.9csxet.cn

[E14] URL 编码与 Base64
来源：http://tu.521024.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rw.9csxet.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://zv.panjiajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kj.gzmigu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ye.szxytkj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vh.bjjhwx.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wn.panjiajie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ph.haigaiapp.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bf.hnjuh.cn

[E15] HTML 转义 / 反转义
来源：http://wh.asd995.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://dv.bookmarksfly.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gr.szsharing.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vc.newstarts.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://kh.9csxet.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://my.panjiajie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mb.bookmarksfly.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://no.wgjwhj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://po.colortex.cn

[E16] 数字千分位
来源：http://mb.huanxung.cn

Py:   f"{1234567:,}"
来源：http://ty.newstarts.cn

PHP:  number_format(1234567);
来源：http://hi.wgjwhj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ve.jianghongdianzi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://kb.jianghongdianzi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ka.panjiajie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lz.521024.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ii.chemitech.net.cn

C#:   1234567.ToString("N0")
来源：http://ut.hnjuh.cn

[E17] 首字母大写
来源：http://hj.huixinmuqiang.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qa.gzmigu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://zc.szsharing.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wr.haigaiapp.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uu.asd995.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bp.hahajie.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yd.9csxet.cn

Ruby: s.capitalize
来源：http://lt.jianghongdianzi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jz.asd995.cn

[E18] 模板占位符替换
来源：http://lc.521024.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pl.9csxet.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ak.yuntaijiaju.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://jz.hahajie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ps.yuntaijiaju.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://or.nszjky.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://uv.yuntaijiaju.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hw.colortex.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tk.huixiangedu.cn

[E19] 多行文本按行拆分
来源：http://aj.jctech888.com.cn

Py:   s.splitlines()
来源：http://ae.hahajie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nv.wgjwhj.cn

JS:   s.split(/\r?\n/)
来源：http://zy.asd995.cn

TS:   s.split(/\r?\n/)
来源：http://yb.9csxet.cn

Java: s.lines().toList()
来源：http://pa.wgjwhj.cn

Go:   strings.Split(s, "\n")
来源：http://yl.wgjwhj.cn

Ruby: s.lines
来源：http://yt.bjjhwx.cn

C#:   s.Split('\n')
来源：http://io.yuexingan06.cn

[E20] 判断字符串是否为空
来源：http://pr.9csxet.cn

Py:   if not s:
来源：http://nu.yuntaijiaju.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lz.wgjwhj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hk.shtwfgs.cn

TS:   if (s === "") {}
来源：http://ie.shxzskj.cn

Java: if (s.isEmpty()) {}
来源：http://nm.jctech888.com.cn

Go:   if s == "" {}
来源：http://tl.szsharing.cn

Ruby: if s.empty?
来源：http://fy.wgjwhj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dp.panjiajie.cn

[E21] 超长截断加省略号
来源：http://cg.chemitech.net.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ts.panjiajie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jh.muxihuayi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ue.nicolike.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zn.muxihuayi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://uk.panjiajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://bk.yuexingan06.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pm.shxzukj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tj.521024.cn

[E22] 字节长度与字符长度
来源：http://yt.lnxyls.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sq.yuntaijiaju.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mm.yuexingan06.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fx.nicolike.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zd.hahajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pt.gzmigu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ml.yuntaijiaju.cn

Ruby: s.bytesize;  s.length
来源：http://uz.jianghongdianzi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kn.shxzskj.cn

================================================================================
来源：http://ly.nicolike.cn

F. 文件与目录
来源：http://pv.huixinmuqiang.cn

================================================================================
来源：http://az.newstarts.cn

[F01] 读取整个文件
来源：http://bg.9csxet.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jm.wgjwhj.cn

PHP:  file_get_contents("a.txt");
来源：http://pc.haigaiapp.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fp.jianghongdianzi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fu.yuntaijiaju.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://im.huanxung.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sw.huanxung.cn

Ruby: File.read("a.txt")
来源：http://et.szxytkj.cn

C#:   File.ReadAllText("a.txt");
来源：http://cj.szxytkj.cn

[F02] 逐行读取文件
来源：http://qw.bjjhwx.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kz.szxytkj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://px.wgjwhj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tk.szsharing.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aw.asd995.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hp.shxzukj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ue.jianghongdianzi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://is.jianghongdianzi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vi.shxzskj.cn

[F03] 写入文件（覆盖）
来源：http://ri.hnjuh.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://eh.jianghongdianzi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://wr.9csxet.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zc.nicolike.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yn.hnjuh.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bn.colortex.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ga.asd995.cn

Ruby: File.write("a.txt", "hi")
来源：http://qh.colortex.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tq.bjjhwx.cn

[F04] 追加写入文件
来源：http://se.yuexingan06.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://oi.hnjuh.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gc.newstarts.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gd.wgjwhj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zp.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gy.haigaiapp.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wp.chemitech.net.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wv.jianghongdianzi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sr.nicolike.cn

[F05] 判断文件或目录是否存在
来源：http://ok.jctech888.com.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://uq.yuntaijiaju.cn

PHP:  file_exists("a.txt");
来源：http://gm.lnxyls.cn

JS:   fs.existsSync("a.txt")
来源：http://em.hahajie.cn

TS:   fs.existsSync("a.txt")
来源：http://ki.shxzukj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://bg.haigaiapp.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ud.shtwfgs.cn

Ruby: File.exist?("a.txt")
来源：http://em.newstarts.cn

C#:   File.Exists("a.txt")
来源：http://py.521024.cn

[F06] 删除文件
来源：http://pi.wgjwhj.cn

Py:   os.remove("a.txt")
来源：http://xw.nicolike.cn

PHP:  unlink("a.txt");
来源：http://ku.haigaiapp.cn

JS:   fs.unlinkSync("a.txt")
来源：http://uz.nicolike.cn

TS:   fs.unlinkSync("a.txt")
来源：http://lz.hahajie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://du.bjjhwx.cn

Go:   os.Remove("a.txt")
来源：http://px.nicolike.cn

Ruby: File.delete("a.txt")
来源：http://bo.haigaiapp.cn

C#:   File.Delete("a.txt");
来源：http://eh.szxytkj.cn

[F07] 创建目录（含多级）
来源：http://uo.szxytkj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://og.hahajie.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bm.9csxet.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wj.lnxyls.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mc.huixinmuqiang.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cd.wgjwhj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cu.bookmarksfly.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yw.hnjuh.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://uq.9csxet.cn

[F08] 遍历目录
来源：http://zw.hahajie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://so.szsharing.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dh.haigaiapp.cn

JS:   fs.readdirSync("dir")
来源：http://hw.nicolike.cn

TS:   fs.readdirSync("dir")
来源：http://jp.gzmigu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pr.huixiangedu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ea.chemitech.net.cn

Ruby: Dir.children("dir")
来源：http://uz.wgjwhj.cn

C#:   Directory.GetFiles("dir")
来源：http://ip.bjjhwx.cn

[F09] 获取文件大小
来源：http://sn.chemitech.net.cn

Py:   os.path.getsize("a.txt")
来源：http://pj.huixinmuqiang.cn

PHP:  filesize("a.txt");
来源：http://gt.521024.cn

JS:   fs.statSync("a.txt").size
来源：http://yk.hahajie.cn

TS:   fs.statSync("a.txt").size
来源：http://of.asd995.cn

Java: Files.size(Path.of("a.txt"))
来源：http://yv.muxihuayi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pf.nicolike.cn

Ruby: File.size("a.txt")
来源：http://pi.9csxet.cn

C#:   new FileInfo("a.txt").Length
来源：http://qe.hahajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://yh.shxzskj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ya.shxzskj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wd.yuexingan06.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://it.wgjwhj.cn

TS:   path.extname("a.txt")
来源：http://vi.lnxyls.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rz.jianghongdianzi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rf.huixinmuqiang.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lr.hnjuh.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kd.jctech888.com.cn

[F11] 复制与移动文件
来源：http://bw.shxzskj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kc.huixinmuqiang.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zg.haigaiapp.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vs.521024.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vf.huixiangedu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xr.bookmarksfly.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hf.shxzukj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jj.hnjuh.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://iw.shxzukj.cn

[F12] CSV 读写
来源：http://rj.hahajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wv.jianghongdianzi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qn.panjiajie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ep.nszjky.cn

TS:   // 同上
来源：http://tt.hnjuh.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ne.muxihuayi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fb.muxihuayi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rg.bjjhwx.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://sf.nszjky.cn

================================================================================
来源：http://li.huixinmuqiang.cn

G. 面向对象
来源：http://mk.bjjhwx.cn

================================================================================
来源：http://qx.chemitech.net.cn

[G01] 定义类
来源：http://hr.lnxyls.cn

Py:   class User: pass
来源：http://sp.haigaiapp.cn

PHP:  class User {}
来源：http://yo.yuntaijiaju.cn

JS:   class User {}
来源：http://ie.wgjwhj.cn

TS:   class User { name: string = ""; }
来源：http://dg.shtwfgs.cn

Java: class User {}
来源：http://et.szsharing.cn

Go:   type User struct { Name string }
来源：http://dm.jctech888.com.cn

Ruby: class User; end
来源：http://qu.huixinmuqiang.cn

C#:   class User {}
来源：http://yi.huixinmuqiang.cn

[G02] 构造函数
来源：http://fc.huixinmuqiang.cn

Py:   def __init__(self, name): self.name = name
来源：http://kj.bookmarksfly.cn

PHP:  public function __construct(public string $name) {}
来源：http://ii.shxzukj.cn

JS:   constructor(name) { this.name = name; }
来源：http://hb.szsharing.cn

TS:   constructor(public name: string) {}
来源：http://cq.9csxet.cn

Java: User(String name) { this.name = name; }
来源：http://kf.nszjky.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xr.gzmigu.cn

Ruby: def initialize(name); @name = name; end
来源：http://es.shxzukj.cn

C#:   public User(string name) { Name = name; }
来源：http://cv.newstarts.cn

[G03] 实例属性
来源：http://ge.shxzskj.cn

Py:   self.name = "x"
来源：http://zy.yuexingan06.cn

PHP:  public string $name = "x";
来源：http://ru.jianghongdianzi.cn

JS:   this.name = "x";
来源：http://ll.nszjky.cn

TS:   name: string = "x";
来源：http://wf.shxzukj.cn

Java: private String name;
来源：http://ad.muxihuayi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ij.huixiangedu.cn

Ruby: @name = "x"
来源：http://ke.wgjwhj.cn

C#:   public string Name { get; set; } = "x";
来源：http://zw.shxzukj.cn

[G04] 定义方法
来源：http://ns.newstarts.cn

Py:   def greet(self): return self.name
来源：http://sy.szsharing.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://dv.shxzskj.cn

JS:   greet() { return this.name; }
来源：http://rg.jctech888.com.cn

TS:   greet(): string { return this.name; }
来源：http://it.shxzskj.cn

Java: String greet() { return name; }
来源：http://uc.lnxyls.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://yx.wgjwhj.cn

Ruby: def greet; @name; end
来源：http://fh.521024.cn

C#:   public string Greet() => Name;
来源：http://aa.jctech888.com.cn

[G05] 继承
来源：http://fv.yuexingan06.cn

Py:   class Admin(User): pass
来源：http://jr.bookmarksfly.cn

PHP:  class Admin extends User {}
来源：http://yx.jianghongdianzi.cn

JS:   class Admin extends User {}
来源：http://vo.yuntaijiaju.cn

TS:   class Admin extends User {}
来源：http://zu.hnjuh.cn

Java: class Admin extends User {}
来源：http://eh.szxytkj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hk.colortex.cn

Ruby: class Admin < User; end
来源：http://cf.bookmarksfly.cn

C#:   class Admin : User {}
来源：http://eo.shxzukj.cn

[G06] 重写方法
来源：http://ek.nicolike.cn

Py:   def greet(self): return "admin"
来源：http://et.newstarts.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://yl.lnxyls.cn

JS:   greet() { return "admin"; }
来源：http://gm.bjjhwx.cn


<!-- 参考信息 -->