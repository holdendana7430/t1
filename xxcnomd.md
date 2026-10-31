代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://ys.9csxet.cn

C#:   s.Substring(1, 3)
来源：http://li.asd995.cn

[E04] 查找子串位置
来源：http://pp.chemitech.net.cn

Py:   s.find("x");  s.index("x")
来源：http://qt.szxytkj.cn

PHP:  strpos($s, "x");
来源：http://yy.bjjhwx.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fa.haigaiapp.cn

TS:   s.indexOf("x")
来源：http://hf.nszjky.cn

Java: s.indexOf("x")
来源：http://lx.hahajie.cn

Go:   strings.Index(s, "x")
来源：http://bw.nicolike.cn

Ruby: s.index("x")
来源：http://vl.521024.cn

C#:   s.IndexOf("x")
来源：http://pz.panjiajie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://td.bookmarksfly.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://is.panjiajie.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sp.panjiajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hl.szxytkj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://fh.shxzukj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://km.shtwfgs.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wh.yuntaijiaju.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ab.bookmarksfly.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yw.shxzukj.cn

[E06] 替换子串
来源：http://op.yuntaijiaju.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vl.bjjhwx.cn

PHP:  str_replace("a", "b", $s);
来源：http://nt.hnjuh.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://re.huixiangedu.cn

TS:   s.replaceAll("a", "b")
来源：http://lk.yuntaijiaju.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ws.bjjhwx.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://px.huixinmuqiang.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yt.yuntaijiaju.cn

C#:   s.Replace("a", "b")
来源：http://xj.shtwfgs.cn

[E07] 按分隔符拆分
来源：http://nb.shxzskj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cp.lnxyls.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wa.bookmarksfly.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://wt.lnxyls.cn

TS:   s.split(",")
来源：http://ov.haigaiapp.cn

Java: s.split(",");  s.split("\\s+")
来源：http://pm.huixinmuqiang.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://be.nicolike.cn

Ruby: s.split(",");  s.split
来源：http://or.jctech888.com.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hv.hnjuh.cn

[E08] 数组按分隔符合并
来源：http://zx.bookmarksfly.cn

Py:   ",".join(items)
来源：http://dq.jctech888.com.cn

PHP:  implode(",", $items);
来源：http://xa.lnxyls.cn

JS:   items.join(",")
来源：http://iz.shxzukj.cn

TS:   items.join(",")
来源：http://he.gzmigu.cn

Java: String.join(",", items)
来源：http://yg.bookmarksfly.cn

Go:   strings.Join(items, ",")
来源：http://ux.521024.cn

Ruby: items.join(",")
来源：http://pc.shxzskj.cn

C#:   string.Join(",", items)
来源：http://pd.huixiangedu.cn

[E09] 去除所有空白字符
来源：http://pq.haigaiapp.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gl.lnxyls.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mi.shtwfgs.cn

JS:   s.replace(/\s+/g, "")
来源：http://jv.bjjhwx.cn

TS:   s.replace(/\s+/g, "")
来源：http://ws.lnxyls.cn

Java: s.replaceAll("\\s+", "")
来源：http://xa.shtwfgs.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://uy.hahajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ru.hnjuh.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ff.newstarts.cn

[E10] 左侧补零 / 定长填充
来源：http://uw.nicolike.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://il.newstarts.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tz.wgjwhj.cn

JS:   "7".padStart(3, "0")
来源：http://fo.muxihuayi.cn

TS:   "7".padStart(3, "0")
来源：http://zo.newstarts.cn

Java: String.format("%03d", 7)
来源：http://sx.shxzskj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://oc.shxzukj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sv.huixiangedu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tn.nicolike.cn

[E11] 反转字符串
来源：http://yn.huixinmuqiang.cn

Py:   s[::-1]
来源：http://tu.521024.cn

PHP:  strrev($s);
来源：http://ov.huixinmuqiang.cn

JS:   [...s].reverse().join("")
来源：http://vw.gzmigu.cn

TS:   [...s].reverse().join("")
来源：http://kn.lnxyls.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://cc.chemitech.net.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://wx.huixinmuqiang.cn

Ruby: s.reverse
来源：http://bz.jianghongdianzi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://tg.szxytkj.cn

[E12] 统计某字符出现次数
来源：http://wt.bjjhwx.cn

Py:   s.count("a")
来源：http://iw.newstarts.cn

PHP:  substr_count($s, "a");
来源：http://da.521024.cn

JS:   s.split("a").length - 1
来源：http://so.szxytkj.cn

TS:   s.split("a").length - 1
来源：http://ug.521024.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xy.lnxyls.cn

Go:   strings.Count(s, "a")
来源：http://dj.colortex.cn

Ruby: s.count("a")
来源：http://qq.nszjky.cn

C#:   s.Count(c => c == 'a')
来源：http://qh.yuntaijiaju.cn

[E13] 逐字符遍历
来源：http://hf.9csxet.cn

Py:   for ch in s: print(ch)
来源：http://lh.panjiajie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wj.jianghongdianzi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://tm.nicolike.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://sd.bookmarksfly.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vi.huixiangedu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ms.colortex.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://mi.wgjwhj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mr.huixinmuqiang.cn

[E14] URL 编码与 Base64
来源：http://pv.jianghongdianzi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dt.huixiangedu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://os.yuntaijiaju.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://sd.9csxet.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pk.newstarts.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tk.huixiangedu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pm.shxzskj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rd.nicolike.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nl.hnjuh.cn

[E15] HTML 转义 / 反转义
来源：http://iw.newstarts.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://lw.chemitech.net.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nm.szsharing.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kj.hnjuh.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://zw.gzmigu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dt.nszjky.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://iz.shxzukj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ca.chemitech.net.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zp.jianghongdianzi.cn

[E16] 数字千分位
来源：http://vj.huanxung.cn

Py:   f"{1234567:,}"
来源：http://lz.lnxyls.cn

PHP:  number_format(1234567);
来源：http://xw.asd995.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://fg.wgjwhj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ci.haigaiapp.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wz.panjiajie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://id.shtwfgs.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wm.nicolike.cn

C#:   1234567.ToString("N0")
来源：http://rd.hahajie.cn

[E17] 首字母大写
来源：http://oe.szxytkj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vi.muxihuayi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ca.asd995.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://up.jianghongdianzi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ox.szsharing.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://iy.asd995.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gm.hnjuh.cn

Ruby: s.capitalize
来源：http://dz.hahajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ez.bookmarksfly.cn

[E18] 模板占位符替换
来源：http://sq.szxytkj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cj.huixiangedu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xg.yuntaijiaju.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://jv.yuexingan06.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ox.muxihuayi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wf.szxytkj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gy.asd995.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jx.hahajie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://av.huixiangedu.cn

[E19] 多行文本按行拆分
来源：http://dn.bjjhwx.cn

Py:   s.splitlines()
来源：http://bi.hahajie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cj.jianghongdianzi.cn

JS:   s.split(/\r?\n/)
来源：http://gx.nszjky.cn

TS:   s.split(/\r?\n/)
来源：http://hs.wgjwhj.cn

Java: s.lines().toList()
来源：http://da.bookmarksfly.cn

Go:   strings.Split(s, "\n")
来源：http://xz.9csxet.cn

Ruby: s.lines
来源：http://kh.nicolike.cn

C#:   s.Split('\n')
来源：http://gm.muxihuayi.cn

[E20] 判断字符串是否为空
来源：http://kl.jianghongdianzi.cn

Py:   if not s:
来源：http://ls.panjiajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jk.bjjhwx.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sx.colortex.cn

TS:   if (s === "") {}
来源：http://pk.gzmigu.cn

Java: if (s.isEmpty()) {}
来源：http://ya.bjjhwx.cn

Go:   if s == "" {}
来源：http://dq.chemitech.net.cn

Ruby: if s.empty?
来源：http://lm.huixinmuqiang.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zb.chemitech.net.cn

[E21] 超长截断加省略号
来源：http://fj.szsharing.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lw.lnxyls.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bc.haigaiapp.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wt.muxihuayi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jr.newstarts.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ee.gzmigu.cn

Go:   // 按 rune 判断长度后截断
来源：http://gn.huixinmuqiang.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gc.nszjky.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qz.lnxyls.cn

[E22] 字节长度与字符长度
来源：http://rt.panjiajie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tv.huixinmuqiang.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kt.jctech888.com.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pu.asd995.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ec.hnjuh.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jw.huixiangedu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xd.shxzskj.cn

Ruby: s.bytesize;  s.length
来源：http://di.huixinmuqiang.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mn.bookmarksfly.cn

================================================================================
来源：http://op.nszjky.cn

F. 文件与目录
来源：http://oj.muxihuayi.cn

================================================================================
来源：http://ca.lnxyls.cn

[F01] 读取整个文件
来源：http://qe.huanxung.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vw.chemitech.net.cn

PHP:  file_get_contents("a.txt");
来源：http://rx.colortex.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vm.szxytkj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ew.hnjuh.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://dm.jctech888.com.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://aq.panjiajie.cn

Ruby: File.read("a.txt")
来源：http://lv.huixiangedu.cn

C#:   File.ReadAllText("a.txt");
来源：http://qq.521024.cn

[F02] 逐行读取文件
来源：http://fc.yuexingan06.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lk.521024.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qy.szsharing.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vh.gzmigu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yc.haigaiapp.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kt.asd995.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zl.gzmigu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://sb.huixinmuqiang.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fj.muxihuayi.cn

[F03] 写入文件（覆盖）
来源：http://xi.yuexingan06.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lb.yuntaijiaju.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://rs.muxihuayi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ia.nicolike.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cz.szxytkj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yk.nszjky.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vu.nszjky.cn

Ruby: File.write("a.txt", "hi")
来源：http://ge.gzmigu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rz.colortex.cn

[F04] 追加写入文件
来源：http://cx.chemitech.net.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cq.muxihuayi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ff.shxzukj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qm.jctech888.com.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fr.hahajie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vz.asd995.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qn.huixiangedu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qn.521024.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qd.jctech888.com.cn

[F05] 判断文件或目录是否存在
来源：http://mp.lnxyls.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ch.nszjky.cn

PHP:  file_exists("a.txt");
来源：http://rt.muxihuayi.cn

JS:   fs.existsSync("a.txt")
来源：http://xe.asd995.cn

TS:   fs.existsSync("a.txt")
来源：http://un.newstarts.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://uc.huixinmuqiang.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cf.huixiangedu.cn

Ruby: File.exist?("a.txt")
来源：http://ku.haigaiapp.cn

C#:   File.Exists("a.txt")
来源：http://ov.9csxet.cn

[F06] 删除文件
来源：http://rs.muxihuayi.cn

Py:   os.remove("a.txt")
来源：http://lm.huanxung.cn

PHP:  unlink("a.txt");
来源：http://qd.nszjky.cn

JS:   fs.unlinkSync("a.txt")
来源：http://sn.lnxyls.cn

TS:   fs.unlinkSync("a.txt")
来源：http://pf.bookmarksfly.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wz.shxzukj.cn

Go:   os.Remove("a.txt")
来源：http://td.shxzskj.cn

Ruby: File.delete("a.txt")
来源：http://zm.lnxyls.cn

C#:   File.Delete("a.txt");
来源：http://rm.nicolike.cn

[F07] 创建目录（含多级）
来源：http://oo.shtwfgs.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mk.huixiangedu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hj.shtwfgs.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wi.yuexingan06.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mc.huanxung.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://en.shxzskj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xi.szxytkj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hj.szxytkj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nv.newstarts.cn

[F08] 遍历目录
来源：http://kd.haigaiapp.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://mb.huanxung.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ds.shtwfgs.cn

JS:   fs.readdirSync("dir")
来源：http://fh.muxihuayi.cn

TS:   fs.readdirSync("dir")
来源：http://xa.lnxyls.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ax.szxytkj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ud.szxytkj.cn

Ruby: Dir.children("dir")
来源：http://aw.shtwfgs.cn

C#:   Directory.GetFiles("dir")
来源：http://ot.yuntaijiaju.cn

[F09] 获取文件大小
来源：http://dh.hnjuh.cn

Py:   os.path.getsize("a.txt")
来源：http://fo.nicolike.cn

PHP:  filesize("a.txt");
来源：http://jg.shxzskj.cn

JS:   fs.statSync("a.txt").size
来源：http://aj.yuexingan06.cn

TS:   fs.statSync("a.txt").size
来源：http://og.huixinmuqiang.cn

Java: Files.size(Path.of("a.txt"))
来源：http://oa.lnxyls.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yy.szxytkj.cn

Ruby: File.size("a.txt")
来源：http://lr.shxzskj.cn

C#:   new FileInfo("a.txt").Length
来源：http://du.shxzskj.cn

[F10] 取文件扩展名 / 文件名
来源：http://vu.yuntaijiaju.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xn.colortex.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tq.hnjuh.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://os.nicolike.cn

TS:   path.extname("a.txt")
来源：http://nd.jctech888.com.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://id.shxzskj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mt.gzmigu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://sg.nicolike.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hx.shtwfgs.cn

[F11] 复制与移动文件
来源：http://ly.haigaiapp.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vx.wgjwhj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://we.haigaiapp.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://if.gzmigu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nu.huixiangedu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lb.bookmarksfly.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://us.panjiajie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ou.bjjhwx.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zf.asd995.cn

[F12] CSV 读写
来源：http://kq.huanxung.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xj.huanxung.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bh.jctech888.com.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://it.colortex.cn

TS:   // 同上
来源：http://ex.huixinmuqiang.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dp.haigaiapp.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nv.nszjky.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bw.gzmigu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://rp.wgjwhj.cn

================================================================================
来源：http://vw.shxzskj.cn

G. 面向对象
来源：http://aq.chemitech.net.cn

================================================================================
来源：http://gh.bjjhwx.cn

[G01] 定义类
来源：http://hh.newstarts.cn

Py:   class User: pass
来源：http://lu.lnxyls.cn

PHP:  class User {}
来源：http://zt.haigaiapp.cn

JS:   class User {}
来源：http://va.colortex.cn

TS:   class User { name: string = ""; }
来源：http://zf.szsharing.cn

Java: class User {}
来源：http://oy.huixinmuqiang.cn

Go:   type User struct { Name string }
来源：http://fr.huanxung.cn

Ruby: class User; end
来源：http://sj.nicolike.cn

C#:   class User {}
来源：http://br.haigaiapp.cn

[G02] 构造函数
来源：http://lh.bookmarksfly.cn

Py:   def __init__(self, name): self.name = name
来源：http://ap.newstarts.cn

PHP:  public function __construct(public string $name) {}
来源：http://au.jianghongdianzi.cn

JS:   constructor(name) { this.name = name; }
来源：http://ck.asd995.cn


<!-- 参考信息 -->