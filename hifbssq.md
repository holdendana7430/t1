代发 wailian999

TS:   "ab".repeat(3)
来源：http://il.yuexingan06.cn

Java: "ab".repeat(3)
来源：http://nz.szxytkj.cn

Go:   strings.Repeat("ab", 3)
来源：http://gr.newstarts.cn

Ruby: "ab" * 3
来源：http://pq.hahajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ha.shxzskj.cn

[E03] 截取子串
来源：http://qt.lnxyls.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nc.szsharing.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vq.9csxet.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gj.panjiajie.cn

TS:   s.slice(1, 4)
来源：http://if.asd995.cn

Java: s.substring(1, 4)
来源：http://wc.jctech888.com.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lo.yuexingan06.cn

Ruby: s[1, 3];  s[1..3]
来源：http://yf.szsharing.cn

C#:   s.Substring(1, 3)
来源：http://jd.bjjhwx.cn

[E04] 查找子串位置
来源：http://jr.hnjuh.cn

Py:   s.find("x");  s.index("x")
来源：http://ya.hahajie.cn

PHP:  strpos($s, "x");
来源：http://wg.huixiangedu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gl.shxzskj.cn

TS:   s.indexOf("x")
来源：http://kg.shtwfgs.cn

Java: s.indexOf("x")
来源：http://pp.9csxet.cn

Go:   strings.Index(s, "x")
来源：http://cn.asd995.cn

Ruby: s.index("x")
来源：http://ua.szsharing.cn

C#:   s.IndexOf("x")
来源：http://lc.9csxet.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xy.colortex.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://oy.shxzskj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lo.hahajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ns.haigaiapp.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qg.newstarts.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ay.huixinmuqiang.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://st.nszjky.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rb.huanxung.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dw.szsharing.cn

[E06] 替换子串
来源：http://ms.hahajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jz.jctech888.com.cn

PHP:  str_replace("a", "b", $s);
来源：http://ma.jctech888.com.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://se.wgjwhj.cn

TS:   s.replaceAll("a", "b")
来源：http://zv.nszjky.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fc.jctech888.com.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cv.jctech888.com.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vr.bjjhwx.cn

C#:   s.Replace("a", "b")
来源：http://ea.jctech888.com.cn

[E07] 按分隔符拆分
来源：http://zy.wgjwhj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wf.bookmarksfly.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ld.haigaiapp.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ig.bjjhwx.cn

TS:   s.split(",")
来源：http://rg.nicolike.cn

Java: s.split(",");  s.split("\\s+")
来源：http://hb.yuntaijiaju.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nr.gzmigu.cn

Ruby: s.split(",");  s.split
来源：http://uv.muxihuayi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ji.gzmigu.cn

[E08] 数组按分隔符合并
来源：http://sg.newstarts.cn

Py:   ",".join(items)
来源：http://vm.bjjhwx.cn

PHP:  implode(",", $items);
来源：http://mb.shxzskj.cn

JS:   items.join(",")
来源：http://ma.haigaiapp.cn

TS:   items.join(",")
来源：http://ya.asd995.cn

Java: String.join(",", items)
来源：http://yb.lnxyls.cn

Go:   strings.Join(items, ",")
来源：http://di.shtwfgs.cn

Ruby: items.join(",")
来源：http://ty.haigaiapp.cn

C#:   string.Join(",", items)
来源：http://zr.521024.cn

[E09] 去除所有空白字符
来源：http://uq.521024.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ia.muxihuayi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bo.panjiajie.cn

JS:   s.replace(/\s+/g, "")
来源：http://ic.hnjuh.cn

TS:   s.replace(/\s+/g, "")
来源：http://ge.asd995.cn

Java: s.replaceAll("\\s+", "")
来源：http://gs.bjjhwx.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://rd.haigaiapp.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xd.szxytkj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ns.panjiajie.cn

[E10] 左侧补零 / 定长填充
来源：http://hm.gzmigu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://os.panjiajie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zz.haigaiapp.cn

JS:   "7".padStart(3, "0")
来源：http://uf.asd995.cn

TS:   "7".padStart(3, "0")
来源：http://fq.9csxet.cn

Java: String.format("%03d", 7)
来源：http://qf.9csxet.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://lh.bookmarksfly.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ns.hahajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jv.huixinmuqiang.cn

[E11] 反转字符串
来源：http://vb.asd995.cn

Py:   s[::-1]
来源：http://jv.panjiajie.cn

PHP:  strrev($s);
来源：http://ds.gzmigu.cn

JS:   [...s].reverse().join("")
来源：http://pf.huanxung.cn

TS:   [...s].reverse().join("")
来源：http://yj.wgjwhj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zs.9csxet.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://fz.jctech888.com.cn

Ruby: s.reverse
来源：http://fi.asd995.cn

C#:   new string(s.Reverse().ToArray())
来源：http://rt.nszjky.cn

[E12] 统计某字符出现次数
来源：http://ce.haigaiapp.cn

Py:   s.count("a")
来源：http://zs.bookmarksfly.cn

PHP:  substr_count($s, "a");
来源：http://np.huixiangedu.cn

JS:   s.split("a").length - 1
来源：http://bo.colortex.cn

TS:   s.split("a").length - 1
来源：http://qq.szsharing.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dz.asd995.cn

Go:   strings.Count(s, "a")
来源：http://rt.shxzukj.cn

Ruby: s.count("a")
来源：http://wg.hnjuh.cn

C#:   s.Count(c => c == 'a')
来源：http://ka.lnxyls.cn

[E13] 逐字符遍历
来源：http://du.bookmarksfly.cn

Py:   for ch in s: print(ch)
来源：http://bb.521024.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bn.chemitech.net.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://of.huanxung.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://fs.panjiajie.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://af.gzmigu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://me.9csxet.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://cn.nicolike.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ni.panjiajie.cn

[E14] URL 编码与 Base64
来源：http://up.chemitech.net.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zt.shxzskj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://pg.huixinmuqiang.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zh.jianghongdianzi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ey.lnxyls.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ad.bookmarksfly.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ws.9csxet.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dm.szxytkj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xp.huanxung.cn

[E15] HTML 转义 / 反转义
来源：http://xk.huixinmuqiang.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://th.shxzskj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nl.wgjwhj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ke.colortex.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://xa.wgjwhj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://be.shxzskj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ko.yuntaijiaju.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ou.huanxung.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pd.chemitech.net.cn

[E16] 数字千分位
来源：http://zg.nszjky.cn

Py:   f"{1234567:,}"
来源：http://xx.wgjwhj.cn

PHP:  number_format(1234567);
来源：http://pf.asd995.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://wh.wgjwhj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ap.szsharing.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://oy.hnjuh.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://af.hnjuh.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xo.hnjuh.cn

C#:   1234567.ToString("N0")
来源：http://yx.bjjhwx.cn

[E17] 首字母大写
来源：http://fk.huixiangedu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wa.9csxet.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://by.hnjuh.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wg.yuexingan06.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gg.shxzukj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jc.szxytkj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yf.wgjwhj.cn

Ruby: s.capitalize
来源：http://ji.huixiangedu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tj.9csxet.cn

[E18] 模板占位符替换
来源：http://fj.521024.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hx.muxihuayi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yn.nszjky.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://bb.jianghongdianzi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://xk.shxzskj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xb.haigaiapp.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vo.muxihuayi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://le.szsharing.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dj.hahajie.cn

[E19] 多行文本按行拆分
来源：http://fn.panjiajie.cn

Py:   s.splitlines()
来源：http://qs.szxytkj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ak.asd995.cn

JS:   s.split(/\r?\n/)
来源：http://oz.shxzukj.cn

TS:   s.split(/\r?\n/)
来源：http://au.shxzskj.cn

Java: s.lines().toList()
来源：http://ty.huanxung.cn

Go:   strings.Split(s, "\n")
来源：http://dl.gzmigu.cn

Ruby: s.lines
来源：http://aa.asd995.cn

C#:   s.Split('\n')
来源：http://ii.haigaiapp.cn

[E20] 判断字符串是否为空
来源：http://ng.szsharing.cn

Py:   if not s:
来源：http://zw.szxytkj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vb.chemitech.net.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://in.bookmarksfly.cn

TS:   if (s === "") {}
来源：http://wp.gzmigu.cn

Java: if (s.isEmpty()) {}
来源：http://jd.panjiajie.cn

Go:   if s == "" {}
来源：http://rk.yuexingan06.cn

Ruby: if s.empty?
来源：http://km.asd995.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://op.yuntaijiaju.cn

[E21] 超长截断加省略号
来源：http://ym.hahajie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tr.hnjuh.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lh.panjiajie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cq.jctech888.com.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wy.huixinmuqiang.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qu.hahajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://ed.chemitech.net.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xs.shxzukj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://am.wgjwhj.cn

[E22] 字节长度与字符长度
来源：http://ap.bookmarksfly.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tj.jianghongdianzi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mc.bookmarksfly.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zc.newstarts.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lp.colortex.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gb.jctech888.com.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mu.9csxet.cn

Ruby: s.bytesize;  s.length
来源：http://vy.hnjuh.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zj.nszjky.cn

================================================================================
来源：http://jd.hahajie.cn

F. 文件与目录
来源：http://aa.muxihuayi.cn

================================================================================
来源：http://iu.chemitech.net.cn

[F01] 读取整个文件
来源：http://yb.nicolike.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hu.wgjwhj.cn

PHP:  file_get_contents("a.txt");
来源：http://sr.bookmarksfly.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://em.bjjhwx.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://io.hahajie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://nd.panjiajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lp.yuexingan06.cn

Ruby: File.read("a.txt")
来源：http://ez.newstarts.cn

C#:   File.ReadAllText("a.txt");
来源：http://dq.muxihuayi.cn

[F02] 逐行读取文件
来源：http://jh.chemitech.net.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vz.szxytkj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pr.huanxung.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://en.hahajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zr.szxytkj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vg.huixinmuqiang.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dx.colortex.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pt.9csxet.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tk.521024.cn

[F03] 写入文件（覆盖）
来源：http://vw.huanxung.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bi.huanxung.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://kt.lnxyls.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tq.hnjuh.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fc.hnjuh.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ji.shxzskj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rx.hnjuh.cn

Ruby: File.write("a.txt", "hi")
来源：http://vl.shxzskj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bn.shtwfgs.cn

[F04] 追加写入文件
来源：http://vs.hahajie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pm.haigaiapp.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kd.jianghongdianzi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nh.lnxyls.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zx.hnjuh.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vv.lnxyls.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yf.yuexingan06.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tx.haigaiapp.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jv.huixinmuqiang.cn

[F05] 判断文件或目录是否存在
来源：http://kt.jianghongdianzi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://il.wgjwhj.cn

PHP:  file_exists("a.txt");
来源：http://ml.huixinmuqiang.cn

JS:   fs.existsSync("a.txt")
来源：http://br.hnjuh.cn

TS:   fs.existsSync("a.txt")
来源：http://ys.newstarts.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://rh.huanxung.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zu.chemitech.net.cn

Ruby: File.exist?("a.txt")
来源：http://pf.bookmarksfly.cn

C#:   File.Exists("a.txt")
来源：http://ph.jianghongdianzi.cn

[F06] 删除文件
来源：http://ld.hnjuh.cn

Py:   os.remove("a.txt")
来源：http://vt.szxytkj.cn

PHP:  unlink("a.txt");
来源：http://ym.jctech888.com.cn

JS:   fs.unlinkSync("a.txt")
来源：http://wu.yuntaijiaju.cn

TS:   fs.unlinkSync("a.txt")
来源：http://pf.szsharing.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jb.gzmigu.cn

Go:   os.Remove("a.txt")
来源：http://cw.asd995.cn

Ruby: File.delete("a.txt")
来源：http://nr.chemitech.net.cn

C#:   File.Delete("a.txt");
来源：http://uw.wgjwhj.cn

[F07] 创建目录（含多级）
来源：http://jo.521024.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ah.yuntaijiaju.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mt.gzmigu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yg.jianghongdianzi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://he.shxzskj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://aq.huixiangedu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ke.asd995.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ny.521024.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://na.nszjky.cn

[F08] 遍历目录
来源：http://rq.nszjky.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://lp.gzmigu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nu.huixinmuqiang.cn

JS:   fs.readdirSync("dir")
来源：http://qr.jianghongdianzi.cn

TS:   fs.readdirSync("dir")
来源：http://qd.yuntaijiaju.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://me.szxytkj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://dq.newstarts.cn

Ruby: Dir.children("dir")
来源：http://xo.jianghongdianzi.cn

C#:   Directory.GetFiles("dir")
来源：http://xp.shtwfgs.cn

[F09] 获取文件大小
来源：http://xv.shxzskj.cn

Py:   os.path.getsize("a.txt")
来源：http://ru.asd995.cn

PHP:  filesize("a.txt");
来源：http://ox.shtwfgs.cn

JS:   fs.statSync("a.txt").size
来源：http://su.nszjky.cn

TS:   fs.statSync("a.txt").size
来源：http://il.szsharing.cn

Java: Files.size(Path.of("a.txt"))
来源：http://yg.huixiangedu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qq.shxzskj.cn

Ruby: File.size("a.txt")
来源：http://ln.shtwfgs.cn

C#:   new FileInfo("a.txt").Length
来源：http://wc.lnxyls.cn

[F10] 取文件扩展名 / 文件名
来源：http://ej.jctech888.com.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://or.hahajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xt.newstarts.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://eb.chemitech.net.cn

TS:   path.extname("a.txt")
来源：http://mq.hnjuh.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lj.haigaiapp.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://by.colortex.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ky.szxytkj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fh.521024.cn

[F11] 复制与移动文件
来源：http://bs.shtwfgs.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jo.jctech888.com.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://az.gzmigu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pi.bjjhwx.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xa.hnjuh.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bb.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://po.haigaiapp.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tt.huanxung.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mo.hahajie.cn

[F12] CSV 读写
来源：http://zs.hahajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pr.jianghongdianzi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fu.huixinmuqiang.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jo.521024.cn

TS:   // 同上
来源：http://ms.jianghongdianzi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yf.nicolike.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kv.lnxyls.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://re.shxzukj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://aj.yuntaijiaju.cn

================================================================================
来源：http://oa.szxytkj.cn

G. 面向对象
来源：http://fo.yuexingan06.cn

================================================================================
来源：http://by.huixiangedu.cn

[G01] 定义类
来源：http://ic.lnxyls.cn


<!-- 参考信息 -->