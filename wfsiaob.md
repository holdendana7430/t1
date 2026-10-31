代发 wailian999

Go:   strings.Index(s, "x")
来源：http://ct.szsharing.cn

Ruby: s.index("x")
来源：http://rs.nicolike.cn

C#:   s.IndexOf("x")
来源：http://tr.haigaiapp.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://tp.shxzskj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ef.huixinmuqiang.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ig.huixinmuqiang.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ru.newstarts.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://nr.huixiangedu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ny.bookmarksfly.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gw.szsharing.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mh.hnjuh.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ef.chemitech.net.cn

[E06] 替换子串
来源：http://sz.muxihuayi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mh.521024.cn

PHP:  str_replace("a", "b", $s);
来源：http://vk.lnxyls.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rm.haigaiapp.cn

TS:   s.replaceAll("a", "b")
来源：http://mo.9csxet.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://js.lnxyls.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vi.szsharing.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ol.9csxet.cn

C#:   s.Replace("a", "b")
来源：http://xe.shxzukj.cn

[E07] 按分隔符拆分
来源：http://vc.newstarts.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qi.hnjuh.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xa.szsharing.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://us.jianghongdianzi.cn

TS:   s.split(",")
来源：http://xj.yuntaijiaju.cn

Java: s.split(",");  s.split("\\s+")
来源：http://oj.shxzukj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nu.gzmigu.cn

Ruby: s.split(",");  s.split
来源：http://jq.panjiajie.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ku.yuexingan06.cn

[E08] 数组按分隔符合并
来源：http://dw.bookmarksfly.cn

Py:   ",".join(items)
来源：http://ag.yuexingan06.cn

PHP:  implode(",", $items);
来源：http://gm.huanxung.cn

JS:   items.join(",")
来源：http://db.521024.cn

TS:   items.join(",")
来源：http://as.huixinmuqiang.cn

Java: String.join(",", items)
来源：http://ab.huixinmuqiang.cn

Go:   strings.Join(items, ",")
来源：http://fi.szxytkj.cn

Ruby: items.join(",")
来源：http://sx.asd995.cn

C#:   string.Join(",", items)
来源：http://qv.huixinmuqiang.cn

[E09] 去除所有空白字符
来源：http://lx.lnxyls.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xy.newstarts.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ap.szxytkj.cn

JS:   s.replace(/\s+/g, "")
来源：http://dt.jctech888.com.cn

TS:   s.replace(/\s+/g, "")
来源：http://sh.szsharing.cn

Java: s.replaceAll("\\s+", "")
来源：http://xr.yuntaijiaju.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://eb.huanxung.cn

Ruby: s.gsub(/\s+/, "")
来源：http://yo.asd995.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://to.muxihuayi.cn

[E10] 左侧补零 / 定长填充
来源：http://oq.shtwfgs.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://os.szsharing.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://os.bookmarksfly.cn

JS:   "7".padStart(3, "0")
来源：http://qx.wgjwhj.cn

TS:   "7".padStart(3, "0")
来源：http://pq.hahajie.cn

Java: String.format("%03d", 7)
来源：http://ij.shtwfgs.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ty.huixinmuqiang.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hf.lnxyls.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fp.colortex.cn

[E11] 反转字符串
来源：http://tq.lnxyls.cn

Py:   s[::-1]
来源：http://af.muxihuayi.cn

PHP:  strrev($s);
来源：http://vi.bjjhwx.cn

JS:   [...s].reverse().join("")
来源：http://al.muxihuayi.cn

TS:   [...s].reverse().join("")
来源：http://ob.nicolike.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zp.huanxung.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ih.asd995.cn

Ruby: s.reverse
来源：http://ms.huanxung.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ss.szxytkj.cn

[E12] 统计某字符出现次数
来源：http://ti.shxzskj.cn

Py:   s.count("a")
来源：http://nd.gzmigu.cn

PHP:  substr_count($s, "a");
来源：http://ro.521024.cn

JS:   s.split("a").length - 1
来源：http://pf.muxihuayi.cn

TS:   s.split("a").length - 1
来源：http://di.yuexingan06.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vp.bookmarksfly.cn

Go:   strings.Count(s, "a")
来源：http://cf.shxzskj.cn

Ruby: s.count("a")
来源：http://wn.lnxyls.cn

C#:   s.Count(c => c == 'a')
来源：http://ex.szxytkj.cn

[E13] 逐字符遍历
来源：http://hq.chemitech.net.cn

Py:   for ch in s: print(ch)
来源：http://kz.asd995.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gp.jctech888.com.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://fa.yuexingan06.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wt.jctech888.com.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ld.huixiangedu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ob.hahajie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://iw.shxzskj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dl.bookmarksfly.cn

[E14] URL 编码与 Base64
来源：http://mi.bjjhwx.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ea.colortex.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://cv.haigaiapp.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mx.panjiajie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qv.shxzukj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://os.jianghongdianzi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xw.nszjky.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://by.nicolike.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ir.nszjky.cn

[E15] HTML 转义 / 反转义
来源：http://sv.521024.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://pe.huixinmuqiang.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gn.hnjuh.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xn.bookmarksfly.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://rt.shtwfgs.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zs.gzmigu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pd.nszjky.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ie.shxzskj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mn.huixiangedu.cn

[E16] 数字千分位
来源：http://kv.jianghongdianzi.cn

Py:   f"{1234567:,}"
来源：http://re.haigaiapp.cn

PHP:  number_format(1234567);
来源：http://ks.colortex.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://cv.lnxyls.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://yx.asd995.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fc.szxytkj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ko.huixinmuqiang.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ln.521024.cn

C#:   1234567.ToString("N0")
来源：http://qw.bookmarksfly.cn

[E17] 首字母大写
来源：http://km.9csxet.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fh.gzmigu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://bf.asd995.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ny.shtwfgs.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yn.9csxet.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gz.hnjuh.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://va.colortex.cn

Ruby: s.capitalize
来源：http://tn.shxzskj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://sw.huixiangedu.cn

[E18] 模板占位符替换
来源：http://ig.nszjky.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bw.huixiangedu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://oa.muxihuayi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://qw.muxihuayi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ij.nszjky.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qu.yuntaijiaju.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nm.haigaiapp.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ot.huanxung.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qh.wgjwhj.cn

[E19] 多行文本按行拆分
来源：http://wx.newstarts.cn

Py:   s.splitlines()
来源：http://ck.szxytkj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ys.yuexingan06.cn

JS:   s.split(/\r?\n/)
来源：http://wx.gzmigu.cn

TS:   s.split(/\r?\n/)
来源：http://cb.panjiajie.cn

Java: s.lines().toList()
来源：http://ya.bjjhwx.cn

Go:   strings.Split(s, "\n")
来源：http://mc.colortex.cn

Ruby: s.lines
来源：http://lh.muxihuayi.cn

C#:   s.Split('\n')
来源：http://ys.shtwfgs.cn

[E20] 判断字符串是否为空
来源：http://zu.colortex.cn

Py:   if not s:
来源：http://mw.nicolike.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ji.jianghongdianzi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kd.huanxung.cn

TS:   if (s === "") {}
来源：http://co.chemitech.net.cn

Java: if (s.isEmpty()) {}
来源：http://ak.nszjky.cn

Go:   if s == "" {}
来源：http://gu.huanxung.cn

Ruby: if s.empty?
来源：http://od.huixinmuqiang.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mz.shxzskj.cn

[E21] 超长截断加省略号
来源：http://tm.szsharing.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qv.hnjuh.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gw.hnjuh.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://to.bjjhwx.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://en.bjjhwx.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ih.huixiangedu.cn

Go:   // 按 rune 判断长度后截断
来源：http://pe.wgjwhj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ft.huanxung.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lh.asd995.cn

[E22] 字节长度与字符长度
来源：http://kx.yuntaijiaju.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://eq.chemitech.net.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vc.yuexingan06.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://uv.haigaiapp.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ax.asd995.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wv.panjiajie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cc.shxzskj.cn

Ruby: s.bytesize;  s.length
来源：http://up.huixiangedu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rq.nszjky.cn

================================================================================
来源：http://ap.lnxyls.cn

F. 文件与目录
来源：http://ue.jctech888.com.cn

================================================================================
来源：http://bd.newstarts.cn

[F01] 读取整个文件
来源：http://ez.newstarts.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://az.gzmigu.cn

PHP:  file_get_contents("a.txt");
来源：http://nk.shxzukj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vb.hnjuh.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nl.gzmigu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://yy.wgjwhj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ci.nicolike.cn

Ruby: File.read("a.txt")
来源：http://kg.bjjhwx.cn

C#:   File.ReadAllText("a.txt");
来源：http://bj.newstarts.cn

[F02] 逐行读取文件
来源：http://kc.shxzskj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ih.szxytkj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://es.9csxet.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rg.haigaiapp.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xc.colortex.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hj.wgjwhj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ib.hahajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://su.panjiajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bj.muxihuayi.cn

[F03] 写入文件（覆盖）
来源：http://vz.shxzukj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ia.huixiangedu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://wn.szsharing.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vi.chemitech.net.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jj.panjiajie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://on.lnxyls.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rl.jctech888.com.cn

Ruby: File.write("a.txt", "hi")
来源：http://th.lnxyls.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nc.9csxet.cn

[F04] 追加写入文件
来源：http://fm.jctech888.com.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xy.hnjuh.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cp.9csxet.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dw.newstarts.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ov.szsharing.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pq.huixinmuqiang.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://va.yuexingan06.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wx.huixinmuqiang.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hr.shxzukj.cn

[F05] 判断文件或目录是否存在
来源：http://mt.szsharing.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tx.gzmigu.cn

PHP:  file_exists("a.txt");
来源：http://ms.panjiajie.cn

JS:   fs.existsSync("a.txt")
来源：http://zb.szxytkj.cn

TS:   fs.existsSync("a.txt")
来源：http://cb.panjiajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://rf.shxzukj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ao.9csxet.cn

Ruby: File.exist?("a.txt")
来源：http://fi.jianghongdianzi.cn

C#:   File.Exists("a.txt")
来源：http://wp.haigaiapp.cn

[F06] 删除文件
来源：http://jo.szxytkj.cn

Py:   os.remove("a.txt")
来源：http://mh.shtwfgs.cn

PHP:  unlink("a.txt");
来源：http://kb.yuexingan06.cn

JS:   fs.unlinkSync("a.txt")
来源：http://tg.huixinmuqiang.cn

TS:   fs.unlinkSync("a.txt")
来源：http://wj.szxytkj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uf.szxytkj.cn

Go:   os.Remove("a.txt")
来源：http://mg.szxytkj.cn

Ruby: File.delete("a.txt")
来源：http://gu.wgjwhj.cn

C#:   File.Delete("a.txt");
来源：http://ri.lnxyls.cn

[F07] 创建目录（含多级）
来源：http://vp.newstarts.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jz.szsharing.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ab.szsharing.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nm.huanxung.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zw.nicolike.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zl.bjjhwx.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ww.wgjwhj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fj.hahajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bj.asd995.cn

[F08] 遍历目录
来源：http://sy.bookmarksfly.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://pn.shxzukj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pi.jctech888.com.cn

JS:   fs.readdirSync("dir")
来源：http://pj.newstarts.cn

TS:   fs.readdirSync("dir")
来源：http://ww.hahajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yo.colortex.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ec.lnxyls.cn

Ruby: Dir.children("dir")
来源：http://lp.chemitech.net.cn

C#:   Directory.GetFiles("dir")
来源：http://ym.gzmigu.cn

[F09] 获取文件大小
来源：http://zf.gzmigu.cn

Py:   os.path.getsize("a.txt")
来源：http://ct.panjiajie.cn

PHP:  filesize("a.txt");
来源：http://id.yuexingan06.cn

JS:   fs.statSync("a.txt").size
来源：http://is.lnxyls.cn

TS:   fs.statSync("a.txt").size
来源：http://az.haigaiapp.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ji.bookmarksfly.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dt.nicolike.cn

Ruby: File.size("a.txt")
来源：http://lf.hnjuh.cn

C#:   new FileInfo("a.txt").Length
来源：http://qx.newstarts.cn

[F10] 取文件扩展名 / 文件名
来源：http://sw.szxytkj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://di.hahajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dn.chemitech.net.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ke.9csxet.cn

TS:   path.extname("a.txt")
来源：http://oe.jctech888.com.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fk.muxihuayi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://em.colortex.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ra.colortex.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ek.521024.cn

[F11] 复制与移动文件
来源：http://wp.haigaiapp.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ql.hnjuh.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://by.jianghongdianzi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://co.asd995.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kz.nicolike.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://da.shxzukj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nb.lnxyls.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sw.hnjuh.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zi.muxihuayi.cn

[F12] CSV 读写
来源：http://ug.bjjhwx.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lf.szsharing.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://er.yuntaijiaju.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tl.wgjwhj.cn

TS:   // 同上
来源：http://jg.huanxung.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yk.newstarts.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qq.yuexingan06.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jo.szxytkj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://fl.panjiajie.cn

================================================================================
来源：http://kt.gzmigu.cn

G. 面向对象
来源：http://xv.shxzukj.cn

================================================================================
来源：http://do.nicolike.cn

[G01] 定义类
来源：http://fp.huanxung.cn

Py:   class User: pass
来源：http://qf.yuntaijiaju.cn

PHP:  class User {}
来源：http://ho.huixinmuqiang.cn

JS:   class User {}
来源：http://zv.bookmarksfly.cn

TS:   class User { name: string = ""; }
来源：http://ly.newstarts.cn

Java: class User {}
来源：http://hc.haigaiapp.cn

Go:   type User struct { Name string }
来源：http://iu.huixiangedu.cn

Ruby: class User; end
来源：http://nr.yuexingan06.cn

C#:   class User {}
来源：http://or.yuntaijiaju.cn

[G02] 构造函数
来源：http://dk.nszjky.cn

Py:   def __init__(self, name): self.name = name
来源：http://kb.huanxung.cn

PHP:  public function __construct(public string $name) {}
来源：http://mb.521024.cn

JS:   constructor(name) { this.name = name; }
来源：http://gy.jianghongdianzi.cn

TS:   constructor(public name: string) {}
来源：http://je.yuexingan06.cn

Java: User(String name) { this.name = name; }
来源：http://sc.haigaiapp.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://uo.shxzskj.cn

Ruby: def initialize(name); @name = name; end
来源：http://pp.jianghongdianzi.cn

C#:   public User(string name) { Name = name; }
来源：http://fy.panjiajie.cn

[G03] 实例属性
来源：http://xa.nszjky.cn

Py:   self.name = "x"
来源：http://hn.huanxung.cn

PHP:  public string $name = "x";
来源：http://su.yuexingan06.cn


<!-- 参考信息 -->