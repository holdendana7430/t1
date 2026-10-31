代发 wailian999

[E06] 替换子串
来源：http://st.newstarts.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ti.haigaiapp.cn

PHP:  str_replace("a", "b", $s);
来源：http://vg.colortex.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nw.jianghongdianzi.cn

TS:   s.replaceAll("a", "b")
来源：http://yv.szxytkj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bo.huixinmuqiang.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vh.lnxyls.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nt.nszjky.cn

C#:   s.Replace("a", "b")
来源：http://mr.asd995.cn

[E07] 按分隔符拆分
来源：http://fc.huanxung.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ws.yuntaijiaju.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gs.gzmigu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://gx.szsharing.cn

TS:   s.split(",")
来源：http://yz.huanxung.cn

Java: s.split(",");  s.split("\\s+")
来源：http://od.bjjhwx.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qv.asd995.cn

Ruby: s.split(",");  s.split
来源：http://vu.jctech888.com.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ok.colortex.cn

[E08] 数组按分隔符合并
来源：http://dg.muxihuayi.cn

Py:   ",".join(items)
来源：http://ev.huixinmuqiang.cn

PHP:  implode(",", $items);
来源：http://gc.lnxyls.cn

JS:   items.join(",")
来源：http://hm.gzmigu.cn

TS:   items.join(",")
来源：http://kj.asd995.cn

Java: String.join(",", items)
来源：http://xf.panjiajie.cn

Go:   strings.Join(items, ",")
来源：http://be.colortex.cn

Ruby: items.join(",")
来源：http://tb.haigaiapp.cn

C#:   string.Join(",", items)
来源：http://sb.jianghongdianzi.cn

[E09] 去除所有空白字符
来源：http://wn.szsharing.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://yf.shtwfgs.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ae.hnjuh.cn

JS:   s.replace(/\s+/g, "")
来源：http://go.shxzskj.cn

TS:   s.replace(/\s+/g, "")
来源：http://we.9csxet.cn

Java: s.replaceAll("\\s+", "")
来源：http://rv.muxihuayi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ek.huanxung.cn

Ruby: s.gsub(/\s+/, "")
来源：http://jg.muxihuayi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sy.9csxet.cn

[E10] 左侧补零 / 定长填充
来源：http://zj.huixinmuqiang.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qx.asd995.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xu.newstarts.cn

JS:   "7".padStart(3, "0")
来源：http://zw.yuexingan06.cn

TS:   "7".padStart(3, "0")
来源：http://iw.lnxyls.cn

Java: String.format("%03d", 7)
来源：http://xl.bookmarksfly.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://rh.colortex.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kk.muxihuayi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://py.chemitech.net.cn

[E11] 反转字符串
来源：http://ox.szsharing.cn

Py:   s[::-1]
来源：http://tj.nszjky.cn

PHP:  strrev($s);
来源：http://yd.szxytkj.cn

JS:   [...s].reverse().join("")
来源：http://vp.shtwfgs.cn

TS:   [...s].reverse().join("")
来源：http://pp.bjjhwx.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wl.lnxyls.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ce.9csxet.cn

Ruby: s.reverse
来源：http://iq.yuexingan06.cn

C#:   new string(s.Reverse().ToArray())
来源：http://jk.lnxyls.cn

[E12] 统计某字符出现次数
来源：http://ja.asd995.cn

Py:   s.count("a")
来源：http://dy.huixinmuqiang.cn

PHP:  substr_count($s, "a");
来源：http://jl.gzmigu.cn

JS:   s.split("a").length - 1
来源：http://re.wgjwhj.cn

TS:   s.split("a").length - 1
来源：http://ux.hnjuh.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://aj.bjjhwx.cn

Go:   strings.Count(s, "a")
来源：http://zn.asd995.cn

Ruby: s.count("a")
来源：http://nj.shxzskj.cn

C#:   s.Count(c => c == 'a')
来源：http://ce.haigaiapp.cn

[E13] 逐字符遍历
来源：http://ff.bookmarksfly.cn

Py:   for ch in s: print(ch)
来源：http://dy.huanxung.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://eo.521024.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://de.szxytkj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ow.jianghongdianzi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://nz.szsharing.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gf.szsharing.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ss.huanxung.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pz.hnjuh.cn

[E14] URL 编码与 Base64
来源：http://ny.wgjwhj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mc.9csxet.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://lo.yuntaijiaju.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pf.huanxung.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://iy.shtwfgs.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gl.asd995.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ti.huanxung.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ak.jctech888.com.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wo.muxihuayi.cn

[E15] HTML 转义 / 反转义
来源：http://nw.jctech888.com.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://nk.nicolike.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ji.panjiajie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://oa.shxzukj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ph.chemitech.net.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vb.huanxung.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ox.colortex.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tv.newstarts.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vx.szsharing.cn

[E16] 数字千分位
来源：http://ez.newstarts.cn

Py:   f"{1234567:,}"
来源：http://nu.huanxung.cn

PHP:  number_format(1234567);
来源：http://re.hnjuh.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://se.huixiangedu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://me.muxihuayi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://js.shxzskj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ka.asd995.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bb.asd995.cn

C#:   1234567.ToString("N0")
来源：http://og.shtwfgs.cn

[E17] 首字母大写
来源：http://tg.asd995.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://er.shxzukj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://yp.nicolike.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://np.jctech888.com.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mq.szxytkj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wx.hnjuh.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ii.huanxung.cn

Ruby: s.capitalize
来源：http://rv.huanxung.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ag.colortex.cn

[E18] 模板占位符替换
来源：http://cu.panjiajie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yq.hahajie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ho.szsharing.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://jq.newstarts.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://vh.chemitech.net.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fo.huanxung.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://iw.muxihuayi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kj.szsharing.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://if.9csxet.cn

[E19] 多行文本按行拆分
来源：http://ga.lnxyls.cn

Py:   s.splitlines()
来源：http://qt.jctech888.com.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gq.lnxyls.cn

JS:   s.split(/\r?\n/)
来源：http://xc.colortex.cn

TS:   s.split(/\r?\n/)
来源：http://du.panjiajie.cn

Java: s.lines().toList()
来源：http://kj.huixiangedu.cn

Go:   strings.Split(s, "\n")
来源：http://oc.szsharing.cn

Ruby: s.lines
来源：http://kr.jctech888.com.cn

C#:   s.Split('\n')
来源：http://im.9csxet.cn

[E20] 判断字符串是否为空
来源：http://pc.colortex.cn

Py:   if not s:
来源：http://ju.colortex.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zk.bookmarksfly.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kt.bookmarksfly.cn

TS:   if (s === "") {}
来源：http://am.huixinmuqiang.cn

Java: if (s.isEmpty()) {}
来源：http://ra.newstarts.cn

Go:   if s == "" {}
来源：http://xi.hahajie.cn

Ruby: if s.empty?
来源：http://sz.9csxet.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ut.asd995.cn

[E21] 超长截断加省略号
来源：http://lh.9csxet.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lb.shxzukj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pq.huanxung.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ff.bookmarksfly.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bv.nszjky.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bu.huixiangedu.cn

Go:   // 按 rune 判断长度后截断
来源：http://ri.jctech888.com.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xw.shxzskj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hv.521024.cn

[E22] 字节长度与字符长度
来源：http://ih.yuntaijiaju.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kg.hnjuh.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ut.huanxung.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rr.nicolike.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yk.szsharing.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qn.szxytkj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zj.521024.cn

Ruby: s.bytesize;  s.length
来源：http://av.jctech888.com.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zz.hahajie.cn

================================================================================
来源：http://ac.gzmigu.cn

F. 文件与目录
来源：http://na.bjjhwx.cn

================================================================================
来源：http://em.hnjuh.cn

[F01] 读取整个文件
来源：http://bi.yuntaijiaju.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bs.jianghongdianzi.cn

PHP:  file_get_contents("a.txt");
来源：http://od.szxytkj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://td.jctech888.com.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dd.nicolike.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://oo.colortex.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zi.newstarts.cn

Ruby: File.read("a.txt")
来源：http://wb.newstarts.cn

C#:   File.ReadAllText("a.txt");
来源：http://aq.huanxung.cn

[F02] 逐行读取文件
来源：http://im.huixiangedu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pv.colortex.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jl.haigaiapp.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fe.huixinmuqiang.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vi.nicolike.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uw.panjiajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://we.lnxyls.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xk.yuntaijiaju.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yw.yuntaijiaju.cn

[F03] 写入文件（覆盖）
来源：http://tc.yuexingan06.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tj.nicolike.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://nk.nszjky.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://op.chemitech.net.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sn.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rv.haigaiapp.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://go.521024.cn

Ruby: File.write("a.txt", "hi")
来源：http://hv.lnxyls.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://sd.hnjuh.cn

[F04] 追加写入文件
来源：http://ks.newstarts.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mp.asd995.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yz.panjiajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fx.huixinmuqiang.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sy.hnjuh.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qz.muxihuayi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hu.muxihuayi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ki.jianghongdianzi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nw.yuexingan06.cn

[F05] 判断文件或目录是否存在
来源：http://cm.huanxung.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ko.hahajie.cn

PHP:  file_exists("a.txt");
来源：http://ma.hahajie.cn

JS:   fs.existsSync("a.txt")
来源：http://qi.shxzskj.cn

TS:   fs.existsSync("a.txt")
来源：http://at.521024.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qe.muxihuayi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ui.wgjwhj.cn

Ruby: File.exist?("a.txt")
来源：http://iv.jianghongdianzi.cn

C#:   File.Exists("a.txt")
来源：http://pg.colortex.cn

[F06] 删除文件
来源：http://bn.hahajie.cn

Py:   os.remove("a.txt")
来源：http://pj.haigaiapp.cn

PHP:  unlink("a.txt");
来源：http://vv.bookmarksfly.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ej.huixiangedu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://rl.lnxyls.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://av.shxzukj.cn

Go:   os.Remove("a.txt")
来源：http://yj.gzmigu.cn

Ruby: File.delete("a.txt")
来源：http://it.chemitech.net.cn

C#:   File.Delete("a.txt");
来源：http://wr.bjjhwx.cn

[F07] 创建目录（含多级）
来源：http://py.lnxyls.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gq.szsharing.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pe.newstarts.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pf.newstarts.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qd.lnxyls.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rf.haigaiapp.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yg.chemitech.net.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fc.asd995.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zo.shtwfgs.cn

[F08] 遍历目录
来源：http://pi.colortex.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ka.huixinmuqiang.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sx.szxytkj.cn

JS:   fs.readdirSync("dir")
来源：http://hh.lnxyls.cn

TS:   fs.readdirSync("dir")
来源：http://cj.hahajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://za.shxzukj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://wb.521024.cn

Ruby: Dir.children("dir")
来源：http://ke.yuntaijiaju.cn

C#:   Directory.GetFiles("dir")
来源：http://lt.haigaiapp.cn

[F09] 获取文件大小
来源：http://hp.bookmarksfly.cn

Py:   os.path.getsize("a.txt")
来源：http://sy.panjiajie.cn

PHP:  filesize("a.txt");
来源：http://tu.521024.cn

JS:   fs.statSync("a.txt").size
来源：http://gy.hnjuh.cn

TS:   fs.statSync("a.txt").size
来源：http://nr.shtwfgs.cn

Java: Files.size(Path.of("a.txt"))
来源：http://gr.nszjky.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://sx.huixinmuqiang.cn

Ruby: File.size("a.txt")
来源：http://ga.yuntaijiaju.cn

C#:   new FileInfo("a.txt").Length
来源：http://yq.jctech888.com.cn

[F10] 取文件扩展名 / 文件名
来源：http://vr.jctech888.com.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ee.yuexingan06.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://sn.jctech888.com.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qf.colortex.cn

TS:   path.extname("a.txt")
来源：http://lw.9csxet.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cv.szsharing.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ma.huixinmuqiang.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ab.shxzukj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ez.szsharing.cn

[F11] 复制与移动文件
来源：http://ot.yuntaijiaju.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hi.shxzskj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://oa.521024.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://av.chemitech.net.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cs.hnjuh.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fm.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qt.panjiajie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ov.huixinmuqiang.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://td.szsharing.cn

[F12] CSV 读写
来源：http://sr.huanxung.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vb.yuexingan06.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fq.lnxyls.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ko.wgjwhj.cn

TS:   // 同上
来源：http://rw.nszjky.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xr.hahajie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ui.hnjuh.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ts.bookmarksfly.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://if.haigaiapp.cn

================================================================================
来源：http://vh.haigaiapp.cn

G. 面向对象
来源：http://dd.9csxet.cn

================================================================================
来源：http://ze.huanxung.cn

[G01] 定义类
来源：http://ts.yuntaijiaju.cn

Py:   class User: pass
来源：http://lp.muxihuayi.cn

PHP:  class User {}
来源：http://xm.nicolike.cn

JS:   class User {}
来源：http://qd.yuexingan06.cn

TS:   class User { name: string = ""; }
来源：http://rx.chemitech.net.cn

Java: class User {}
来源：http://sb.yuntaijiaju.cn

Go:   type User struct { Name string }
来源：http://jl.szsharing.cn

Ruby: class User; end
来源：http://ex.muxihuayi.cn

C#:   class User {}
来源：http://pg.panjiajie.cn

[G02] 构造函数
来源：http://ma.jianghongdianzi.cn

Py:   def __init__(self, name): self.name = name
来源：http://hv.haigaiapp.cn

PHP:  public function __construct(public string $name) {}
来源：http://xi.huanxung.cn

JS:   constructor(name) { this.name = name; }
来源：http://um.chemitech.net.cn

TS:   constructor(public name: string) {}
来源：http://ql.huixinmuqiang.cn

Java: User(String name) { this.name = name; }
来源：http://nu.asd995.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lq.bjjhwx.cn

Ruby: def initialize(name); @name = name; end
来源：http://no.bookmarksfly.cn

C#:   public User(string name) { Name = name; }
来源：http://tq.huanxung.cn

[G03] 实例属性
来源：http://bg.szxytkj.cn

Py:   self.name = "x"
来源：http://ik.huanxung.cn

PHP:  public string $name = "x";
来源：http://vz.yuntaijiaju.cn

JS:   this.name = "x";
来源：http://pl.colortex.cn

TS:   name: string = "x";
来源：http://hx.haigaiapp.cn

Java: private String name;
来源：http://hp.bjjhwx.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fu.jctech888.com.cn

Ruby: @name = "x"
来源：http://yj.huixinmuqiang.cn

C#:   public string Name { get; set; } = "x";
来源：http://oo.huixinmuqiang.cn

[G04] 定义方法
来源：http://db.shxzukj.cn

Py:   def greet(self): return self.name
来源：http://vw.yuntaijiaju.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://so.haigaiapp.cn

JS:   greet() { return this.name; }
来源：http://as.asd995.cn

TS:   greet(): string { return this.name; }
来源：http://zo.yuntaijiaju.cn

Java: String greet() { return name; }
来源：http://li.huixiangedu.cn


<!-- 参考信息 -->