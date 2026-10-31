代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rr.nicolike.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kg.panjiajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zm.jctech888.com.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qq.gzmigu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bg.wgjwhj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rk.panjiajie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zk.bjjhwx.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qv.hnjuh.cn

[E06] 替换子串
来源：http://ei.jctech888.com.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lq.chemitech.net.cn

PHP:  str_replace("a", "b", $s);
来源：http://fg.hahajie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uo.hahajie.cn

TS:   s.replaceAll("a", "b")
来源：http://lz.huixinmuqiang.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gv.haigaiapp.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kw.huixiangedu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cc.nicolike.cn

C#:   s.Replace("a", "b")
来源：http://ar.colortex.cn

[E07] 按分隔符拆分
来源：http://zf.colortex.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gb.gzmigu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://df.chemitech.net.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ge.muxihuayi.cn

TS:   s.split(",")
来源：http://ap.haigaiapp.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ja.nicolike.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ms.colortex.cn

Ruby: s.split(",");  s.split
来源：http://wv.nicolike.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qa.9csxet.cn

[E08] 数组按分隔符合并
来源：http://kx.szxytkj.cn

Py:   ",".join(items)
来源：http://mb.hahajie.cn

PHP:  implode(",", $items);
来源：http://el.huixinmuqiang.cn

JS:   items.join(",")
来源：http://gw.hahajie.cn

TS:   items.join(",")
来源：http://qj.lnxyls.cn

Java: String.join(",", items)
来源：http://fn.colortex.cn

Go:   strings.Join(items, ",")
来源：http://aa.wgjwhj.cn

Ruby: items.join(",")
来源：http://cx.muxihuayi.cn

C#:   string.Join(",", items)
来源：http://pe.haigaiapp.cn

[E09] 去除所有空白字符
来源：http://sq.jianghongdianzi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://yr.bookmarksfly.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nq.shxzskj.cn

JS:   s.replace(/\s+/g, "")
来源：http://iy.hahajie.cn

TS:   s.replace(/\s+/g, "")
来源：http://bv.lnxyls.cn

Java: s.replaceAll("\\s+", "")
来源：http://zx.hnjuh.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://my.yuexingan06.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ez.chemitech.net.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ma.shxzskj.cn

[E10] 左侧补零 / 定长填充
来源：http://na.szxytkj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mq.521024.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kr.bookmarksfly.cn

JS:   "7".padStart(3, "0")
来源：http://ae.panjiajie.cn

TS:   "7".padStart(3, "0")
来源：http://yb.shxzukj.cn

Java: String.format("%03d", 7)
来源：http://gz.szxytkj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://lx.newstarts.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cz.huixiangedu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cr.nszjky.cn

[E11] 反转字符串
来源：http://pf.lnxyls.cn

Py:   s[::-1]
来源：http://qh.jctech888.com.cn

PHP:  strrev($s);
来源：http://ym.asd995.cn

JS:   [...s].reverse().join("")
来源：http://rh.521024.cn

TS:   [...s].reverse().join("")
来源：http://lv.hahajie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://vo.szxytkj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://xh.yuntaijiaju.cn

Ruby: s.reverse
来源：http://mb.szsharing.cn

C#:   new string(s.Reverse().ToArray())
来源：http://aq.bjjhwx.cn

[E12] 统计某字符出现次数
来源：http://sf.nszjky.cn

Py:   s.count("a")
来源：http://fl.bjjhwx.cn

PHP:  substr_count($s, "a");
来源：http://qy.bookmarksfly.cn

JS:   s.split("a").length - 1
来源：http://rw.panjiajie.cn

TS:   s.split("a").length - 1
来源：http://rh.panjiajie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yp.jctech888.com.cn

Go:   strings.Count(s, "a")
来源：http://xq.wgjwhj.cn

Ruby: s.count("a")
来源：http://cx.huixinmuqiang.cn

C#:   s.Count(c => c == 'a')
来源：http://ur.muxihuayi.cn

[E13] 逐字符遍历
来源：http://hw.szxytkj.cn

Py:   for ch in s: print(ch)
来源：http://io.haigaiapp.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zd.9csxet.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://dv.hnjuh.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://sq.newstarts.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xv.nicolike.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xg.wgjwhj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://tf.newstarts.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lm.jctech888.com.cn

[E14] URL 编码与 Base64
来源：http://as.hnjuh.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jo.521024.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://su.9csxet.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://un.yuntaijiaju.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hp.nszjky.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qs.szsharing.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://le.newstarts.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jy.yuexingan06.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pb.asd995.cn

[E15] HTML 转义 / 反转义
来源：http://dl.newstarts.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://fm.nicolike.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yc.hahajie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wm.hnjuh.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ta.huanxung.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://sr.hahajie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ux.shxzukj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xj.huanxung.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cp.colortex.cn

[E16] 数字千分位
来源：http://qv.shxzukj.cn

Py:   f"{1234567:,}"
来源：http://si.gzmigu.cn

PHP:  number_format(1234567);
来源：http://ah.hahajie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ob.shxzukj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://te.gzmigu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qj.shtwfgs.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ce.jctech888.com.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cr.shxzukj.cn

C#:   1234567.ToString("N0")
来源：http://qc.shxzskj.cn

[E17] 首字母大写
来源：http://rt.hahajie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://el.nicolike.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://dr.yuntaijiaju.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gx.szxytkj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://im.jctech888.com.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wb.newstarts.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lw.huanxung.cn

Ruby: s.capitalize
来源：http://zs.nicolike.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ce.wgjwhj.cn

[E18] 模板占位符替换
来源：http://zh.colortex.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fg.colortex.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zv.wgjwhj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://sd.huixinmuqiang.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ge.huixinmuqiang.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fb.szsharing.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://it.haigaiapp.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zn.newstarts.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gt.nszjky.cn

[E19] 多行文本按行拆分
来源：http://qo.yuntaijiaju.cn

Py:   s.splitlines()
来源：http://ln.huixiangedu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ne.muxihuayi.cn

JS:   s.split(/\r?\n/)
来源：http://jm.yuntaijiaju.cn

TS:   s.split(/\r?\n/)
来源：http://lx.gzmigu.cn

Java: s.lines().toList()
来源：http://gh.chemitech.net.cn

Go:   strings.Split(s, "\n")
来源：http://tv.nicolike.cn

Ruby: s.lines
来源：http://bu.jianghongdianzi.cn

C#:   s.Split('\n')
来源：http://ud.colortex.cn

[E20] 判断字符串是否为空
来源：http://ah.szsharing.cn

Py:   if not s:
来源：http://rt.nicolike.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pr.asd995.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ha.hnjuh.cn

TS:   if (s === "") {}
来源：http://rv.bjjhwx.cn

Java: if (s.isEmpty()) {}
来源：http://xo.jianghongdianzi.cn

Go:   if s == "" {}
来源：http://ia.shtwfgs.cn

Ruby: if s.empty?
来源：http://er.asd995.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rb.asd995.cn

[E21] 超长截断加省略号
来源：http://qi.hnjuh.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ls.nszjky.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dg.jianghongdianzi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://al.szsharing.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xw.newstarts.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tq.wgjwhj.cn

Go:   // 按 rune 判断长度后截断
来源：http://iw.huanxung.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ba.panjiajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wj.huixiangedu.cn

[E22] 字节长度与字符长度
来源：http://by.huanxung.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://st.521024.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ev.hnjuh.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dm.bjjhwx.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://oq.nszjky.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qq.asd995.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hk.521024.cn

Ruby: s.bytesize;  s.length
来源：http://ay.chemitech.net.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dw.lnxyls.cn

================================================================================
来源：http://nh.muxihuayi.cn

F. 文件与目录
来源：http://yn.9csxet.cn

================================================================================
来源：http://ru.bookmarksfly.cn

[F01] 读取整个文件
来源：http://on.hahajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ee.huanxung.cn

PHP:  file_get_contents("a.txt");
来源：http://kj.huixinmuqiang.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://io.hahajie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gz.wgjwhj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://oe.shtwfgs.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://it.shxzskj.cn

Ruby: File.read("a.txt")
来源：http://jm.yuexingan06.cn

C#:   File.ReadAllText("a.txt");
来源：http://ab.huixinmuqiang.cn

[F02] 逐行读取文件
来源：http://cp.yuntaijiaju.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://eu.panjiajie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pb.gzmigu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vz.9csxet.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cq.szxytkj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wf.yuexingan06.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yx.szxytkj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dy.lnxyls.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sy.chemitech.net.cn

[F03] 写入文件（覆盖）
来源：http://hn.huanxung.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rn.521024.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://da.bjjhwx.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jw.bjjhwx.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://om.bjjhwx.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://on.szsharing.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qv.gzmigu.cn

Ruby: File.write("a.txt", "hi")
来源：http://yz.nicolike.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fk.szsharing.cn

[F04] 追加写入文件
来源：http://uj.szxytkj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bt.yuntaijiaju.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ew.panjiajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fj.hahajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jj.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xd.muxihuayi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://le.shxzskj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://on.haigaiapp.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fa.nicolike.cn

[F05] 判断文件或目录是否存在
来源：http://qk.asd995.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fl.muxihuayi.cn

PHP:  file_exists("a.txt");
来源：http://mn.panjiajie.cn

JS:   fs.existsSync("a.txt")
来源：http://ek.szxytkj.cn

TS:   fs.existsSync("a.txt")
来源：http://ua.huanxung.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://lf.hahajie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fn.yuexingan06.cn

Ruby: File.exist?("a.txt")
来源：http://om.yuntaijiaju.cn

C#:   File.Exists("a.txt")
来源：http://mh.szsharing.cn

[F06] 删除文件
来源：http://ic.colortex.cn

Py:   os.remove("a.txt")
来源：http://zm.yuntaijiaju.cn

PHP:  unlink("a.txt");
来源：http://tn.jctech888.com.cn

JS:   fs.unlinkSync("a.txt")
来源：http://lo.gzmigu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ey.huixiangedu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pt.newstarts.cn

Go:   os.Remove("a.txt")
来源：http://ww.chemitech.net.cn

Ruby: File.delete("a.txt")
来源：http://yu.shtwfgs.cn

C#:   File.Delete("a.txt");
来源：http://do.shxzukj.cn

[F07] 创建目录（含多级）
来源：http://pk.nszjky.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ef.szsharing.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ah.nicolike.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bx.9csxet.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ga.hahajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qu.gzmigu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dm.nicolike.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vk.jianghongdianzi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zj.yuntaijiaju.cn

[F08] 遍历目录
来源：http://ha.521024.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://mp.bjjhwx.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ke.nicolike.cn

JS:   fs.readdirSync("dir")
来源：http://ij.wgjwhj.cn

TS:   fs.readdirSync("dir")
来源：http://et.szxytkj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ax.9csxet.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://gj.chemitech.net.cn

Ruby: Dir.children("dir")
来源：http://iq.haigaiapp.cn

C#:   Directory.GetFiles("dir")
来源：http://kv.gzmigu.cn

[F09] 获取文件大小
来源：http://qa.bjjhwx.cn

Py:   os.path.getsize("a.txt")
来源：http://gm.shxzukj.cn

PHP:  filesize("a.txt");
来源：http://sq.huixinmuqiang.cn

JS:   fs.statSync("a.txt").size
来源：http://rd.hahajie.cn

TS:   fs.statSync("a.txt").size
来源：http://dn.asd995.cn

Java: Files.size(Path.of("a.txt"))
来源：http://kh.panjiajie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vv.521024.cn

Ruby: File.size("a.txt")
来源：http://ji.yuexingan06.cn

C#:   new FileInfo("a.txt").Length
来源：http://mu.colortex.cn

[F10] 取文件扩展名 / 文件名
来源：http://wr.haigaiapp.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://re.shxzukj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://da.521024.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zz.colortex.cn

TS:   path.extname("a.txt")
来源：http://rl.jctech888.com.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tv.haigaiapp.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fa.jctech888.com.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rz.shxzskj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rf.newstarts.cn

[F11] 复制与移动文件
来源：http://fg.yuexingan06.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fn.wgjwhj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://au.bjjhwx.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bn.nszjky.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dv.huixiangedu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ye.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://uo.hahajie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ad.nicolike.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ir.panjiajie.cn

[F12] CSV 读写
来源：http://kw.shtwfgs.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ik.jctech888.com.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qx.hahajie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qe.wgjwhj.cn

TS:   // 同上
来源：http://nl.nicolike.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jf.hahajie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://is.yuexingan06.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ln.9csxet.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ft.huixinmuqiang.cn

================================================================================
来源：http://vw.huixinmuqiang.cn

G. 面向对象
来源：http://wm.huixiangedu.cn

================================================================================
来源：http://jg.huanxung.cn

[G01] 定义类
来源：http://lj.bookmarksfly.cn

Py:   class User: pass
来源：http://jr.jctech888.com.cn

PHP:  class User {}
来源：http://ej.jianghongdianzi.cn

JS:   class User {}
来源：http://kh.jianghongdianzi.cn

TS:   class User { name: string = ""; }
来源：http://dq.nicolike.cn

Java: class User {}
来源：http://zn.asd995.cn

Go:   type User struct { Name string }
来源：http://xq.nicolike.cn

Ruby: class User; end
来源：http://ag.panjiajie.cn

C#:   class User {}
来源：http://wv.nicolike.cn

[G02] 构造函数
来源：http://ls.nszjky.cn

Py:   def __init__(self, name): self.name = name
来源：http://wq.nicolike.cn

PHP:  public function __construct(public string $name) {}
来源：http://ck.lnxyls.cn

JS:   constructor(name) { this.name = name; }
来源：http://fo.panjiajie.cn

TS:   constructor(public name: string) {}
来源：http://wj.huixinmuqiang.cn

Java: User(String name) { this.name = name; }
来源：http://gj.nicolike.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ad.huixiangedu.cn

Ruby: def initialize(name); @name = name; end
来源：http://yf.9csxet.cn

C#:   public User(string name) { Name = name; }
来源：http://mk.shxzukj.cn

[G03] 实例属性
来源：http://db.szxytkj.cn

Py:   self.name = "x"
来源：http://ph.nicolike.cn

PHP:  public string $name = "x";
来源：http://yp.nicolike.cn

JS:   this.name = "x";
来源：http://zm.521024.cn

TS:   name: string = "x";
来源：http://ri.shxzukj.cn

Java: private String name;
来源：http://wd.colortex.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://uo.bjjhwx.cn


<!-- 参考信息 -->