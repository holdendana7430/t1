代发 wailian999

[E06] 替换子串
来源：http://tr.wgjwhj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://en.newstarts.cn

PHP:  str_replace("a", "b", $s);
来源：http://uk.yuexingan06.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hk.jctech888.com.cn

TS:   s.replaceAll("a", "b")
来源：http://ku.gzmigu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ee.szxytkj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ql.gzmigu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://sy.nszjky.cn

C#:   s.Replace("a", "b")
来源：http://fd.asd995.cn

[E07] 按分隔符拆分
来源：http://xs.panjiajie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dw.yuntaijiaju.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mm.wgjwhj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://td.jctech888.com.cn

TS:   s.split(",")
来源：http://sj.bjjhwx.cn

Java: s.split(",");  s.split("\\s+")
来源：http://hj.nicolike.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lj.huixiangedu.cn

Ruby: s.split(",");  s.split
来源：http://wu.huanxung.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gb.wgjwhj.cn

[E08] 数组按分隔符合并
来源：http://ts.huixinmuqiang.cn

Py:   ",".join(items)
来源：http://mf.521024.cn

PHP:  implode(",", $items);
来源：http://hp.jianghongdianzi.cn

JS:   items.join(",")
来源：http://qs.muxihuayi.cn

TS:   items.join(",")
来源：http://xh.huixiangedu.cn

Java: String.join(",", items)
来源：http://ta.chemitech.net.cn

Go:   strings.Join(items, ",")
来源：http://ns.huixiangedu.cn

Ruby: items.join(",")
来源：http://oo.szxytkj.cn

C#:   string.Join(",", items)
来源：http://ao.bookmarksfly.cn

[E09] 去除所有空白字符
来源：http://uy.bjjhwx.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ca.panjiajie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ug.nszjky.cn

JS:   s.replace(/\s+/g, "")
来源：http://zq.hnjuh.cn

TS:   s.replace(/\s+/g, "")
来源：http://nq.shxzskj.cn

Java: s.replaceAll("\\s+", "")
来源：http://kn.shxzukj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://eu.hnjuh.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ua.lnxyls.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://my.panjiajie.cn

[E10] 左侧补零 / 定长填充
来源：http://nj.hahajie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yd.9csxet.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rm.nicolike.cn

JS:   "7".padStart(3, "0")
来源：http://sw.huanxung.cn

TS:   "7".padStart(3, "0")
来源：http://xg.lnxyls.cn

Java: String.format("%03d", 7)
来源：http://jp.bjjhwx.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://qa.9csxet.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hk.haigaiapp.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jr.jianghongdianzi.cn

[E11] 反转字符串
来源：http://uw.szsharing.cn

Py:   s[::-1]
来源：http://tb.huanxung.cn

PHP:  strrev($s);
来源：http://oi.chemitech.net.cn

JS:   [...s].reverse().join("")
来源：http://iv.gzmigu.cn

TS:   [...s].reverse().join("")
来源：http://oj.gzmigu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ht.huixiangedu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zg.colortex.cn

Ruby: s.reverse
来源：http://cl.nicolike.cn

C#:   new string(s.Reverse().ToArray())
来源：http://by.gzmigu.cn

[E12] 统计某字符出现次数
来源：http://jy.gzmigu.cn

Py:   s.count("a")
来源：http://cp.huixiangedu.cn

PHP:  substr_count($s, "a");
来源：http://qi.panjiajie.cn

JS:   s.split("a").length - 1
来源：http://bv.colortex.cn

TS:   s.split("a").length - 1
来源：http://no.bjjhwx.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pa.nszjky.cn

Go:   strings.Count(s, "a")
来源：http://vy.wgjwhj.cn

Ruby: s.count("a")
来源：http://iu.asd995.cn

C#:   s.Count(c => c == 'a')
来源：http://sb.szxytkj.cn

[E13] 逐字符遍历
来源：http://uy.521024.cn

Py:   for ch in s: print(ch)
来源：http://dq.shxzukj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ys.hnjuh.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ob.bjjhwx.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://fg.wgjwhj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jd.nicolike.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://et.chemitech.net.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://uj.lnxyls.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cf.hahajie.cn

[E14] URL 编码与 Base64
来源：http://xl.szxytkj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rh.bookmarksfly.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://yv.panjiajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://br.bookmarksfly.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cw.lnxyls.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://in.huixinmuqiang.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fg.colortex.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bw.nicolike.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yn.hnjuh.cn

[E15] HTML 转义 / 反转义
来源：http://hv.nszjky.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://lt.panjiajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://iu.shxzskj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://uc.shxzukj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://xl.9csxet.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ue.chemitech.net.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bu.bookmarksfly.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ae.shxzskj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hk.hahajie.cn

[E16] 数字千分位
来源：http://hs.wgjwhj.cn

Py:   f"{1234567:,}"
来源：http://si.yuexingan06.cn

PHP:  number_format(1234567);
来源：http://an.panjiajie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://wo.panjiajie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ik.9csxet.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://uv.hnjuh.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hp.chemitech.net.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bn.shxzukj.cn

C#:   1234567.ToString("N0")
来源：http://hf.huixiangedu.cn

[E17] 首字母大写
来源：http://sd.bookmarksfly.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bt.bookmarksfly.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://er.szxytkj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dz.huixiangedu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hy.yuexingan06.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jx.hnjuh.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gb.yuexingan06.cn

Ruby: s.capitalize
来源：http://kr.huixiangedu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hu.colortex.cn

[E18] 模板占位符替换
来源：http://lk.haigaiapp.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tx.nicolike.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wq.colortex.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ic.nicolike.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://wr.szxytkj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ls.hnjuh.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ut.jianghongdianzi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://sq.shtwfgs.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ak.newstarts.cn

[E19] 多行文本按行拆分
来源：http://yk.9csxet.cn

Py:   s.splitlines()
来源：http://ul.jianghongdianzi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ur.bookmarksfly.cn

JS:   s.split(/\r?\n/)
来源：http://du.haigaiapp.cn

TS:   s.split(/\r?\n/)
来源：http://qi.nszjky.cn

Java: s.lines().toList()
来源：http://xa.bookmarksfly.cn

Go:   strings.Split(s, "\n")
来源：http://np.bjjhwx.cn

Ruby: s.lines
来源：http://xn.nszjky.cn

C#:   s.Split('\n')
来源：http://vj.newstarts.cn

[E20] 判断字符串是否为空
来源：http://xc.huanxung.cn

Py:   if not s:
来源：http://gb.jctech888.com.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ya.huixiangedu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dw.lnxyls.cn

TS:   if (s === "") {}
来源：http://xa.colortex.cn

Java: if (s.isEmpty()) {}
来源：http://ds.panjiajie.cn

Go:   if s == "" {}
来源：http://os.hnjuh.cn

Ruby: if s.empty?
来源：http://bv.huixiangedu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fv.chemitech.net.cn

[E21] 超长截断加省略号
来源：http://rk.huixinmuqiang.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zl.yuexingan06.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kd.yuexingan06.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oy.huixinmuqiang.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gs.yuexingan06.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wg.newstarts.cn

Go:   // 按 rune 判断长度后截断
来源：http://aq.huixiangedu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mj.huixinmuqiang.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ve.huanxung.cn

[E22] 字节长度与字符长度
来源：http://qn.chemitech.net.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ar.nszjky.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hh.huixiangedu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jq.shxzskj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mo.nszjky.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://po.lnxyls.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jw.yuntaijiaju.cn

Ruby: s.bytesize;  s.length
来源：http://yt.huixinmuqiang.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ct.nszjky.cn

================================================================================
来源：http://lp.muxihuayi.cn

F. 文件与目录
来源：http://ek.bookmarksfly.cn

================================================================================
来源：http://ex.chemitech.net.cn

[F01] 读取整个文件
来源：http://zt.newstarts.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://et.gzmigu.cn

PHP:  file_get_contents("a.txt");
来源：http://tj.nicolike.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zc.szsharing.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fi.muxihuayi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hu.yuntaijiaju.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wh.hahajie.cn

Ruby: File.read("a.txt")
来源：http://of.nicolike.cn

C#:   File.ReadAllText("a.txt");
来源：http://zw.gzmigu.cn

[F02] 逐行读取文件
来源：http://cj.shxzskj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://sv.szsharing.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ad.panjiajie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vx.yuexingan06.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pe.jctech888.com.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qn.hahajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://eu.bookmarksfly.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gs.shxzskj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://og.wgjwhj.cn

[F03] 写入文件（覆盖）
来源：http://an.gzmigu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ix.jianghongdianzi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://bb.hahajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://za.colortex.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ll.9csxet.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zc.shtwfgs.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tf.jctech888.com.cn

Ruby: File.write("a.txt", "hi")
来源：http://ol.shtwfgs.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ul.huixinmuqiang.cn

[F04] 追加写入文件
来源：http://ep.haigaiapp.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wh.haigaiapp.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qc.haigaiapp.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ls.521024.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ix.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cm.huixinmuqiang.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://sf.szsharing.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://td.9csxet.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tj.jianghongdianzi.cn

[F05] 判断文件或目录是否存在
来源：http://hj.nszjky.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://oo.shtwfgs.cn

PHP:  file_exists("a.txt");
来源：http://nb.521024.cn

JS:   fs.existsSync("a.txt")
来源：http://zg.panjiajie.cn

TS:   fs.existsSync("a.txt")
来源：http://wo.jctech888.com.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.newstarts.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cm.szxytkj.cn

Ruby: File.exist?("a.txt")
来源：http://fh.szxytkj.cn

C#:   File.Exists("a.txt")
来源：http://yi.huanxung.cn

[F06] 删除文件
来源：http://oc.lnxyls.cn

Py:   os.remove("a.txt")
来源：http://gp.9csxet.cn

PHP:  unlink("a.txt");
来源：http://gr.szsharing.cn

JS:   fs.unlinkSync("a.txt")
来源：http://gj.521024.cn

TS:   fs.unlinkSync("a.txt")
来源：http://og.521024.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lj.gzmigu.cn

Go:   os.Remove("a.txt")
来源：http://dc.521024.cn

Ruby: File.delete("a.txt")
来源：http://fn.chemitech.net.cn

C#:   File.Delete("a.txt");
来源：http://ir.huixinmuqiang.cn

[F07] 创建目录（含多级）
来源：http://ce.521024.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wn.jianghongdianzi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://eh.9csxet.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jm.shtwfgs.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xd.shtwfgs.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ju.panjiajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ih.huixiangedu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lo.jctech888.com.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ew.nszjky.cn

[F08] 遍历目录
来源：http://hn.nicolike.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zr.muxihuayi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bt.huanxung.cn

JS:   fs.readdirSync("dir")
来源：http://em.panjiajie.cn

TS:   fs.readdirSync("dir")
来源：http://bv.colortex.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://te.wgjwhj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://rp.jianghongdianzi.cn

Ruby: Dir.children("dir")
来源：http://ae.shtwfgs.cn

C#:   Directory.GetFiles("dir")
来源：http://ls.haigaiapp.cn

[F09] 获取文件大小
来源：http://xc.nicolike.cn

Py:   os.path.getsize("a.txt")
来源：http://jr.nicolike.cn

PHP:  filesize("a.txt");
来源：http://se.huixinmuqiang.cn

JS:   fs.statSync("a.txt").size
来源：http://vj.muxihuayi.cn

TS:   fs.statSync("a.txt").size
来源：http://un.gzmigu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://gf.colortex.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xf.jianghongdianzi.cn

Ruby: File.size("a.txt")
来源：http://va.szsharing.cn

C#:   new FileInfo("a.txt").Length
来源：http://hw.colortex.cn

[F10] 取文件扩展名 / 文件名
来源：http://lo.szxytkj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tp.huixinmuqiang.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vm.yuexingan06.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vy.shxzskj.cn

TS:   path.extname("a.txt")
来源：http://rz.9csxet.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pe.shxzukj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://iu.shtwfgs.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ki.huixinmuqiang.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vu.9csxet.cn

[F11] 复制与移动文件
来源：http://tx.wgjwhj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jw.newstarts.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mf.shxzukj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kh.shxzukj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bz.haigaiapp.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fi.gzmigu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ec.nszjky.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zx.nicolike.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ev.hahajie.cn

[F12] CSV 读写
来源：http://vt.shxzskj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://so.shxzskj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tv.yuexingan06.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://js.huixinmuqiang.cn

TS:   // 同上
来源：http://ou.nicolike.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wz.haigaiapp.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jm.gzmigu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vp.nicolike.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qb.nicolike.cn

================================================================================
来源：http://mz.nszjky.cn

G. 面向对象
来源：http://gj.muxihuayi.cn

================================================================================
来源：http://nt.huixiangedu.cn

[G01] 定义类
来源：http://kw.9csxet.cn

Py:   class User: pass
来源：http://sg.newstarts.cn

PHP:  class User {}
来源：http://vo.bookmarksfly.cn

JS:   class User {}
来源：http://vu.shxzukj.cn

TS:   class User { name: string = ""; }
来源：http://yy.lnxyls.cn

Java: class User {}
来源：http://lt.panjiajie.cn

Go:   type User struct { Name string }
来源：http://yy.bjjhwx.cn

Ruby: class User; end
来源：http://gf.9csxet.cn

C#:   class User {}
来源：http://fx.muxihuayi.cn

[G02] 构造函数
来源：http://qw.huixinmuqiang.cn

Py:   def __init__(self, name): self.name = name
来源：http://iz.gzmigu.cn

PHP:  public function __construct(public string $name) {}
来源：http://ph.bjjhwx.cn

JS:   constructor(name) { this.name = name; }
来源：http://oe.szxytkj.cn

TS:   constructor(public name: string) {}
来源：http://bf.szsharing.cn

Java: User(String name) { this.name = name; }
来源：http://ue.huanxung.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rj.nicolike.cn

Ruby: def initialize(name); @name = name; end
来源：http://hd.chemitech.net.cn

C#:   public User(string name) { Name = name; }
来源：http://nn.jctech888.com.cn

[G03] 实例属性
来源：http://mt.newstarts.cn

Py:   self.name = "x"
来源：http://ck.colortex.cn

PHP:  public string $name = "x";
来源：http://kp.lnxyls.cn

JS:   this.name = "x";
来源：http://ar.hnjuh.cn

TS:   name: string = "x";
来源：http://hf.huixinmuqiang.cn

Java: private String name;
来源：http://hn.chemitech.net.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kw.hnjuh.cn

Ruby: @name = "x"
来源：http://us.jctech888.com.cn

C#:   public string Name { get; set; } = "x";
来源：http://wc.huanxung.cn

[G04] 定义方法
来源：http://hw.hahajie.cn

Py:   def greet(self): return self.name
来源：http://tw.lnxyls.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://tb.shtwfgs.cn

JS:   greet() { return this.name; }
来源：http://xu.9csxet.cn

TS:   greet(): string { return this.name; }
来源：http://oq.gzmigu.cn

Java: String greet() { return name; }
来源：http://bh.bookmarksfly.cn


<!-- 参考信息 -->