代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cv.shxzskj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rw.bjjhwx.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zh.9csxet.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ev.gzmigu.cn

[E06] 替换子串
来源：http://fy.muxihuayi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xg.asd995.cn

PHP:  str_replace("a", "b", $s);
来源：http://of.lnxyls.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hm.bookmarksfly.cn

TS:   s.replaceAll("a", "b")
来源：http://yg.chemitech.net.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xs.jianghongdianzi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nt.nicolike.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bq.colortex.cn

C#:   s.Replace("a", "b")
来源：http://os.jianghongdianzi.cn

[E07] 按分隔符拆分
来源：http://bb.chemitech.net.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ei.nszjky.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rf.bookmarksfly.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://wg.jianghongdianzi.cn

TS:   s.split(",")
来源：http://pz.bjjhwx.cn

Java: s.split(",");  s.split("\\s+")
来源：http://kf.huanxung.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pc.huanxung.cn

Ruby: s.split(",");  s.split
来源：http://nb.huanxung.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gv.lnxyls.cn

[E08] 数组按分隔符合并
来源：http://qi.muxihuayi.cn

Py:   ",".join(items)
来源：http://pt.521024.cn

PHP:  implode(",", $items);
来源：http://jr.yuntaijiaju.cn

JS:   items.join(",")
来源：http://ig.bjjhwx.cn

TS:   items.join(",")
来源：http://ls.huixinmuqiang.cn

Java: String.join(",", items)
来源：http://hh.huixiangedu.cn

Go:   strings.Join(items, ",")
来源：http://vv.huixinmuqiang.cn

Ruby: items.join(",")
来源：http://oa.jctech888.com.cn

C#:   string.Join(",", items)
来源：http://zz.szsharing.cn

[E09] 去除所有空白字符
来源：http://pg.yuntaijiaju.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://yv.muxihuayi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xe.huixinmuqiang.cn

JS:   s.replace(/\s+/g, "")
来源：http://mq.9csxet.cn

TS:   s.replace(/\s+/g, "")
来源：http://ur.hnjuh.cn

Java: s.replaceAll("\\s+", "")
来源：http://sf.nszjky.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://zg.521024.cn

Ruby: s.gsub(/\s+/, "")
来源：http://hk.haigaiapp.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vn.muxihuayi.cn

[E10] 左侧补零 / 定长填充
来源：http://cf.chemitech.net.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://td.huixiangedu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ij.nicolike.cn

JS:   "7".padStart(3, "0")
来源：http://rc.panjiajie.cn

TS:   "7".padStart(3, "0")
来源：http://qp.nicolike.cn

Java: String.format("%03d", 7)
来源：http://wv.newstarts.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://hh.yuntaijiaju.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bw.bookmarksfly.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xx.bookmarksfly.cn

[E11] 反转字符串
来源：http://qd.jctech888.com.cn

Py:   s[::-1]
来源：http://pu.nicolike.cn

PHP:  strrev($s);
来源：http://em.nicolike.cn

JS:   [...s].reverse().join("")
来源：http://ou.9csxet.cn

TS:   [...s].reverse().join("")
来源：http://fr.yuexingan06.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://sy.bjjhwx.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://vx.wgjwhj.cn

Ruby: s.reverse
来源：http://vq.gzmigu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ym.yuexingan06.cn

[E12] 统计某字符出现次数
来源：http://le.haigaiapp.cn

Py:   s.count("a")
来源：http://tb.haigaiapp.cn

PHP:  substr_count($s, "a");
来源：http://iy.bjjhwx.cn

JS:   s.split("a").length - 1
来源：http://en.shxzskj.cn

TS:   s.split("a").length - 1
来源：http://uo.muxihuayi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://me.colortex.cn

Go:   strings.Count(s, "a")
来源：http://xy.yuntaijiaju.cn

Ruby: s.count("a")
来源：http://jy.huanxung.cn

C#:   s.Count(c => c == 'a')
来源：http://md.yuexingan06.cn

[E13] 逐字符遍历
来源：http://lx.jianghongdianzi.cn

Py:   for ch in s: print(ch)
来源：http://ai.shtwfgs.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ol.lnxyls.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://np.panjiajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ce.muxihuayi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zi.nszjky.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lv.hahajie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://so.hnjuh.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://os.lnxyls.cn

[E14] URL 编码与 Base64
来源：http://hw.shxzskj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sg.bjjhwx.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://dp.chemitech.net.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://we.shxzukj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://iq.lnxyls.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wa.asd995.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ue.yuexingan06.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://up.shxzskj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hx.muxihuayi.cn

[E15] HTML 转义 / 反转义
来源：http://pd.chemitech.net.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://bj.nicolike.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://af.haigaiapp.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ds.jctech888.com.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://st.colortex.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vt.bjjhwx.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ub.bookmarksfly.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bk.asd995.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mu.hnjuh.cn

[E16] 数字千分位
来源：http://dl.szxytkj.cn

Py:   f"{1234567:,}"
来源：http://bj.lnxyls.cn

PHP:  number_format(1234567);
来源：http://to.9csxet.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://eg.newstarts.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://pq.nicolike.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ga.wgjwhj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ur.wgjwhj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pa.asd995.cn

C#:   1234567.ToString("N0")
来源：http://vr.shxzskj.cn

[E17] 首字母大写
来源：http://yr.szxytkj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qj.wgjwhj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xo.szsharing.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hj.bjjhwx.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ir.wgjwhj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wj.szsharing.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qn.jctech888.com.cn

Ruby: s.capitalize
来源：http://xq.wgjwhj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xc.bjjhwx.cn

[E18] 模板占位符替换
来源：http://gh.colortex.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fj.shxzukj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ow.nszjky.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zt.chemitech.net.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://nc.hnjuh.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jb.yuexingan06.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zs.szxytkj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vq.hahajie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://do.chemitech.net.cn

[E19] 多行文本按行拆分
来源：http://bh.colortex.cn

Py:   s.splitlines()
来源：http://nv.haigaiapp.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jl.yuntaijiaju.cn

JS:   s.split(/\r?\n/)
来源：http://sv.9csxet.cn

TS:   s.split(/\r?\n/)
来源：http://ph.521024.cn

Java: s.lines().toList()
来源：http://tt.muxihuayi.cn

Go:   strings.Split(s, "\n")
来源：http://ct.szxytkj.cn

Ruby: s.lines
来源：http://zz.colortex.cn

C#:   s.Split('\n')
来源：http://di.hnjuh.cn

[E20] 判断字符串是否为空
来源：http://yq.wgjwhj.cn

Py:   if not s:
来源：http://wl.panjiajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://aj.9csxet.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nh.jctech888.com.cn

TS:   if (s === "") {}
来源：http://em.bjjhwx.cn

Java: if (s.isEmpty()) {}
来源：http://ix.hahajie.cn

Go:   if s == "" {}
来源：http://fm.hahajie.cn

Ruby: if s.empty?
来源：http://gg.newstarts.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fp.bookmarksfly.cn

[E21] 超长截断加省略号
来源：http://oo.shtwfgs.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ot.newstarts.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zi.gzmigu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oq.shxzskj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://an.colortex.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dy.huanxung.cn

Go:   // 按 rune 判断长度后截断
来源：http://dc.hnjuh.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wf.huixiangedu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sr.jctech888.com.cn

[E22] 字节长度与字符长度
来源：http://jq.muxihuayi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ea.shxzukj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xd.lnxyls.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pt.gzmigu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kg.jctech888.com.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yu.chemitech.net.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gj.yuexingan06.cn

Ruby: s.bytesize;  s.length
来源：http://kd.huanxung.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hh.hahajie.cn

================================================================================
来源：http://xm.huixiangedu.cn

F. 文件与目录
来源：http://zf.nicolike.cn

================================================================================
来源：http://bx.hahajie.cn

[F01] 读取整个文件
来源：http://uc.huixinmuqiang.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ct.hnjuh.cn

PHP:  file_get_contents("a.txt");
来源：http://ja.jctech888.com.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://aw.jctech888.com.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ch.hnjuh.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://tg.gzmigu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kd.huixinmuqiang.cn

Ruby: File.read("a.txt")
来源：http://qg.nicolike.cn

C#:   File.ReadAllText("a.txt");
来源：http://oi.szxytkj.cn

[F02] 逐行读取文件
来源：http://fi.nicolike.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wk.newstarts.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://an.szsharing.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pn.szsharing.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xj.panjiajie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fn.bookmarksfly.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rl.nicolike.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zt.shxzukj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tq.hnjuh.cn

[F03] 写入文件（覆盖）
来源：http://hu.asd995.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tf.gzmigu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://zu.nicolike.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://es.panjiajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gi.shtwfgs.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://un.nszjky.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://go.nszjky.cn

Ruby: File.write("a.txt", "hi")
来源：http://cn.521024.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://du.521024.cn

[F04] 追加写入文件
来源：http://gb.shxzskj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yj.521024.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://is.asd995.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cz.panjiajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ib.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xn.hahajie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ka.bookmarksfly.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://na.jianghongdianzi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vk.9csxet.cn

[F05] 判断文件或目录是否存在
来源：http://hs.nicolike.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rn.bookmarksfly.cn

PHP:  file_exists("a.txt");
来源：http://fw.nicolike.cn

JS:   fs.existsSync("a.txt")
来源：http://du.hnjuh.cn

TS:   fs.existsSync("a.txt")
来源：http://ll.newstarts.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://zt.colortex.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fv.lnxyls.cn

Ruby: File.exist?("a.txt")
来源：http://sb.chemitech.net.cn

C#:   File.Exists("a.txt")
来源：http://eo.gzmigu.cn

[F06] 删除文件
来源：http://gc.yuntaijiaju.cn

Py:   os.remove("a.txt")
来源：http://tk.szsharing.cn

PHP:  unlink("a.txt");
来源：http://qj.nszjky.cn

JS:   fs.unlinkSync("a.txt")
来源：http://be.huixinmuqiang.cn

TS:   fs.unlinkSync("a.txt")
来源：http://qm.wgjwhj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://we.asd995.cn

Go:   os.Remove("a.txt")
来源：http://qv.bjjhwx.cn

Ruby: File.delete("a.txt")
来源：http://fh.9csxet.cn

C#:   File.Delete("a.txt");
来源：http://df.huixiangedu.cn

[F07] 创建目录（含多级）
来源：http://ft.newstarts.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mf.huixinmuqiang.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uz.jctech888.com.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ej.szxytkj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nx.yuntaijiaju.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ai.huanxung.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jd.szsharing.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xf.9csxet.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://py.gzmigu.cn

[F08] 遍历目录
来源：http://qy.bookmarksfly.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://qo.nszjky.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tt.jianghongdianzi.cn

JS:   fs.readdirSync("dir")
来源：http://hg.szsharing.cn

TS:   fs.readdirSync("dir")
来源：http://rz.panjiajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yh.szxytkj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://jt.wgjwhj.cn

Ruby: Dir.children("dir")
来源：http://la.lnxyls.cn

C#:   Directory.GetFiles("dir")
来源：http://be.lnxyls.cn

[F09] 获取文件大小
来源：http://ts.wgjwhj.cn

Py:   os.path.getsize("a.txt")
来源：http://lw.yuexingan06.cn

PHP:  filesize("a.txt");
来源：http://ou.shxzukj.cn

JS:   fs.statSync("a.txt").size
来源：http://qq.muxihuayi.cn

TS:   fs.statSync("a.txt").size
来源：http://fm.newstarts.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ys.wgjwhj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://uf.hnjuh.cn

Ruby: File.size("a.txt")
来源：http://cm.shxzskj.cn

C#:   new FileInfo("a.txt").Length
来源：http://jf.shxzukj.cn

[F10] 取文件扩展名 / 文件名
来源：http://jf.521024.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://yz.yuexingan06.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://il.colortex.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qz.shtwfgs.cn

TS:   path.extname("a.txt")
来源：http://cf.hahajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xp.szxytkj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vy.haigaiapp.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dl.szsharing.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://at.yuntaijiaju.cn

[F11] 复制与移动文件
来源：http://cm.shxzukj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ye.haigaiapp.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://oa.colortex.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hv.colortex.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hb.521024.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vs.yuexingan06.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xn.newstarts.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://py.szsharing.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lw.bookmarksfly.cn

[F12] CSV 读写
来源：http://ny.haigaiapp.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ez.shtwfgs.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yi.lnxyls.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://oe.szxytkj.cn

TS:   // 同上
来源：http://rw.shxzukj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dq.bookmarksfly.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hx.yuexingan06.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qa.wgjwhj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://oy.muxihuayi.cn

================================================================================
来源：http://xi.hahajie.cn

G. 面向对象
来源：http://at.9csxet.cn

================================================================================
来源：http://zi.newstarts.cn

[G01] 定义类
来源：http://yk.newstarts.cn

Py:   class User: pass
来源：http://je.521024.cn

PHP:  class User {}
来源：http://nr.colortex.cn

JS:   class User {}
来源：http://mq.szsharing.cn

TS:   class User { name: string = ""; }
来源：http://mq.haigaiapp.cn

Java: class User {}
来源：http://ev.huixiangedu.cn

Go:   type User struct { Name string }
来源：http://gg.521024.cn

Ruby: class User; end
来源：http://jt.gzmigu.cn

C#:   class User {}
来源：http://gq.huixiangedu.cn

[G02] 构造函数
来源：http://mz.hahajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://sv.huixiangedu.cn

PHP:  public function __construct(public string $name) {}
来源：http://eh.colortex.cn

JS:   constructor(name) { this.name = name; }
来源：http://ta.huixiangedu.cn

TS:   constructor(public name: string) {}
来源：http://qq.yuntaijiaju.cn

Java: User(String name) { this.name = name; }
来源：http://vh.521024.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ij.wgjwhj.cn

Ruby: def initialize(name); @name = name; end
来源：http://yr.shtwfgs.cn

C#:   public User(string name) { Name = name; }
来源：http://rc.haigaiapp.cn

[G03] 实例属性
来源：http://qf.yuexingan06.cn

Py:   self.name = "x"
来源：http://dd.asd995.cn

PHP:  public string $name = "x";
来源：http://po.shtwfgs.cn

JS:   this.name = "x";
来源：http://ck.newstarts.cn

TS:   name: string = "x";
来源：http://ek.colortex.cn

Java: private String name;
来源：http://an.chemitech.net.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fw.521024.cn

Ruby: @name = "x"
来源：http://zj.jianghongdianzi.cn

C#:   public string Name { get; set; } = "x";
来源：http://rg.shtwfgs.cn

[G04] 定义方法
来源：http://sz.jctech888.com.cn

Py:   def greet(self): return self.name
来源：http://hb.asd995.cn


<!-- 参考信息 -->