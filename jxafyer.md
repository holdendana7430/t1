代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cn.shxzukj.cn

TS:   s.slice(1, 4)
来源：http://lr.shxzukj.cn

Java: s.substring(1, 4)
来源：http://ln.huixinmuqiang.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jv.panjiajie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ta.9csxet.cn

C#:   s.Substring(1, 3)
来源：http://ci.szxytkj.cn

[E04] 查找子串位置
来源：http://jt.asd995.cn

Py:   s.find("x");  s.index("x")
来源：http://as.newstarts.cn

PHP:  strpos($s, "x");
来源：http://vi.muxihuayi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rx.gzmigu.cn

TS:   s.indexOf("x")
来源：http://fg.jctech888.com.cn

Java: s.indexOf("x")
来源：http://oe.shxzskj.cn

Go:   strings.Index(s, "x")
来源：http://ko.yuexingan06.cn

Ruby: s.index("x")
来源：http://nv.bjjhwx.cn

C#:   s.IndexOf("x")
来源：http://tp.colortex.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ac.nicolike.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tv.nicolike.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wx.chemitech.net.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zn.wgjwhj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://jd.hnjuh.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rg.9csxet.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fp.colortex.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://np.bjjhwx.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ng.hnjuh.cn

[E06] 替换子串
来源：http://xw.lnxyls.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zd.chemitech.net.cn

PHP:  str_replace("a", "b", $s);
来源：http://ns.huanxung.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mu.nszjky.cn

TS:   s.replaceAll("a", "b")
来源：http://ym.haigaiapp.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dz.muxihuayi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://em.9csxet.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qv.chemitech.net.cn

C#:   s.Replace("a", "b")
来源：http://pe.shxzukj.cn

[E07] 按分隔符拆分
来源：http://pl.wgjwhj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://of.jianghongdianzi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lg.lnxyls.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://oh.hahajie.cn

TS:   s.split(",")
来源：http://cu.asd995.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ix.szxytkj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rg.shtwfgs.cn

Ruby: s.split(",");  s.split
来源：http://wk.shxzskj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://to.szxytkj.cn

[E08] 数组按分隔符合并
来源：http://xf.szxytkj.cn

Py:   ",".join(items)
来源：http://ef.asd995.cn

PHP:  implode(",", $items);
来源：http://dy.haigaiapp.cn

JS:   items.join(",")
来源：http://bs.hnjuh.cn

TS:   items.join(",")
来源：http://zd.9csxet.cn

Java: String.join(",", items)
来源：http://dl.szxytkj.cn

Go:   strings.Join(items, ",")
来源：http://vo.szxytkj.cn

Ruby: items.join(",")
来源：http://bl.colortex.cn

C#:   string.Join(",", items)
来源：http://xv.jctech888.com.cn

[E09] 去除所有空白字符
来源：http://yd.nszjky.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.muxihuayi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xb.panjiajie.cn

JS:   s.replace(/\s+/g, "")
来源：http://oq.521024.cn

TS:   s.replace(/\s+/g, "")
来源：http://fw.yuntaijiaju.cn

Java: s.replaceAll("\\s+", "")
来源：http://bo.newstarts.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://vh.yuexingan06.cn

Ruby: s.gsub(/\s+/, "")
来源：http://iy.yuntaijiaju.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hd.nicolike.cn

[E10] 左侧补零 / 定长填充
来源：http://cx.szxytkj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gc.nicolike.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ao.shxzukj.cn

JS:   "7".padStart(3, "0")
来源：http://rk.lnxyls.cn

TS:   "7".padStart(3, "0")
来源：http://lu.nszjky.cn

Java: String.format("%03d", 7)
来源：http://jx.shtwfgs.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://hy.jianghongdianzi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://go.yuntaijiaju.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gh.newstarts.cn

[E11] 反转字符串
来源：http://ql.hnjuh.cn

Py:   s[::-1]
来源：http://cr.huixiangedu.cn

PHP:  strrev($s);
来源：http://ou.yuexingan06.cn

JS:   [...s].reverse().join("")
来源：http://xm.panjiajie.cn

TS:   [...s].reverse().join("")
来源：http://be.nicolike.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://iz.shxzukj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://hv.lnxyls.cn

Ruby: s.reverse
来源：http://fx.newstarts.cn

C#:   new string(s.Reverse().ToArray())
来源：http://kp.shxzskj.cn

[E12] 统计某字符出现次数
来源：http://ie.shxzskj.cn

Py:   s.count("a")
来源：http://kx.huanxung.cn

PHP:  substr_count($s, "a");
来源：http://bt.521024.cn

JS:   s.split("a").length - 1
来源：http://lq.chemitech.net.cn

TS:   s.split("a").length - 1
来源：http://wo.panjiajie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://we.szsharing.cn

Go:   strings.Count(s, "a")
来源：http://ax.jctech888.com.cn

Ruby: s.count("a")
来源：http://ax.panjiajie.cn

C#:   s.Count(c => c == 'a')
来源：http://zr.huixiangedu.cn

[E13] 逐字符遍历
来源：http://gf.jianghongdianzi.cn

Py:   for ch in s: print(ch)
来源：http://av.huixiangedu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qi.shtwfgs.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://kj.colortex.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://fv.521024.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qg.huanxung.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ts.shxzukj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://oc.shxzskj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mc.szsharing.cn

[E14] URL 编码与 Base64
来源：http://sk.shtwfgs.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sv.colortex.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://vd.muxihuayi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wd.yuntaijiaju.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bx.shxzukj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nv.yuntaijiaju.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xz.bookmarksfly.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cw.nicolike.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vl.shtwfgs.cn

[E15] HTML 转义 / 反转义
来源：http://pn.szxytkj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://tw.hahajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ld.hnjuh.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yz.bjjhwx.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ig.colortex.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://af.muxihuayi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mf.jctech888.com.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ln.shxzskj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pa.shxzskj.cn

[E16] 数字千分位
来源：http://nz.shxzskj.cn

Py:   f"{1234567:,}"
来源：http://fd.chemitech.net.cn

PHP:  number_format(1234567);
来源：http://iq.jianghongdianzi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://pj.huanxung.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://xe.jianghongdianzi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hd.shxzskj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jl.huixiangedu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://sf.haigaiapp.cn

C#:   1234567.ToString("N0")
来源：http://vh.szsharing.cn

[E17] 首字母大写
来源：http://qs.hnjuh.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dr.bookmarksfly.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://si.jianghongdianzi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ir.bjjhwx.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fq.haigaiapp.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kt.muxihuayi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gr.nszjky.cn

Ruby: s.capitalize
来源：http://gr.shxzukj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jn.lnxyls.cn

[E18] 模板占位符替换
来源：http://sk.asd995.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nv.bookmarksfly.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fl.nszjky.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://jb.shxzskj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://it.hahajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ie.newstarts.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lj.asd995.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rw.yuntaijiaju.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lx.shtwfgs.cn

[E19] 多行文本按行拆分
来源：http://sg.lnxyls.cn

Py:   s.splitlines()
来源：http://wa.yuexingan06.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wu.haigaiapp.cn

JS:   s.split(/\r?\n/)
来源：http://cx.nszjky.cn

TS:   s.split(/\r?\n/)
来源：http://fu.haigaiapp.cn

Java: s.lines().toList()
来源：http://pl.jianghongdianzi.cn

Go:   strings.Split(s, "\n")
来源：http://gm.shxzskj.cn

Ruby: s.lines
来源：http://xp.nszjky.cn

C#:   s.Split('\n')
来源：http://bh.chemitech.net.cn

[E20] 判断字符串是否为空
来源：http://sc.9csxet.cn

Py:   if not s:
来源：http://yf.yuntaijiaju.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vw.shxzskj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://oy.bjjhwx.cn

TS:   if (s === "") {}
来源：http://dl.nicolike.cn

Java: if (s.isEmpty()) {}
来源：http://jq.hnjuh.cn

Go:   if s == "" {}
来源：http://uo.yuexingan06.cn

Ruby: if s.empty?
来源：http://di.bjjhwx.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lv.jianghongdianzi.cn

[E21] 超长截断加省略号
来源：http://yl.panjiajie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zr.hnjuh.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://su.bjjhwx.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hv.haigaiapp.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://po.jianghongdianzi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hw.bjjhwx.cn

Go:   // 按 rune 判断长度后截断
来源：http://ek.bookmarksfly.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gk.wgjwhj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cf.gzmigu.cn

[E22] 字节长度与字符长度
来源：http://dd.wgjwhj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://th.shxzukj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bc.bjjhwx.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rf.huixinmuqiang.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zg.nicolike.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rl.gzmigu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ew.bjjhwx.cn

Ruby: s.bytesize;  s.length
来源：http://vx.haigaiapp.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qa.9csxet.cn

================================================================================
来源：http://oo.jctech888.com.cn

F. 文件与目录
来源：http://xf.colortex.cn

================================================================================
来源：http://kk.bookmarksfly.cn

[F01] 读取整个文件
来源：http://jb.lnxyls.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tp.gzmigu.cn

PHP:  file_get_contents("a.txt");
来源：http://rh.jctech888.com.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fc.chemitech.net.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://td.newstarts.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://yi.szxytkj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uf.nszjky.cn

Ruby: File.read("a.txt")
来源：http://ol.szsharing.cn

C#:   File.ReadAllText("a.txt");
来源：http://fp.shxzskj.cn

[F02] 逐行读取文件
来源：http://bz.jctech888.com.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://yk.colortex.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://yg.colortex.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uw.gzmigu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zv.bjjhwx.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zo.chemitech.net.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tu.hahajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vm.521024.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ui.yuexingan06.cn

[F03] 写入文件（覆盖）
来源：http://ro.yuntaijiaju.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gi.colortex.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://gt.bookmarksfly.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qj.hahajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ph.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xr.jctech888.com.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ke.bjjhwx.cn

Ruby: File.write("a.txt", "hi")
来源：http://zx.colortex.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bk.yuntaijiaju.cn

[F04] 追加写入文件
来源：http://gj.panjiajie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yi.bjjhwx.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ej.gzmigu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tt.shtwfgs.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vh.szsharing.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sb.jctech888.com.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ng.haigaiapp.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qq.gzmigu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ed.shtwfgs.cn

[F05] 判断文件或目录是否存在
来源：http://fa.521024.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lj.muxihuayi.cn

PHP:  file_exists("a.txt");
来源：http://ig.yuexingan06.cn

JS:   fs.existsSync("a.txt")
来源：http://su.huixiangedu.cn

TS:   fs.existsSync("a.txt")
来源：http://lf.gzmigu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://sw.gzmigu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gx.huanxung.cn

Ruby: File.exist?("a.txt")
来源：http://lc.hnjuh.cn

C#:   File.Exists("a.txt")
来源：http://qs.huixiangedu.cn

[F06] 删除文件
来源：http://dt.panjiajie.cn

Py:   os.remove("a.txt")
来源：http://mp.yuexingan06.cn

PHP:  unlink("a.txt");
来源：http://mo.9csxet.cn

JS:   fs.unlinkSync("a.txt")
来源：http://us.haigaiapp.cn

TS:   fs.unlinkSync("a.txt")
来源：http://yt.panjiajie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cp.shxzukj.cn

Go:   os.Remove("a.txt")
来源：http://ea.shxzukj.cn

Ruby: File.delete("a.txt")
来源：http://xq.huixinmuqiang.cn

C#:   File.Delete("a.txt");
来源：http://iz.huanxung.cn

[F07] 创建目录（含多级）
来源：http://lg.chemitech.net.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nm.bookmarksfly.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kr.newstarts.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bp.huanxung.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ao.bjjhwx.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rn.lnxyls.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cp.nszjky.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kl.shxzskj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rq.shxzskj.cn

[F08] 遍历目录
来源：http://ax.yuntaijiaju.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://tf.jctech888.com.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zz.huixinmuqiang.cn

JS:   fs.readdirSync("dir")
来源：http://oy.yuexingan06.cn

TS:   fs.readdirSync("dir")
来源：http://ol.muxihuayi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qj.yuexingan06.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ma.yuntaijiaju.cn

Ruby: Dir.children("dir")
来源：http://of.muxihuayi.cn

C#:   Directory.GetFiles("dir")
来源：http://tk.gzmigu.cn

[F09] 获取文件大小
来源：http://zf.bookmarksfly.cn

Py:   os.path.getsize("a.txt")
来源：http://pr.newstarts.cn

PHP:  filesize("a.txt");
来源：http://nz.hahajie.cn

JS:   fs.statSync("a.txt").size
来源：http://io.shxzskj.cn

TS:   fs.statSync("a.txt").size
来源：http://ww.shxzukj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://uz.hnjuh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fv.nszjky.cn

Ruby: File.size("a.txt")
来源：http://ws.wgjwhj.cn

C#:   new FileInfo("a.txt").Length
来源：http://ka.bookmarksfly.cn

[F10] 取文件扩展名 / 文件名
来源：http://aq.jianghongdianzi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ub.szsharing.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rf.asd995.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.bjjhwx.cn

TS:   path.extname("a.txt")
来源：http://se.jctech888.com.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://po.shxzskj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ra.szxytkj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ic.haigaiapp.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cb.huanxung.cn

[F11] 复制与移动文件
来源：http://xd.yuntaijiaju.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ye.nicolike.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://sk.muxihuayi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ao.colortex.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qt.jctech888.com.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tc.hnjuh.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fl.huanxung.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lm.shtwfgs.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gc.hahajie.cn

[F12] CSV 读写
来源：http://xo.shtwfgs.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xd.lnxyls.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qw.szsharing.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tl.huixinmuqiang.cn

TS:   // 同上
来源：http://tj.jianghongdianzi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yp.szsharing.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ix.huanxung.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dd.jianghongdianzi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://de.muxihuayi.cn

================================================================================
来源：http://al.wgjwhj.cn

G. 面向对象
来源：http://yh.shxzskj.cn

================================================================================
来源：http://kd.panjiajie.cn

[G01] 定义类
来源：http://yc.bjjhwx.cn

Py:   class User: pass
来源：http://cn.9csxet.cn

PHP:  class User {}
来源：http://os.shxzukj.cn

JS:   class User {}
来源：http://ip.jianghongdianzi.cn

TS:   class User { name: string = ""; }
来源：http://ls.szsharing.cn

Java: class User {}
来源：http://qi.shxzukj.cn

Go:   type User struct { Name string }
来源：http://bb.yuntaijiaju.cn

Ruby: class User; end
来源：http://rz.bjjhwx.cn

C#:   class User {}
来源：http://kp.jianghongdianzi.cn


<!-- 参考信息 -->