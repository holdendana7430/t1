代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qc.huanxung.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gx.wgjwhj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zy.huixinmuqiang.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://la.bookmarksfly.cn

[E06] 替换子串
来源：http://df.newstarts.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://md.jctech888.com.cn

PHP:  str_replace("a", "b", $s);
来源：http://jn.nicolike.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ak.nicolike.cn

TS:   s.replaceAll("a", "b")
来源：http://hd.bjjhwx.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://en.nicolike.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mx.huixiangedu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://io.wgjwhj.cn

C#:   s.Replace("a", "b")
来源：http://vw.yuntaijiaju.cn

[E07] 按分隔符拆分
来源：http://yx.shtwfgs.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kt.9csxet.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rl.wgjwhj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://lr.bjjhwx.cn

TS:   s.split(",")
来源：http://bv.jctech888.com.cn

Java: s.split(",");  s.split("\\s+")
来源：http://gh.wgjwhj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tu.szxytkj.cn

Ruby: s.split(",");  s.split
来源：http://em.jctech888.com.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://im.shtwfgs.cn

[E08] 数组按分隔符合并
来源：http://pb.yuntaijiaju.cn

Py:   ",".join(items)
来源：http://qg.huixiangedu.cn

PHP:  implode(",", $items);
来源：http://uh.jianghongdianzi.cn

JS:   items.join(",")
来源：http://lv.huixinmuqiang.cn

TS:   items.join(",")
来源：http://er.9csxet.cn

Java: String.join(",", items)
来源：http://io.newstarts.cn

Go:   strings.Join(items, ",")
来源：http://mm.shxzukj.cn

Ruby: items.join(",")
来源：http://za.asd995.cn

C#:   string.Join(",", items)
来源：http://oz.bookmarksfly.cn

[E09] 去除所有空白字符
来源：http://fe.9csxet.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wn.colortex.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hq.bjjhwx.cn

JS:   s.replace(/\s+/g, "")
来源：http://dw.bookmarksfly.cn

TS:   s.replace(/\s+/g, "")
来源：http://bu.huixiangedu.cn

Java: s.replaceAll("\\s+", "")
来源：http://vu.shxzukj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://bv.muxihuayi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://rv.newstarts.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ck.huanxung.cn

[E10] 左侧补零 / 定长填充
来源：http://yq.huanxung.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://uo.bookmarksfly.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ax.huixiangedu.cn

JS:   "7".padStart(3, "0")
来源：http://rp.nicolike.cn

TS:   "7".padStart(3, "0")
来源：http://vc.shxzukj.cn

Java: String.format("%03d", 7)
来源：http://mi.jianghongdianzi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://yc.szsharing.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://oe.asd995.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://po.huanxung.cn

[E11] 反转字符串
来源：http://ph.nszjky.cn

Py:   s[::-1]
来源：http://oo.9csxet.cn

PHP:  strrev($s);
来源：http://zl.haigaiapp.cn

JS:   [...s].reverse().join("")
来源：http://co.newstarts.cn

TS:   [...s].reverse().join("")
来源：http://ml.nszjky.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://gc.jctech888.com.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://xn.bjjhwx.cn

Ruby: s.reverse
来源：http://zb.jctech888.com.cn

C#:   new string(s.Reverse().ToArray())
来源：http://et.haigaiapp.cn

[E12] 统计某字符出现次数
来源：http://oz.huixiangedu.cn

Py:   s.count("a")
来源：http://km.hnjuh.cn

PHP:  substr_count($s, "a");
来源：http://se.bjjhwx.cn

JS:   s.split("a").length - 1
来源：http://ik.jianghongdianzi.cn

TS:   s.split("a").length - 1
来源：http://nu.newstarts.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xt.chemitech.net.cn

Go:   strings.Count(s, "a")
来源：http://gq.panjiajie.cn

Ruby: s.count("a")
来源：http://zy.hnjuh.cn

C#:   s.Count(c => c == 'a')
来源：http://ba.colortex.cn

[E13] 逐字符遍历
来源：http://xr.huixiangedu.cn

Py:   for ch in s: print(ch)
来源：http://do.huanxung.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://af.wgjwhj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://km.asd995.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://mb.szxytkj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jq.gzmigu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bt.shxzskj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://fp.chemitech.net.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://de.shtwfgs.cn

[E14] URL 编码与 Base64
来源：http://tv.chemitech.net.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://js.yuntaijiaju.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://tq.newstarts.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://sw.huixiangedu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ew.9csxet.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xa.panjiajie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jj.bookmarksfly.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pk.muxihuayi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nh.asd995.cn

[E15] HTML 转义 / 反转义
来源：http://wq.hnjuh.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://co.huixiangedu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bi.9csxet.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://te.huanxung.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://al.asd995.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bj.szxytkj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qs.haigaiapp.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cw.newstarts.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bn.hahajie.cn

[E16] 数字千分位
来源：http://cb.jianghongdianzi.cn

Py:   f"{1234567:,}"
来源：http://jr.9csxet.cn

PHP:  number_format(1234567);
来源：http://jk.huixinmuqiang.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://na.yuntaijiaju.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://el.jctech888.com.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zv.yuntaijiaju.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dp.panjiajie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wa.colortex.cn

C#:   1234567.ToString("N0")
来源：http://uo.chemitech.net.cn

[E17] 首字母大写
来源：http://lx.yuexingan06.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://oy.szxytkj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://qe.yuntaijiaju.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://br.lnxyls.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hc.huixiangedu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xg.jianghongdianzi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ag.nszjky.cn

Ruby: s.capitalize
来源：http://lr.jctech888.com.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://oe.haigaiapp.cn

[E18] 模板占位符替换
来源：http://rb.lnxyls.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nd.nszjky.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tk.wgjwhj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://lq.szsharing.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://vw.colortex.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qq.szsharing.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jp.gzmigu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lf.colortex.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://im.yuntaijiaju.cn

[E19] 多行文本按行拆分
来源：http://ts.nszjky.cn

Py:   s.splitlines()
来源：http://jf.bookmarksfly.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kk.nicolike.cn

JS:   s.split(/\r?\n/)
来源：http://yn.bjjhwx.cn

TS:   s.split(/\r?\n/)
来源：http://cx.521024.cn

Java: s.lines().toList()
来源：http://dq.jianghongdianzi.cn

Go:   strings.Split(s, "\n")
来源：http://ke.haigaiapp.cn

Ruby: s.lines
来源：http://et.nszjky.cn

C#:   s.Split('\n')
来源：http://bq.huixinmuqiang.cn

[E20] 判断字符串是否为空
来源：http://yl.panjiajie.cn

Py:   if not s:
来源：http://lt.shtwfgs.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cr.asd995.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fe.nszjky.cn

TS:   if (s === "") {}
来源：http://uu.muxihuayi.cn

Java: if (s.isEmpty()) {}
来源：http://ao.colortex.cn

Go:   if s == "" {}
来源：http://mf.gzmigu.cn

Ruby: if s.empty?
来源：http://vd.gzmigu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qc.521024.cn

[E21] 超长截断加省略号
来源：http://ku.yuexingan06.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ev.jctech888.com.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hu.colortex.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bj.muxihuayi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xy.newstarts.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cp.szxytkj.cn

Go:   // 按 rune 判断长度后截断
来源：http://mg.shtwfgs.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gj.chemitech.net.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mc.shtwfgs.cn

[E22] 字节长度与字符长度
来源：http://uc.panjiajie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ia.huanxung.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mh.nszjky.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dz.szsharing.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tg.newstarts.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jr.nicolike.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wp.nicolike.cn

Ruby: s.bytesize;  s.length
来源：http://vc.hnjuh.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://om.huixinmuqiang.cn

================================================================================
来源：http://jz.lnxyls.cn

F. 文件与目录
来源：http://vv.huixinmuqiang.cn

================================================================================
来源：http://jw.jianghongdianzi.cn

[F01] 读取整个文件
来源：http://sv.hnjuh.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://iu.shxzskj.cn

PHP:  file_get_contents("a.txt");
来源：http://ag.chemitech.net.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ds.shtwfgs.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://am.chemitech.net.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://sm.colortex.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ok.521024.cn

Ruby: File.read("a.txt")
来源：http://ly.colortex.cn

C#:   File.ReadAllText("a.txt");
来源：http://js.bjjhwx.cn

[F02] 逐行读取文件
来源：http://qx.521024.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bf.szsharing.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qd.hnjuh.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kc.shtwfgs.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ek.colortex.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://va.huixinmuqiang.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qg.muxihuayi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://by.hahajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yc.chemitech.net.cn

[F03] 写入文件（覆盖）
来源：http://is.newstarts.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hg.haigaiapp.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://bk.hnjuh.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ta.lnxyls.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tq.9csxet.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tz.bookmarksfly.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nj.yuexingan06.cn

Ruby: File.write("a.txt", "hi")
来源：http://iz.colortex.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mm.panjiajie.cn

[F04] 追加写入文件
来源：http://id.chemitech.net.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xb.nicolike.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mv.panjiajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pu.colortex.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ra.huixinmuqiang.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gy.yuntaijiaju.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://sq.nicolike.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nq.colortex.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ww.haigaiapp.cn

[F05] 判断文件或目录是否存在
来源：http://kx.gzmigu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ae.lnxyls.cn

PHP:  file_exists("a.txt");
来源：http://sy.yuntaijiaju.cn

JS:   fs.existsSync("a.txt")
来源：http://la.haigaiapp.cn

TS:   fs.existsSync("a.txt")
来源：http://lw.hahajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://rj.nicolike.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vo.9csxet.cn

Ruby: File.exist?("a.txt")
来源：http://dj.jianghongdianzi.cn

C#:   File.Exists("a.txt")
来源：http://os.szxytkj.cn

[F06] 删除文件
来源：http://zt.asd995.cn

Py:   os.remove("a.txt")
来源：http://rp.muxihuayi.cn

PHP:  unlink("a.txt");
来源：http://jv.bookmarksfly.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ts.nicolike.cn

TS:   fs.unlinkSync("a.txt")
来源：http://af.huixiangedu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ju.shxzukj.cn

Go:   os.Remove("a.txt")
来源：http://px.huanxung.cn

Ruby: File.delete("a.txt")
来源：http://rl.szsharing.cn

C#:   File.Delete("a.txt");
来源：http://rl.wgjwhj.cn

[F07] 创建目录（含多级）
来源：http://ab.huixinmuqiang.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vz.szsharing.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lh.jianghongdianzi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ak.szsharing.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ny.panjiajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ma.wgjwhj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ag.shxzskj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zx.nszjky.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gh.wgjwhj.cn

[F08] 遍历目录
来源：http://lj.shtwfgs.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://un.szsharing.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vs.hahajie.cn

JS:   fs.readdirSync("dir")
来源：http://ym.huixinmuqiang.cn

TS:   fs.readdirSync("dir")
来源：http://nw.yuexingan06.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ci.gzmigu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://wo.hnjuh.cn

Ruby: Dir.children("dir")
来源：http://th.huixinmuqiang.cn

C#:   Directory.GetFiles("dir")
来源：http://wc.shtwfgs.cn

[F09] 获取文件大小
来源：http://sv.szsharing.cn

Py:   os.path.getsize("a.txt")
来源：http://av.yuntaijiaju.cn

PHP:  filesize("a.txt");
来源：http://rk.yuexingan06.cn

JS:   fs.statSync("a.txt").size
来源：http://gz.wgjwhj.cn

TS:   fs.statSync("a.txt").size
来源：http://og.huanxung.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ed.yuntaijiaju.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ux.hnjuh.cn

Ruby: File.size("a.txt")
来源：http://sa.szxytkj.cn

C#:   new FileInfo("a.txt").Length
来源：http://rz.bookmarksfly.cn

[F10] 取文件扩展名 / 文件名
来源：http://ac.szxytkj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pi.colortex.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kp.yuexingan06.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://oo.jianghongdianzi.cn

TS:   path.extname("a.txt")
来源：http://uh.muxihuayi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xy.szsharing.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ii.muxihuayi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ur.yuexingan06.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ot.yuexingan06.cn

[F11] 复制与移动文件
来源：http://ai.muxihuayi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mb.huanxung.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pz.asd995.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ij.hnjuh.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hc.bjjhwx.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ip.wgjwhj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ut.shtwfgs.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ub.jctech888.com.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wa.bjjhwx.cn

[F12] CSV 读写
来源：http://xy.521024.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rv.hnjuh.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zm.shxzukj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fw.newstarts.cn

TS:   // 同上
来源：http://dx.hnjuh.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fy.521024.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ne.shxzukj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zm.bjjhwx.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://rx.nicolike.cn

================================================================================
来源：http://we.huixiangedu.cn

G. 面向对象
来源：http://ig.lnxyls.cn

================================================================================
来源：http://ch.hnjuh.cn

[G01] 定义类
来源：http://wt.newstarts.cn

Py:   class User: pass
来源：http://fc.colortex.cn

PHP:  class User {}
来源：http://vv.muxihuayi.cn

JS:   class User {}
来源：http://xc.haigaiapp.cn

TS:   class User { name: string = ""; }
来源：http://bn.521024.cn

Java: class User {}
来源：http://za.panjiajie.cn

Go:   type User struct { Name string }
来源：http://fm.lnxyls.cn

Ruby: class User; end
来源：http://nf.nicolike.cn

C#:   class User {}
来源：http://of.hahajie.cn

[G02] 构造函数
来源：http://hf.muxihuayi.cn

Py:   def __init__(self, name): self.name = name
来源：http://nc.lnxyls.cn

PHP:  public function __construct(public string $name) {}
来源：http://vn.szxytkj.cn

JS:   constructor(name) { this.name = name; }
来源：http://wa.asd995.cn

TS:   constructor(public name: string) {}
来源：http://fy.shtwfgs.cn

Java: User(String name) { this.name = name; }
来源：http://vc.shtwfgs.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ix.yuexingan06.cn

Ruby: def initialize(name); @name = name; end
来源：http://ew.huixinmuqiang.cn

C#:   public User(string name) { Name = name; }
来源：http://ow.asd995.cn

[G03] 实例属性
来源：http://rc.chemitech.net.cn

Py:   self.name = "x"
来源：http://kn.9csxet.cn

PHP:  public string $name = "x";
来源：http://ks.gzmigu.cn

JS:   this.name = "x";
来源：http://jz.newstarts.cn

TS:   name: string = "x";
来源：http://qf.huixiangedu.cn

Java: private String name;
来源：http://ks.hahajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sy.newstarts.cn

Ruby: @name = "x"
来源：http://wx.bookmarksfly.cn

C#:   public string Name { get; set; } = "x";
来源：http://ra.huixinmuqiang.cn

[G04] 定义方法
来源：http://en.huanxung.cn

Py:   def greet(self): return self.name
来源：http://qx.521024.cn


<!-- 参考信息 -->