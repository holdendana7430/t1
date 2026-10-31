代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://sw.chemitech.net.cn

C#:   s.Substring(1, 3)
来源：http://yw.huixinmuqiang.cn

[E04] 查找子串位置
来源：http://nl.panjiajie.cn

Py:   s.find("x");  s.index("x")
来源：http://mk.nszjky.cn

PHP:  strpos($s, "x");
来源：http://ol.lnxyls.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wc.9csxet.cn

TS:   s.indexOf("x")
来源：http://fo.yuexingan06.cn

Java: s.indexOf("x")
来源：http://zo.panjiajie.cn

Go:   strings.Index(s, "x")
来源：http://uv.jianghongdianzi.cn

Ruby: s.index("x")
来源：http://mo.szxytkj.cn

C#:   s.IndexOf("x")
来源：http://dg.hnjuh.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://jl.huanxung.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ct.hnjuh.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kd.shtwfgs.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bg.gzmigu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ty.9csxet.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zx.szsharing.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://az.shxzukj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ym.huanxung.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yx.colortex.cn

[E06] 替换子串
来源：http://lj.huixinmuqiang.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dt.nszjky.cn

PHP:  str_replace("a", "b", $s);
来源：http://pm.jctech888.com.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rl.szxytkj.cn

TS:   s.replaceAll("a", "b")
来源：http://qf.shxzukj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ag.panjiajie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xi.gzmigu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vx.hahajie.cn

C#:   s.Replace("a", "b")
来源：http://av.hahajie.cn

[E07] 按分隔符拆分
来源：http://gw.asd995.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://po.newstarts.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mc.szxytkj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://vf.nicolike.cn

TS:   s.split(",")
来源：http://jk.muxihuayi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ed.huixiangedu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://um.bjjhwx.cn

Ruby: s.split(",");  s.split
来源：http://lo.bjjhwx.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xd.szsharing.cn

[E08] 数组按分隔符合并
来源：http://it.colortex.cn

Py:   ",".join(items)
来源：http://mh.panjiajie.cn

PHP:  implode(",", $items);
来源：http://ps.haigaiapp.cn

JS:   items.join(",")
来源：http://ha.jianghongdianzi.cn

TS:   items.join(",")
来源：http://nv.panjiajie.cn

Java: String.join(",", items)
来源：http://me.jctech888.com.cn

Go:   strings.Join(items, ",")
来源：http://jz.chemitech.net.cn

Ruby: items.join(",")
来源：http://po.yuexingan06.cn

C#:   string.Join(",", items)
来源：http://df.wgjwhj.cn

[E09] 去除所有空白字符
来源：http://jz.shtwfgs.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wv.bookmarksfly.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zq.nicolike.cn

JS:   s.replace(/\s+/g, "")
来源：http://bo.nszjky.cn

TS:   s.replace(/\s+/g, "")
来源：http://ef.521024.cn

Java: s.replaceAll("\\s+", "")
来源：http://po.chemitech.net.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://iz.wgjwhj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://pa.yuntaijiaju.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fn.521024.cn

[E10] 左侧补零 / 定长填充
来源：http://xi.wgjwhj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jy.newstarts.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://yu.chemitech.net.cn

JS:   "7".padStart(3, "0")
来源：http://vn.bjjhwx.cn

TS:   "7".padStart(3, "0")
来源：http://yx.bookmarksfly.cn

Java: String.format("%03d", 7)
来源：http://ix.huixiangedu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://pg.521024.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sb.huanxung.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pd.bjjhwx.cn

[E11] 反转字符串
来源：http://kd.chemitech.net.cn

Py:   s[::-1]
来源：http://vz.bookmarksfly.cn

PHP:  strrev($s);
来源：http://zz.yuexingan06.cn

JS:   [...s].reverse().join("")
来源：http://ga.lnxyls.cn

TS:   [...s].reverse().join("")
来源：http://uv.hnjuh.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://on.bookmarksfly.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://lw.szxytkj.cn

Ruby: s.reverse
来源：http://xu.shxzukj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ig.yuntaijiaju.cn

[E12] 统计某字符出现次数
来源：http://dr.9csxet.cn

Py:   s.count("a")
来源：http://ig.bookmarksfly.cn

PHP:  substr_count($s, "a");
来源：http://ie.yuntaijiaju.cn

JS:   s.split("a").length - 1
来源：http://kh.wgjwhj.cn

TS:   s.split("a").length - 1
来源：http://ov.bjjhwx.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rg.chemitech.net.cn

Go:   strings.Count(s, "a")
来源：http://pd.newstarts.cn

Ruby: s.count("a")
来源：http://mm.bookmarksfly.cn

C#:   s.Count(c => c == 'a')
来源：http://yz.jianghongdianzi.cn

[E13] 逐字符遍历
来源：http://rm.yuexingan06.cn

Py:   for ch in s: print(ch)
来源：http://zi.hahajie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wi.gzmigu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ap.yuntaijiaju.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ws.newstarts.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bq.szsharing.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zb.hnjuh.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://zm.newstarts.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lx.huixinmuqiang.cn

[E14] URL 编码与 Base64
来源：http://mn.szsharing.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sl.nszjky.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://kv.szsharing.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wa.jctech888.com.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sw.nicolike.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://he.szxytkj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xu.szxytkj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://py.jianghongdianzi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ha.muxihuayi.cn

[E15] HTML 转义 / 反转义
来源：http://kf.szxytkj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://nr.521024.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kf.jctech888.com.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gv.jctech888.com.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://fw.jctech888.com.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xj.521024.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gu.huanxung.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cz.huanxung.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mh.shxzukj.cn

[E16] 数字千分位
来源：http://gx.szsharing.cn

Py:   f"{1234567:,}"
来源：http://xb.szxytkj.cn

PHP:  number_format(1234567);
来源：http://hr.wgjwhj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://kp.huanxung.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://cz.bookmarksfly.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mv.9csxet.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ck.wgjwhj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qp.panjiajie.cn

C#:   1234567.ToString("N0")
来源：http://rv.haigaiapp.cn

[E17] 首字母大写
来源：http://dy.hnjuh.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tc.gzmigu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://hy.szsharing.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mu.shxzukj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://og.huixiangedu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jt.panjiajie.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yn.shtwfgs.cn

Ruby: s.capitalize
来源：http://bj.jctech888.com.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fz.521024.cn

[E18] 模板占位符替换
来源：http://ss.huanxung.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://of.lnxyls.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yx.lnxyls.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://he.lnxyls.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://yp.huixiangedu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tc.panjiajie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gr.chemitech.net.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fb.shxzskj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kz.huixiangedu.cn

[E19] 多行文本按行拆分
来源：http://uw.lnxyls.cn

Py:   s.splitlines()
来源：http://pb.jctech888.com.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jv.newstarts.cn

JS:   s.split(/\r?\n/)
来源：http://st.shxzukj.cn

TS:   s.split(/\r?\n/)
来源：http://rn.hnjuh.cn

Java: s.lines().toList()
来源：http://mb.jctech888.com.cn

Go:   strings.Split(s, "\n")
来源：http://ot.panjiajie.cn

Ruby: s.lines
来源：http://wp.gzmigu.cn

C#:   s.Split('\n')
来源：http://ve.hnjuh.cn

[E20] 判断字符串是否为空
来源：http://fi.huanxung.cn

Py:   if not s:
来源：http://fc.hnjuh.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bg.nicolike.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nd.nszjky.cn

TS:   if (s === "") {}
来源：http://ko.yuntaijiaju.cn

Java: if (s.isEmpty()) {}
来源：http://we.nszjky.cn

Go:   if s == "" {}
来源：http://ug.huanxung.cn

Ruby: if s.empty?
来源：http://mq.bjjhwx.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://px.gzmigu.cn

[E21] 超长截断加省略号
来源：http://oh.shxzukj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://iw.jianghongdianzi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://at.jctech888.com.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pj.521024.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jx.yuexingan06.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pc.shtwfgs.cn

Go:   // 按 rune 判断长度后截断
来源：http://qq.521024.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fz.muxihuayi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://uj.jctech888.com.cn

[E22] 字节长度与字符长度
来源：http://ku.huixinmuqiang.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yx.jianghongdianzi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ec.9csxet.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cw.huanxung.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://oo.lnxyls.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ft.gzmigu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jx.hnjuh.cn

Ruby: s.bytesize;  s.length
来源：http://fe.jctech888.com.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jd.muxihuayi.cn

================================================================================
来源：http://nn.chemitech.net.cn

F. 文件与目录
来源：http://lk.521024.cn

================================================================================
来源：http://uo.huixinmuqiang.cn

[F01] 读取整个文件
来源：http://vu.521024.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rx.jctech888.com.cn

PHP:  file_get_contents("a.txt");
来源：http://bv.hnjuh.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bt.chemitech.net.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fb.shtwfgs.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://es.chemitech.net.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sh.jianghongdianzi.cn

Ruby: File.read("a.txt")
来源：http://fl.nszjky.cn

C#:   File.ReadAllText("a.txt");
来源：http://ti.panjiajie.cn

[F02] 逐行读取文件
来源：http://sp.521024.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fm.bookmarksfly.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://iu.asd995.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cc.521024.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hk.nszjky.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://am.jianghongdianzi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qm.gzmigu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wm.9csxet.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ec.9csxet.cn

[F03] 写入文件（覆盖）
来源：http://mu.yuntaijiaju.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gr.lnxyls.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://af.hnjuh.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zh.hahajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hk.jctech888.com.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ij.jianghongdianzi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ko.colortex.cn

Ruby: File.write("a.txt", "hi")
来源：http://hu.huixinmuqiang.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lz.jctech888.com.cn

[F04] 追加写入文件
来源：http://tj.chemitech.net.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ct.chemitech.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rv.yuexingan06.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lj.huixinmuqiang.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lj.nicolike.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lh.521024.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://uf.hnjuh.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nq.bjjhwx.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fp.bjjhwx.cn

[F05] 判断文件或目录是否存在
来源：http://oz.hahajie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xd.shtwfgs.cn

PHP:  file_exists("a.txt");
来源：http://mh.jianghongdianzi.cn

JS:   fs.existsSync("a.txt")
来源：http://ej.panjiajie.cn

TS:   fs.existsSync("a.txt")
来源：http://zz.bjjhwx.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://jf.hahajie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://br.wgjwhj.cn

Ruby: File.exist?("a.txt")
来源：http://gy.colortex.cn

C#:   File.Exists("a.txt")
来源：http://ur.szsharing.cn

[F06] 删除文件
来源：http://vx.szxytkj.cn

Py:   os.remove("a.txt")
来源：http://mh.nicolike.cn

PHP:  unlink("a.txt");
来源：http://cr.hahajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://by.jianghongdianzi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ex.yuexingan06.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jh.szxytkj.cn

Go:   os.Remove("a.txt")
来源：http://pv.yuexingan06.cn

Ruby: File.delete("a.txt")
来源：http://dz.huixiangedu.cn

C#:   File.Delete("a.txt");
来源：http://et.shxzskj.cn

[F07] 创建目录（含多级）
来源：http://nj.hahajie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://en.nicolike.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qv.asd995.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zb.huixiangedu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oy.muxihuayi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tq.huixiangedu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nk.szsharing.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dm.haigaiapp.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hu.shxzskj.cn

[F08] 遍历目录
来源：http://li.asd995.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xc.jctech888.com.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sz.szxytkj.cn

JS:   fs.readdirSync("dir")
来源：http://bw.shxzukj.cn

TS:   fs.readdirSync("dir")
来源：http://dz.jianghongdianzi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kf.jctech888.com.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://bc.jctech888.com.cn

Ruby: Dir.children("dir")
来源：http://bm.szxytkj.cn

C#:   Directory.GetFiles("dir")
来源：http://dn.yuntaijiaju.cn

[F09] 获取文件大小
来源：http://it.newstarts.cn

Py:   os.path.getsize("a.txt")
来源：http://ig.haigaiapp.cn

PHP:  filesize("a.txt");
来源：http://ab.nszjky.cn

JS:   fs.statSync("a.txt").size
来源：http://cy.haigaiapp.cn

TS:   fs.statSync("a.txt").size
来源：http://xs.szxytkj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://sh.wgjwhj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://uz.szxytkj.cn

Ruby: File.size("a.txt")
来源：http://qv.nszjky.cn

C#:   new FileInfo("a.txt").Length
来源：http://yh.gzmigu.cn

[F10] 取文件扩展名 / 文件名
来源：http://aj.hnjuh.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://lo.nicolike.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ur.9csxet.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xo.521024.cn

TS:   path.extname("a.txt")
来源：http://dq.hnjuh.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vj.nicolike.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bt.521024.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ii.shtwfgs.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zj.hahajie.cn

[F11] 复制与移动文件
来源：http://sj.shtwfgs.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rk.gzmigu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zt.bookmarksfly.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pv.bookmarksfly.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://il.asd995.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tt.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gh.nszjky.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zc.colortex.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vp.nszjky.cn

[F12] CSV 读写
来源：http://io.colortex.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bi.nicolike.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lz.newstarts.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jg.hahajie.cn

TS:   // 同上
来源：http://kz.9csxet.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hh.bookmarksfly.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kp.nszjky.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ub.521024.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://kn.wgjwhj.cn

================================================================================
来源：http://zi.chemitech.net.cn

G. 面向对象
来源：http://vu.shtwfgs.cn

================================================================================
来源：http://tq.panjiajie.cn

[G01] 定义类
来源：http://kg.hnjuh.cn

Py:   class User: pass
来源：http://ma.jianghongdianzi.cn

PHP:  class User {}
来源：http://rc.szxytkj.cn

JS:   class User {}
来源：http://fn.yuexingan06.cn

TS:   class User { name: string = ""; }
来源：http://ma.muxihuayi.cn

Java: class User {}
来源：http://mt.nszjky.cn

Go:   type User struct { Name string }
来源：http://no.jianghongdianzi.cn

Ruby: class User; end
来源：http://lz.newstarts.cn

C#:   class User {}
来源：http://ek.bookmarksfly.cn

[G02] 构造函数
来源：http://at.panjiajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://sk.yuntaijiaju.cn

PHP:  public function __construct(public string $name) {}
来源：http://cp.shxzukj.cn

JS:   constructor(name) { this.name = name; }
来源：http://ij.asd995.cn


<!-- 参考信息 -->