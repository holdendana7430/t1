代发 wailian999

Go:   strings.Index(s, "x")
来源：http://ul.huixinmuqiang.cn

Ruby: s.index("x")
来源：http://pq.lnxyls.cn

C#:   s.IndexOf("x")
来源：http://so.huixinmuqiang.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ds.jctech888.com.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://il.bookmarksfly.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wf.haigaiapp.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sd.jianghongdianzi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ap.muxihuayi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ou.muxihuayi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ci.9csxet.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://sd.shxzukj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sb.muxihuayi.cn

[E06] 替换子串
来源：http://ef.huixinmuqiang.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sq.asd995.cn

PHP:  str_replace("a", "b", $s);
来源：http://tf.nszjky.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cs.haigaiapp.cn

TS:   s.replaceAll("a", "b")
来源：http://bm.shtwfgs.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pm.shxzskj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kr.shxzskj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vm.nszjky.cn

C#:   s.Replace("a", "b")
来源：http://ic.colortex.cn

[E07] 按分隔符拆分
来源：http://np.yuexingan06.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fx.hahajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://uw.colortex.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://jg.huixiangedu.cn

TS:   s.split(",")
来源：http://vv.gzmigu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://oh.haigaiapp.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hn.haigaiapp.cn

Ruby: s.split(",");  s.split
来源：http://kx.nicolike.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ys.9csxet.cn

[E08] 数组按分隔符合并
来源：http://bv.chemitech.net.cn

Py:   ",".join(items)
来源：http://el.lnxyls.cn

PHP:  implode(",", $items);
来源：http://fn.wgjwhj.cn

JS:   items.join(",")
来源：http://gz.yuntaijiaju.cn

TS:   items.join(",")
来源：http://bs.hahajie.cn

Java: String.join(",", items)
来源：http://bs.gzmigu.cn

Go:   strings.Join(items, ",")
来源：http://ka.hnjuh.cn

Ruby: items.join(",")
来源：http://iv.9csxet.cn

C#:   string.Join(",", items)
来源：http://od.colortex.cn

[E09] 去除所有空白字符
来源：http://hi.bookmarksfly.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ye.9csxet.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://sh.nszjky.cn

JS:   s.replace(/\s+/g, "")
来源：http://mv.bjjhwx.cn

TS:   s.replace(/\s+/g, "")
来源：http://sb.chemitech.net.cn

Java: s.replaceAll("\\s+", "")
来源：http://hq.panjiajie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://gg.bjjhwx.cn

Ruby: s.gsub(/\s+/, "")
来源：http://gl.shtwfgs.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nl.newstarts.cn

[E10] 左侧补零 / 定长填充
来源：http://af.hnjuh.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xf.shtwfgs.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nc.shxzukj.cn

JS:   "7".padStart(3, "0")
来源：http://gn.shxzskj.cn

TS:   "7".padStart(3, "0")
来源：http://ay.szsharing.cn

Java: String.format("%03d", 7)
来源：http://sy.jctech888.com.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://zf.hnjuh.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bw.muxihuayi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xv.yuexingan06.cn

[E11] 反转字符串
来源：http://ou.nicolike.cn

Py:   s[::-1]
来源：http://tw.nicolike.cn

PHP:  strrev($s);
来源：http://cv.hahajie.cn

JS:   [...s].reverse().join("")
来源：http://jo.muxihuayi.cn

TS:   [...s].reverse().join("")
来源：http://yk.jianghongdianzi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ja.hahajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://rn.shxzskj.cn

Ruby: s.reverse
来源：http://lc.gzmigu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://is.colortex.cn

[E12] 统计某字符出现次数
来源：http://we.huixiangedu.cn

Py:   s.count("a")
来源：http://gm.szsharing.cn

PHP:  substr_count($s, "a");
来源：http://ci.wgjwhj.cn

JS:   s.split("a").length - 1
来源：http://tg.szsharing.cn

TS:   s.split("a").length - 1
来源：http://ju.wgjwhj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://uf.gzmigu.cn

Go:   strings.Count(s, "a")
来源：http://pq.bjjhwx.cn

Ruby: s.count("a")
来源：http://ds.huanxung.cn

C#:   s.Count(c => c == 'a')
来源：http://mc.wgjwhj.cn

[E13] 逐字符遍历
来源：http://vr.jctech888.com.cn

Py:   for ch in s: print(ch)
来源：http://ai.9csxet.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hn.hnjuh.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://av.newstarts.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://iy.jctech888.com.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xx.hahajie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jk.muxihuayi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://um.szxytkj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dv.szsharing.cn

[E14] URL 编码与 Base64
来源：http://ve.bookmarksfly.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ss.wgjwhj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://vv.bookmarksfly.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pn.hahajie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yy.wgjwhj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lr.lnxyls.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lm.521024.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ml.huixinmuqiang.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://im.chemitech.net.cn

[E15] HTML 转义 / 反转义
来源：http://ee.haigaiapp.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://nq.gzmigu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nl.huixinmuqiang.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ha.shtwfgs.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://aq.nszjky.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xd.szxytkj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ae.chemitech.net.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yn.huixinmuqiang.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nj.haigaiapp.cn

[E16] 数字千分位
来源：http://ra.jianghongdianzi.cn

Py:   f"{1234567:,}"
来源：http://lh.gzmigu.cn

PHP:  number_format(1234567);
来源：http://nf.shxzukj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://wz.9csxet.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://vo.shtwfgs.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ln.shxzskj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yb.bookmarksfly.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gh.gzmigu.cn

C#:   1234567.ToString("N0")
来源：http://js.gzmigu.cn

[E17] 首字母大写
来源：http://er.newstarts.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cs.shxzukj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://tp.asd995.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zj.chemitech.net.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dw.hahajie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://iy.panjiajie.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://oh.szxytkj.cn

Ruby: s.capitalize
来源：http://cb.huanxung.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ry.lnxyls.cn

[E18] 模板占位符替换
来源：http://yc.jianghongdianzi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ij.huixiangedu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lo.newstarts.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://sz.jctech888.com.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://dv.hahajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vm.jianghongdianzi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ef.nszjky.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://yh.nicolike.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vs.chemitech.net.cn

[E19] 多行文本按行拆分
来源：http://hk.wgjwhj.cn

Py:   s.splitlines()
来源：http://qu.jctech888.com.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ww.panjiajie.cn

JS:   s.split(/\r?\n/)
来源：http://ew.hahajie.cn

TS:   s.split(/\r?\n/)
来源：http://ty.haigaiapp.cn

Java: s.lines().toList()
来源：http://un.huixinmuqiang.cn

Go:   strings.Split(s, "\n")
来源：http://wk.jctech888.com.cn

Ruby: s.lines
来源：http://xy.colortex.cn

C#:   s.Split('\n')
来源：http://st.nszjky.cn

[E20] 判断字符串是否为空
来源：http://aa.shtwfgs.cn

Py:   if not s:
来源：http://sd.lnxyls.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zu.yuntaijiaju.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rb.hahajie.cn

TS:   if (s === "") {}
来源：http://ak.huixiangedu.cn

Java: if (s.isEmpty()) {}
来源：http://mg.lnxyls.cn

Go:   if s == "" {}
来源：http://ok.lnxyls.cn

Ruby: if s.empty?
来源：http://kx.shxzskj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vc.muxihuayi.cn

[E21] 超长截断加省略号
来源：http://hs.nszjky.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zf.huixiangedu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ut.huixiangedu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://de.newstarts.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fj.wgjwhj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fn.jianghongdianzi.cn

Go:   // 按 rune 判断长度后截断
来源：http://rq.521024.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ds.haigaiapp.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sj.shxzukj.cn

[E22] 字节长度与字符长度
来源：http://as.jianghongdianzi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qa.521024.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nn.szxytkj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kp.asd995.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fk.hahajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tt.szsharing.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tk.gzmigu.cn

Ruby: s.bytesize;  s.length
来源：http://jn.yuexingan06.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://im.hnjuh.cn

================================================================================
来源：http://wj.shxzukj.cn

F. 文件与目录
来源：http://vo.asd995.cn

================================================================================
来源：http://mk.gzmigu.cn

[F01] 读取整个文件
来源：http://bl.wgjwhj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bf.panjiajie.cn

PHP:  file_get_contents("a.txt");
来源：http://op.szsharing.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dz.gzmigu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zz.chemitech.net.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://xd.wgjwhj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ut.hahajie.cn

Ruby: File.read("a.txt")
来源：http://rp.9csxet.cn

C#:   File.ReadAllText("a.txt");
来源：http://cd.yuntaijiaju.cn

[F02] 逐行读取文件
来源：http://po.huanxung.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bm.szxytkj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bi.szsharing.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zq.wgjwhj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fr.wgjwhj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ji.gzmigu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wr.newstarts.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wo.szxytkj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mv.colortex.cn

[F03] 写入文件（覆盖）
来源：http://tc.colortex.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wi.lnxyls.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://bj.yuexingan06.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iu.szsharing.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lg.yuntaijiaju.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zh.muxihuayi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://th.shtwfgs.cn

Ruby: File.write("a.txt", "hi")
来源：http://sg.chemitech.net.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mt.shtwfgs.cn

[F04] 追加写入文件
来源：http://bs.muxihuayi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qj.panjiajie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lj.nszjky.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kc.muxihuayi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qb.bookmarksfly.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hj.jctech888.com.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dy.colortex.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jg.huixiangedu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gp.jctech888.com.cn

[F05] 判断文件或目录是否存在
来源：http://lw.huanxung.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tq.szxytkj.cn

PHP:  file_exists("a.txt");
来源：http://bw.newstarts.cn

JS:   fs.existsSync("a.txt")
来源：http://co.szsharing.cn

TS:   fs.existsSync("a.txt")
来源：http://oy.bookmarksfly.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ja.521024.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://md.nszjky.cn

Ruby: File.exist?("a.txt")
来源：http://sx.shxzukj.cn

C#:   File.Exists("a.txt")
来源：http://mi.hnjuh.cn

[F06] 删除文件
来源：http://xr.szxytkj.cn

Py:   os.remove("a.txt")
来源：http://cz.shxzukj.cn

PHP:  unlink("a.txt");
来源：http://fg.521024.cn

JS:   fs.unlinkSync("a.txt")
来源：http://fw.yuexingan06.cn

TS:   fs.unlinkSync("a.txt")
来源：http://mo.haigaiapp.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bb.haigaiapp.cn

Go:   os.Remove("a.txt")
来源：http://fd.wgjwhj.cn

Ruby: File.delete("a.txt")
来源：http://kr.haigaiapp.cn

C#:   File.Delete("a.txt");
来源：http://ek.jctech888.com.cn

[F07] 创建目录（含多级）
来源：http://mn.lnxyls.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zy.shtwfgs.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bg.jianghongdianzi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ty.bookmarksfly.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rt.hnjuh.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://oc.shtwfgs.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wq.nicolike.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://oi.colortex.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://au.bookmarksfly.cn

[F08] 遍历目录
来源：http://ek.wgjwhj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://vm.muxihuayi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://oh.jctech888.com.cn

JS:   fs.readdirSync("dir")
来源：http://fr.haigaiapp.cn

TS:   fs.readdirSync("dir")
来源：http://vi.newstarts.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xm.9csxet.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://yo.bookmarksfly.cn

Ruby: Dir.children("dir")
来源：http://xh.huixiangedu.cn

C#:   Directory.GetFiles("dir")
来源：http://yc.lnxyls.cn

[F09] 获取文件大小
来源：http://nx.wgjwhj.cn

Py:   os.path.getsize("a.txt")
来源：http://aq.colortex.cn

PHP:  filesize("a.txt");
来源：http://al.lnxyls.cn

JS:   fs.statSync("a.txt").size
来源：http://dp.yuntaijiaju.cn

TS:   fs.statSync("a.txt").size
来源：http://yy.asd995.cn

Java: Files.size(Path.of("a.txt"))
来源：http://yl.jctech888.com.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xl.szsharing.cn

Ruby: File.size("a.txt")
来源：http://vb.bookmarksfly.cn

C#:   new FileInfo("a.txt").Length
来源：http://ou.panjiajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://yg.hnjuh.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://df.huanxung.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qa.panjiajie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zd.szxytkj.cn

TS:   path.extname("a.txt")
来源：http://xg.asd995.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pb.huanxung.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xg.chemitech.net.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zi.wgjwhj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://oy.asd995.cn

[F11] 复制与移动文件
来源：http://sy.hnjuh.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ha.asd995.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cv.yuexingan06.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kr.huanxung.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nm.chemitech.net.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zh.yuexingan06.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dq.yuexingan06.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gq.hnjuh.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fz.bjjhwx.cn

[F12] CSV 读写
来源：http://pw.muxihuayi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://oc.jianghongdianzi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rz.szsharing.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://oc.nszjky.cn

TS:   // 同上
来源：http://ug.521024.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gs.jctech888.com.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://co.nicolike.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zf.huanxung.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://fq.nicolike.cn

================================================================================
来源：http://gg.yuntaijiaju.cn

G. 面向对象
来源：http://ia.huixiangedu.cn

================================================================================
来源：http://av.9csxet.cn

[G01] 定义类
来源：http://ic.shxzskj.cn

Py:   class User: pass
来源：http://in.hahajie.cn

PHP:  class User {}
来源：http://hc.jianghongdianzi.cn

JS:   class User {}
来源：http://yj.wgjwhj.cn

TS:   class User { name: string = ""; }
来源：http://do.hahajie.cn

Java: class User {}
来源：http://rx.gzmigu.cn

Go:   type User struct { Name string }
来源：http://uy.shxzukj.cn

Ruby: class User; end
来源：http://in.nicolike.cn

C#:   class User {}
来源：http://zy.lnxyls.cn

[G02] 构造函数
来源：http://pm.lnxyls.cn

Py:   def __init__(self, name): self.name = name
来源：http://ck.szxytkj.cn

PHP:  public function __construct(public string $name) {}
来源：http://nd.bookmarksfly.cn

JS:   constructor(name) { this.name = name; }
来源：http://cs.szsharing.cn

TS:   constructor(public name: string) {}
来源：http://or.nicolike.cn

Java: User(String name) { this.name = name; }
来源：http://fv.hnjuh.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xi.muxihuayi.cn

Ruby: def initialize(name); @name = name; end
来源：http://rg.nszjky.cn

C#:   public User(string name) { Name = name; }
来源：http://wh.haigaiapp.cn

[G03] 实例属性
来源：http://ls.521024.cn

Py:   self.name = "x"
来源：http://gd.szxytkj.cn

PHP:  public string $name = "x";
来源：http://vd.huixinmuqiang.cn


<!-- 参考信息 -->