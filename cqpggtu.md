代发 wailian999

Go:   strings.Index(s, "x")
来源：http://rt.szxytkj.cn

Ruby: s.index("x")
来源：http://ii.lnxyls.cn

C#:   s.IndexOf("x")
来源：http://kr.jctech888.com.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://tc.asd995.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ua.nicolike.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://oz.hnjuh.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ir.szxytkj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://yi.huanxung.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zi.asd995.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mi.yuexingan06.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zr.yuntaijiaju.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sb.yuntaijiaju.cn

[E06] 替换子串
来源：http://fw.521024.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ad.muxihuayi.cn

PHP:  str_replace("a", "b", $s);
来源：http://lb.chemitech.net.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bu.huixinmuqiang.cn

TS:   s.replaceAll("a", "b")
来源：http://ow.huixinmuqiang.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zz.gzmigu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ty.panjiajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rf.hnjuh.cn

C#:   s.Replace("a", "b")
来源：http://sp.huixinmuqiang.cn

[E07] 按分隔符拆分
来源：http://jy.lnxyls.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gf.jctech888.com.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ub.szsharing.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://oc.shtwfgs.cn

TS:   s.split(",")
来源：http://ok.yuexingan06.cn

Java: s.split(",");  s.split("\\s+")
来源：http://li.521024.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wh.asd995.cn

Ruby: s.split(",");  s.split
来源：http://dv.521024.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mp.yuexingan06.cn

[E08] 数组按分隔符合并
来源：http://xy.hahajie.cn

Py:   ",".join(items)
来源：http://bh.jctech888.com.cn

PHP:  implode(",", $items);
来源：http://gq.shtwfgs.cn

JS:   items.join(",")
来源：http://yp.9csxet.cn

TS:   items.join(",")
来源：http://hf.yuntaijiaju.cn

Java: String.join(",", items)
来源：http://wk.panjiajie.cn

Go:   strings.Join(items, ",")
来源：http://ws.colortex.cn

Ruby: items.join(",")
来源：http://ij.muxihuayi.cn

C#:   string.Join(",", items)
来源：http://ig.huanxung.cn

[E09] 去除所有空白字符
来源：http://aj.bjjhwx.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pu.hahajie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://os.yuntaijiaju.cn

JS:   s.replace(/\s+/g, "")
来源：http://yf.hnjuh.cn

TS:   s.replace(/\s+/g, "")
来源：http://kt.yuntaijiaju.cn

Java: s.replaceAll("\\s+", "")
来源：http://zd.521024.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://mw.panjiajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://bq.shxzukj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://om.521024.cn

[E10] 左侧补零 / 定长填充
来源：http://ea.huixinmuqiang.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kw.haigaiapp.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cz.haigaiapp.cn

JS:   "7".padStart(3, "0")
来源：http://yv.colortex.cn

TS:   "7".padStart(3, "0")
来源：http://ym.haigaiapp.cn

Java: String.format("%03d", 7)
来源：http://cr.521024.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://pz.haigaiapp.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://km.muxihuayi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://oo.yuexingan06.cn

[E11] 反转字符串
来源：http://ha.521024.cn

Py:   s[::-1]
来源：http://gy.huixiangedu.cn

PHP:  strrev($s);
来源：http://tw.gzmigu.cn

JS:   [...s].reverse().join("")
来源：http://om.newstarts.cn

TS:   [...s].reverse().join("")
来源：http://uz.chemitech.net.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ks.521024.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://pk.szsharing.cn

Ruby: s.reverse
来源：http://ur.jctech888.com.cn

C#:   new string(s.Reverse().ToArray())
来源：http://nx.muxihuayi.cn

[E12] 统计某字符出现次数
来源：http://fd.lnxyls.cn

Py:   s.count("a")
来源：http://rc.shtwfgs.cn

PHP:  substr_count($s, "a");
来源：http://fd.chemitech.net.cn

JS:   s.split("a").length - 1
来源：http://uh.gzmigu.cn

TS:   s.split("a").length - 1
来源：http://ds.nicolike.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cm.shxzukj.cn

Go:   strings.Count(s, "a")
来源：http://zx.panjiajie.cn

Ruby: s.count("a")
来源：http://oo.shxzskj.cn

C#:   s.Count(c => c == 'a')
来源：http://mv.hnjuh.cn

[E13] 逐字符遍历
来源：http://ji.nicolike.cn

Py:   for ch in s: print(ch)
来源：http://qy.nicolike.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tb.haigaiapp.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://dk.hnjuh.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://sf.chemitech.net.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ue.9csxet.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ou.shxzskj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://sj.colortex.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hv.panjiajie.cn

[E14] URL 编码与 Base64
来源：http://cx.hnjuh.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cc.wgjwhj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://pi.newstarts.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uc.muxihuayi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kz.yuexingan06.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fc.haigaiapp.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kb.bookmarksfly.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ma.gzmigu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ou.nszjky.cn

[E15] HTML 转义 / 反转义
来源：http://qo.wgjwhj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://bg.panjiajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cj.newstarts.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gt.panjiajie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ob.wgjwhj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mx.lnxyls.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xg.shxzskj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://du.9csxet.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://im.yuexingan06.cn

[E16] 数字千分位
来源：http://eu.lnxyls.cn

Py:   f"{1234567:,}"
来源：http://rf.nicolike.cn

PHP:  number_format(1234567);
来源：http://tx.szsharing.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://zf.huanxung.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://qp.asd995.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lg.nszjky.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nf.hahajie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ck.muxihuayi.cn

C#:   1234567.ToString("N0")
来源：http://lv.wgjwhj.cn

[E17] 首字母大写
来源：http://wr.haigaiapp.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pj.yuexingan06.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ub.newstarts.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bv.yuexingan06.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://to.haigaiapp.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sx.hnjuh.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://to.muxihuayi.cn

Ruby: s.capitalize
来源：http://bz.nszjky.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ok.jctech888.com.cn

[E18] 模板占位符替换
来源：http://dc.chemitech.net.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qj.haigaiapp.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ed.huixinmuqiang.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://dm.521024.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://fs.chemitech.net.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://my.panjiajie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hp.gzmigu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lo.newstarts.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qq.521024.cn

[E19] 多行文本按行拆分
来源：http://wo.hnjuh.cn

Py:   s.splitlines()
来源：http://jt.bookmarksfly.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pm.haigaiapp.cn

JS:   s.split(/\r?\n/)
来源：http://hp.9csxet.cn

TS:   s.split(/\r?\n/)
来源：http://wr.521024.cn

Java: s.lines().toList()
来源：http://lf.huanxung.cn

Go:   strings.Split(s, "\n")
来源：http://de.panjiajie.cn

Ruby: s.lines
来源：http://wv.shtwfgs.cn

C#:   s.Split('\n')
来源：http://az.bjjhwx.cn

[E20] 判断字符串是否为空
来源：http://bu.jianghongdianzi.cn

Py:   if not s:
来源：http://an.gzmigu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fj.panjiajie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://em.nicolike.cn

TS:   if (s === "") {}
来源：http://zf.lnxyls.cn

Java: if (s.isEmpty()) {}
来源：http://gn.chemitech.net.cn

Go:   if s == "" {}
来源：http://nt.bjjhwx.cn

Ruby: if s.empty?
来源：http://jy.szsharing.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wj.nicolike.cn

[E21] 超长截断加省略号
来源：http://hh.huixinmuqiang.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ob.huixinmuqiang.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dk.shxzukj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nf.haigaiapp.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ze.gzmigu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://uv.yuntaijiaju.cn

Go:   // 按 rune 判断长度后截断
来源：http://ud.szsharing.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ve.huixinmuqiang.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ij.9csxet.cn

[E22] 字节长度与字符长度
来源：http://gy.colortex.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ez.huixinmuqiang.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://so.gzmigu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zc.wgjwhj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mn.yuexingan06.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fx.chemitech.net.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xz.nszjky.cn

Ruby: s.bytesize;  s.length
来源：http://ce.hnjuh.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pq.szsharing.cn

================================================================================
来源：http://nn.chemitech.net.cn

F. 文件与目录
来源：http://ta.shxzukj.cn

================================================================================
来源：http://ov.haigaiapp.cn

[F01] 读取整个文件
来源：http://hh.szsharing.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ev.shxzskj.cn

PHP:  file_get_contents("a.txt");
来源：http://gb.szsharing.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yv.hahajie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ug.jctech888.com.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://du.szsharing.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jr.bjjhwx.cn

Ruby: File.read("a.txt")
来源：http://ay.haigaiapp.cn

C#:   File.ReadAllText("a.txt");
来源：http://ds.szxytkj.cn

[F02] 逐行读取文件
来源：http://di.jianghongdianzi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xk.jianghongdianzi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uu.huixiangedu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ba.shxzukj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fv.wgjwhj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jt.huixinmuqiang.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fb.muxihuayi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pv.bookmarksfly.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vs.newstarts.cn

[F03] 写入文件（覆盖）
来源：http://nt.lnxyls.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gy.asd995.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vo.gzmigu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mo.gzmigu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ul.hnjuh.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jz.lnxyls.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ha.haigaiapp.cn

Ruby: File.write("a.txt", "hi")
来源：http://wf.haigaiapp.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://co.newstarts.cn

[F04] 追加写入文件
来源：http://ip.huixinmuqiang.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mc.nicolike.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gp.9csxet.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ps.yuntaijiaju.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pm.szsharing.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ml.huanxung.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ff.haigaiapp.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://po.shtwfgs.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://eh.shxzukj.cn

[F05] 判断文件或目录是否存在
来源：http://yg.szsharing.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ti.asd995.cn

PHP:  file_exists("a.txt");
来源：http://vf.lnxyls.cn

JS:   fs.existsSync("a.txt")
来源：http://dn.jctech888.com.cn

TS:   fs.existsSync("a.txt")
来源：http://my.gzmigu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xw.wgjwhj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://az.nicolike.cn

Ruby: File.exist?("a.txt")
来源：http://rm.huixinmuqiang.cn

C#:   File.Exists("a.txt")
来源：http://mk.hnjuh.cn

[F06] 删除文件
来源：http://ji.bookmarksfly.cn

Py:   os.remove("a.txt")
来源：http://me.huixiangedu.cn

PHP:  unlink("a.txt");
来源：http://vg.shxzukj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://kv.yuexingan06.cn

TS:   fs.unlinkSync("a.txt")
来源：http://gt.szsharing.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tl.shxzskj.cn

Go:   os.Remove("a.txt")
来源：http://sq.shtwfgs.cn

Ruby: File.delete("a.txt")
来源：http://yi.haigaiapp.cn

C#:   File.Delete("a.txt");
来源：http://fn.asd995.cn

[F07] 创建目录（含多级）
来源：http://ux.newstarts.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pb.hahajie.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rl.haigaiapp.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jh.panjiajie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ee.huixinmuqiang.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pq.huixinmuqiang.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rh.nszjky.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vt.haigaiapp.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jf.nszjky.cn

[F08] 遍历目录
来源：http://tv.wgjwhj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://yt.9csxet.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xy.panjiajie.cn

JS:   fs.readdirSync("dir")
来源：http://oq.chemitech.net.cn

TS:   fs.readdirSync("dir")
来源：http://aj.521024.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://da.asd995.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://lh.lnxyls.cn

Ruby: Dir.children("dir")
来源：http://ni.nicolike.cn

C#:   Directory.GetFiles("dir")
来源：http://ej.szsharing.cn

[F09] 获取文件大小
来源：http://we.bookmarksfly.cn

Py:   os.path.getsize("a.txt")
来源：http://iv.bjjhwx.cn

PHP:  filesize("a.txt");
来源：http://qj.huixiangedu.cn

JS:   fs.statSync("a.txt").size
来源：http://go.panjiajie.cn

TS:   fs.statSync("a.txt").size
来源：http://bh.nszjky.cn

Java: Files.size(Path.of("a.txt"))
来源：http://xp.lnxyls.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hm.shtwfgs.cn

Ruby: File.size("a.txt")
来源：http://zk.nicolike.cn

C#:   new FileInfo("a.txt").Length
来源：http://ua.521024.cn

[F10] 取文件扩展名 / 文件名
来源：http://tm.shxzskj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vh.chemitech.net.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://oh.newstarts.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ij.9csxet.cn

TS:   path.extname("a.txt")
来源：http://gx.szsharing.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gh.wgjwhj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dy.yuntaijiaju.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mx.huixinmuqiang.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tg.shxzskj.cn

[F11] 复制与移动文件
来源：http://bc.colortex.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fa.wgjwhj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fw.yuexingan06.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cz.huanxung.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sl.huixinmuqiang.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ng.9csxet.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dr.nicolike.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rx.hnjuh.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mu.haigaiapp.cn

[F12] CSV 读写
来源：http://wt.huanxung.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ol.bookmarksfly.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gp.shtwfgs.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wd.bjjhwx.cn

TS:   // 同上
来源：http://jh.wgjwhj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yf.shxzukj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lh.huanxung.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cn.newstarts.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ga.huanxung.cn

================================================================================
来源：http://df.nszjky.cn

G. 面向对象
来源：http://yz.jianghongdianzi.cn

================================================================================
来源：http://kz.muxihuayi.cn

[G01] 定义类
来源：http://wd.huixinmuqiang.cn

Py:   class User: pass
来源：http://np.huanxung.cn

PHP:  class User {}
来源：http://ar.haigaiapp.cn

JS:   class User {}
来源：http://ld.gzmigu.cn

TS:   class User { name: string = ""; }
来源：http://dx.huixinmuqiang.cn

Java: class User {}
来源：http://kw.szsharing.cn

Go:   type User struct { Name string }
来源：http://fb.yuntaijiaju.cn

Ruby: class User; end
来源：http://be.jianghongdianzi.cn

C#:   class User {}
来源：http://kk.szsharing.cn

[G02] 构造函数
来源：http://wa.hnjuh.cn

Py:   def __init__(self, name): self.name = name
来源：http://qq.lnxyls.cn

PHP:  public function __construct(public string $name) {}
来源：http://oc.nszjky.cn

JS:   constructor(name) { this.name = name; }
来源：http://cw.huanxung.cn

TS:   constructor(public name: string) {}
来源：http://zv.shxzskj.cn

Java: User(String name) { this.name = name; }
来源：http://ht.huixinmuqiang.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ju.shxzukj.cn

Ruby: def initialize(name); @name = name; end
来源：http://su.asd995.cn

C#:   public User(string name) { Name = name; }
来源：http://an.chemitech.net.cn

[G03] 实例属性
来源：http://tl.szsharing.cn

Py:   self.name = "x"
来源：http://to.bookmarksfly.cn

PHP:  public string $name = "x";
来源：http://gj.lnxyls.cn


<!-- 参考信息 -->