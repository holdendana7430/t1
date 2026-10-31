代发 wailian999

PHP:  strpos($s, "x");
来源：http://xy.9csxet.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fo.jianghongdianzi.cn

TS:   s.indexOf("x")
来源：http://gq.yuexingan06.cn

Java: s.indexOf("x")
来源：http://li.bookmarksfly.cn

Go:   strings.Index(s, "x")
来源：http://it.szxytkj.cn

Ruby: s.index("x")
来源：http://qp.yuexingan06.cn

C#:   s.IndexOf("x")
来源：http://bv.hnjuh.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://dz.asd995.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ke.nszjky.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ki.lnxyls.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gv.bookmarksfly.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qx.nszjky.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://of.521024.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ce.chemitech.net.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nj.bookmarksfly.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ee.huixinmuqiang.cn

[E06] 替换子串
来源：http://jg.asd995.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://oa.jctech888.com.cn

PHP:  str_replace("a", "b", $s);
来源：http://tb.gzmigu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pm.9csxet.cn

TS:   s.replaceAll("a", "b")
来源：http://rj.521024.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ue.szsharing.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sn.szsharing.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tb.haigaiapp.cn

C#:   s.Replace("a", "b")
来源：http://pz.shtwfgs.cn

[E07] 按分隔符拆分
来源：http://zq.newstarts.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pi.newstarts.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gk.hnjuh.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://oj.haigaiapp.cn

TS:   s.split(",")
来源：http://hd.lnxyls.cn

Java: s.split(",");  s.split("\\s+")
来源：http://rx.chemitech.net.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wb.colortex.cn

Ruby: s.split(",");  s.split
来源：http://gd.hnjuh.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jy.gzmigu.cn

[E08] 数组按分隔符合并
来源：http://ch.yuntaijiaju.cn

Py:   ",".join(items)
来源：http://au.9csxet.cn

PHP:  implode(",", $items);
来源：http://od.yuntaijiaju.cn

JS:   items.join(",")
来源：http://rx.colortex.cn

TS:   items.join(",")
来源：http://sc.shxzskj.cn

Java: String.join(",", items)
来源：http://lm.wgjwhj.cn

Go:   strings.Join(items, ",")
来源：http://gf.huixiangedu.cn

Ruby: items.join(",")
来源：http://si.bookmarksfly.cn

C#:   string.Join(",", items)
来源：http://gp.9csxet.cn

[E09] 去除所有空白字符
来源：http://tq.jctech888.com.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lj.jianghongdianzi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wl.szxytkj.cn

JS:   s.replace(/\s+/g, "")
来源：http://og.bjjhwx.cn

TS:   s.replace(/\s+/g, "")
来源：http://la.jctech888.com.cn

Java: s.replaceAll("\\s+", "")
来源：http://in.bjjhwx.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://av.shxzskj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://aj.hnjuh.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ak.wgjwhj.cn

[E10] 左侧补零 / 定长填充
来源：http://mv.huixiangedu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://op.bookmarksfly.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ev.gzmigu.cn

JS:   "7".padStart(3, "0")
来源：http://xx.szsharing.cn

TS:   "7".padStart(3, "0")
来源：http://ca.shtwfgs.cn

Java: String.format("%03d", 7)
来源：http://di.yuexingan06.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://pm.shtwfgs.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://er.panjiajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xr.shxzskj.cn

[E11] 反转字符串
来源：http://iq.yuntaijiaju.cn

Py:   s[::-1]
来源：http://bm.chemitech.net.cn

PHP:  strrev($s);
来源：http://dd.hnjuh.cn

JS:   [...s].reverse().join("")
来源：http://is.hahajie.cn

TS:   [...s].reverse().join("")
来源：http://yv.lnxyls.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://jz.nicolike.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ic.panjiajie.cn

Ruby: s.reverse
来源：http://jt.gzmigu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://fs.szsharing.cn

[E12] 统计某字符出现次数
来源：http://hc.521024.cn

Py:   s.count("a")
来源：http://vt.bjjhwx.cn

PHP:  substr_count($s, "a");
来源：http://bz.jctech888.com.cn

JS:   s.split("a").length - 1
来源：http://sh.huixinmuqiang.cn

TS:   s.split("a").length - 1
来源：http://yg.shtwfgs.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dz.newstarts.cn

Go:   strings.Count(s, "a")
来源：http://gk.wgjwhj.cn

Ruby: s.count("a")
来源：http://pj.yuexingan06.cn

C#:   s.Count(c => c == 'a')
来源：http://cp.asd995.cn

[E13] 逐字符遍历
来源：http://xt.szsharing.cn

Py:   for ch in s: print(ch)
来源：http://xv.szxytkj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yj.nszjky.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://mn.wgjwhj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://oi.nszjky.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ti.szsharing.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://om.nicolike.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://mg.yuntaijiaju.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://se.haigaiapp.cn

[E14] URL 编码与 Base64
来源：http://xj.nicolike.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qu.haigaiapp.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://eh.muxihuayi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rr.shtwfgs.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vo.lnxyls.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fs.chemitech.net.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bb.yuexingan06.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hw.shtwfgs.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://um.hnjuh.cn

[E15] HTML 转义 / 反转义
来源：http://gg.shxzskj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ui.panjiajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://na.panjiajie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gc.shxzukj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.shxzukj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kv.huanxung.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://is.szsharing.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jy.huanxung.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dx.colortex.cn

[E16] 数字千分位
来源：http://nx.nszjky.cn

Py:   f"{1234567:,}"
来源：http://wt.jianghongdianzi.cn

PHP:  number_format(1234567);
来源：http://tc.hnjuh.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://kc.hnjuh.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://xz.9csxet.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ib.panjiajie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://el.lnxyls.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://uh.huixinmuqiang.cn

C#:   1234567.ToString("N0")
来源：http://eh.haigaiapp.cn

[E17] 首字母大写
来源：http://az.gzmigu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rm.lnxyls.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://va.wgjwhj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://me.muxihuayi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ey.hnjuh.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://di.huixiangedu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jl.szsharing.cn

Ruby: s.capitalize
来源：http://oi.chemitech.net.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fx.huixinmuqiang.cn

[E18] 模板占位符替换
来源：http://kn.shtwfgs.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://eg.yuntaijiaju.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kd.newstarts.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://bx.huanxung.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://il.521024.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ti.hnjuh.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ss.nicolike.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ea.nicolike.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yl.asd995.cn

[E19] 多行文本按行拆分
来源：http://od.shxzskj.cn

Py:   s.splitlines()
来源：http://xp.newstarts.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ul.szsharing.cn

JS:   s.split(/\r?\n/)
来源：http://ct.chemitech.net.cn

TS:   s.split(/\r?\n/)
来源：http://wh.nicolike.cn

Java: s.lines().toList()
来源：http://ht.panjiajie.cn

Go:   strings.Split(s, "\n")
来源：http://aa.yuntaijiaju.cn

Ruby: s.lines
来源：http://yg.szxytkj.cn

C#:   s.Split('\n')
来源：http://tu.huixiangedu.cn

[E20] 判断字符串是否为空
来源：http://bk.muxihuayi.cn

Py:   if not s:
来源：http://qk.jctech888.com.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ho.hnjuh.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qi.jianghongdianzi.cn

TS:   if (s === "") {}
来源：http://cv.gzmigu.cn

Java: if (s.isEmpty()) {}
来源：http://yg.panjiajie.cn

Go:   if s == "" {}
来源：http://no.521024.cn

Ruby: if s.empty?
来源：http://ku.panjiajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xz.521024.cn

[E21] 超长截断加省略号
来源：http://nx.521024.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rh.huixinmuqiang.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zd.newstarts.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vt.lnxyls.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gc.nicolike.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mj.haigaiapp.cn

Go:   // 按 rune 判断长度后截断
来源：http://am.panjiajie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ss.9csxet.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ck.lnxyls.cn

[E22] 字节长度与字符长度
来源：http://vt.chemitech.net.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hs.gzmigu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://up.szsharing.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zk.shxzskj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gi.chemitech.net.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xb.nszjky.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xm.huixinmuqiang.cn

Ruby: s.bytesize;  s.length
来源：http://mi.muxihuayi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xw.bookmarksfly.cn

================================================================================
来源：http://xp.colortex.cn

F. 文件与目录
来源：http://xs.colortex.cn

================================================================================
来源：http://an.gzmigu.cn

[F01] 读取整个文件
来源：http://mc.haigaiapp.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rf.hahajie.cn

PHP:  file_get_contents("a.txt");
来源：http://mz.huixinmuqiang.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ck.lnxyls.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jq.9csxet.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fo.chemitech.net.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://na.bookmarksfly.cn

Ruby: File.read("a.txt")
来源：http://jl.9csxet.cn

C#:   File.ReadAllText("a.txt");
来源：http://gn.huanxung.cn

[F02] 逐行读取文件
来源：http://qr.hahajie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://yg.bookmarksfly.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qk.szxytkj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bd.muxihuayi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vy.521024.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gc.gzmigu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://eu.jianghongdianzi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lr.yuexingan06.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qw.huixiangedu.cn

[F03] 写入文件（覆盖）
来源：http://sb.szxytkj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xz.asd995.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://np.yuntaijiaju.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rm.asd995.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lt.colortex.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fc.haigaiapp.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ef.shxzukj.cn

Ruby: File.write("a.txt", "hi")
来源：http://nv.colortex.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jh.nicolike.cn

[F04] 追加写入文件
来源：http://ke.huixinmuqiang.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qc.shxzukj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fc.colortex.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hx.huanxung.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hy.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://oj.shxzukj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tj.szxytkj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://sj.haigaiapp.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xo.shxzukj.cn

[F05] 判断文件或目录是否存在
来源：http://we.wgjwhj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yv.yuexingan06.cn

PHP:  file_exists("a.txt");
来源：http://tp.jianghongdianzi.cn

JS:   fs.existsSync("a.txt")
来源：http://kq.hahajie.cn

TS:   fs.existsSync("a.txt")
来源：http://ui.haigaiapp.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://pd.wgjwhj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://md.haigaiapp.cn

Ruby: File.exist?("a.txt")
来源：http://fa.lnxyls.cn

C#:   File.Exists("a.txt")
来源：http://mi.hahajie.cn

[F06] 删除文件
来源：http://ht.shxzukj.cn

Py:   os.remove("a.txt")
来源：http://yh.shtwfgs.cn

PHP:  unlink("a.txt");
来源：http://pi.chemitech.net.cn

JS:   fs.unlinkSync("a.txt")
来源：http://gx.chemitech.net.cn

TS:   fs.unlinkSync("a.txt")
来源：http://xa.nicolike.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://td.hnjuh.cn

Go:   os.Remove("a.txt")
来源：http://fl.shxzukj.cn

Ruby: File.delete("a.txt")
来源：http://tx.bjjhwx.cn

C#:   File.Delete("a.txt");
来源：http://se.521024.cn

[F07] 创建目录（含多级）
来源：http://vt.shxzukj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mb.gzmigu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://be.521024.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ab.huixiangedu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wr.huanxung.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zc.gzmigu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://un.521024.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hh.haigaiapp.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lf.shxzskj.cn

[F08] 遍历目录
来源：http://vd.chemitech.net.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://kx.shxzskj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yi.shxzukj.cn

JS:   fs.readdirSync("dir")
来源：http://nu.panjiajie.cn

TS:   fs.readdirSync("dir")
来源：http://sf.huanxung.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hc.nszjky.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://iu.9csxet.cn

Ruby: Dir.children("dir")
来源：http://ha.muxihuayi.cn

C#:   Directory.GetFiles("dir")
来源：http://eg.jctech888.com.cn

[F09] 获取文件大小
来源：http://ky.chemitech.net.cn

Py:   os.path.getsize("a.txt")
来源：http://ku.huanxung.cn

PHP:  filesize("a.txt");
来源：http://kz.huixiangedu.cn

JS:   fs.statSync("a.txt").size
来源：http://xr.nicolike.cn

TS:   fs.statSync("a.txt").size
来源：http://sj.chemitech.net.cn

Java: Files.size(Path.of("a.txt"))
来源：http://lf.huixinmuqiang.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vz.521024.cn

Ruby: File.size("a.txt")
来源：http://zt.panjiajie.cn

C#:   new FileInfo("a.txt").Length
来源：http://rm.colortex.cn

[F10] 取文件扩展名 / 文件名
来源：http://qd.hnjuh.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rt.szxytkj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://eq.huixiangedu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zo.yuntaijiaju.cn

TS:   path.extname("a.txt")
来源：http://xw.szsharing.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zb.shxzukj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dg.jctech888.com.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://et.yuntaijiaju.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ua.colortex.cn

[F11] 复制与移动文件
来源：http://hm.9csxet.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ae.colortex.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vh.jianghongdianzi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bo.bjjhwx.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rv.shxzukj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lw.chemitech.net.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rj.jctech888.com.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://av.521024.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hw.szsharing.cn

[F12] CSV 读写
来源：http://zi.bookmarksfly.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mu.bjjhwx.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zf.colortex.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mn.colortex.cn

TS:   // 同上
来源：http://lv.hahajie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ps.wgjwhj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rp.bookmarksfly.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wk.asd995.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ow.shxzskj.cn

================================================================================
来源：http://op.shxzskj.cn

G. 面向对象
来源：http://it.gzmigu.cn

================================================================================
来源：http://ft.yuntaijiaju.cn

[G01] 定义类
来源：http://jv.muxihuayi.cn

Py:   class User: pass
来源：http://bw.szxytkj.cn

PHP:  class User {}
来源：http://os.nicolike.cn

JS:   class User {}
来源：http://qb.jianghongdianzi.cn

TS:   class User { name: string = ""; }
来源：http://gm.huixiangedu.cn

Java: class User {}
来源：http://eg.yuntaijiaju.cn

Go:   type User struct { Name string }
来源：http://uc.shtwfgs.cn

Ruby: class User; end
来源：http://he.bjjhwx.cn

C#:   class User {}
来源：http://ce.521024.cn

[G02] 构造函数
来源：http://ym.panjiajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://kt.hnjuh.cn

PHP:  public function __construct(public string $name) {}
来源：http://jq.haigaiapp.cn

JS:   constructor(name) { this.name = name; }
来源：http://mv.muxihuayi.cn

TS:   constructor(public name: string) {}
来源：http://hd.panjiajie.cn

Java: User(String name) { this.name = name; }
来源：http://pw.colortex.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://em.lnxyls.cn

Ruby: def initialize(name); @name = name; end
来源：http://na.huixiangedu.cn


<!-- 参考信息 -->