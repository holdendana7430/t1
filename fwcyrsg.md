代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wi.asd995.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mf.hnjuh.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fp.yuntaijiaju.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://on.521024.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ce.jctech888.com.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nq.yuntaijiaju.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cr.newstarts.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bw.muxihuayi.cn

[E06] 替换子串
来源：http://fl.haigaiapp.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://am.shtwfgs.cn

PHP:  str_replace("a", "b", $s);
来源：http://hx.nicolike.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eu.yuexingan06.cn

TS:   s.replaceAll("a", "b")
来源：http://wy.jctech888.com.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xm.9csxet.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nc.lnxyls.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ny.9csxet.cn

C#:   s.Replace("a", "b")
来源：http://md.asd995.cn

[E07] 按分隔符拆分
来源：http://ti.huixiangedu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tm.asd995.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wi.nszjky.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ex.szsharing.cn

TS:   s.split(",")
来源：http://vf.asd995.cn

Java: s.split(",");  s.split("\\s+")
来源：http://gw.9csxet.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zx.panjiajie.cn

Ruby: s.split(",");  s.split
来源：http://hv.bookmarksfly.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zg.muxihuayi.cn

[E08] 数组按分隔符合并
来源：http://kg.nszjky.cn

Py:   ",".join(items)
来源：http://dk.yuexingan06.cn

PHP:  implode(",", $items);
来源：http://zt.newstarts.cn

JS:   items.join(",")
来源：http://np.shxzskj.cn

TS:   items.join(",")
来源：http://ti.shxzskj.cn

Java: String.join(",", items)
来源：http://bn.huanxung.cn

Go:   strings.Join(items, ",")
来源：http://pg.shtwfgs.cn

Ruby: items.join(",")
来源：http://pr.colortex.cn

C#:   string.Join(",", items)
来源：http://fi.hnjuh.cn

[E09] 去除所有空白字符
来源：http://kk.521024.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://sq.wgjwhj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://sh.szxytkj.cn

JS:   s.replace(/\s+/g, "")
来源：http://jd.shtwfgs.cn

TS:   s.replace(/\s+/g, "")
来源：http://zm.hahajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://kc.nicolike.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://xu.shxzukj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://pk.yuntaijiaju.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://oz.panjiajie.cn

[E10] 左侧补零 / 定长填充
来源：http://he.nicolike.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vf.gzmigu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xp.muxihuayi.cn

JS:   "7".padStart(3, "0")
来源：http://eb.panjiajie.cn

TS:   "7".padStart(3, "0")
来源：http://pq.nszjky.cn

Java: String.format("%03d", 7)
来源：http://ul.muxihuayi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xp.muxihuayi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yw.hnjuh.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mn.gzmigu.cn

[E11] 反转字符串
来源：http://tc.wgjwhj.cn

Py:   s[::-1]
来源：http://ar.colortex.cn

PHP:  strrev($s);
来源：http://ye.jianghongdianzi.cn

JS:   [...s].reverse().join("")
来源：http://kt.shxzskj.cn

TS:   [...s].reverse().join("")
来源：http://nk.haigaiapp.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ls.bookmarksfly.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://sh.shtwfgs.cn

Ruby: s.reverse
来源：http://ya.9csxet.cn

C#:   new string(s.Reverse().ToArray())
来源：http://pn.shxzskj.cn

[E12] 统计某字符出现次数
来源：http://ar.huanxung.cn

Py:   s.count("a")
来源：http://ji.hahajie.cn

PHP:  substr_count($s, "a");
来源：http://yj.colortex.cn

JS:   s.split("a").length - 1
来源：http://nu.huanxung.cn

TS:   s.split("a").length - 1
来源：http://ey.newstarts.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ox.shxzukj.cn

Go:   strings.Count(s, "a")
来源：http://tl.bjjhwx.cn

Ruby: s.count("a")
来源：http://cj.panjiajie.cn

C#:   s.Count(c => c == 'a')
来源：http://wg.huixinmuqiang.cn

[E13] 逐字符遍历
来源：http://iz.hahajie.cn

Py:   for ch in s: print(ch)
来源：http://nr.521024.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jx.colortex.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://hn.haigaiapp.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://gu.nicolike.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://uh.haigaiapp.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hy.yuexingan06.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://mz.szsharing.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mv.shxzukj.cn

[E14] URL 编码与 Base64
来源：http://ki.521024.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ln.huixinmuqiang.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ve.chemitech.net.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nl.yuexingan06.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kk.newstarts.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zh.lnxyls.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ic.nicolike.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://la.szsharing.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fc.muxihuayi.cn

[E15] HTML 转义 / 反转义
来源：http://gp.chemitech.net.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://eo.shxzskj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://te.yuntaijiaju.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qk.jianghongdianzi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ek.huixinmuqiang.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://on.lnxyls.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://du.shxzskj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mx.asd995.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://na.hahajie.cn

[E16] 数字千分位
来源：http://sv.huixiangedu.cn

Py:   f"{1234567:,}"
来源：http://hu.jianghongdianzi.cn

PHP:  number_format(1234567);
来源：http://db.nszjky.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://cl.muxihuayi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://nj.newstarts.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kw.haigaiapp.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ja.newstarts.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://eo.521024.cn

C#:   1234567.ToString("N0")
来源：http://xb.newstarts.cn

[E17] 首字母大写
来源：http://zm.szsharing.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cw.nszjky.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ec.lnxyls.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ci.huanxung.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bi.shxzukj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jf.wgjwhj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bw.jctech888.com.cn

Ruby: s.capitalize
来源：http://yg.huixinmuqiang.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rx.yuexingan06.cn

[E18] 模板占位符替换
来源：http://wk.nicolike.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ko.shxzskj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dp.yuexingan06.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ta.newstarts.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://nb.jctech888.com.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jv.hnjuh.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ms.jianghongdianzi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lw.shxzskj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uc.muxihuayi.cn

[E19] 多行文本按行拆分
来源：http://by.nicolike.cn

Py:   s.splitlines()
来源：http://lb.shxzukj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ff.9csxet.cn

JS:   s.split(/\r?\n/)
来源：http://nu.muxihuayi.cn

TS:   s.split(/\r?\n/)
来源：http://lk.lnxyls.cn

Java: s.lines().toList()
来源：http://nn.huixinmuqiang.cn

Go:   strings.Split(s, "\n")
来源：http://iv.9csxet.cn

Ruby: s.lines
来源：http://wi.nicolike.cn

C#:   s.Split('\n')
来源：http://pf.gzmigu.cn

[E20] 判断字符串是否为空
来源：http://rj.huixinmuqiang.cn

Py:   if not s:
来源：http://om.panjiajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sn.chemitech.net.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tj.nicolike.cn

TS:   if (s === "") {}
来源：http://sp.nszjky.cn

Java: if (s.isEmpty()) {}
来源：http://qg.nszjky.cn

Go:   if s == "" {}
来源：http://ee.shtwfgs.cn

Ruby: if s.empty?
来源：http://nr.newstarts.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://aq.nszjky.cn

[E21] 超长截断加省略号
来源：http://yt.huixinmuqiang.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xx.9csxet.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qb.9csxet.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mf.hnjuh.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://db.nicolike.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ue.bjjhwx.cn

Go:   // 按 rune 判断长度后截断
来源：http://lr.shxzskj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://iy.jianghongdianzi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mc.jctech888.com.cn

[E22] 字节长度与字符长度
来源：http://gg.asd995.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ss.hahajie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xk.szsharing.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://di.yuntaijiaju.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mp.nszjky.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bg.yuexingan06.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qo.muxihuayi.cn

Ruby: s.bytesize;  s.length
来源：http://uk.hahajie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wi.jianghongdianzi.cn

================================================================================
来源：http://xi.jianghongdianzi.cn

F. 文件与目录
来源：http://qq.nszjky.cn

================================================================================
来源：http://wk.huanxung.cn

[F01] 读取整个文件
来源：http://lm.huixiangedu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://js.9csxet.cn

PHP:  file_get_contents("a.txt");
来源：http://ur.hnjuh.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://il.bookmarksfly.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gh.yuexingan06.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://on.chemitech.net.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kz.jctech888.com.cn

Ruby: File.read("a.txt")
来源：http://jk.szsharing.cn

C#:   File.ReadAllText("a.txt");
来源：http://fo.panjiajie.cn

[F02] 逐行读取文件
来源：http://fx.bjjhwx.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fv.wgjwhj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kf.huanxung.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dd.wgjwhj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kz.asd995.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ht.yuntaijiaju.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yd.gzmigu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kv.jctech888.com.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nn.huanxung.cn

[F03] 写入文件（覆盖）
来源：http://xx.huixiangedu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zp.chemitech.net.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://gm.szxytkj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kq.huanxung.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zw.colortex.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tu.panjiajie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ir.jctech888.com.cn

Ruby: File.write("a.txt", "hi")
来源：http://od.szsharing.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vo.yuntaijiaju.cn

[F04] 追加写入文件
来源：http://bw.huanxung.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yt.bjjhwx.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://sv.shtwfgs.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hj.haigaiapp.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ut.nszjky.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ru.gzmigu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://md.bjjhwx.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dc.nicolike.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bo.shxzukj.cn

[F05] 判断文件或目录是否存在
来源：http://jm.bookmarksfly.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://iv.haigaiapp.cn

PHP:  file_exists("a.txt");
来源：http://ew.9csxet.cn

JS:   fs.existsSync("a.txt")
来源：http://si.nicolike.cn

TS:   fs.existsSync("a.txt")
来源：http://ox.hahajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://wp.asd995.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tx.bjjhwx.cn

Ruby: File.exist?("a.txt")
来源：http://qu.521024.cn

C#:   File.Exists("a.txt")
来源：http://dv.wgjwhj.cn

[F06] 删除文件
来源：http://zz.huanxung.cn

Py:   os.remove("a.txt")
来源：http://as.newstarts.cn

PHP:  unlink("a.txt");
来源：http://nc.newstarts.cn

JS:   fs.unlinkSync("a.txt")
来源：http://lg.yuntaijiaju.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ci.nszjky.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gu.lnxyls.cn

Go:   os.Remove("a.txt")
来源：http://ub.colortex.cn

Ruby: File.delete("a.txt")
来源：http://pv.shxzukj.cn

C#:   File.Delete("a.txt");
来源：http://ov.yuexingan06.cn

[F07] 创建目录（含多级）
来源：http://uo.hahajie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ha.gzmigu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://aq.shxzskj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yv.szsharing.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tx.huanxung.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jo.lnxyls.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://st.lnxyls.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://io.hahajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kr.huixiangedu.cn

[F08] 遍历目录
来源：http://vu.szsharing.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://mh.bjjhwx.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mx.bjjhwx.cn

JS:   fs.readdirSync("dir")
来源：http://uy.9csxet.cn

TS:   fs.readdirSync("dir")
来源：http://dr.wgjwhj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pp.9csxet.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://sm.hnjuh.cn

Ruby: Dir.children("dir")
来源：http://rg.huixinmuqiang.cn

C#:   Directory.GetFiles("dir")
来源：http://es.yuntaijiaju.cn

[F09] 获取文件大小
来源：http://xl.shxzskj.cn

Py:   os.path.getsize("a.txt")
来源：http://es.huixiangedu.cn

PHP:  filesize("a.txt");
来源：http://kj.chemitech.net.cn

JS:   fs.statSync("a.txt").size
来源：http://ft.9csxet.cn

TS:   fs.statSync("a.txt").size
来源：http://qt.hnjuh.cn

Java: Files.size(Path.of("a.txt"))
来源：http://eq.9csxet.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tj.bjjhwx.cn

Ruby: File.size("a.txt")
来源：http://wc.shxzukj.cn

C#:   new FileInfo("a.txt").Length
来源：http://lh.nicolike.cn

[F10] 取文件扩展名 / 文件名
来源：http://va.shtwfgs.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://yt.hnjuh.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zu.bjjhwx.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mn.shtwfgs.cn

TS:   path.extname("a.txt")
来源：http://du.panjiajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ow.asd995.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hx.bookmarksfly.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://me.yuntaijiaju.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jd.huixinmuqiang.cn

[F11] 复制与移动文件
来源：http://ti.jianghongdianzi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vi.newstarts.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://do.shxzukj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ec.wgjwhj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cj.nicolike.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ts.szsharing.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fp.panjiajie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sk.chemitech.net.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qf.szxytkj.cn

[F12] CSV 读写
来源：http://ms.nicolike.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sr.huixiangedu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mc.panjiajie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://sr.shxzukj.cn

TS:   // 同上
来源：http://ug.muxihuayi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gn.panjiajie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qk.9csxet.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hk.szsharing.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://np.huixiangedu.cn

================================================================================
来源：http://ok.huixinmuqiang.cn

G. 面向对象
来源：http://dg.nicolike.cn

================================================================================
来源：http://gu.9csxet.cn

[G01] 定义类
来源：http://tu.wgjwhj.cn

Py:   class User: pass
来源：http://yo.asd995.cn

PHP:  class User {}
来源：http://yr.yuntaijiaju.cn

JS:   class User {}
来源：http://jd.yuntaijiaju.cn

TS:   class User { name: string = ""; }
来源：http://ho.szsharing.cn

Java: class User {}
来源：http://wd.gzmigu.cn

Go:   type User struct { Name string }
来源：http://op.szsharing.cn

Ruby: class User; end
来源：http://av.wgjwhj.cn

C#:   class User {}
来源：http://rv.wgjwhj.cn

[G02] 构造函数
来源：http://oq.jctech888.com.cn

Py:   def __init__(self, name): self.name = name
来源：http://th.9csxet.cn

PHP:  public function __construct(public string $name) {}
来源：http://jj.szxytkj.cn

JS:   constructor(name) { this.name = name; }
来源：http://iq.huanxung.cn

TS:   constructor(public name: string) {}
来源：http://yl.hahajie.cn

Java: User(String name) { this.name = name; }
来源：http://ua.colortex.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ey.nszjky.cn

Ruby: def initialize(name); @name = name; end
来源：http://db.panjiajie.cn

C#:   public User(string name) { Name = name; }
来源：http://cf.shxzukj.cn

[G03] 实例属性
来源：http://ts.shtwfgs.cn

Py:   self.name = "x"
来源：http://ne.muxihuayi.cn

PHP:  public string $name = "x";
来源：http://es.jctech888.com.cn

JS:   this.name = "x";
来源：http://gt.nicolike.cn

TS:   name: string = "x";
来源：http://qk.szxytkj.cn

Java: private String name;
来源：http://ih.nicolike.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://eu.9csxet.cn


<!-- 参考信息 -->