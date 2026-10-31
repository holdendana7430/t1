代发 wailian999

PHP:  implode(",", $items);
来源：http://vf.yuntaijiaju.cn

JS:   items.join(",")
来源：http://na.shxzukj.cn

TS:   items.join(",")
来源：http://hx.shxzskj.cn

Java: String.join(",", items)
来源：http://vh.nszjky.cn

Go:   strings.Join(items, ",")
来源：http://qe.bookmarksfly.cn

Ruby: items.join(",")
来源：http://ly.haigaiapp.cn

C#:   string.Join(",", items)
来源：http://hl.chemitech.net.cn

[E09] 去除所有空白字符
来源：http://sl.huanxung.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jd.colortex.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://uh.muxihuayi.cn

JS:   s.replace(/\s+/g, "")
来源：http://yz.jianghongdianzi.cn

TS:   s.replace(/\s+/g, "")
来源：http://wy.colortex.cn

Java: s.replaceAll("\\s+", "")
来源：http://jc.colortex.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ea.colortex.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ux.shxzskj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://et.haigaiapp.cn

[E10] 左侧补零 / 定长填充
来源：http://mn.yuntaijiaju.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://am.nicolike.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://yi.nszjky.cn

JS:   "7".padStart(3, "0")
来源：http://cd.panjiajie.cn

TS:   "7".padStart(3, "0")
来源：http://hh.jctech888.com.cn

Java: String.format("%03d", 7)
来源：http://hr.lnxyls.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ie.newstarts.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yd.nszjky.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ts.szxytkj.cn

[E11] 反转字符串
来源：http://gn.muxihuayi.cn

Py:   s[::-1]
来源：http://yg.nszjky.cn

PHP:  strrev($s);
来源：http://jb.muxihuayi.cn

JS:   [...s].reverse().join("")
来源：http://fv.shxzukj.cn

TS:   [...s].reverse().join("")
来源：http://ma.gzmigu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://se.shtwfgs.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://wo.panjiajie.cn

Ruby: s.reverse
来源：http://vk.colortex.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ss.haigaiapp.cn

[E12] 统计某字符出现次数
来源：http://be.jianghongdianzi.cn

Py:   s.count("a")
来源：http://pd.gzmigu.cn

PHP:  substr_count($s, "a");
来源：http://ro.wgjwhj.cn

JS:   s.split("a").length - 1
来源：http://nx.chemitech.net.cn

TS:   s.split("a").length - 1
来源：http://wn.asd995.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lr.nszjky.cn

Go:   strings.Count(s, "a")
来源：http://xw.colortex.cn

Ruby: s.count("a")
来源：http://nv.lnxyls.cn

C#:   s.Count(c => c == 'a')
来源：http://il.yuntaijiaju.cn

[E13] 逐字符遍历
来源：http://oj.lnxyls.cn

Py:   for ch in s: print(ch)
来源：http://am.chemitech.net.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://oo.panjiajie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://yt.jctech888.com.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://xo.jianghongdianzi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bb.nszjky.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fq.lnxyls.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ac.wgjwhj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ap.newstarts.cn

[E14] URL 编码与 Base64
来源：http://kz.shxzukj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ms.lnxyls.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ns.hahajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zc.muxihuayi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mb.asd995.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ud.shxzskj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.nicolike.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ik.hahajie.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://da.shxzukj.cn

[E15] HTML 转义 / 反转义
来源：http://ak.newstarts.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://lo.muxihuayi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://iu.huanxung.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://me.shtwfgs.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://bc.panjiajie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dm.hahajie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://my.wgjwhj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dt.colortex.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://df.szxytkj.cn

[E16] 数字千分位
来源：http://nt.bookmarksfly.cn

Py:   f"{1234567:,}"
来源：http://bt.bookmarksfly.cn

PHP:  number_format(1234567);
来源：http://uq.9csxet.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://dr.asd995.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://rj.nszjky.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://yl.bjjhwx.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ag.huanxung.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nb.shxzukj.cn

C#:   1234567.ToString("N0")
来源：http://fb.huanxung.cn

[E17] 首字母大写
来源：http://yk.huixiangedu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ye.jianghongdianzi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ys.nszjky.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kc.jianghongdianzi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yv.muxihuayi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wo.huanxung.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vj.shxzskj.cn

Ruby: s.capitalize
来源：http://mg.colortex.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qe.newstarts.cn

[E18] 模板占位符替换
来源：http://uk.nszjky.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tn.bjjhwx.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ib.huixiangedu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://gg.nicolike.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://pp.bjjhwx.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://br.asd995.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ib.9csxet.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cm.nicolike.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ay.huixiangedu.cn

[E19] 多行文本按行拆分
来源：http://hd.szxytkj.cn

Py:   s.splitlines()
来源：http://wz.jctech888.com.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ew.shtwfgs.cn

JS:   s.split(/\r?\n/)
来源：http://ij.colortex.cn

TS:   s.split(/\r?\n/)
来源：http://hc.colortex.cn

Java: s.lines().toList()
来源：http://ij.bookmarksfly.cn

Go:   strings.Split(s, "\n")
来源：http://ok.wgjwhj.cn

Ruby: s.lines
来源：http://tr.521024.cn

C#:   s.Split('\n')
来源：http://yw.bjjhwx.cn

[E20] 判断字符串是否为空
来源：http://hq.shxzukj.cn

Py:   if not s:
来源：http://oy.huixinmuqiang.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nx.newstarts.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qj.yuexingan06.cn

TS:   if (s === "") {}
来源：http://cr.nszjky.cn

Java: if (s.isEmpty()) {}
来源：http://vu.jianghongdianzi.cn

Go:   if s == "" {}
来源：http://fl.szsharing.cn

Ruby: if s.empty?
来源：http://uq.shtwfgs.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fl.asd995.cn

[E21] 超长截断加省略号
来源：http://ws.shtwfgs.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qv.bookmarksfly.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pn.shxzskj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://it.huanxung.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ri.haigaiapp.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kg.9csxet.cn

Go:   // 按 rune 判断长度后截断
来源：http://gi.huixiangedu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fw.shxzskj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://yd.yuexingan06.cn

[E22] 字节长度与字符长度
来源：http://cj.szsharing.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nj.jianghongdianzi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zt.jctech888.com.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ao.haigaiapp.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bc.bookmarksfly.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fy.gzmigu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wh.panjiajie.cn

Ruby: s.bytesize;  s.length
来源：http://gw.bookmarksfly.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wr.bjjhwx.cn

================================================================================
来源：http://ag.haigaiapp.cn

F. 文件与目录
来源：http://uo.newstarts.cn

================================================================================
来源：http://tl.huixiangedu.cn

[F01] 读取整个文件
来源：http://zu.haigaiapp.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vp.lnxyls.cn

PHP:  file_get_contents("a.txt");
来源：http://mm.huanxung.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fb.shxzskj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cm.jctech888.com.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://mt.shxzskj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uc.hnjuh.cn

Ruby: File.read("a.txt")
来源：http://us.hahajie.cn

C#:   File.ReadAllText("a.txt");
来源：http://er.szxytkj.cn

[F02] 逐行读取文件
来源：http://xb.szxytkj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vs.jctech888.com.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ae.9csxet.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pf.panjiajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pg.bookmarksfly.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://se.lnxyls.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gj.panjiajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://iu.haigaiapp.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://in.nicolike.cn

[F03] 写入文件（覆盖）
来源：http://wr.huixinmuqiang.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ac.jianghongdianzi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://bq.szxytkj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vm.huixiangedu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bs.shxzukj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hp.shtwfgs.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fy.wgjwhj.cn

Ruby: File.write("a.txt", "hi")
来源：http://gj.chemitech.net.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xj.hnjuh.cn

[F04] 追加写入文件
来源：http://qo.huixinmuqiang.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://iq.szxytkj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zp.bookmarksfly.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uj.yuntaijiaju.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cu.panjiajie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gw.yuexingan06.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wv.shxzskj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dx.bjjhwx.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gr.huanxung.cn

[F05] 判断文件或目录是否存在
来源：http://zp.bjjhwx.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://at.haigaiapp.cn

PHP:  file_exists("a.txt");
来源：http://gh.bookmarksfly.cn

JS:   fs.existsSync("a.txt")
来源：http://cv.szxytkj.cn

TS:   fs.existsSync("a.txt")
来源：http://qk.wgjwhj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://dy.yuexingan06.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://im.panjiajie.cn

Ruby: File.exist?("a.txt")
来源：http://vf.yuexingan06.cn

C#:   File.Exists("a.txt")
来源：http://yv.nszjky.cn

[F06] 删除文件
来源：http://cl.asd995.cn

Py:   os.remove("a.txt")
来源：http://zm.chemitech.net.cn

PHP:  unlink("a.txt");
来源：http://rf.bjjhwx.cn

JS:   fs.unlinkSync("a.txt")
来源：http://jt.521024.cn

TS:   fs.unlinkSync("a.txt")
来源：http://oa.shxzskj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zr.newstarts.cn

Go:   os.Remove("a.txt")
来源：http://ze.asd995.cn

Ruby: File.delete("a.txt")
来源：http://nj.hnjuh.cn

C#:   File.Delete("a.txt");
来源：http://sf.colortex.cn

[F07] 创建目录（含多级）
来源：http://fr.huixinmuqiang.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://yd.muxihuayi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://co.panjiajie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dc.nszjky.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fw.bjjhwx.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qe.szsharing.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pw.shxzskj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qy.newstarts.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xc.shxzukj.cn

[F08] 遍历目录
来源：http://ov.huixinmuqiang.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ga.lnxyls.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wi.huixiangedu.cn

JS:   fs.readdirSync("dir")
来源：http://nm.bookmarksfly.cn

TS:   fs.readdirSync("dir")
来源：http://uz.521024.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gr.asd995.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://er.haigaiapp.cn

Ruby: Dir.children("dir")
来源：http://jy.yuntaijiaju.cn

C#:   Directory.GetFiles("dir")
来源：http://uu.huixiangedu.cn

[F09] 获取文件大小
来源：http://jo.asd995.cn

Py:   os.path.getsize("a.txt")
来源：http://hw.nicolike.cn

PHP:  filesize("a.txt");
来源：http://pz.lnxyls.cn

JS:   fs.statSync("a.txt").size
来源：http://vf.yuexingan06.cn

TS:   fs.statSync("a.txt").size
来源：http://bk.chemitech.net.cn

Java: Files.size(Path.of("a.txt"))
来源：http://si.muxihuayi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ya.gzmigu.cn

Ruby: File.size("a.txt")
来源：http://hb.wgjwhj.cn

C#:   new FileInfo("a.txt").Length
来源：http://jr.gzmigu.cn

[F10] 取文件扩展名 / 文件名
来源：http://sp.huixinmuqiang.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cg.gzmigu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fm.szxytkj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://of.muxihuayi.cn

TS:   path.extname("a.txt")
来源：http://ph.jctech888.com.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bo.huanxung.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rg.521024.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mx.hnjuh.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xo.yuexingan06.cn

[F11] 复制与移动文件
来源：http://ka.521024.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bg.szxytkj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fs.jctech888.com.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zu.jianghongdianzi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jw.wgjwhj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jt.nszjky.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lg.yuntaijiaju.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zw.huanxung.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kb.huanxung.cn

[F12] CSV 读写
来源：http://re.szsharing.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fa.hnjuh.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sd.newstarts.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rq.newstarts.cn

TS:   // 同上
来源：http://gd.huanxung.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xf.gzmigu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bw.521024.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jn.haigaiapp.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://xt.panjiajie.cn

================================================================================
来源：http://kc.9csxet.cn

G. 面向对象
来源：http://kv.newstarts.cn

================================================================================
来源：http://ea.nszjky.cn

[G01] 定义类
来源：http://jv.shxzukj.cn

Py:   class User: pass
来源：http://ht.szxytkj.cn

PHP:  class User {}
来源：http://kf.wgjwhj.cn

JS:   class User {}
来源：http://gs.nszjky.cn

TS:   class User { name: string = ""; }
来源：http://ni.chemitech.net.cn

Java: class User {}
来源：http://my.wgjwhj.cn

Go:   type User struct { Name string }
来源：http://ot.521024.cn

Ruby: class User; end
来源：http://do.yuexingan06.cn

C#:   class User {}
来源：http://mv.nszjky.cn

[G02] 构造函数
来源：http://qt.wgjwhj.cn

Py:   def __init__(self, name): self.name = name
来源：http://qe.panjiajie.cn

PHP:  public function __construct(public string $name) {}
来源：http://dv.chemitech.net.cn

JS:   constructor(name) { this.name = name; }
来源：http://yj.shxzskj.cn

TS:   constructor(public name: string) {}
来源：http://yi.gzmigu.cn

Java: User(String name) { this.name = name; }
来源：http://ic.chemitech.net.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://be.nszjky.cn

Ruby: def initialize(name); @name = name; end
来源：http://cq.lnxyls.cn

C#:   public User(string name) { Name = name; }
来源：http://wx.hnjuh.cn

[G03] 实例属性
来源：http://tp.bjjhwx.cn

Py:   self.name = "x"
来源：http://pu.newstarts.cn

PHP:  public string $name = "x";
来源：http://fy.yuntaijiaju.cn

JS:   this.name = "x";
来源：http://ey.yuexingan06.cn

TS:   name: string = "x";
来源：http://af.9csxet.cn

Java: private String name;
来源：http://hv.newstarts.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bv.hnjuh.cn

Ruby: @name = "x"
来源：http://hf.gzmigu.cn

C#:   public string Name { get; set; } = "x";
来源：http://rr.chemitech.net.cn

[G04] 定义方法
来源：http://vy.hahajie.cn

Py:   def greet(self): return self.name
来源：http://tz.hnjuh.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://pw.nicolike.cn

JS:   greet() { return this.name; }
来源：http://zk.bjjhwx.cn

TS:   greet(): string { return this.name; }
来源：http://ga.huixiangedu.cn

Java: String greet() { return name; }
来源：http://et.shtwfgs.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://jw.huixiangedu.cn

Ruby: def greet; @name; end
来源：http://uk.jctech888.com.cn

C#:   public string Greet() => Name;
来源：http://xq.panjiajie.cn

[G05] 继承
来源：http://qh.haigaiapp.cn

Py:   class Admin(User): pass
来源：http://az.hnjuh.cn

PHP:  class Admin extends User {}
来源：http://rm.yuntaijiaju.cn

JS:   class Admin extends User {}
来源：http://mv.bookmarksfly.cn

TS:   class Admin extends User {}
来源：http://ln.shxzskj.cn

Java: class Admin extends User {}
来源：http://oo.muxihuayi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wh.bookmarksfly.cn

Ruby: class Admin < User; end
来源：http://bu.shxzskj.cn

C#:   class Admin : User {}
来源：http://gp.nicolike.cn

[G06] 重写方法
来源：http://gd.shxzskj.cn

Py:   def greet(self): return "admin"
来源：http://qp.panjiajie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://zr.jctech888.com.cn

JS:   greet() { return "admin"; }
来源：http://iw.muxihuayi.cn

TS:   greet(): string { return "admin"; }
来源：http://mr.huixiangedu.cn

Java: @Override String greet() { return "admin"; }
来源：http://fh.nicolike.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://az.colortex.cn

Ruby: def greet; "admin"; end
来源：http://rf.szsharing.cn


<!-- 参考信息 -->