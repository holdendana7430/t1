代发 wailian999

[E06] 替换子串
来源：http://jn.shxzskj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://de.asd995.cn

PHP:  str_replace("a", "b", $s);
来源：http://py.hahajie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fv.hnjuh.cn

TS:   s.replaceAll("a", "b")
来源：http://od.asd995.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sw.lnxyls.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fs.lnxyls.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://am.hahajie.cn

C#:   s.Replace("a", "b")
来源：http://ba.bookmarksfly.cn

[E07] 按分隔符拆分
来源：http://cf.shxzskj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vg.asd995.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://oe.bookmarksfly.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://sx.bookmarksfly.cn

TS:   s.split(",")
来源：http://ee.nicolike.cn

Java: s.split(",");  s.split("\\s+")
来源：http://qq.9csxet.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pv.colortex.cn

Ruby: s.split(",");  s.split
来源：http://aa.jianghongdianzi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yl.lnxyls.cn

[E08] 数组按分隔符合并
来源：http://ex.lnxyls.cn

Py:   ",".join(items)
来源：http://mx.szsharing.cn

PHP:  implode(",", $items);
来源：http://ss.shtwfgs.cn

JS:   items.join(",")
来源：http://gk.haigaiapp.cn

TS:   items.join(",")
来源：http://dv.shxzukj.cn

Java: String.join(",", items)
来源：http://br.shxzukj.cn

Go:   strings.Join(items, ",")
来源：http://ln.panjiajie.cn

Ruby: items.join(",")
来源：http://wm.jianghongdianzi.cn

C#:   string.Join(",", items)
来源：http://im.gzmigu.cn

[E09] 去除所有空白字符
来源：http://oa.shtwfgs.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pm.nicolike.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dl.huixiangedu.cn

JS:   s.replace(/\s+/g, "")
来源：http://ck.gzmigu.cn

TS:   s.replace(/\s+/g, "")
来源：http://iy.wgjwhj.cn

Java: s.replaceAll("\\s+", "")
来源：http://dk.huixinmuqiang.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ei.szsharing.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ms.muxihuayi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rm.colortex.cn

[E10] 左侧补零 / 定长填充
来源：http://qa.nicolike.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yf.wgjwhj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://im.9csxet.cn

JS:   "7".padStart(3, "0")
来源：http://ki.panjiajie.cn

TS:   "7".padStart(3, "0")
来源：http://pj.yuntaijiaju.cn

Java: String.format("%03d", 7)
来源：http://kl.jianghongdianzi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://bq.szxytkj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pz.bookmarksfly.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hb.wgjwhj.cn

[E11] 反转字符串
来源：http://rl.shxzukj.cn

Py:   s[::-1]
来源：http://xv.gzmigu.cn

PHP:  strrev($s);
来源：http://gr.gzmigu.cn

JS:   [...s].reverse().join("")
来源：http://gg.muxihuayi.cn

TS:   [...s].reverse().join("")
来源：http://nx.szxytkj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://hr.jctech888.com.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://gw.haigaiapp.cn

Ruby: s.reverse
来源：http://uu.shxzukj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://rc.lnxyls.cn

[E12] 统计某字符出现次数
来源：http://uh.9csxet.cn

Py:   s.count("a")
来源：http://by.haigaiapp.cn

PHP:  substr_count($s, "a");
来源：http://dt.shxzskj.cn

JS:   s.split("a").length - 1
来源：http://el.jianghongdianzi.cn

TS:   s.split("a").length - 1
来源：http://pn.jctech888.com.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qt.huanxung.cn

Go:   strings.Count(s, "a")
来源：http://cu.colortex.cn

Ruby: s.count("a")
来源：http://ly.9csxet.cn

C#:   s.Count(c => c == 'a')
来源：http://tg.hnjuh.cn

[E13] 逐字符遍历
来源：http://uk.jianghongdianzi.cn

Py:   for ch in s: print(ch)
来源：http://fc.newstarts.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tv.hnjuh.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://qy.yuexingan06.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wg.yuntaijiaju.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sm.yuntaijiaju.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://oo.szxytkj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://hc.colortex.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tv.jianghongdianzi.cn

[E14] URL 编码与 Base64
来源：http://ka.jianghongdianzi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kz.yuntaijiaju.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qj.shxzukj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fk.jianghongdianzi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://li.hnjuh.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jp.nicolike.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zw.muxihuayi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://za.asd995.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://eb.bjjhwx.cn

[E15] HTML 转义 / 反转义
来源：http://cq.jctech888.com.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://mz.szsharing.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ja.asd995.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cd.9csxet.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://jl.huixiangedu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hk.chemitech.net.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cl.shxzskj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qm.nicolike.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xj.panjiajie.cn

[E16] 数字千分位
来源：http://su.nszjky.cn

Py:   f"{1234567:,}"
来源：http://kp.nszjky.cn

PHP:  number_format(1234567);
来源：http://wm.gzmigu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://nr.jctech888.com.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ln.nicolike.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hx.nszjky.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xx.shxzskj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bo.shtwfgs.cn

C#:   1234567.ToString("N0")
来源：http://sj.yuexingan06.cn

[E17] 首字母大写
来源：http://ht.colortex.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ds.wgjwhj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ni.huixiangedu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sd.jctech888.com.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://df.muxihuayi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rj.hnjuh.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pc.bookmarksfly.cn

Ruby: s.capitalize
来源：http://ca.muxihuayi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jv.yuntaijiaju.cn

[E18] 模板占位符替换
来源：http://dr.9csxet.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://db.shxzukj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mw.chemitech.net.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://eu.huixinmuqiang.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://tj.huanxung.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ap.hnjuh.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yk.hahajie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gu.521024.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zs.hnjuh.cn

[E19] 多行文本按行拆分
来源：http://zy.huixinmuqiang.cn

Py:   s.splitlines()
来源：http://vm.shxzukj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jo.asd995.cn

JS:   s.split(/\r?\n/)
来源：http://nw.hnjuh.cn

TS:   s.split(/\r?\n/)
来源：http://gx.huanxung.cn

Java: s.lines().toList()
来源：http://of.chemitech.net.cn

Go:   strings.Split(s, "\n")
来源：http://gy.bjjhwx.cn

Ruby: s.lines
来源：http://st.huixiangedu.cn

C#:   s.Split('\n')
来源：http://ta.yuntaijiaju.cn

[E20] 判断字符串是否为空
来源：http://qs.chemitech.net.cn

Py:   if not s:
来源：http://dg.yuexingan06.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tk.yuexingan06.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sy.9csxet.cn

TS:   if (s === "") {}
来源：http://xh.shtwfgs.cn

Java: if (s.isEmpty()) {}
来源：http://pe.jctech888.com.cn

Go:   if s == "" {}
来源：http://hg.newstarts.cn

Ruby: if s.empty?
来源：http://zx.wgjwhj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ui.panjiajie.cn

[E21] 超长截断加省略号
来源：http://go.nszjky.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://uo.huanxung.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://td.chemitech.net.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://of.shtwfgs.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ux.huixiangedu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jn.lnxyls.cn

Go:   // 按 rune 判断长度后截断
来源：http://pg.521024.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wf.jctech888.com.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mx.9csxet.cn

[E22] 字节长度与字符长度
来源：http://ff.9csxet.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://de.bookmarksfly.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gh.nicolike.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ja.shxzukj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://od.shxzskj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rp.jianghongdianzi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mb.jianghongdianzi.cn

Ruby: s.bytesize;  s.length
来源：http://wy.haigaiapp.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uv.muxihuayi.cn

================================================================================
来源：http://et.yuntaijiaju.cn

F. 文件与目录
来源：http://jm.asd995.cn

================================================================================
来源：http://pl.colortex.cn

[F01] 读取整个文件
来源：http://dk.colortex.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tt.nicolike.cn

PHP:  file_get_contents("a.txt");
来源：http://rx.newstarts.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fg.asd995.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hg.szsharing.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://be.chemitech.net.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cv.panjiajie.cn

Ruby: File.read("a.txt")
来源：http://gz.newstarts.cn

C#:   File.ReadAllText("a.txt");
来源：http://vo.huanxung.cn

[F02] 逐行读取文件
来源：http://zi.521024.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ae.shtwfgs.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uu.huanxung.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nw.521024.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zl.haigaiapp.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ch.haigaiapp.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ax.shxzskj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fq.newstarts.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ky.gzmigu.cn

[F03] 写入文件（覆盖）
来源：http://rd.nszjky.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://li.lnxyls.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://rn.bookmarksfly.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://in.shxzskj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hm.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cl.hahajie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ad.jianghongdianzi.cn

Ruby: File.write("a.txt", "hi")
来源：http://za.szsharing.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nd.nicolike.cn

[F04] 追加写入文件
来源：http://hr.huixiangedu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qm.nszjky.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yr.shtwfgs.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fj.yuntaijiaju.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ee.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ka.panjiajie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ag.9csxet.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qv.shxzskj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vi.huixinmuqiang.cn

[F05] 判断文件或目录是否存在
来源：http://nu.panjiajie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nc.nszjky.cn

PHP:  file_exists("a.txt");
来源：http://gr.lnxyls.cn

JS:   fs.existsSync("a.txt")
来源：http://pf.szxytkj.cn

TS:   fs.existsSync("a.txt")
来源：http://md.shxzukj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gy.asd995.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ev.yuntaijiaju.cn

Ruby: File.exist?("a.txt")
来源：http://qc.yuntaijiaju.cn

C#:   File.Exists("a.txt")
来源：http://pz.bookmarksfly.cn

[F06] 删除文件
来源：http://zq.nszjky.cn

Py:   os.remove("a.txt")
来源：http://do.nicolike.cn

PHP:  unlink("a.txt");
来源：http://aw.yuexingan06.cn

JS:   fs.unlinkSync("a.txt")
来源：http://xd.yuexingan06.cn

TS:   fs.unlinkSync("a.txt")
来源：http://dw.lnxyls.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ue.9csxet.cn

Go:   os.Remove("a.txt")
来源：http://em.newstarts.cn

Ruby: File.delete("a.txt")
来源：http://zk.huixiangedu.cn

C#:   File.Delete("a.txt");
来源：http://ni.szxytkj.cn

[F07] 创建目录（含多级）
来源：http://ki.chemitech.net.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vg.bjjhwx.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zw.521024.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ct.yuexingan06.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vl.9csxet.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cp.huixiangedu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cg.bjjhwx.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qn.nszjky.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ut.colortex.cn

[F08] 遍历目录
来源：http://hw.chemitech.net.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://cz.shtwfgs.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vt.szsharing.cn

JS:   fs.readdirSync("dir")
来源：http://hi.521024.cn

TS:   fs.readdirSync("dir")
来源：http://hu.szsharing.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mn.9csxet.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://bn.jianghongdianzi.cn

Ruby: Dir.children("dir")
来源：http://cm.asd995.cn

C#:   Directory.GetFiles("dir")
来源：http://ar.shxzskj.cn

[F09] 获取文件大小
来源：http://km.muxihuayi.cn

Py:   os.path.getsize("a.txt")
来源：http://fk.nszjky.cn

PHP:  filesize("a.txt");
来源：http://hq.gzmigu.cn

JS:   fs.statSync("a.txt").size
来源：http://ro.jctech888.com.cn

TS:   fs.statSync("a.txt").size
来源：http://yn.wgjwhj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://wr.lnxyls.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xi.hnjuh.cn

Ruby: File.size("a.txt")
来源：http://mf.colortex.cn

C#:   new FileInfo("a.txt").Length
来源：http://of.bookmarksfly.cn

[F10] 取文件扩展名 / 文件名
来源：http://tc.jctech888.com.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dz.jianghongdianzi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fn.521024.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nx.bjjhwx.cn

TS:   path.extname("a.txt")
来源：http://cc.hnjuh.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xi.nicolike.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zz.hnjuh.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://iw.haigaiapp.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xi.jctech888.com.cn

[F11] 复制与移动文件
来源：http://ht.yuexingan06.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pv.huixinmuqiang.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://to.haigaiapp.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wk.lnxyls.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://za.hahajie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yq.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rh.jianghongdianzi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rj.wgjwhj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qn.haigaiapp.cn

[F12] CSV 读写
来源：http://ue.yuntaijiaju.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ig.nszjky.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rs.shxzukj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hd.yuexingan06.cn

TS:   // 同上
来源：http://ss.nszjky.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zd.hnjuh.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dp.bjjhwx.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bo.shxzskj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://cj.nicolike.cn

================================================================================
来源：http://pg.szsharing.cn

G. 面向对象
来源：http://yu.shtwfgs.cn

================================================================================
来源：http://oe.muxihuayi.cn

[G01] 定义类
来源：http://mk.panjiajie.cn

Py:   class User: pass
来源：http://jf.yuexingan06.cn

PHP:  class User {}
来源：http://ao.shxzukj.cn

JS:   class User {}
来源：http://pv.gzmigu.cn

TS:   class User { name: string = ""; }
来源：http://tx.gzmigu.cn

Java: class User {}
来源：http://do.shxzskj.cn

Go:   type User struct { Name string }
来源：http://su.huixiangedu.cn

Ruby: class User; end
来源：http://wa.yuexingan06.cn

C#:   class User {}
来源：http://rr.huixinmuqiang.cn

[G02] 构造函数
来源：http://mh.nszjky.cn

Py:   def __init__(self, name): self.name = name
来源：http://js.yuexingan06.cn

PHP:  public function __construct(public string $name) {}
来源：http://ku.panjiajie.cn

JS:   constructor(name) { this.name = name; }
来源：http://tq.hahajie.cn

TS:   constructor(public name: string) {}
来源：http://dk.nszjky.cn

Java: User(String name) { this.name = name; }
来源：http://wh.hahajie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fu.hnjuh.cn

Ruby: def initialize(name); @name = name; end
来源：http://bt.nszjky.cn

C#:   public User(string name) { Name = name; }
来源：http://sv.nicolike.cn

[G03] 实例属性
来源：http://xc.nicolike.cn

Py:   self.name = "x"
来源：http://sx.haigaiapp.cn

PHP:  public string $name = "x";
来源：http://wz.jctech888.com.cn

JS:   this.name = "x";
来源：http://be.panjiajie.cn

TS:   name: string = "x";
来源：http://hg.shxzukj.cn

Java: private String name;
来源：http://by.chemitech.net.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://iv.bjjhwx.cn

Ruby: @name = "x"
来源：http://qq.shtwfgs.cn

C#:   public string Name { get; set; } = "x";
来源：http://ng.huixinmuqiang.cn

[G04] 定义方法
来源：http://hr.chemitech.net.cn

Py:   def greet(self): return self.name
来源：http://tv.wgjwhj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ya.newstarts.cn

JS:   greet() { return this.name; }
来源：http://hw.szxytkj.cn

TS:   greet(): string { return this.name; }
来源：http://sv.lnxyls.cn

Java: String greet() { return name; }
来源：http://he.hnjuh.cn


<!-- 参考信息 -->