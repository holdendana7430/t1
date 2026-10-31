代发 wailian999

Go:   strings.Join(items, ",")
来源：http://gq.shxzukj.cn

Ruby: items.join(",")
来源：http://wj.nicolike.cn

C#:   string.Join(",", items)
来源：http://cu.bjjhwx.cn

[E09] 去除所有空白字符
来源：http://ek.huixinmuqiang.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fy.jctech888.com.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hg.gzmigu.cn

JS:   s.replace(/\s+/g, "")
来源：http://wq.9csxet.cn

TS:   s.replace(/\s+/g, "")
来源：http://lz.chemitech.net.cn

Java: s.replaceAll("\\s+", "")
来源：http://wr.muxihuayi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://yt.chemitech.net.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ot.yuexingan06.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ky.haigaiapp.cn

[E10] 左侧补零 / 定长填充
来源：http://ub.9csxet.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xm.lnxyls.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mn.asd995.cn

JS:   "7".padStart(3, "0")
来源：http://uv.newstarts.cn

TS:   "7".padStart(3, "0")
来源：http://jg.shtwfgs.cn

Java: String.format("%03d", 7)
来源：http://bq.panjiajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://yc.lnxyls.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jx.muxihuayi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kp.nszjky.cn

[E11] 反转字符串
来源：http://np.huixinmuqiang.cn

Py:   s[::-1]
来源：http://pc.szsharing.cn

PHP:  strrev($s);
来源：http://ud.jianghongdianzi.cn

JS:   [...s].reverse().join("")
来源：http://bh.yuexingan06.cn

TS:   [...s].reverse().join("")
来源：http://ms.hnjuh.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://xm.newstarts.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://pu.yuntaijiaju.cn

Ruby: s.reverse
来源：http://vi.huixiangedu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://yh.hahajie.cn

[E12] 统计某字符出现次数
来源：http://km.panjiajie.cn

Py:   s.count("a")
来源：http://kt.haigaiapp.cn

PHP:  substr_count($s, "a");
来源：http://dz.yuntaijiaju.cn

JS:   s.split("a").length - 1
来源：http://zn.nszjky.cn

TS:   s.split("a").length - 1
来源：http://lc.gzmigu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://su.chemitech.net.cn

Go:   strings.Count(s, "a")
来源：http://ye.bjjhwx.cn

Ruby: s.count("a")
来源：http://xn.huanxung.cn

C#:   s.Count(c => c == 'a')
来源：http://zt.521024.cn

[E13] 逐字符遍历
来源：http://lr.huanxung.cn

Py:   for ch in s: print(ch)
来源：http://zu.huanxung.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mc.shxzskj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://mu.colortex.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://yw.nicolike.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ji.nszjky.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://oi.asd995.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://mj.jctech888.com.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mf.huixiangedu.cn

[E14] URL 编码与 Base64
来源：http://uc.hnjuh.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tg.huanxung.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bi.bjjhwx.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://et.panjiajie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dp.hahajie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lk.huanxung.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yf.gzmigu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kr.huanxung.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cv.bookmarksfly.cn

[E15] HTML 转义 / 反转义
来源：http://uk.wgjwhj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://an.szxytkj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wu.nszjky.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jt.nicolike.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://yz.jctech888.com.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://za.9csxet.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pq.asd995.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yb.huixiangedu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hq.shxzskj.cn

[E16] 数字千分位
来源：http://qm.hahajie.cn

Py:   f"{1234567:,}"
来源：http://nd.jctech888.com.cn

PHP:  number_format(1234567);
来源：http://oc.lnxyls.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ye.nicolike.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ad.bookmarksfly.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cq.yuntaijiaju.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://av.chemitech.net.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://eo.newstarts.cn

C#:   1234567.ToString("N0")
来源：http://ev.yuntaijiaju.cn

[E17] 首字母大写
来源：http://bd.gzmigu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wp.wgjwhj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://mk.colortex.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lw.haigaiapp.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uh.yuntaijiaju.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lg.9csxet.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hu.bookmarksfly.cn

Ruby: s.capitalize
来源：http://fu.yuexingan06.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rr.gzmigu.cn

[E18] 模板占位符替换
来源：http://we.hahajie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wv.chemitech.net.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ru.yuntaijiaju.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://iw.nszjky.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://tx.lnxyls.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bz.gzmigu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sw.yuexingan06.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gf.huixiangedu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wi.huanxung.cn

[E19] 多行文本按行拆分
来源：http://ix.hahajie.cn

Py:   s.splitlines()
来源：http://he.hnjuh.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vn.hnjuh.cn

JS:   s.split(/\r?\n/)
来源：http://nd.szsharing.cn

TS:   s.split(/\r?\n/)
来源：http://og.jianghongdianzi.cn

Java: s.lines().toList()
来源：http://fb.shtwfgs.cn

Go:   strings.Split(s, "\n")
来源：http://uk.haigaiapp.cn

Ruby: s.lines
来源：http://lj.huanxung.cn

C#:   s.Split('\n')
来源：http://dl.gzmigu.cn

[E20] 判断字符串是否为空
来源：http://mn.shtwfgs.cn

Py:   if not s:
来源：http://iu.asd995.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kd.shxzukj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xe.yuexingan06.cn

TS:   if (s === "") {}
来源：http://ai.521024.cn

Java: if (s.isEmpty()) {}
来源：http://od.hahajie.cn

Go:   if s == "" {}
来源：http://qw.yuntaijiaju.cn

Ruby: if s.empty?
来源：http://vq.bjjhwx.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nr.muxihuayi.cn

[E21] 超长截断加省略号
来源：http://dd.haigaiapp.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cr.gzmigu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://az.9csxet.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bs.bjjhwx.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zj.chemitech.net.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fq.colortex.cn

Go:   // 按 rune 判断长度后截断
来源：http://yt.muxihuayi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://in.jianghongdianzi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qb.bjjhwx.cn

[E22] 字节长度与字符长度
来源：http://qf.yuntaijiaju.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hc.colortex.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fr.hnjuh.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ly.hnjuh.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rx.chemitech.net.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jf.nicolike.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://su.colortex.cn

Ruby: s.bytesize;  s.length
来源：http://lt.bookmarksfly.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sp.bookmarksfly.cn

================================================================================
来源：http://hu.hahajie.cn

F. 文件与目录
来源：http://nq.jianghongdianzi.cn

================================================================================
来源：http://ve.521024.cn

[F01] 读取整个文件
来源：http://fs.szxytkj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mu.jctech888.com.cn

PHP:  file_get_contents("a.txt");
来源：http://ux.huixinmuqiang.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://km.szxytkj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fx.asd995.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zd.bjjhwx.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ck.newstarts.cn

Ruby: File.read("a.txt")
来源：http://mk.shtwfgs.cn

C#:   File.ReadAllText("a.txt");
来源：http://bu.szsharing.cn

[F02] 逐行读取文件
来源：http://lz.jctech888.com.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mh.huixinmuqiang.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rm.huixinmuqiang.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ne.lnxyls.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uz.wgjwhj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://io.yuntaijiaju.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qv.shtwfgs.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://or.jctech888.com.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zt.szsharing.cn

[F03] 写入文件（覆盖）
来源：http://pk.hnjuh.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wk.hahajie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vo.shtwfgs.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://su.shxzskj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pe.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dq.wgjwhj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://uf.colortex.cn

Ruby: File.write("a.txt", "hi")
来源：http://tp.szsharing.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fn.wgjwhj.cn

[F04] 追加写入文件
来源：http://tb.szsharing.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yf.gzmigu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://br.bjjhwx.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zh.shxzukj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ta.huixiangedu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gc.shxzskj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mf.huanxung.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ol.haigaiapp.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ft.gzmigu.cn

[F05] 判断文件或目录是否存在
来源：http://nd.521024.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hq.hahajie.cn

PHP:  file_exists("a.txt");
来源：http://dc.huixiangedu.cn

JS:   fs.existsSync("a.txt")
来源：http://jd.hnjuh.cn

TS:   fs.existsSync("a.txt")
来源：http://oc.chemitech.net.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xl.shxzukj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qb.521024.cn

Ruby: File.exist?("a.txt")
来源：http://gm.szsharing.cn

C#:   File.Exists("a.txt")
来源：http://vk.shxzskj.cn

[F06] 删除文件
来源：http://tw.hahajie.cn

Py:   os.remove("a.txt")
来源：http://mh.asd995.cn

PHP:  unlink("a.txt");
来源：http://jv.yuexingan06.cn

JS:   fs.unlinkSync("a.txt")
来源：http://nj.yuntaijiaju.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ca.szxytkj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fu.huixiangedu.cn

Go:   os.Remove("a.txt")
来源：http://ih.nicolike.cn

Ruby: File.delete("a.txt")
来源：http://ea.bookmarksfly.cn

C#:   File.Delete("a.txt");
来源：http://gs.muxihuayi.cn

[F07] 创建目录（含多级）
来源：http://bp.colortex.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://yb.colortex.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://um.haigaiapp.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ax.gzmigu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://el.yuntaijiaju.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gr.muxihuayi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://uy.wgjwhj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://uy.newstarts.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gl.chemitech.net.cn

[F08] 遍历目录
来源：http://lv.colortex.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://km.haigaiapp.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ym.hnjuh.cn

JS:   fs.readdirSync("dir")
来源：http://fp.9csxet.cn

TS:   fs.readdirSync("dir")
来源：http://my.jianghongdianzi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dm.huixiangedu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://rw.panjiajie.cn

Ruby: Dir.children("dir")
来源：http://ta.wgjwhj.cn

C#:   Directory.GetFiles("dir")
来源：http://cf.lnxyls.cn

[F09] 获取文件大小
来源：http://yq.huanxung.cn

Py:   os.path.getsize("a.txt")
来源：http://oi.shxzukj.cn

PHP:  filesize("a.txt");
来源：http://pa.yuexingan06.cn

JS:   fs.statSync("a.txt").size
来源：http://he.yuntaijiaju.cn

TS:   fs.statSync("a.txt").size
来源：http://ib.newstarts.cn

Java: Files.size(Path.of("a.txt"))
来源：http://oz.wgjwhj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mo.newstarts.cn

Ruby: File.size("a.txt")
来源：http://se.huixiangedu.cn

C#:   new FileInfo("a.txt").Length
来源：http://un.szxytkj.cn

[F10] 取文件扩展名 / 文件名
来源：http://yf.yuexingan06.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gv.panjiajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://px.newstarts.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fd.nszjky.cn

TS:   path.extname("a.txt")
来源：http://ek.huixinmuqiang.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rh.yuexingan06.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hs.yuexingan06.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bs.shxzukj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gv.panjiajie.cn

[F11] 复制与移动文件
来源：http://jb.bookmarksfly.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://eq.wgjwhj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tc.wgjwhj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rb.newstarts.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ak.huanxung.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ca.szxytkj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dj.huixiangedu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cq.muxihuayi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lh.yuntaijiaju.cn

[F12] CSV 读写
来源：http://eg.bjjhwx.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://df.521024.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://so.haigaiapp.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ev.bjjhwx.cn

TS:   // 同上
来源：http://lb.yuntaijiaju.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wo.9csxet.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://es.colortex.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://uv.chemitech.net.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://im.yuexingan06.cn

================================================================================
来源：http://sk.shtwfgs.cn

G. 面向对象
来源：http://nb.huixiangedu.cn

================================================================================
来源：http://vm.hnjuh.cn

[G01] 定义类
来源：http://vm.muxihuayi.cn

Py:   class User: pass
来源：http://pp.szxytkj.cn

PHP:  class User {}
来源：http://bm.gzmigu.cn

JS:   class User {}
来源：http://oq.newstarts.cn

TS:   class User { name: string = ""; }
来源：http://la.newstarts.cn

Java: class User {}
来源：http://yd.bookmarksfly.cn

Go:   type User struct { Name string }
来源：http://ho.colortex.cn

Ruby: class User; end
来源：http://jt.yuexingan06.cn

C#:   class User {}
来源：http://ro.huixiangedu.cn

[G02] 构造函数
来源：http://jl.nszjky.cn

Py:   def __init__(self, name): self.name = name
来源：http://kh.9csxet.cn

PHP:  public function __construct(public string $name) {}
来源：http://pg.9csxet.cn

JS:   constructor(name) { this.name = name; }
来源：http://wa.yuexingan06.cn

TS:   constructor(public name: string) {}
来源：http://ne.haigaiapp.cn

Java: User(String name) { this.name = name; }
来源：http://ha.9csxet.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bm.wgjwhj.cn

Ruby: def initialize(name); @name = name; end
来源：http://fw.huanxung.cn

C#:   public User(string name) { Name = name; }
来源：http://zn.jctech888.com.cn

[G03] 实例属性
来源：http://je.shxzukj.cn

Py:   self.name = "x"
来源：http://yv.huixiangedu.cn

PHP:  public string $name = "x";
来源：http://mg.bookmarksfly.cn

JS:   this.name = "x";
来源：http://ob.bookmarksfly.cn

TS:   name: string = "x";
来源：http://qg.newstarts.cn

Java: private String name;
来源：http://mc.huixinmuqiang.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://md.shtwfgs.cn

Ruby: @name = "x"
来源：http://vx.yuexingan06.cn

C#:   public string Name { get; set; } = "x";
来源：http://vd.muxihuayi.cn

[G04] 定义方法
来源：http://mr.szsharing.cn

Py:   def greet(self): return self.name
来源：http://kg.9csxet.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://py.shtwfgs.cn

JS:   greet() { return this.name; }
来源：http://do.shtwfgs.cn

TS:   greet(): string { return this.name; }
来源：http://mx.muxihuayi.cn

Java: String greet() { return name; }
来源：http://je.panjiajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://dn.yuexingan06.cn

Ruby: def greet; @name; end
来源：http://ck.panjiajie.cn

C#:   public string Greet() => Name;
来源：http://ie.chemitech.net.cn

[G05] 继承
来源：http://mr.jianghongdianzi.cn

Py:   class Admin(User): pass
来源：http://qs.shxzskj.cn

PHP:  class Admin extends User {}
来源：http://nt.shxzukj.cn

JS:   class Admin extends User {}
来源：http://iu.nicolike.cn

TS:   class Admin extends User {}
来源：http://li.panjiajie.cn

Java: class Admin extends User {}
来源：http://fm.panjiajie.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ow.huixinmuqiang.cn

Ruby: class Admin < User; end
来源：http://ry.panjiajie.cn

C#:   class Admin : User {}
来源：http://lk.jctech888.com.cn

[G06] 重写方法
来源：http://fz.huanxung.cn

Py:   def greet(self): return "admin"
来源：http://za.shxzukj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ay.bookmarksfly.cn

JS:   greet() { return "admin"; }
来源：http://lt.shtwfgs.cn

TS:   greet(): string { return "admin"; }
来源：http://eo.jctech888.com.cn

Java: @Override String greet() { return "admin"; }
来源：http://kr.bookmarksfly.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nl.hnjuh.cn

Ruby: def greet; "admin"; end
来源：http://fi.shtwfgs.cn

C#:   public override string Greet() => "admin";
来源：http://yq.yuexingan06.cn

[G07] 调用父类方法
来源：http://er.haigaiapp.cn

Py:   super().greet()
来源：http://ma.muxihuayi.cn

PHP:  parent::greet();
来源：http://wy.nicolike.cn


<!-- 参考信息 -->