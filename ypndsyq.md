代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://uj.nicolike.cn

TS:   s.slice(1, 4)
来源：http://kn.nicolike.cn

Java: s.substring(1, 4)
来源：http://ho.jianghongdianzi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ar.muxihuayi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://gm.hnjuh.cn

C#:   s.Substring(1, 3)
来源：http://of.9csxet.cn

[E04] 查找子串位置
来源：http://ca.shtwfgs.cn

Py:   s.find("x");  s.index("x")
来源：http://rn.shxzukj.cn

PHP:  strpos($s, "x");
来源：http://od.9csxet.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sb.shtwfgs.cn

TS:   s.indexOf("x")
来源：http://ak.szxytkj.cn

Java: s.indexOf("x")
来源：http://ub.szsharing.cn

Go:   strings.Index(s, "x")
来源：http://vb.shtwfgs.cn

Ruby: s.index("x")
来源：http://dj.shtwfgs.cn

C#:   s.IndexOf("x")
来源：http://gx.shxzskj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://cl.huanxung.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bf.gzmigu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nx.hnjuh.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://iv.huixiangedu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://dp.chemitech.net.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ch.jianghongdianzi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jt.gzmigu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://od.huanxung.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xg.shtwfgs.cn

[E06] 替换子串
来源：http://ow.hahajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zh.yuexingan06.cn

PHP:  str_replace("a", "b", $s);
来源：http://cd.nszjky.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sb.huanxung.cn

TS:   s.replaceAll("a", "b")
来源：http://zl.hnjuh.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ru.chemitech.net.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bn.nszjky.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wl.yuexingan06.cn

C#:   s.Replace("a", "b")
来源：http://zy.bjjhwx.cn

[E07] 按分隔符拆分
来源：http://bf.haigaiapp.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sn.nszjky.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kb.9csxet.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ff.huanxung.cn

TS:   s.split(",")
来源：http://dx.panjiajie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://sa.521024.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xt.newstarts.cn

Ruby: s.split(",");  s.split
来源：http://tv.wgjwhj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xm.szxytkj.cn

[E08] 数组按分隔符合并
来源：http://tv.nszjky.cn

Py:   ",".join(items)
来源：http://tm.huixinmuqiang.cn

PHP:  implode(",", $items);
来源：http://tl.521024.cn

JS:   items.join(",")
来源：http://fo.huixinmuqiang.cn

TS:   items.join(",")
来源：http://ns.yuntaijiaju.cn

Java: String.join(",", items)
来源：http://yy.muxihuayi.cn

Go:   strings.Join(items, ",")
来源：http://qi.jctech888.com.cn

Ruby: items.join(",")
来源：http://xa.yuexingan06.cn

C#:   string.Join(",", items)
来源：http://lt.haigaiapp.cn

[E09] 去除所有空白字符
来源：http://hq.huixiangedu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lg.panjiajie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cn.asd995.cn

JS:   s.replace(/\s+/g, "")
来源：http://gm.shxzukj.cn

TS:   s.replace(/\s+/g, "")
来源：http://qm.gzmigu.cn

Java: s.replaceAll("\\s+", "")
来源：http://ay.colortex.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://sl.gzmigu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://pc.szxytkj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zt.521024.cn

[E10] 左侧补零 / 定长填充
来源：http://kp.nszjky.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gx.jianghongdianzi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://do.szsharing.cn

JS:   "7".padStart(3, "0")
来源：http://ep.bjjhwx.cn

TS:   "7".padStart(3, "0")
来源：http://bb.nszjky.cn

Java: String.format("%03d", 7)
来源：http://cv.bjjhwx.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://dl.szsharing.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rb.jctech888.com.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qc.lnxyls.cn

[E11] 反转字符串
来源：http://ak.hahajie.cn

Py:   s[::-1]
来源：http://fe.gzmigu.cn

PHP:  strrev($s);
来源：http://of.asd995.cn

JS:   [...s].reverse().join("")
来源：http://rl.yuexingan06.cn

TS:   [...s].reverse().join("")
来源：http://pb.wgjwhj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://lj.muxihuayi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://oc.chemitech.net.cn

Ruby: s.reverse
来源：http://zv.jianghongdianzi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://cy.huixinmuqiang.cn

[E12] 统计某字符出现次数
来源：http://gl.asd995.cn

Py:   s.count("a")
来源：http://df.chemitech.net.cn

PHP:  substr_count($s, "a");
来源：http://gj.yuntaijiaju.cn

JS:   s.split("a").length - 1
来源：http://xy.huixiangedu.cn

TS:   s.split("a").length - 1
来源：http://rd.9csxet.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yy.huanxung.cn

Go:   strings.Count(s, "a")
来源：http://wx.nszjky.cn

Ruby: s.count("a")
来源：http://zj.huanxung.cn

C#:   s.Count(c => c == 'a')
来源：http://yd.chemitech.net.cn

[E13] 逐字符遍历
来源：http://og.colortex.cn

Py:   for ch in s: print(ch)
来源：http://qv.bjjhwx.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jo.nszjky.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ht.lnxyls.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://zi.colortex.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bi.wgjwhj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nd.nicolike.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://oy.muxihuayi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ji.huixiangedu.cn

[E14] URL 编码与 Base64
来源：http://ou.hnjuh.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://iy.asd995.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://sh.jianghongdianzi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ya.lnxyls.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pc.shxzukj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lm.yuexingan06.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rh.szxytkj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vh.yuntaijiaju.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yl.yuexingan06.cn

[E15] HTML 转义 / 反转义
来源：http://oh.szsharing.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://nw.jctech888.com.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pa.hnjuh.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nd.gzmigu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://qm.9csxet.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://nw.newstarts.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bm.muxihuayi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zp.huixiangedu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xq.colortex.cn

[E16] 数字千分位
来源：http://rv.521024.cn

Py:   f"{1234567:,}"
来源：http://rd.haigaiapp.cn

PHP:  number_format(1234567);
来源：http://kj.szxytkj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://dh.newstarts.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://gg.9csxet.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qx.bookmarksfly.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ix.szsharing.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://uq.bjjhwx.cn

C#:   1234567.ToString("N0")
来源：http://mk.shxzskj.cn

[E17] 首字母大写
来源：http://by.haigaiapp.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lt.chemitech.net.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://km.huixiangedu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://es.colortex.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fp.panjiajie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sp.huanxung.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nn.panjiajie.cn

Ruby: s.capitalize
来源：http://to.521024.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ft.gzmigu.cn

[E18] 模板占位符替换
来源：http://qe.panjiajie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://eb.huanxung.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://no.hnjuh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://gl.yuntaijiaju.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ji.bookmarksfly.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://an.panjiajie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ic.huixinmuqiang.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wg.yuntaijiaju.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zz.hnjuh.cn

[E19] 多行文本按行拆分
来源：http://wu.chemitech.net.cn

Py:   s.splitlines()
来源：http://ss.gzmigu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dm.9csxet.cn

JS:   s.split(/\r?\n/)
来源：http://ck.asd995.cn

TS:   s.split(/\r?\n/)
来源：http://ap.lnxyls.cn

Java: s.lines().toList()
来源：http://fc.chemitech.net.cn

Go:   strings.Split(s, "\n")
来源：http://pq.chemitech.net.cn

Ruby: s.lines
来源：http://aq.szsharing.cn

C#:   s.Split('\n')
来源：http://pp.huixinmuqiang.cn

[E20] 判断字符串是否为空
来源：http://jy.szxytkj.cn

Py:   if not s:
来源：http://ty.wgjwhj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rg.shxzukj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ks.wgjwhj.cn

TS:   if (s === "") {}
来源：http://qc.bjjhwx.cn

Java: if (s.isEmpty()) {}
来源：http://xr.nszjky.cn

Go:   if s == "" {}
来源：http://zx.yuexingan06.cn

Ruby: if s.empty?
来源：http://pk.colortex.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bu.chemitech.net.cn

[E21] 超长截断加省略号
来源：http://zc.hahajie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bi.shxzskj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cf.521024.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lo.huixinmuqiang.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mr.hnjuh.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xl.bjjhwx.cn

Go:   // 按 rune 判断长度后截断
来源：http://qf.chemitech.net.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lx.huixiangedu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://js.haigaiapp.cn

[E22] 字节长度与字符长度
来源：http://th.yuexingan06.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hw.hnjuh.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ix.521024.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://sd.shxzskj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mx.9csxet.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yy.nszjky.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://et.yuexingan06.cn

Ruby: s.bytesize;  s.length
来源：http://nd.panjiajie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bn.szxytkj.cn

================================================================================
来源：http://zi.huixiangedu.cn

F. 文件与目录
来源：http://vf.bookmarksfly.cn

================================================================================
来源：http://jo.nicolike.cn

[F01] 读取整个文件
来源：http://kb.jctech888.com.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fm.hnjuh.cn

PHP:  file_get_contents("a.txt");
来源：http://af.nicolike.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tk.yuexingan06.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gm.newstarts.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hn.9csxet.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fb.muxihuayi.cn

Ruby: File.read("a.txt")
来源：http://mf.shxzukj.cn

C#:   File.ReadAllText("a.txt");
来源：http://as.hahajie.cn

[F02] 逐行读取文件
来源：http://me.jianghongdianzi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rq.lnxyls.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vv.yuntaijiaju.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nt.huixinmuqiang.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fh.lnxyls.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qw.huixinmuqiang.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ln.haigaiapp.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://go.wgjwhj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ok.nicolike.cn

[F03] 写入文件（覆盖）
来源：http://ua.9csxet.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ky.colortex.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://bn.colortex.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qb.szsharing.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kc.hnjuh.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rb.huixinmuqiang.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xs.szsharing.cn

Ruby: File.write("a.txt", "hi")
来源：http://jl.colortex.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cq.nicolike.cn

[F04] 追加写入文件
来源：http://jf.jctech888.com.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zr.jianghongdianzi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ct.wgjwhj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xh.huanxung.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cr.hahajie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yi.newstarts.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jg.jianghongdianzi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fh.colortex.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ma.szxytkj.cn

[F05] 判断文件或目录是否存在
来源：http://su.521024.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kg.jianghongdianzi.cn

PHP:  file_exists("a.txt");
来源：http://wq.9csxet.cn

JS:   fs.existsSync("a.txt")
来源：http://yq.hnjuh.cn

TS:   fs.existsSync("a.txt")
来源：http://sl.asd995.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://dg.wgjwhj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qb.huanxung.cn

Ruby: File.exist?("a.txt")
来源：http://yi.lnxyls.cn

C#:   File.Exists("a.txt")
来源：http://qm.nicolike.cn

[F06] 删除文件
来源：http://hf.szxytkj.cn

Py:   os.remove("a.txt")
来源：http://uc.shtwfgs.cn

PHP:  unlink("a.txt");
来源：http://dg.newstarts.cn

JS:   fs.unlinkSync("a.txt")
来源：http://qu.hahajie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://rm.bookmarksfly.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://oa.shxzskj.cn

Go:   os.Remove("a.txt")
来源：http://ko.huanxung.cn

Ruby: File.delete("a.txt")
来源：http://ip.newstarts.cn

C#:   File.Delete("a.txt");
来源：http://ns.huanxung.cn

[F07] 创建目录（含多级）
来源：http://wt.huixiangedu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dr.hnjuh.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ln.521024.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wt.shxzukj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lb.newstarts.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nc.jianghongdianzi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lp.hahajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kh.jctech888.com.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jj.shxzskj.cn

[F08] 遍历目录
来源：http://sy.muxihuayi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://yv.wgjwhj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jw.szsharing.cn

JS:   fs.readdirSync("dir")
来源：http://at.szxytkj.cn

TS:   fs.readdirSync("dir")
来源：http://tm.lnxyls.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qz.jctech888.com.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://oy.jctech888.com.cn

Ruby: Dir.children("dir")
来源：http://rx.asd995.cn

C#:   Directory.GetFiles("dir")
来源：http://dv.lnxyls.cn

[F09] 获取文件大小
来源：http://ek.colortex.cn

Py:   os.path.getsize("a.txt")
来源：http://hd.huanxung.cn

PHP:  filesize("a.txt");
来源：http://ui.gzmigu.cn

JS:   fs.statSync("a.txt").size
来源：http://gv.nszjky.cn

TS:   fs.statSync("a.txt").size
来源：http://my.szsharing.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ym.9csxet.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ab.colortex.cn

Ruby: File.size("a.txt")
来源：http://uh.huanxung.cn

C#:   new FileInfo("a.txt").Length
来源：http://wm.shxzukj.cn

[F10] 取文件扩展名 / 文件名
来源：http://py.hahajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fn.huixiangedu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://iw.colortex.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mc.jianghongdianzi.cn

TS:   path.extname("a.txt")
来源：http://mf.yuexingan06.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yg.jctech888.com.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cx.bookmarksfly.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://uf.shxzukj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yl.nszjky.cn

[F11] 复制与移动文件
来源：http://ic.huixiangedu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mg.szsharing.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bd.jctech888.com.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://od.jctech888.com.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ad.bjjhwx.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xb.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zb.nicolike.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ym.yuntaijiaju.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nv.jctech888.com.cn

[F12] CSV 读写
来源：http://zv.newstarts.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vv.newstarts.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cq.muxihuayi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ec.huixiangedu.cn

TS:   // 同上
来源：http://co.haigaiapp.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dg.9csxet.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lq.huixinmuqiang.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ny.panjiajie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ne.gzmigu.cn

================================================================================
来源：http://cm.szsharing.cn

G. 面向对象
来源：http://qr.shxzskj.cn

================================================================================
来源：http://qx.hahajie.cn

[G01] 定义类
来源：http://yy.yuexingan06.cn

Py:   class User: pass
来源：http://ro.nicolike.cn

PHP:  class User {}
来源：http://tz.9csxet.cn

JS:   class User {}
来源：http://fe.huixinmuqiang.cn

TS:   class User { name: string = ""; }
来源：http://vc.9csxet.cn

Java: class User {}
来源：http://pv.shxzukj.cn

Go:   type User struct { Name string }
来源：http://dt.panjiajie.cn

Ruby: class User; end
来源：http://yp.shxzskj.cn

C#:   class User {}
来源：http://uv.hahajie.cn


<!-- 参考信息 -->