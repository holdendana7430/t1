代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hf.szsharing.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wd.gzmigu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dy.shxzukj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ju.huanxung.cn

[E06] 替换子串
来源：http://ly.chemitech.net.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fb.bjjhwx.cn

PHP:  str_replace("a", "b", $s);
来源：http://rj.shxzskj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rl.jctech888.com.cn

TS:   s.replaceAll("a", "b")
来源：http://od.panjiajie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wy.wgjwhj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xe.hahajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pg.huixiangedu.cn

C#:   s.Replace("a", "b")
来源：http://ht.yuntaijiaju.cn

[E07] 按分隔符拆分
来源：http://gv.chemitech.net.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://om.huixiangedu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gq.hnjuh.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://qj.muxihuayi.cn

TS:   s.split(",")
来源：http://ky.bjjhwx.cn

Java: s.split(",");  s.split("\\s+")
来源：http://cm.lnxyls.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vf.lnxyls.cn

Ruby: s.split(",");  s.split
来源：http://ox.yuntaijiaju.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tg.szsharing.cn

[E08] 数组按分隔符合并
来源：http://po.jctech888.com.cn

Py:   ",".join(items)
来源：http://al.521024.cn

PHP:  implode(",", $items);
来源：http://ma.hnjuh.cn

JS:   items.join(",")
来源：http://vs.huanxung.cn

TS:   items.join(",")
来源：http://lv.bookmarksfly.cn

Java: String.join(",", items)
来源：http://cw.nicolike.cn

Go:   strings.Join(items, ",")
来源：http://am.muxihuayi.cn

Ruby: items.join(",")
来源：http://po.jctech888.com.cn

C#:   string.Join(",", items)
来源：http://gf.nszjky.cn

[E09] 去除所有空白字符
来源：http://tu.szxytkj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cp.nszjky.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ut.yuntaijiaju.cn

JS:   s.replace(/\s+/g, "")
来源：http://zg.yuntaijiaju.cn

TS:   s.replace(/\s+/g, "")
来源：http://rc.shxzukj.cn

Java: s.replaceAll("\\s+", "")
来源：http://bd.bjjhwx.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://yn.jctech888.com.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ye.colortex.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lr.521024.cn

[E10] 左侧补零 / 定长填充
来源：http://xc.jianghongdianzi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://si.shxzukj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xa.gzmigu.cn

JS:   "7".padStart(3, "0")
来源：http://ru.nicolike.cn

TS:   "7".padStart(3, "0")
来源：http://cv.jianghongdianzi.cn

Java: String.format("%03d", 7)
来源：http://dp.521024.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://dx.huixinmuqiang.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vj.nszjky.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rp.shxzskj.cn

[E11] 反转字符串
来源：http://pu.newstarts.cn

Py:   s[::-1]
来源：http://sy.9csxet.cn

PHP:  strrev($s);
来源：http://rw.muxihuayi.cn

JS:   [...s].reverse().join("")
来源：http://dm.nicolike.cn

TS:   [...s].reverse().join("")
来源：http://qj.9csxet.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://gr.panjiajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://cr.yuntaijiaju.cn

Ruby: s.reverse
来源：http://ue.shxzukj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://fp.lnxyls.cn

[E12] 统计某字符出现次数
来源：http://em.szxytkj.cn

Py:   s.count("a")
来源：http://qe.hahajie.cn

PHP:  substr_count($s, "a");
来源：http://vw.jctech888.com.cn

JS:   s.split("a").length - 1
来源：http://rf.yuntaijiaju.cn

TS:   s.split("a").length - 1
来源：http://ax.huixinmuqiang.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bz.wgjwhj.cn

Go:   strings.Count(s, "a")
来源：http://ly.yuexingan06.cn

Ruby: s.count("a")
来源：http://ya.szxytkj.cn

C#:   s.Count(c => c == 'a')
来源：http://st.haigaiapp.cn

[E13] 逐字符遍历
来源：http://pt.shxzskj.cn

Py:   for ch in s: print(ch)
来源：http://zh.shxzukj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://aj.yuexingan06.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://gz.521024.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://pj.shxzukj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://nb.huixinmuqiang.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jo.wgjwhj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rc.wgjwhj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dg.huixiangedu.cn

[E14] URL 编码与 Base64
来源：http://qm.bookmarksfly.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://os.asd995.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://kl.nicolike.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hy.nszjky.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zx.colortex.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mv.jianghongdianzi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nz.chemitech.net.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bj.haigaiapp.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ne.wgjwhj.cn

[E15] HTML 转义 / 反转义
来源：http://xh.gzmigu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xc.9csxet.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ll.panjiajie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zh.huixinmuqiang.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://gg.hahajie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jj.521024.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pt.jctech888.com.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mx.szxytkj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wo.muxihuayi.cn

[E16] 数字千分位
来源：http://on.yuntaijiaju.cn

Py:   f"{1234567:,}"
来源：http://dr.newstarts.cn

PHP:  number_format(1234567);
来源：http://iz.yuntaijiaju.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://yo.521024.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wg.gzmigu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kk.szxytkj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ag.colortex.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hx.jianghongdianzi.cn

C#:   1234567.ToString("N0")
来源：http://gt.9csxet.cn

[E17] 首字母大写
来源：http://ge.jianghongdianzi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gu.nszjky.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://yc.nicolike.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sf.asd995.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pa.yuexingan06.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ay.lnxyls.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://me.yuexingan06.cn

Ruby: s.capitalize
来源：http://gj.9csxet.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nx.gzmigu.cn

[E18] 模板占位符替换
来源：http://gz.yuexingan06.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ep.521024.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tv.szsharing.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xv.yuntaijiaju.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://bt.bookmarksfly.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ex.huixinmuqiang.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cx.gzmigu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fr.shxzukj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xg.chemitech.net.cn

[E19] 多行文本按行拆分
来源：http://je.colortex.cn

Py:   s.splitlines()
来源：http://nt.chemitech.net.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bk.gzmigu.cn

JS:   s.split(/\r?\n/)
来源：http://lq.asd995.cn

TS:   s.split(/\r?\n/)
来源：http://yu.shtwfgs.cn

Java: s.lines().toList()
来源：http://kp.panjiajie.cn

Go:   strings.Split(s, "\n")
来源：http://hu.newstarts.cn

Ruby: s.lines
来源：http://if.jctech888.com.cn

C#:   s.Split('\n')
来源：http://by.muxihuayi.cn

[E20] 判断字符串是否为空
来源：http://qq.shtwfgs.cn

Py:   if not s:
来源：http://zu.chemitech.net.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bs.lnxyls.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jd.nszjky.cn

TS:   if (s === "") {}
来源：http://kr.shxzskj.cn

Java: if (s.isEmpty()) {}
来源：http://dn.jianghongdianzi.cn

Go:   if s == "" {}
来源：http://bt.asd995.cn

Ruby: if s.empty?
来源：http://lg.huixinmuqiang.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://is.yuntaijiaju.cn

[E21] 超长截断加省略号
来源：http://at.panjiajie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hj.huixinmuqiang.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xu.hnjuh.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qg.wgjwhj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://me.shxzskj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mn.jianghongdianzi.cn

Go:   // 按 rune 判断长度后截断
来源：http://vx.shtwfgs.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sb.colortex.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jw.haigaiapp.cn

[E22] 字节长度与字符长度
来源：http://pc.nicolike.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xb.hnjuh.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rt.yuexingan06.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gg.asd995.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sa.hahajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rr.shxzskj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lv.shxzskj.cn

Ruby: s.bytesize;  s.length
来源：http://uq.yuexingan06.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bk.asd995.cn

================================================================================
来源：http://sf.huanxung.cn

F. 文件与目录
来源：http://cg.bookmarksfly.cn

================================================================================
来源：http://jh.jianghongdianzi.cn

[F01] 读取整个文件
来源：http://al.yuntaijiaju.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ks.wgjwhj.cn

PHP:  file_get_contents("a.txt");
来源：http://rt.lnxyls.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nw.szsharing.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://eo.szsharing.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://qw.chemitech.net.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nd.shtwfgs.cn

Ruby: File.read("a.txt")
来源：http://ep.521024.cn

C#:   File.ReadAllText("a.txt");
来源：http://tk.jctech888.com.cn

[F02] 逐行读取文件
来源：http://ml.shxzukj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hp.hnjuh.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ln.jctech888.com.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jt.lnxyls.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hi.bookmarksfly.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nz.lnxyls.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fh.haigaiapp.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ul.colortex.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jy.yuntaijiaju.cn

[F03] 写入文件（覆盖）
来源：http://cx.yuntaijiaju.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ud.huixiangedu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://fa.hahajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xs.huanxung.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vf.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ry.shxzskj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vm.szxytkj.cn

Ruby: File.write("a.txt", "hi")
来源：http://sq.chemitech.net.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zm.521024.cn

[F04] 追加写入文件
来源：http://zr.nicolike.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://px.panjiajie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qd.panjiajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ak.huixinmuqiang.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://po.521024.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nc.shtwfgs.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vc.shxzskj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nm.szxytkj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xt.muxihuayi.cn

[F05] 判断文件或目录是否存在
来源：http://qi.nszjky.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ex.521024.cn

PHP:  file_exists("a.txt");
来源：http://aq.gzmigu.cn

JS:   fs.existsSync("a.txt")
来源：http://qe.hnjuh.cn

TS:   fs.existsSync("a.txt")
来源：http://kv.9csxet.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ai.wgjwhj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dp.yuexingan06.cn

Ruby: File.exist?("a.txt")
来源：http://bk.muxihuayi.cn

C#:   File.Exists("a.txt")
来源：http://mk.yuexingan06.cn

[F06] 删除文件
来源：http://lz.9csxet.cn

Py:   os.remove("a.txt")
来源：http://sd.panjiajie.cn

PHP:  unlink("a.txt");
来源：http://tx.bookmarksfly.cn

JS:   fs.unlinkSync("a.txt")
来源：http://jg.jianghongdianzi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vy.shxzukj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vh.jctech888.com.cn

Go:   os.Remove("a.txt")
来源：http://va.hahajie.cn

Ruby: File.delete("a.txt")
来源：http://yg.hnjuh.cn

C#:   File.Delete("a.txt");
来源：http://tn.hahajie.cn

[F07] 创建目录（含多级）
来源：http://li.huanxung.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xj.521024.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pr.hahajie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ry.wgjwhj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ek.shtwfgs.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dl.yuntaijiaju.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ei.shxzskj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ea.hnjuh.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wa.asd995.cn

[F08] 遍历目录
来源：http://zo.huanxung.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://dp.muxihuayi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rg.hnjuh.cn

JS:   fs.readdirSync("dir")
来源：http://ue.colortex.cn

TS:   fs.readdirSync("dir")
来源：http://hr.yuntaijiaju.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rp.yuexingan06.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://en.yuntaijiaju.cn

Ruby: Dir.children("dir")
来源：http://qy.muxihuayi.cn

C#:   Directory.GetFiles("dir")
来源：http://om.jctech888.com.cn

[F09] 获取文件大小
来源：http://co.asd995.cn

Py:   os.path.getsize("a.txt")
来源：http://mh.shtwfgs.cn

PHP:  filesize("a.txt");
来源：http://cd.521024.cn

JS:   fs.statSync("a.txt").size
来源：http://nl.yuexingan06.cn

TS:   fs.statSync("a.txt").size
来源：http://zh.nszjky.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hh.panjiajie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bc.jianghongdianzi.cn

Ruby: File.size("a.txt")
来源：http://kr.jctech888.com.cn

C#:   new FileInfo("a.txt").Length
来源：http://cl.gzmigu.cn

[F10] 取文件扩展名 / 文件名
来源：http://ck.nszjky.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rf.jianghongdianzi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gd.521024.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tz.shtwfgs.cn

TS:   path.extname("a.txt")
来源：http://md.shxzskj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mc.yuexingan06.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ts.shtwfgs.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lj.huixinmuqiang.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xo.muxihuayi.cn

[F11] 复制与移动文件
来源：http://kz.bjjhwx.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.huanxung.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mq.lnxyls.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ci.hahajie.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nt.yuexingan06.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ks.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bi.shxzskj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wd.panjiajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zi.gzmigu.cn

[F12] CSV 读写
来源：http://oo.huixinmuqiang.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ab.nszjky.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://de.bjjhwx.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kx.shxzukj.cn

TS:   // 同上
来源：http://tr.gzmigu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://op.shtwfgs.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xm.szxytkj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rl.szxytkj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://bm.shxzskj.cn

================================================================================
来源：http://ua.huixiangedu.cn

G. 面向对象
来源：http://ts.jctech888.com.cn

================================================================================
来源：http://ke.shxzskj.cn

[G01] 定义类
来源：http://pg.szxytkj.cn

Py:   class User: pass
来源：http://do.huixinmuqiang.cn

PHP:  class User {}
来源：http://bx.szxytkj.cn

JS:   class User {}
来源：http://dz.jianghongdianzi.cn

TS:   class User { name: string = ""; }
来源：http://lb.szxytkj.cn

Java: class User {}
来源：http://kq.gzmigu.cn

Go:   type User struct { Name string }
来源：http://rv.yuntaijiaju.cn

Ruby: class User; end
来源：http://hh.panjiajie.cn

C#:   class User {}
来源：http://hq.haigaiapp.cn

[G02] 构造函数
来源：http://ea.szsharing.cn

Py:   def __init__(self, name): self.name = name
来源：http://ae.asd995.cn

PHP:  public function __construct(public string $name) {}
来源：http://pw.newstarts.cn

JS:   constructor(name) { this.name = name; }
来源：http://lx.hahajie.cn

TS:   constructor(public name: string) {}
来源：http://cz.jianghongdianzi.cn

Java: User(String name) { this.name = name; }
来源：http://vi.bjjhwx.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jd.newstarts.cn

Ruby: def initialize(name); @name = name; end
来源：http://bf.bjjhwx.cn

C#:   public User(string name) { Name = name; }
来源：http://no.asd995.cn

[G03] 实例属性
来源：http://ng.szsharing.cn

Py:   self.name = "x"
来源：http://ms.huixinmuqiang.cn

PHP:  public string $name = "x";
来源：http://kk.shtwfgs.cn

JS:   this.name = "x";
来源：http://rv.huixiangedu.cn

TS:   name: string = "x";
来源：http://pp.shtwfgs.cn

Java: private String name;
来源：http://qp.jctech888.com.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mz.wgjwhj.cn

Ruby: @name = "x"
来源：http://px.gzmigu.cn

C#:   public string Name { get; set; } = "x";
来源：http://vx.szxytkj.cn

[G04] 定义方法
来源：http://xg.yuntaijiaju.cn

Py:   def greet(self): return self.name
来源：http://id.szsharing.cn


<!-- 参考信息 -->