代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://uk.gzmigu.cn

TS:   s.split(",")
来源：http://an.hahajie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://jc.shxzukj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cq.panjiajie.cn

Ruby: s.split(",");  s.split
来源：http://fa.jctech888.com.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sy.521024.cn

[E08] 数组按分隔符合并
来源：http://qk.521024.cn

Py:   ",".join(items)
来源：http://jj.huanxung.cn

PHP:  implode(",", $items);
来源：http://xq.muxihuayi.cn

JS:   items.join(",")
来源：http://ho.yuexingan06.cn

TS:   items.join(",")
来源：http://ai.nszjky.cn

Java: String.join(",", items)
来源：http://gn.huixiangedu.cn

Go:   strings.Join(items, ",")
来源：http://ny.jctech888.com.cn

Ruby: items.join(",")
来源：http://wx.huixiangedu.cn

C#:   string.Join(",", items)
来源：http://gk.wgjwhj.cn

[E09] 去除所有空白字符
来源：http://sm.panjiajie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wx.huixinmuqiang.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://it.szxytkj.cn

JS:   s.replace(/\s+/g, "")
来源：http://zc.chemitech.net.cn

TS:   s.replace(/\s+/g, "")
来源：http://gk.newstarts.cn

Java: s.replaceAll("\\s+", "")
来源：http://cr.szxytkj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://mb.asd995.cn

Ruby: s.gsub(/\s+/, "")
来源：http://yk.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://so.yuexingan06.cn

[E10] 左侧补零 / 定长填充
来源：http://wl.panjiajie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hv.jctech888.com.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rg.shtwfgs.cn

JS:   "7".padStart(3, "0")
来源：http://kp.nicolike.cn

TS:   "7".padStart(3, "0")
来源：http://fu.asd995.cn

Java: String.format("%03d", 7)
来源：http://hq.szxytkj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://aj.szxytkj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://og.gzmigu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://we.huixinmuqiang.cn

[E11] 反转字符串
来源：http://py.hnjuh.cn

Py:   s[::-1]
来源：http://bu.wgjwhj.cn

PHP:  strrev($s);
来源：http://cu.colortex.cn

JS:   [...s].reverse().join("")
来源：http://gn.hnjuh.cn

TS:   [...s].reverse().join("")
来源：http://dk.bookmarksfly.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://qh.gzmigu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ar.szxytkj.cn

Ruby: s.reverse
来源：http://aw.yuexingan06.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vf.gzmigu.cn

[E12] 统计某字符出现次数
来源：http://de.hnjuh.cn

Py:   s.count("a")
来源：http://qz.hnjuh.cn

PHP:  substr_count($s, "a");
来源：http://ra.muxihuayi.cn

JS:   s.split("a").length - 1
来源：http://ig.521024.cn

TS:   s.split("a").length - 1
来源：http://hy.shxzskj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://oh.colortex.cn

Go:   strings.Count(s, "a")
来源：http://kc.asd995.cn

Ruby: s.count("a")
来源：http://tu.chemitech.net.cn

C#:   s.Count(c => c == 'a')
来源：http://ir.huixiangedu.cn

[E13] 逐字符遍历
来源：http://cl.szsharing.cn

Py:   for ch in s: print(ch)
来源：http://tu.shxzskj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hr.muxihuayi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://eu.szsharing.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ic.shxzukj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://uk.jianghongdianzi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://uu.nicolike.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ot.gzmigu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ij.gzmigu.cn

[E14] URL 编码与 Base64
来源：http://ty.wgjwhj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fz.szsharing.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ov.huixiangedu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gu.yuntaijiaju.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nb.bookmarksfly.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://va.521024.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cb.shxzukj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dj.wgjwhj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://am.colortex.cn

[E15] HTML 转义 / 反转义
来源：http://ur.haigaiapp.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://bw.nicolike.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cl.nszjky.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pq.asd995.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://eu.szsharing.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ui.szsharing.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qw.gzmigu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vj.huanxung.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://it.yuexingan06.cn

[E16] 数字千分位
来源：http://tt.shtwfgs.cn

Py:   f"{1234567:,}"
来源：http://wp.yuntaijiaju.cn

PHP:  number_format(1234567);
来源：http://tq.colortex.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vl.lnxyls.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://gg.nicolike.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ga.haigaiapp.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xs.haigaiapp.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cv.muxihuayi.cn

C#:   1234567.ToString("N0")
来源：http://uy.wgjwhj.cn

[E17] 首字母大写
来源：http://he.bjjhwx.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://os.colortex.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://hv.nszjky.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://he.chemitech.net.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zw.nszjky.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ub.szxytkj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cc.colortex.cn

Ruby: s.capitalize
来源：http://dk.colortex.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fp.colortex.cn

[E18] 模板占位符替换
来源：http://up.muxihuayi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nx.haigaiapp.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://et.hahajie.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://yv.521024.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://sp.hahajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ml.asd995.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qy.lnxyls.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zl.nszjky.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qg.9csxet.cn

[E19] 多行文本按行拆分
来源：http://wl.muxihuayi.cn

Py:   s.splitlines()
来源：http://ob.szxytkj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pz.lnxyls.cn

JS:   s.split(/\r?\n/)
来源：http://pt.szxytkj.cn

TS:   s.split(/\r?\n/)
来源：http://hp.jctech888.com.cn

Java: s.lines().toList()
来源：http://pa.chemitech.net.cn

Go:   strings.Split(s, "\n")
来源：http://qa.9csxet.cn

Ruby: s.lines
来源：http://fg.521024.cn

C#:   s.Split('\n')
来源：http://ts.szxytkj.cn

[E20] 判断字符串是否为空
来源：http://dr.chemitech.net.cn

Py:   if not s:
来源：http://io.jctech888.com.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sh.yuexingan06.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yz.521024.cn

TS:   if (s === "") {}
来源：http://gp.nicolike.cn

Java: if (s.isEmpty()) {}
来源：http://fa.jctech888.com.cn

Go:   if s == "" {}
来源：http://xo.bjjhwx.cn

Ruby: if s.empty?
来源：http://jq.hahajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jx.huixinmuqiang.cn

[E21] 超长截断加省略号
来源：http://mh.jctech888.com.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ox.hnjuh.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yw.jctech888.com.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oc.521024.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lv.shtwfgs.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wk.shtwfgs.cn

Go:   // 按 rune 判断长度后截断
来源：http://jy.nicolike.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mq.hahajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ib.szxytkj.cn

[E22] 字节长度与字符长度
来源：http://dn.nicolike.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ku.shtwfgs.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://do.bookmarksfly.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://es.huixinmuqiang.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://km.huanxung.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ay.jctech888.com.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ij.lnxyls.cn

Ruby: s.bytesize;  s.length
来源：http://nd.newstarts.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rh.521024.cn

================================================================================
来源：http://zf.wgjwhj.cn

F. 文件与目录
来源：http://wi.szsharing.cn

================================================================================
来源：http://ij.chemitech.net.cn

[F01] 读取整个文件
来源：http://aa.szsharing.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kh.nicolike.cn

PHP:  file_get_contents("a.txt");
来源：http://oy.bjjhwx.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kn.jctech888.com.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qx.muxihuayi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://xk.shxzskj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ic.nszjky.cn

Ruby: File.read("a.txt")
来源：http://vu.hnjuh.cn

C#:   File.ReadAllText("a.txt");
来源：http://lg.yuntaijiaju.cn

[F02] 逐行读取文件
来源：http://ae.huixinmuqiang.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tt.jianghongdianzi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cy.bjjhwx.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jv.9csxet.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gq.shtwfgs.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nw.bjjhwx.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rn.jctech888.com.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hf.szsharing.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dm.colortex.cn

[F03] 写入文件（覆盖）
来源：http://gi.huixiangedu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wl.szsharing.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://np.shtwfgs.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gr.521024.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yg.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hp.jianghongdianzi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kv.jctech888.com.cn

Ruby: File.write("a.txt", "hi")
来源：http://gg.hnjuh.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zl.shtwfgs.cn

[F04] 追加写入文件
来源：http://bb.huixiangedu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ro.9csxet.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vt.gzmigu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cn.jianghongdianzi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bt.szsharing.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rx.9csxet.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bv.yuntaijiaju.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ia.jctech888.com.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gw.panjiajie.cn

[F05] 判断文件或目录是否存在
来源：http://rf.huixiangedu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xv.muxihuayi.cn

PHP:  file_exists("a.txt");
来源：http://mu.yuexingan06.cn

JS:   fs.existsSync("a.txt")
来源：http://ps.hahajie.cn

TS:   fs.existsSync("a.txt")
来源：http://oa.szsharing.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://bd.shtwfgs.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sb.hahajie.cn

Ruby: File.exist?("a.txt")
来源：http://oc.hahajie.cn

C#:   File.Exists("a.txt")
来源：http://ao.shtwfgs.cn

[F06] 删除文件
来源：http://xb.hnjuh.cn

Py:   os.remove("a.txt")
来源：http://et.shxzskj.cn

PHP:  unlink("a.txt");
来源：http://jr.lnxyls.cn

JS:   fs.unlinkSync("a.txt")
来源：http://lk.muxihuayi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://op.lnxyls.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pt.hnjuh.cn

Go:   os.Remove("a.txt")
来源：http://bc.shtwfgs.cn

Ruby: File.delete("a.txt")
来源：http://lj.haigaiapp.cn

C#:   File.Delete("a.txt");
来源：http://vb.bjjhwx.cn

[F07] 创建目录（含多级）
来源：http://dm.newstarts.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://al.jianghongdianzi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bk.nicolike.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ni.panjiajie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://te.huixinmuqiang.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zd.newstarts.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://py.yuexingan06.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dz.gzmigu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ze.jctech888.com.cn

[F08] 遍历目录
来源：http://ve.huixiangedu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zf.bjjhwx.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hg.huixinmuqiang.cn

JS:   fs.readdirSync("dir")
来源：http://wf.huixinmuqiang.cn

TS:   fs.readdirSync("dir")
来源：http://ky.gzmigu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sb.muxihuayi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://dc.newstarts.cn

Ruby: Dir.children("dir")
来源：http://fv.panjiajie.cn

C#:   Directory.GetFiles("dir")
来源：http://je.shxzskj.cn

[F09] 获取文件大小
来源：http://gt.huanxung.cn

Py:   os.path.getsize("a.txt")
来源：http://dx.jctech888.com.cn

PHP:  filesize("a.txt");
来源：http://ry.9csxet.cn

JS:   fs.statSync("a.txt").size
来源：http://ty.huixinmuqiang.cn

TS:   fs.statSync("a.txt").size
来源：http://pm.szsharing.cn

Java: Files.size(Path.of("a.txt"))
来源：http://kc.shtwfgs.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dp.521024.cn

Ruby: File.size("a.txt")
来源：http://by.hnjuh.cn

C#:   new FileInfo("a.txt").Length
来源：http://jg.bjjhwx.cn

[F10] 取文件扩展名 / 文件名
来源：http://zo.szsharing.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qb.shxzskj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dr.chemitech.net.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rh.nicolike.cn

TS:   path.extname("a.txt")
来源：http://nm.shxzukj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sm.nszjky.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mu.newstarts.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://my.colortex.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hf.hahajie.cn

[F11] 复制与移动文件
来源：http://dn.nicolike.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rv.huixiangedu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fu.wgjwhj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bx.521024.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pr.jctech888.com.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yo.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kq.gzmigu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wa.yuntaijiaju.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cr.haigaiapp.cn

[F12] CSV 读写
来源：http://dl.jctech888.com.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rn.newstarts.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ei.colortex.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://aw.bookmarksfly.cn

TS:   // 同上
来源：http://ly.shtwfgs.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nl.hahajie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ur.521024.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qg.newstarts.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://cf.jianghongdianzi.cn

================================================================================
来源：http://bj.huanxung.cn

G. 面向对象
来源：http://yx.shxzskj.cn

================================================================================
来源：http://pn.newstarts.cn

[G01] 定义类
来源：http://kh.newstarts.cn

Py:   class User: pass
来源：http://xw.wgjwhj.cn

PHP:  class User {}
来源：http://iz.huixiangedu.cn

JS:   class User {}
来源：http://vl.chemitech.net.cn

TS:   class User { name: string = ""; }
来源：http://xq.wgjwhj.cn

Java: class User {}
来源：http://ml.shxzukj.cn

Go:   type User struct { Name string }
来源：http://yi.bookmarksfly.cn

Ruby: class User; end
来源：http://yo.szsharing.cn

C#:   class User {}
来源：http://gg.jctech888.com.cn

[G02] 构造函数
来源：http://ma.yuntaijiaju.cn

Py:   def __init__(self, name): self.name = name
来源：http://zn.newstarts.cn

PHP:  public function __construct(public string $name) {}
来源：http://gx.asd995.cn

JS:   constructor(name) { this.name = name; }
来源：http://gg.muxihuayi.cn

TS:   constructor(public name: string) {}
来源：http://sh.nszjky.cn

Java: User(String name) { this.name = name; }
来源：http://qd.asd995.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://oy.shtwfgs.cn

Ruby: def initialize(name); @name = name; end
来源：http://qd.newstarts.cn

C#:   public User(string name) { Name = name; }
来源：http://cz.muxihuayi.cn

[G03] 实例属性
来源：http://ts.panjiajie.cn

Py:   self.name = "x"
来源：http://wh.bookmarksfly.cn

PHP:  public string $name = "x";
来源：http://vo.huixinmuqiang.cn

JS:   this.name = "x";
来源：http://vl.newstarts.cn

TS:   name: string = "x";
来源：http://tz.jianghongdianzi.cn

Java: private String name;
来源：http://uc.szsharing.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fc.9csxet.cn

Ruby: @name = "x"
来源：http://rv.nicolike.cn

C#:   public string Name { get; set; } = "x";
来源：http://zi.jianghongdianzi.cn

[G04] 定义方法
来源：http://jg.jctech888.com.cn

Py:   def greet(self): return self.name
来源：http://yc.gzmigu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://fo.nszjky.cn

JS:   greet() { return this.name; }
来源：http://zq.hahajie.cn

TS:   greet(): string { return this.name; }
来源：http://qu.gzmigu.cn

Java: String greet() { return name; }
来源：http://sc.huanxung.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://pe.szsharing.cn

Ruby: def greet; @name; end
来源：http://sc.yuexingan06.cn

C#:   public string Greet() => Name;
来源：http://hm.szxytkj.cn

[G05] 继承
来源：http://ew.colortex.cn

Py:   class Admin(User): pass
来源：http://os.szxytkj.cn

PHP:  class Admin extends User {}
来源：http://kf.yuexingan06.cn

JS:   class Admin extends User {}
来源：http://vw.hnjuh.cn

TS:   class Admin extends User {}
来源：http://vf.shxzukj.cn

Java: class Admin extends User {}
来源：http://rx.szsharing.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rv.lnxyls.cn

Ruby: class Admin < User; end
来源：http://jd.haigaiapp.cn

C#:   class Admin : User {}
来源：http://az.panjiajie.cn


<!-- 参考信息 -->