代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://js.asd995.cn

[E03] 截取子串
来源：http://lp.panjiajie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lj.shtwfgs.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zv.szsharing.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gt.shtwfgs.cn

TS:   s.slice(1, 4)
来源：http://jy.newstarts.cn

Java: s.substring(1, 4)
来源：http://sg.521024.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sc.9csxet.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ta.szsharing.cn

C#:   s.Substring(1, 3)
来源：http://br.panjiajie.cn

[E04] 查找子串位置
来源：http://mf.jctech888.com.cn

Py:   s.find("x");  s.index("x")
来源：http://nw.jctech888.com.cn

PHP:  strpos($s, "x");
来源：http://qn.9csxet.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vz.haigaiapp.cn

TS:   s.indexOf("x")
来源：http://st.huixinmuqiang.cn

Java: s.indexOf("x")
来源：http://mx.yuexingan06.cn

Go:   strings.Index(s, "x")
来源：http://is.gzmigu.cn

Ruby: s.index("x")
来源：http://va.gzmigu.cn

C#:   s.IndexOf("x")
来源：http://eq.huanxung.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://em.bjjhwx.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ge.muxihuayi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sh.jctech888.com.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://aj.huixinmuqiang.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://sj.shtwfgs.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vb.nszjky.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zv.yuexingan06.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zk.jctech888.com.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://un.shtwfgs.cn

[E06] 替换子串
来源：http://lg.jctech888.com.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ke.szsharing.cn

PHP:  str_replace("a", "b", $s);
来源：http://bb.lnxyls.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gt.9csxet.cn

TS:   s.replaceAll("a", "b")
来源：http://mp.yuexingan06.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yi.gzmigu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ya.jianghongdianzi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://et.chemitech.net.cn

C#:   s.Replace("a", "b")
来源：http://yn.haigaiapp.cn

[E07] 按分隔符拆分
来源：http://zm.gzmigu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wu.hnjuh.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ka.panjiajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://pg.hnjuh.cn

TS:   s.split(",")
来源：http://xh.shxzukj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://yo.shxzukj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nz.haigaiapp.cn

Ruby: s.split(",");  s.split
来源：http://mi.jianghongdianzi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nz.huanxung.cn

[E08] 数组按分隔符合并
来源：http://tn.nszjky.cn

Py:   ",".join(items)
来源：http://py.szxytkj.cn

PHP:  implode(",", $items);
来源：http://ve.asd995.cn

JS:   items.join(",")
来源：http://qu.jianghongdianzi.cn

TS:   items.join(",")
来源：http://wk.szxytkj.cn

Java: String.join(",", items)
来源：http://fp.newstarts.cn

Go:   strings.Join(items, ",")
来源：http://ep.shxzskj.cn

Ruby: items.join(",")
来源：http://mm.panjiajie.cn

C#:   string.Join(",", items)
来源：http://mp.szxytkj.cn

[E09] 去除所有空白字符
来源：http://qk.panjiajie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lp.nszjky.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ea.chemitech.net.cn

JS:   s.replace(/\s+/g, "")
来源：http://jq.huixinmuqiang.cn

TS:   s.replace(/\s+/g, "")
来源：http://lz.hnjuh.cn

Java: s.replaceAll("\\s+", "")
来源：http://mt.huixinmuqiang.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://fg.shxzskj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://za.szxytkj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ut.hahajie.cn

[E10] 左侧补零 / 定长填充
来源：http://ys.panjiajie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zz.huixiangedu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vv.lnxyls.cn

JS:   "7".padStart(3, "0")
来源：http://xd.9csxet.cn

TS:   "7".padStart(3, "0")
来源：http://wq.shtwfgs.cn

Java: String.format("%03d", 7)
来源：http://nz.panjiajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ou.hnjuh.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rn.asd995.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ed.jianghongdianzi.cn

[E11] 反转字符串
来源：http://tr.hahajie.cn

Py:   s[::-1]
来源：http://zd.shxzskj.cn

PHP:  strrev($s);
来源：http://qc.colortex.cn

JS:   [...s].reverse().join("")
来源：http://ck.haigaiapp.cn

TS:   [...s].reverse().join("")
来源：http://nh.panjiajie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://tp.huixiangedu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://fd.huixiangedu.cn

Ruby: s.reverse
来源：http://ls.hnjuh.cn

C#:   new string(s.Reverse().ToArray())
来源：http://cm.nicolike.cn

[E12] 统计某字符出现次数
来源：http://tc.shxzskj.cn

Py:   s.count("a")
来源：http://oj.hahajie.cn

PHP:  substr_count($s, "a");
来源：http://es.lnxyls.cn

JS:   s.split("a").length - 1
来源：http://rc.9csxet.cn

TS:   s.split("a").length - 1
来源：http://xf.shxzskj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ip.hahajie.cn

Go:   strings.Count(s, "a")
来源：http://eh.panjiajie.cn

Ruby: s.count("a")
来源：http://zp.lnxyls.cn

C#:   s.Count(c => c == 'a')
来源：http://ji.newstarts.cn

[E13] 逐字符遍历
来源：http://il.hnjuh.cn

Py:   for ch in s: print(ch)
来源：http://vm.haigaiapp.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jl.shxzukj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ri.hahajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://zi.yuntaijiaju.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pz.9csxet.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jp.shxzskj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://bq.yuexingan06.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lr.yuexingan06.cn

[E14] URL 编码与 Base64
来源：http://zh.haigaiapp.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hk.newstarts.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://sg.521024.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kz.bookmarksfly.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ob.chemitech.net.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zk.panjiajie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pg.bjjhwx.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zs.jianghongdianzi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ia.yuntaijiaju.cn

[E15] HTML 转义 / 反转义
来源：http://nz.newstarts.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://oo.haigaiapp.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gb.lnxyls.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ls.nicolike.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://bz.szxytkj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fq.asd995.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sh.shxzukj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cz.yuexingan06.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://td.shxzukj.cn

[E16] 数字千分位
来源：http://dk.521024.cn

Py:   f"{1234567:,}"
来源：http://ru.newstarts.cn

PHP:  number_format(1234567);
来源：http://pr.nicolike.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://lp.hahajie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ii.chemitech.net.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://th.wgjwhj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rx.9csxet.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://aa.wgjwhj.cn

C#:   1234567.ToString("N0")
来源：http://pu.szxytkj.cn

[E17] 首字母大写
来源：http://rm.nicolike.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://em.muxihuayi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ig.panjiajie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rp.bjjhwx.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qi.newstarts.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vq.chemitech.net.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ez.shtwfgs.cn

Ruby: s.capitalize
来源：http://bu.newstarts.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xv.yuexingan06.cn

[E18] 模板占位符替换
来源：http://me.jctech888.com.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uq.szsharing.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jh.hnjuh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ud.bookmarksfly.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ne.jianghongdianzi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://df.jctech888.com.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://az.gzmigu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ni.szsharing.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ph.huixiangedu.cn

[E19] 多行文本按行拆分
来源：http://lu.panjiajie.cn

Py:   s.splitlines()
来源：http://rz.bjjhwx.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qw.wgjwhj.cn

JS:   s.split(/\r?\n/)
来源：http://kj.hnjuh.cn

TS:   s.split(/\r?\n/)
来源：http://bv.muxihuayi.cn

Java: s.lines().toList()
来源：http://hf.nicolike.cn

Go:   strings.Split(s, "\n")
来源：http://hk.chemitech.net.cn

Ruby: s.lines
来源：http://cd.gzmigu.cn

C#:   s.Split('\n')
来源：http://en.nszjky.cn

[E20] 判断字符串是否为空
来源：http://vz.panjiajie.cn

Py:   if not s:
来源：http://hz.newstarts.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://uv.9csxet.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vs.szxytkj.cn

TS:   if (s === "") {}
来源：http://xv.szxytkj.cn

Java: if (s.isEmpty()) {}
来源：http://md.chemitech.net.cn

Go:   if s == "" {}
来源：http://qq.szsharing.cn

Ruby: if s.empty?
来源：http://pf.bookmarksfly.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sn.muxihuayi.cn

[E21] 超长截断加省略号
来源：http://tc.wgjwhj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hc.chemitech.net.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://oc.yuntaijiaju.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bb.521024.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mt.muxihuayi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://uj.colortex.cn

Go:   // 按 rune 判断长度后截断
来源：http://jg.szxytkj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pe.szxytkj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wf.bookmarksfly.cn

[E22] 字节长度与字符长度
来源：http://nv.asd995.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qu.panjiajie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rw.newstarts.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gw.hnjuh.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zd.bookmarksfly.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kb.asd995.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mf.shxzukj.cn

Ruby: s.bytesize;  s.length
来源：http://xv.szsharing.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qb.yuexingan06.cn

================================================================================
来源：http://qx.bookmarksfly.cn

F. 文件与目录
来源：http://ur.bookmarksfly.cn

================================================================================
来源：http://kp.gzmigu.cn

[F01] 读取整个文件
来源：http://li.shxzskj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ho.colortex.cn

PHP:  file_get_contents("a.txt");
来源：http://zk.gzmigu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ye.hahajie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mj.yuntaijiaju.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://or.nszjky.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://oo.shxzukj.cn

Ruby: File.read("a.txt")
来源：http://wx.yuntaijiaju.cn

C#:   File.ReadAllText("a.txt");
来源：http://fu.jctech888.com.cn

[F02] 逐行读取文件
来源：http://yb.shxzskj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gi.shtwfgs.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ry.nicolike.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ek.szxytkj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rc.9csxet.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nf.szsharing.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ht.asd995.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ax.yuntaijiaju.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yv.hahajie.cn

[F03] 写入文件（覆盖）
来源：http://wd.panjiajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lp.szxytkj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://iw.lnxyls.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://us.shxzukj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mx.asd995.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dj.chemitech.net.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pw.asd995.cn

Ruby: File.write("a.txt", "hi")
来源：http://bi.jianghongdianzi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xj.szxytkj.cn

[F04] 追加写入文件
来源：http://fb.hnjuh.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kz.hnjuh.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mu.huanxung.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ul.9csxet.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hl.nicolike.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sj.hnjuh.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wh.huanxung.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hj.asd995.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sy.huixiangedu.cn

[F05] 判断文件或目录是否存在
来源：http://jy.9csxet.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ec.shxzukj.cn

PHP:  file_exists("a.txt");
来源：http://dv.bookmarksfly.cn

JS:   fs.existsSync("a.txt")
来源：http://ww.nszjky.cn

TS:   fs.existsSync("a.txt")
来源：http://kp.newstarts.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://jj.szsharing.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bk.yuntaijiaju.cn

Ruby: File.exist?("a.txt")
来源：http://ni.asd995.cn

C#:   File.Exists("a.txt")
来源：http://co.bookmarksfly.cn

[F06] 删除文件
来源：http://tt.huixiangedu.cn

Py:   os.remove("a.txt")
来源：http://xg.hahajie.cn

PHP:  unlink("a.txt");
来源：http://ul.lnxyls.cn

JS:   fs.unlinkSync("a.txt")
来源：http://tb.shtwfgs.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ne.huixinmuqiang.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xy.shtwfgs.cn

Go:   os.Remove("a.txt")
来源：http://xj.colortex.cn

Ruby: File.delete("a.txt")
来源：http://lz.asd995.cn

C#:   File.Delete("a.txt");
来源：http://ha.huixinmuqiang.cn

[F07] 创建目录（含多级）
来源：http://dg.nicolike.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fb.chemitech.net.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pt.hnjuh.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://th.huanxung.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://td.asd995.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ru.hnjuh.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pv.muxihuayi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zg.newstarts.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://og.yuntaijiaju.cn

[F08] 遍历目录
来源：http://dg.shxzskj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://iy.szsharing.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://aj.chemitech.net.cn

JS:   fs.readdirSync("dir")
来源：http://yu.gzmigu.cn

TS:   fs.readdirSync("dir")
来源：http://fr.hahajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tt.asd995.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://or.huixinmuqiang.cn

Ruby: Dir.children("dir")
来源：http://nr.asd995.cn

C#:   Directory.GetFiles("dir")
来源：http://zj.colortex.cn

[F09] 获取文件大小
来源：http://oh.yuexingan06.cn

Py:   os.path.getsize("a.txt")
来源：http://ja.gzmigu.cn

PHP:  filesize("a.txt");
来源：http://rf.jianghongdianzi.cn

JS:   fs.statSync("a.txt").size
来源：http://rx.9csxet.cn

TS:   fs.statSync("a.txt").size
来源：http://id.haigaiapp.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ch.shxzukj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qc.hahajie.cn

Ruby: File.size("a.txt")
来源：http://ci.haigaiapp.cn

C#:   new FileInfo("a.txt").Length
来源：http://zq.panjiajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://js.wgjwhj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fs.hahajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vk.huixiangedu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ur.asd995.cn

TS:   path.extname("a.txt")
来源：http://lk.newstarts.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://od.9csxet.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tw.yuntaijiaju.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://at.gzmigu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hh.hahajie.cn

[F11] 复制与移动文件
来源：http://hm.szxytkj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://de.panjiajie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rv.hnjuh.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sq.haigaiapp.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ca.yuntaijiaju.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yf.szxytkj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bp.panjiajie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yg.9csxet.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jz.shxzukj.cn

[F12] CSV 读写
来源：http://wb.chemitech.net.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bc.huixinmuqiang.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vz.hahajie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://uz.newstarts.cn

TS:   // 同上
来源：http://zo.jianghongdianzi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vv.asd995.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rl.shtwfgs.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://re.panjiajie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://xj.huixiangedu.cn

================================================================================
来源：http://ic.wgjwhj.cn

G. 面向对象
来源：http://at.shtwfgs.cn

================================================================================
来源：http://im.panjiajie.cn

[G01] 定义类
来源：http://cz.jctech888.com.cn

Py:   class User: pass
来源：http://oe.bjjhwx.cn

PHP:  class User {}
来源：http://xs.panjiajie.cn

JS:   class User {}
来源：http://wy.huixinmuqiang.cn

TS:   class User { name: string = ""; }
来源：http://cb.nicolike.cn


<!-- 参考信息 -->