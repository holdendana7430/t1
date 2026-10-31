代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://mu.wgjwhj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pj.nicolike.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dd.muxihuayi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://js.shxzukj.cn

C#:   s.Replace("a", "b")
来源：http://ky.nszjky.cn

[E07] 按分隔符拆分
来源：http://wr.lnxyls.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vi.szxytkj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lb.newstarts.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://bz.asd995.cn

TS:   s.split(",")
来源：http://tz.chemitech.net.cn

Java: s.split(",");  s.split("\\s+")
来源：http://fl.yuexingan06.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cq.wgjwhj.cn

Ruby: s.split(",");  s.split
来源：http://fc.shxzukj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sr.gzmigu.cn

[E08] 数组按分隔符合并
来源：http://ka.9csxet.cn

Py:   ",".join(items)
来源：http://rw.szxytkj.cn

PHP:  implode(",", $items);
来源：http://tp.nicolike.cn

JS:   items.join(",")
来源：http://eg.colortex.cn

TS:   items.join(",")
来源：http://th.gzmigu.cn

Java: String.join(",", items)
来源：http://rd.nszjky.cn

Go:   strings.Join(items, ",")
来源：http://ue.haigaiapp.cn

Ruby: items.join(",")
来源：http://zg.colortex.cn

C#:   string.Join(",", items)
来源：http://fa.panjiajie.cn

[E09] 去除所有空白字符
来源：http://nj.wgjwhj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://in.wgjwhj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vk.shxzukj.cn

JS:   s.replace(/\s+/g, "")
来源：http://cv.jctech888.com.cn

TS:   s.replace(/\s+/g, "")
来源：http://fn.szxytkj.cn

Java: s.replaceAll("\\s+", "")
来源：http://ou.shxzskj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ws.nszjky.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ek.shxzskj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dv.szsharing.cn

[E10] 左侧补零 / 定长填充
来源：http://gc.shxzskj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://in.bookmarksfly.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://oq.wgjwhj.cn

JS:   "7".padStart(3, "0")
来源：http://co.wgjwhj.cn

TS:   "7".padStart(3, "0")
来源：http://tn.yuexingan06.cn

Java: String.format("%03d", 7)
来源：http://xn.9csxet.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://tu.colortex.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ab.szsharing.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rt.jianghongdianzi.cn

[E11] 反转字符串
来源：http://qu.shxzskj.cn

Py:   s[::-1]
来源：http://go.hahajie.cn

PHP:  strrev($s);
来源：http://yn.szsharing.cn

JS:   [...s].reverse().join("")
来源：http://pd.hnjuh.cn

TS:   [...s].reverse().join("")
来源：http://qx.huanxung.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://vs.shxzskj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://yp.newstarts.cn

Ruby: s.reverse
来源：http://ul.wgjwhj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vk.nszjky.cn

[E12] 统计某字符出现次数
来源：http://lu.wgjwhj.cn

Py:   s.count("a")
来源：http://bi.jianghongdianzi.cn

PHP:  substr_count($s, "a");
来源：http://sk.huixinmuqiang.cn

JS:   s.split("a").length - 1
来源：http://ot.haigaiapp.cn

TS:   s.split("a").length - 1
来源：http://au.szxytkj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://oy.szxytkj.cn

Go:   strings.Count(s, "a")
来源：http://jc.gzmigu.cn

Ruby: s.count("a")
来源：http://zf.chemitech.net.cn

C#:   s.Count(c => c == 'a')
来源：http://oq.haigaiapp.cn

[E13] 逐字符遍历
来源：http://bg.nicolike.cn

Py:   for ch in s: print(ch)
来源：http://af.huanxung.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://av.hnjuh.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://aq.jianghongdianzi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://iu.huanxung.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bk.jianghongdianzi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rx.521024.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://jn.huixinmuqiang.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zb.gzmigu.cn

[E14] URL 编码与 Base64
来源：http://dy.hnjuh.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yz.wgjwhj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://yk.szsharing.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qo.asd995.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sw.huanxung.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://sq.huixinmuqiang.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://md.shxzskj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://un.szsharing.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ba.wgjwhj.cn

[E15] HTML 转义 / 反转义
来源：http://fq.shxzskj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://pe.huixiangedu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pl.asd995.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ht.huixiangedu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://xs.jianghongdianzi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qu.hnjuh.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://lg.9csxet.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xi.asd995.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ut.newstarts.cn

[E16] 数字千分位
来源：http://we.bookmarksfly.cn

Py:   f"{1234567:,}"
来源：http://uc.shxzskj.cn

PHP:  number_format(1234567);
来源：http://jo.panjiajie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://bt.bookmarksfly.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://bo.panjiajie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hh.panjiajie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ra.521024.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://oz.haigaiapp.cn

C#:   1234567.ToString("N0")
来源：http://qn.wgjwhj.cn

[E17] 首字母大写
来源：http://lp.yuntaijiaju.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://np.jctech888.com.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://sw.huixinmuqiang.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://it.huixiangedu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dk.huixiangedu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jd.nszjky.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sj.shtwfgs.cn

Ruby: s.capitalize
来源：http://rf.jianghongdianzi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://om.shxzskj.cn

[E18] 模板占位符替换
来源：http://mn.shxzskj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zc.lnxyls.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ix.muxihuayi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://yo.panjiajie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://mp.shxzskj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tp.shxzukj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yw.haigaiapp.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ga.szxytkj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://np.nicolike.cn

[E19] 多行文本按行拆分
来源：http://kk.newstarts.cn

Py:   s.splitlines()
来源：http://jw.newstarts.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zm.huixiangedu.cn

JS:   s.split(/\r?\n/)
来源：http://xx.muxihuayi.cn

TS:   s.split(/\r?\n/)
来源：http://ta.hahajie.cn

Java: s.lines().toList()
来源：http://za.gzmigu.cn

Go:   strings.Split(s, "\n")
来源：http://nf.haigaiapp.cn

Ruby: s.lines
来源：http://fn.chemitech.net.cn

C#:   s.Split('\n')
来源：http://jx.jianghongdianzi.cn

[E20] 判断字符串是否为空
来源：http://mq.haigaiapp.cn

Py:   if not s:
来源：http://de.colortex.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jb.nszjky.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vn.yuntaijiaju.cn

TS:   if (s === "") {}
来源：http://dw.jctech888.com.cn

Java: if (s.isEmpty()) {}
来源：http://fp.lnxyls.cn

Go:   if s == "" {}
来源：http://dm.jianghongdianzi.cn

Ruby: if s.empty?
来源：http://rr.nicolike.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ze.yuexingan06.cn

[E21] 超长截断加省略号
来源：http://hh.hahajie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gm.haigaiapp.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://js.huanxung.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ni.nszjky.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kv.nicolike.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://sc.lnxyls.cn

Go:   // 按 rune 判断长度后截断
来源：http://ue.bjjhwx.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yb.lnxyls.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sr.nicolike.cn

[E22] 字节长度与字符长度
来源：http://zy.wgjwhj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hh.yuexingan06.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uu.panjiajie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://sk.hahajie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ib.newstarts.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://os.nicolike.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hk.nicolike.cn

Ruby: s.bytesize;  s.length
来源：http://eu.szxytkj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yt.shxzskj.cn

================================================================================
来源：http://bw.521024.cn

F. 文件与目录
来源：http://mw.panjiajie.cn

================================================================================
来源：http://zh.shxzskj.cn

[F01] 读取整个文件
来源：http://ha.huanxung.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mv.jianghongdianzi.cn

PHP:  file_get_contents("a.txt");
来源：http://lu.newstarts.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ct.shxzukj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zj.wgjwhj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://oh.wgjwhj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ph.521024.cn

Ruby: File.read("a.txt")
来源：http://cf.bjjhwx.cn

C#:   File.ReadAllText("a.txt");
来源：http://xl.bjjhwx.cn

[F02] 逐行读取文件
来源：http://uo.wgjwhj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ei.huixiangedu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rw.hnjuh.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qf.shxzskj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qs.9csxet.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ty.szsharing.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ry.nszjky.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qd.szxytkj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://af.wgjwhj.cn

[F03] 写入文件（覆盖）
来源：http://ga.yuexingan06.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://um.yuntaijiaju.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://fc.colortex.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sm.huixinmuqiang.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vg.nszjky.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://td.panjiajie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://sk.gzmigu.cn

Ruby: File.write("a.txt", "hi")
来源：http://nv.hahajie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kl.colortex.cn

[F04] 追加写入文件
来源：http://nj.colortex.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://le.colortex.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zw.gzmigu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ti.nszjky.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kb.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kj.haigaiapp.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bs.huixiangedu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://br.asd995.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gk.haigaiapp.cn

[F05] 判断文件或目录是否存在
来源：http://pp.asd995.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://by.bookmarksfly.cn

PHP:  file_exists("a.txt");
来源：http://cy.yuexingan06.cn

JS:   fs.existsSync("a.txt")
来源：http://ln.hahajie.cn

TS:   fs.existsSync("a.txt")
来源：http://bm.gzmigu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://il.muxihuayi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zm.jianghongdianzi.cn

Ruby: File.exist?("a.txt")
来源：http://kc.huixiangedu.cn

C#:   File.Exists("a.txt")
来源：http://qn.nicolike.cn

[F06] 删除文件
来源：http://wv.panjiajie.cn

Py:   os.remove("a.txt")
来源：http://hk.huanxung.cn

PHP:  unlink("a.txt");
来源：http://xi.jianghongdianzi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://jc.shtwfgs.cn

TS:   fs.unlinkSync("a.txt")
来源：http://or.shxzukj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://th.gzmigu.cn

Go:   os.Remove("a.txt")
来源：http://yy.jianghongdianzi.cn

Ruby: File.delete("a.txt")
来源：http://bo.huanxung.cn

C#:   File.Delete("a.txt");
来源：http://op.huanxung.cn

[F07] 创建目录（含多级）
来源：http://lz.hnjuh.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://of.9csxet.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bj.yuntaijiaju.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rc.nicolike.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uq.szxytkj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xj.9csxet.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fv.hahajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cj.chemitech.net.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://px.newstarts.cn

[F08] 遍历目录
来源：http://ul.chemitech.net.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://em.hahajie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kv.panjiajie.cn

JS:   fs.readdirSync("dir")
来源：http://fd.bjjhwx.cn

TS:   fs.readdirSync("dir")
来源：http://yw.huixiangedu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ca.shtwfgs.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://wf.newstarts.cn

Ruby: Dir.children("dir")
来源：http://zr.shxzskj.cn

C#:   Directory.GetFiles("dir")
来源：http://rz.nszjky.cn

[F09] 获取文件大小
来源：http://px.gzmigu.cn

Py:   os.path.getsize("a.txt")
来源：http://cq.jianghongdianzi.cn

PHP:  filesize("a.txt");
来源：http://iz.szsharing.cn

JS:   fs.statSync("a.txt").size
来源：http://jb.huanxung.cn

TS:   fs.statSync("a.txt").size
来源：http://wl.yuexingan06.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hk.huixiangedu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://su.shtwfgs.cn

Ruby: File.size("a.txt")
来源：http://mh.panjiajie.cn

C#:   new FileInfo("a.txt").Length
来源：http://eq.muxihuayi.cn

[F10] 取文件扩展名 / 文件名
来源：http://yx.jctech888.com.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qs.yuntaijiaju.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ik.szsharing.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jz.muxihuayi.cn

TS:   path.extname("a.txt")
来源：http://jx.bjjhwx.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mk.yuexingan06.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wd.jianghongdianzi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vz.colortex.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vz.asd995.cn

[F11] 复制与移动文件
来源：http://gr.bjjhwx.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gz.huixinmuqiang.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bq.shtwfgs.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zt.chemitech.net.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eh.huixiangedu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://va.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mu.colortex.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bd.jctech888.com.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xv.colortex.cn

[F12] CSV 读写
来源：http://fm.521024.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://do.shxzskj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dj.521024.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qq.chemitech.net.cn

TS:   // 同上
来源：http://bh.hnjuh.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://em.bookmarksfly.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hb.panjiajie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yj.hahajie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://nh.yuexingan06.cn

================================================================================
来源：http://lm.bookmarksfly.cn

G. 面向对象
来源：http://bw.jianghongdianzi.cn

================================================================================
来源：http://mc.lnxyls.cn

[G01] 定义类
来源：http://gj.shxzskj.cn

Py:   class User: pass
来源：http://sj.shxzukj.cn

PHP:  class User {}
来源：http://os.shtwfgs.cn

JS:   class User {}
来源：http://dg.huanxung.cn

TS:   class User { name: string = ""; }
来源：http://xi.szxytkj.cn

Java: class User {}
来源：http://nn.muxihuayi.cn

Go:   type User struct { Name string }
来源：http://cn.lnxyls.cn

Ruby: class User; end
来源：http://ra.shxzskj.cn

C#:   class User {}
来源：http://lw.shxzukj.cn

[G02] 构造函数
来源：http://kf.shxzskj.cn

Py:   def __init__(self, name): self.name = name
来源：http://ak.yuexingan06.cn

PHP:  public function __construct(public string $name) {}
来源：http://yt.hahajie.cn

JS:   constructor(name) { this.name = name; }
来源：http://gb.jianghongdianzi.cn

TS:   constructor(public name: string) {}
来源：http://lj.haigaiapp.cn

Java: User(String name) { this.name = name; }
来源：http://qe.wgjwhj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wp.jianghongdianzi.cn

Ruby: def initialize(name); @name = name; end
来源：http://sy.huanxung.cn

C#:   public User(string name) { Name = name; }
来源：http://rn.panjiajie.cn

[G03] 实例属性
来源：http://oy.bjjhwx.cn

Py:   self.name = "x"
来源：http://ji.bjjhwx.cn

PHP:  public string $name = "x";
来源：http://ht.huanxung.cn

JS:   this.name = "x";
来源：http://jh.jianghongdianzi.cn

TS:   name: string = "x";
来源：http://ns.521024.cn

Java: private String name;
来源：http://li.muxihuayi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bl.huixinmuqiang.cn

Ruby: @name = "x"
来源：http://ph.szsharing.cn

C#:   public string Name { get; set; } = "x";
来源：http://yw.shxzukj.cn

[G04] 定义方法
来源：http://ot.yuntaijiaju.cn

Py:   def greet(self): return self.name
来源：http://oh.huanxung.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://kd.bjjhwx.cn

JS:   greet() { return this.name; }
来源：http://tg.panjiajie.cn

TS:   greet(): string { return this.name; }
来源：http://rt.wgjwhj.cn

Java: String greet() { return name; }
来源：http://af.shtwfgs.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://mj.hnjuh.cn

Ruby: def greet; @name; end
来源：http://bw.yuexingan06.cn

C#:   public string Greet() => Name;
来源：http://ky.huixiangedu.cn

[G05] 继承
来源：http://cr.panjiajie.cn


<!-- 参考信息 -->