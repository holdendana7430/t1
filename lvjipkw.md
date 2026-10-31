代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://er.shxzskj.cn

C#:   s.Substring(1, 3)
来源：http://rq.yuntaijiaju.cn

[E04] 查找子串位置
来源：http://jo.bookmarksfly.cn

Py:   s.find("x");  s.index("x")
来源：http://kr.haigaiapp.cn

PHP:  strpos($s, "x");
来源：http://st.hahajie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ju.newstarts.cn

TS:   s.indexOf("x")
来源：http://ct.shxzskj.cn

Java: s.indexOf("x")
来源：http://qb.bjjhwx.cn

Go:   strings.Index(s, "x")
来源：http://ki.szxytkj.cn

Ruby: s.index("x")
来源：http://jg.colortex.cn

C#:   s.IndexOf("x")
来源：http://nn.huixiangedu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://lb.szsharing.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jo.shtwfgs.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kw.wgjwhj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ug.bjjhwx.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://el.haigaiapp.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://am.gzmigu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ye.yuntaijiaju.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zr.shxzskj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ss.muxihuayi.cn

[E06] 替换子串
来源：http://mf.panjiajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wk.newstarts.cn

PHP:  str_replace("a", "b", $s);
来源：http://pe.hahajie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mz.colortex.cn

TS:   s.replaceAll("a", "b")
来源：http://cs.wgjwhj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://is.panjiajie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cd.haigaiapp.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://se.huixinmuqiang.cn

C#:   s.Replace("a", "b")
来源：http://dr.bjjhwx.cn

[E07] 按分隔符拆分
来源：http://re.chemitech.net.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://es.hnjuh.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://uf.jianghongdianzi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://pl.yuntaijiaju.cn

TS:   s.split(",")
来源：http://yf.9csxet.cn

Java: s.split(",");  s.split("\\s+")
来源：http://bb.wgjwhj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vj.huanxung.cn

Ruby: s.split(",");  s.split
来源：http://je.szsharing.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qt.wgjwhj.cn

[E08] 数组按分隔符合并
来源：http://qa.shxzskj.cn

Py:   ",".join(items)
来源：http://ka.chemitech.net.cn

PHP:  implode(",", $items);
来源：http://it.huanxung.cn

JS:   items.join(",")
来源：http://er.hahajie.cn

TS:   items.join(",")
来源：http://ct.muxihuayi.cn

Java: String.join(",", items)
来源：http://dp.muxihuayi.cn

Go:   strings.Join(items, ",")
来源：http://es.newstarts.cn

Ruby: items.join(",")
来源：http://xd.hahajie.cn

C#:   string.Join(",", items)
来源：http://wg.szxytkj.cn

[E09] 去除所有空白字符
来源：http://iq.shtwfgs.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ox.chemitech.net.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qh.huixinmuqiang.cn

JS:   s.replace(/\s+/g, "")
来源：http://kf.bjjhwx.cn

TS:   s.replace(/\s+/g, "")
来源：http://nj.wgjwhj.cn

Java: s.replaceAll("\\s+", "")
来源：http://wl.nicolike.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://px.jctech888.com.cn

Ruby: s.gsub(/\s+/, "")
来源：http://mr.9csxet.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hg.jianghongdianzi.cn

[E10] 左侧补零 / 定长填充
来源：http://kf.huixinmuqiang.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hw.521024.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qy.huanxung.cn

JS:   "7".padStart(3, "0")
来源：http://jy.szsharing.cn

TS:   "7".padStart(3, "0")
来源：http://hz.wgjwhj.cn

Java: String.format("%03d", 7)
来源：http://gl.muxihuayi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ki.yuexingan06.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tl.szsharing.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cj.muxihuayi.cn

[E11] 反转字符串
来源：http://tg.szsharing.cn

Py:   s[::-1]
来源：http://jm.wgjwhj.cn

PHP:  strrev($s);
来源：http://jj.chemitech.net.cn

JS:   [...s].reverse().join("")
来源：http://ui.shxzukj.cn

TS:   [...s].reverse().join("")
来源：http://af.yuexingan06.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://vi.chemitech.net.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ll.shxzskj.cn

Ruby: s.reverse
来源：http://fv.shxzskj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://lr.haigaiapp.cn

[E12] 统计某字符出现次数
来源：http://vf.lnxyls.cn

Py:   s.count("a")
来源：http://hv.yuntaijiaju.cn

PHP:  substr_count($s, "a");
来源：http://ts.jctech888.com.cn

JS:   s.split("a").length - 1
来源：http://fv.gzmigu.cn

TS:   s.split("a").length - 1
来源：http://xz.shxzskj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ao.huixinmuqiang.cn

Go:   strings.Count(s, "a")
来源：http://xg.szxytkj.cn

Ruby: s.count("a")
来源：http://nd.huanxung.cn

C#:   s.Count(c => c == 'a')
来源：http://do.lnxyls.cn

[E13] 逐字符遍历
来源：http://xf.szsharing.cn

Py:   for ch in s: print(ch)
来源：http://io.shxzskj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ef.huanxung.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ol.hnjuh.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qg.nicolike.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xz.newstarts.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gd.lnxyls.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://qt.colortex.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://oj.newstarts.cn

[E14] URL 编码与 Base64
来源：http://av.chemitech.net.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rx.panjiajie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://xh.521024.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zt.hnjuh.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://er.huixinmuqiang.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zy.szxytkj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jp.huixinmuqiang.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hk.yuexingan06.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zw.shtwfgs.cn

[E15] HTML 转义 / 反转义
来源：http://qu.huanxung.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://rb.lnxyls.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ni.newstarts.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jd.yuexingan06.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://zz.szxytkj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zm.huanxung.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ed.521024.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zl.bjjhwx.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ik.gzmigu.cn

[E16] 数字千分位
来源：http://ga.bjjhwx.cn

Py:   f"{1234567:,}"
来源：http://wn.hahajie.cn

PHP:  number_format(1234567);
来源：http://jd.chemitech.net.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://cy.wgjwhj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://gk.bjjhwx.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ih.chemitech.net.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zt.yuexingan06.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pa.lnxyls.cn

C#:   1234567.ToString("N0")
来源：http://ev.nicolike.cn

[E17] 首字母大写
来源：http://gb.lnxyls.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fe.haigaiapp.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://hw.wgjwhj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xb.haigaiapp.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pn.shxzukj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zv.lnxyls.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zo.szxytkj.cn

Ruby: s.capitalize
来源：http://cb.bookmarksfly.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xp.yuntaijiaju.cn

[E18] 模板占位符替换
来源：http://mv.yuntaijiaju.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://co.newstarts.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://du.chemitech.net.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://br.gzmigu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://gw.shxzskj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zd.haigaiapp.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wv.chemitech.net.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lh.shxzskj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yj.bjjhwx.cn

[E19] 多行文本按行拆分
来源：http://ni.9csxet.cn

Py:   s.splitlines()
来源：http://vn.9csxet.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tg.asd995.cn

JS:   s.split(/\r?\n/)
来源：http://dp.bookmarksfly.cn

TS:   s.split(/\r?\n/)
来源：http://ln.szsharing.cn

Java: s.lines().toList()
来源：http://iy.huixinmuqiang.cn

Go:   strings.Split(s, "\n")
来源：http://al.haigaiapp.cn

Ruby: s.lines
来源：http://rm.bjjhwx.cn

C#:   s.Split('\n')
来源：http://ny.nicolike.cn

[E20] 判断字符串是否为空
来源：http://yb.szxytkj.cn

Py:   if not s:
来源：http://ul.huixiangedu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lv.bookmarksfly.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xh.huixiangedu.cn

TS:   if (s === "") {}
来源：http://di.wgjwhj.cn

Java: if (s.isEmpty()) {}
来源：http://xq.colortex.cn

Go:   if s == "" {}
来源：http://aq.yuexingan06.cn

Ruby: if s.empty?
来源：http://ux.huixiangedu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vo.haigaiapp.cn

[E21] 超长截断加省略号
来源：http://lj.521024.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hw.shxzskj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pk.szxytkj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qc.hahajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rw.szsharing.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yw.yuexingan06.cn

Go:   // 按 rune 判断长度后截断
来源：http://en.newstarts.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://eg.nicolike.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pk.panjiajie.cn

[E22] 字节长度与字符长度
来源：http://tk.wgjwhj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fr.bookmarksfly.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://md.asd995.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wp.bookmarksfly.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ms.nszjky.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wo.huixinmuqiang.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zf.newstarts.cn

Ruby: s.bytesize;  s.length
来源：http://pc.521024.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mr.muxihuayi.cn

================================================================================
来源：http://nm.szsharing.cn

F. 文件与目录
来源：http://od.gzmigu.cn

================================================================================
来源：http://ei.shtwfgs.cn

[F01] 读取整个文件
来源：http://ce.shtwfgs.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mk.521024.cn

PHP:  file_get_contents("a.txt");
来源：http://zj.gzmigu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nx.chemitech.net.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yt.wgjwhj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://az.yuexingan06.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ct.chemitech.net.cn

Ruby: File.read("a.txt")
来源：http://cl.muxihuayi.cn

C#:   File.ReadAllText("a.txt");
来源：http://uw.gzmigu.cn

[F02] 逐行读取文件
来源：http://sw.hnjuh.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lt.jctech888.com.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://aw.gzmigu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ik.shxzukj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://er.asd995.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vi.huanxung.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://sp.huixinmuqiang.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mr.wgjwhj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mw.chemitech.net.cn

[F03] 写入文件（覆盖）
来源：http://bm.wgjwhj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bc.huixinmuqiang.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://yq.shtwfgs.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ds.szsharing.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wc.9csxet.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hs.lnxyls.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ce.panjiajie.cn

Ruby: File.write("a.txt", "hi")
来源：http://jq.asd995.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yy.huixiangedu.cn

[F04] 追加写入文件
来源：http://ij.shtwfgs.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xd.panjiajie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ri.wgjwhj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qk.wgjwhj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hu.huixinmuqiang.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yn.haigaiapp.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ia.szsharing.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ds.huixinmuqiang.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://it.huixinmuqiang.cn

[F05] 判断文件或目录是否存在
来源：http://ja.jianghongdianzi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gd.shxzukj.cn

PHP:  file_exists("a.txt");
来源：http://cb.huanxung.cn

JS:   fs.existsSync("a.txt")
来源：http://iz.szxytkj.cn

TS:   fs.existsSync("a.txt")
来源：http://ka.nicolike.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ew.nicolike.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://oo.jianghongdianzi.cn

Ruby: File.exist?("a.txt")
来源：http://ie.huanxung.cn

C#:   File.Exists("a.txt")
来源：http://pc.asd995.cn

[F06] 删除文件
来源：http://fz.gzmigu.cn

Py:   os.remove("a.txt")
来源：http://ei.newstarts.cn

PHP:  unlink("a.txt");
来源：http://sk.panjiajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://rx.lnxyls.cn

TS:   fs.unlinkSync("a.txt")
来源：http://kh.huixiangedu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://po.jianghongdianzi.cn

Go:   os.Remove("a.txt")
来源：http://gf.bjjhwx.cn

Ruby: File.delete("a.txt")
来源：http://le.nicolike.cn

C#:   File.Delete("a.txt");
来源：http://sr.shxzskj.cn

[F07] 创建目录（含多级）
来源：http://ka.jianghongdianzi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://uf.chemitech.net.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xj.bjjhwx.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gq.asd995.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nc.bookmarksfly.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nx.huixiangedu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nt.newstarts.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://sn.wgjwhj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://uq.gzmigu.cn

[F08] 遍历目录
来源：http://gd.hnjuh.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://cs.hahajie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pu.521024.cn

JS:   fs.readdirSync("dir")
来源：http://rz.hahajie.cn

TS:   fs.readdirSync("dir")
来源：http://qr.9csxet.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://id.chemitech.net.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://pj.colortex.cn

Ruby: Dir.children("dir")
来源：http://rf.hnjuh.cn

C#:   Directory.GetFiles("dir")
来源：http://vj.nicolike.cn

[F09] 获取文件大小
来源：http://kw.shxzukj.cn

Py:   os.path.getsize("a.txt")
来源：http://ul.yuexingan06.cn

PHP:  filesize("a.txt");
来源：http://ky.newstarts.cn

JS:   fs.statSync("a.txt").size
来源：http://aj.chemitech.net.cn

TS:   fs.statSync("a.txt").size
来源：http://tn.panjiajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://gt.yuntaijiaju.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ky.jctech888.com.cn

Ruby: File.size("a.txt")
来源：http://ij.muxihuayi.cn

C#:   new FileInfo("a.txt").Length
来源：http://hq.shxzukj.cn

[F10] 取文件扩展名 / 文件名
来源：http://zp.jianghongdianzi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hu.nicolike.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ld.szsharing.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ew.huanxung.cn

TS:   path.extname("a.txt")
来源：http://iv.huixinmuqiang.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ve.shtwfgs.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://oq.bjjhwx.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://de.shxzukj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ec.jctech888.com.cn

[F11] 复制与移动文件
来源：http://et.bjjhwx.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pb.hnjuh.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://du.9csxet.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://or.asd995.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bd.nicolike.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ue.9csxet.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zj.bjjhwx.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hq.yuntaijiaju.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://aj.bjjhwx.cn

[F12] CSV 读写
来源：http://pc.521024.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qt.yuntaijiaju.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pi.shxzukj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fq.jianghongdianzi.cn

TS:   // 同上
来源：http://yg.yuexingan06.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://eo.nicolike.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hx.shxzukj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fl.asd995.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://dt.shxzskj.cn

================================================================================
来源：http://rx.huixiangedu.cn

G. 面向对象
来源：http://tz.shtwfgs.cn

================================================================================
来源：http://fk.gzmigu.cn

[G01] 定义类
来源：http://uy.szxytkj.cn

Py:   class User: pass
来源：http://xp.hahajie.cn

PHP:  class User {}
来源：http://ky.9csxet.cn

JS:   class User {}
来源：http://hb.wgjwhj.cn

TS:   class User { name: string = ""; }
来源：http://af.haigaiapp.cn

Java: class User {}
来源：http://lr.yuntaijiaju.cn

Go:   type User struct { Name string }
来源：http://xy.bjjhwx.cn

Ruby: class User; end
来源：http://yf.jctech888.com.cn

C#:   class User {}
来源：http://rs.wgjwhj.cn

[G02] 构造函数
来源：http://nb.asd995.cn

Py:   def __init__(self, name): self.name = name
来源：http://if.shtwfgs.cn

PHP:  public function __construct(public string $name) {}
来源：http://as.huixinmuqiang.cn

JS:   constructor(name) { this.name = name; }
来源：http://kk.chemitech.net.cn


<!-- 参考信息 -->