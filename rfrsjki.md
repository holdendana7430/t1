代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://mp.hnjuh.cn

C#:   s.Substring(1, 3)
来源：http://hv.huixinmuqiang.cn

[E04] 查找子串位置
来源：http://cz.9csxet.cn

Py:   s.find("x");  s.index("x")
来源：http://dj.asd995.cn

PHP:  strpos($s, "x");
来源：http://mx.shxzukj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dv.shxzukj.cn

TS:   s.indexOf("x")
来源：http://nj.huanxung.cn

Java: s.indexOf("x")
来源：http://pn.9csxet.cn

Go:   strings.Index(s, "x")
来源：http://co.lnxyls.cn

Ruby: s.index("x")
来源：http://sv.szsharing.cn

C#:   s.IndexOf("x")
来源：http://hu.hnjuh.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://vz.yuexingan06.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ks.shxzukj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://uq.muxihuayi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://po.asd995.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://uz.szsharing.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vw.huanxung.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fh.gzmigu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rb.newstarts.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ym.haigaiapp.cn

[E06] 替换子串
来源：http://cp.bookmarksfly.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zj.huixinmuqiang.cn

PHP:  str_replace("a", "b", $s);
来源：http://hn.shxzukj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tl.huixiangedu.cn

TS:   s.replaceAll("a", "b")
来源：http://mk.bjjhwx.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vm.bookmarksfly.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vc.521024.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ty.shtwfgs.cn

C#:   s.Replace("a", "b")
来源：http://hi.nszjky.cn

[E07] 按分隔符拆分
来源：http://hp.huanxung.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://il.huixiangedu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ld.huixiangedu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://la.haigaiapp.cn

TS:   s.split(",")
来源：http://yy.nicolike.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ko.jianghongdianzi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nk.nicolike.cn

Ruby: s.split(",");  s.split
来源：http://iw.nicolike.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://av.jianghongdianzi.cn

[E08] 数组按分隔符合并
来源：http://ds.hnjuh.cn

Py:   ",".join(items)
来源：http://fi.9csxet.cn

PHP:  implode(",", $items);
来源：http://zp.jianghongdianzi.cn

JS:   items.join(",")
来源：http://cx.muxihuayi.cn

TS:   items.join(",")
来源：http://kp.hahajie.cn

Java: String.join(",", items)
来源：http://gp.hnjuh.cn

Go:   strings.Join(items, ",")
来源：http://pc.szsharing.cn

Ruby: items.join(",")
来源：http://aj.nszjky.cn

C#:   string.Join(",", items)
来源：http://rx.haigaiapp.cn

[E09] 去除所有空白字符
来源：http://ns.521024.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kd.yuexingan06.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zg.colortex.cn

JS:   s.replace(/\s+/g, "")
来源：http://ym.shtwfgs.cn

TS:   s.replace(/\s+/g, "")
来源：http://mg.nicolike.cn

Java: s.replaceAll("\\s+", "")
来源：http://cq.szxytkj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://oz.yuexingan06.cn

Ruby: s.gsub(/\s+/, "")
来源：http://hq.nicolike.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vl.lnxyls.cn

[E10] 左侧补零 / 定长填充
来源：http://au.huixinmuqiang.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ht.panjiajie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bb.shxzskj.cn

JS:   "7".padStart(3, "0")
来源：http://xd.yuexingan06.cn

TS:   "7".padStart(3, "0")
来源：http://mj.huanxung.cn

Java: String.format("%03d", 7)
来源：http://yc.asd995.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://hg.yuntaijiaju.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ta.hahajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://py.huixinmuqiang.cn

[E11] 反转字符串
来源：http://bd.newstarts.cn

Py:   s[::-1]
来源：http://ol.jianghongdianzi.cn

PHP:  strrev($s);
来源：http://xx.9csxet.cn

JS:   [...s].reverse().join("")
来源：http://bb.nszjky.cn

TS:   [...s].reverse().join("")
来源：http://jo.shtwfgs.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wf.yuexingan06.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ft.gzmigu.cn

Ruby: s.reverse
来源：http://qp.shtwfgs.cn

C#:   new string(s.Reverse().ToArray())
来源：http://mu.jianghongdianzi.cn

[E12] 统计某字符出现次数
来源：http://by.panjiajie.cn

Py:   s.count("a")
来源：http://ma.colortex.cn

PHP:  substr_count($s, "a");
来源：http://ak.9csxet.cn

JS:   s.split("a").length - 1
来源：http://bg.asd995.cn

TS:   s.split("a").length - 1
来源：http://fl.hnjuh.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lz.huanxung.cn

Go:   strings.Count(s, "a")
来源：http://vn.shxzskj.cn

Ruby: s.count("a")
来源：http://eg.jctech888.com.cn

C#:   s.Count(c => c == 'a')
来源：http://ft.yuexingan06.cn

[E13] 逐字符遍历
来源：http://lh.szxytkj.cn

Py:   for ch in s: print(ch)
来源：http://bh.szsharing.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bl.521024.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://zh.gzmigu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://fs.nszjky.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tq.jianghongdianzi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ps.bookmarksfly.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://in.newstarts.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ir.bjjhwx.cn

[E14] URL 编码与 Base64
来源：http://jg.jianghongdianzi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bf.chemitech.net.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://my.szxytkj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gm.yuexingan06.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jz.yuexingan06.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kt.wgjwhj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://il.lnxyls.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qy.gzmigu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ax.jctech888.com.cn

[E15] HTML 转义 / 反转义
来源：http://hh.nszjky.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://zk.muxihuayi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mr.hnjuh.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fc.jctech888.com.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://if.muxihuayi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fk.9csxet.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qi.asd995.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://og.shtwfgs.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bp.nicolike.cn

[E16] 数字千分位
来源：http://gy.shxzskj.cn

Py:   f"{1234567:,}"
来源：http://rl.panjiajie.cn

PHP:  number_format(1234567);
来源：http://fr.gzmigu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://jp.shxzukj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://pn.gzmigu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sj.haigaiapp.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jx.newstarts.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hj.haigaiapp.cn

C#:   1234567.ToString("N0")
来源：http://ia.gzmigu.cn

[E17] 首字母大写
来源：http://vm.huixiangedu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cv.shxzskj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://uk.panjiajie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zq.jianghongdianzi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rt.yuntaijiaju.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bs.hahajie.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vh.huanxung.cn

Ruby: s.capitalize
来源：http://eo.jctech888.com.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hp.shxzskj.cn

[E18] 模板占位符替换
来源：http://uv.nicolike.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ne.chemitech.net.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zu.newstarts.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://iz.9csxet.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ee.521024.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://do.521024.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lt.jctech888.com.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pr.szsharing.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yw.szxytkj.cn

[E19] 多行文本按行拆分
来源：http://qd.shxzskj.cn

Py:   s.splitlines()
来源：http://jo.szsharing.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hd.bookmarksfly.cn

JS:   s.split(/\r?\n/)
来源：http://tm.chemitech.net.cn

TS:   s.split(/\r?\n/)
来源：http://pf.shxzskj.cn

Java: s.lines().toList()
来源：http://on.huixiangedu.cn

Go:   strings.Split(s, "\n")
来源：http://pp.yuntaijiaju.cn

Ruby: s.lines
来源：http://fd.colortex.cn

C#:   s.Split('\n')
来源：http://cz.huanxung.cn

[E20] 判断字符串是否为空
来源：http://cd.bookmarksfly.cn

Py:   if not s:
来源：http://lx.huixinmuqiang.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xc.bookmarksfly.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pt.newstarts.cn

TS:   if (s === "") {}
来源：http://im.bookmarksfly.cn

Java: if (s.isEmpty()) {}
来源：http://cp.bookmarksfly.cn

Go:   if s == "" {}
来源：http://px.hahajie.cn

Ruby: if s.empty?
来源：http://hf.szxytkj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://th.shxzskj.cn

[E21] 超长截断加省略号
来源：http://op.huixiangedu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://uy.gzmigu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cg.9csxet.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cn.bjjhwx.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cm.huixiangedu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gw.wgjwhj.cn

Go:   // 按 rune 判断长度后截断
来源：http://ey.jctech888.com.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ns.hnjuh.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://si.colortex.cn

[E22] 字节长度与字符长度
来源：http://qc.bjjhwx.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ol.shxzskj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gd.521024.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vf.huanxung.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ji.jctech888.com.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ld.hahajie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ie.szsharing.cn

Ruby: s.bytesize;  s.length
来源：http://hk.521024.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hf.wgjwhj.cn

================================================================================
来源：http://li.newstarts.cn

F. 文件与目录
来源：http://ic.shtwfgs.cn

================================================================================
来源：http://kr.nicolike.cn

[F01] 读取整个文件
来源：http://tl.haigaiapp.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ez.huixiangedu.cn

PHP:  file_get_contents("a.txt");
来源：http://cw.shxzskj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gl.huixinmuqiang.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vc.jianghongdianzi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://nj.nicolike.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yn.yuexingan06.cn

Ruby: File.read("a.txt")
来源：http://jz.lnxyls.cn

C#:   File.ReadAllText("a.txt");
来源：http://bv.hahajie.cn

[F02] 逐行读取文件
来源：http://gj.shtwfgs.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qv.shxzskj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cu.hnjuh.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://se.yuntaijiaju.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hx.bookmarksfly.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uh.shtwfgs.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lq.panjiajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://li.bookmarksfly.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://am.shtwfgs.cn

[F03] 写入文件（覆盖）
来源：http://kz.jctech888.com.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cu.colortex.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ck.yuntaijiaju.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mg.jctech888.com.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cw.nszjky.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rt.lnxyls.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ca.newstarts.cn

Ruby: File.write("a.txt", "hi")
来源：http://kq.jctech888.com.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vw.asd995.cn

[F04] 追加写入文件
来源：http://uj.521024.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hx.chemitech.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zz.lnxyls.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hq.nicolike.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kp.hnjuh.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bq.521024.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pc.nicolike.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jk.yuexingan06.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vn.muxihuayi.cn

[F05] 判断文件或目录是否存在
来源：http://pd.bjjhwx.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://by.jianghongdianzi.cn

PHP:  file_exists("a.txt");
来源：http://ac.yuntaijiaju.cn

JS:   fs.existsSync("a.txt")
来源：http://mm.szxytkj.cn

TS:   fs.existsSync("a.txt")
来源：http://jz.shtwfgs.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://mo.szxytkj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://iu.lnxyls.cn

Ruby: File.exist?("a.txt")
来源：http://am.bookmarksfly.cn

C#:   File.Exists("a.txt")
来源：http://qa.wgjwhj.cn

[F06] 删除文件
来源：http://vg.lnxyls.cn

Py:   os.remove("a.txt")
来源：http://xg.9csxet.cn

PHP:  unlink("a.txt");
来源：http://dp.bookmarksfly.cn

JS:   fs.unlinkSync("a.txt")
来源：http://lu.wgjwhj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://gq.yuexingan06.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xv.shxzukj.cn

Go:   os.Remove("a.txt")
来源：http://kn.shtwfgs.cn

Ruby: File.delete("a.txt")
来源：http://fj.hnjuh.cn

C#:   File.Delete("a.txt");
来源：http://mj.9csxet.cn

[F07] 创建目录（含多级）
来源：http://jl.haigaiapp.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ow.szsharing.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://oc.nicolike.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xp.asd995.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wl.9csxet.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wu.hnjuh.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ee.asd995.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gm.yuexingan06.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://za.nszjky.cn

[F08] 遍历目录
来源：http://jz.panjiajie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://hw.shtwfgs.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dy.bookmarksfly.cn

JS:   fs.readdirSync("dir")
来源：http://xv.gzmigu.cn

TS:   fs.readdirSync("dir")
来源：http://yt.szsharing.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ta.hnjuh.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://yw.bookmarksfly.cn

Ruby: Dir.children("dir")
来源：http://tu.lnxyls.cn

C#:   Directory.GetFiles("dir")
来源：http://sv.szsharing.cn

[F09] 获取文件大小
来源：http://uv.shxzskj.cn

Py:   os.path.getsize("a.txt")
来源：http://vc.bookmarksfly.cn

PHP:  filesize("a.txt");
来源：http://ti.asd995.cn

JS:   fs.statSync("a.txt").size
来源：http://nw.huanxung.cn

TS:   fs.statSync("a.txt").size
来源：http://ts.huanxung.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ei.szxytkj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vt.bookmarksfly.cn

Ruby: File.size("a.txt")
来源：http://av.bookmarksfly.cn

C#:   new FileInfo("a.txt").Length
来源：http://bh.jianghongdianzi.cn

[F10] 取文件扩展名 / 文件名
来源：http://qc.hnjuh.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dm.gzmigu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://za.haigaiapp.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vo.panjiajie.cn

TS:   path.extname("a.txt")
来源：http://mk.hahajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fs.szxytkj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wn.lnxyls.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.nszjky.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://oq.huixinmuqiang.cn

[F11] 复制与移动文件
来源：http://dk.bjjhwx.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fd.shxzskj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lp.gzmigu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qv.hahajie.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kz.asd995.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zh.szxytkj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://co.yuntaijiaju.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ok.hnjuh.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zy.wgjwhj.cn

[F12] CSV 读写
来源：http://kt.muxihuayi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qt.hahajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vc.huixiangedu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tk.szsharing.cn

TS:   // 同上
来源：http://qe.szsharing.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yd.yuntaijiaju.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yz.nszjky.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bt.haigaiapp.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gf.newstarts.cn

================================================================================
来源：http://fi.nicolike.cn

G. 面向对象
来源：http://fb.colortex.cn

================================================================================
来源：http://rp.jianghongdianzi.cn

[G01] 定义类
来源：http://uf.asd995.cn

Py:   class User: pass
来源：http://gp.colortex.cn

PHP:  class User {}
来源：http://lz.shxzukj.cn

JS:   class User {}
来源：http://sh.panjiajie.cn

TS:   class User { name: string = ""; }
来源：http://oi.bookmarksfly.cn

Java: class User {}
来源：http://ra.muxihuayi.cn

Go:   type User struct { Name string }
来源：http://zd.bookmarksfly.cn

Ruby: class User; end
来源：http://fd.bookmarksfly.cn

C#:   class User {}
来源：http://jl.lnxyls.cn

[G02] 构造函数
来源：http://ce.shxzskj.cn

Py:   def __init__(self, name): self.name = name
来源：http://ek.bjjhwx.cn

PHP:  public function __construct(public string $name) {}
来源：http://af.yuntaijiaju.cn

JS:   constructor(name) { this.name = name; }
来源：http://qj.shtwfgs.cn


<!-- 参考信息 -->