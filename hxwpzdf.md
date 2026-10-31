代发 wailian999

[E06] 替换子串
来源：http://kw.wgjwhj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hp.szxytkj.cn

PHP:  str_replace("a", "b", $s);
来源：http://ex.lnxyls.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jv.bjjhwx.cn

TS:   s.replaceAll("a", "b")
来源：http://vt.muxihuayi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tc.nszjky.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://iz.nszjky.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yb.hnjuh.cn

C#:   s.Replace("a", "b")
来源：http://zi.lnxyls.cn

[E07] 按分隔符拆分
来源：http://pl.hahajie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pq.521024.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qj.newstarts.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://da.huixiangedu.cn

TS:   s.split(",")
来源：http://uw.haigaiapp.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ek.haigaiapp.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jf.bjjhwx.cn

Ruby: s.split(",");  s.split
来源：http://jk.wgjwhj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nt.gzmigu.cn

[E08] 数组按分隔符合并
来源：http://pc.huanxung.cn

Py:   ",".join(items)
来源：http://uq.huixiangedu.cn

PHP:  implode(",", $items);
来源：http://lh.521024.cn

JS:   items.join(",")
来源：http://hv.newstarts.cn

TS:   items.join(",")
来源：http://mo.chemitech.net.cn

Java: String.join(",", items)
来源：http://wi.shxzskj.cn

Go:   strings.Join(items, ",")
来源：http://mk.nicolike.cn

Ruby: items.join(",")
来源：http://fv.colortex.cn

C#:   string.Join(",", items)
来源：http://lq.wgjwhj.cn

[E09] 去除所有空白字符
来源：http://jy.521024.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://po.9csxet.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://oe.9csxet.cn

JS:   s.replace(/\s+/g, "")
来源：http://zu.wgjwhj.cn

TS:   s.replace(/\s+/g, "")
来源：http://go.wgjwhj.cn

Java: s.replaceAll("\\s+", "")
来源：http://pe.szsharing.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ir.nszjky.cn

Ruby: s.gsub(/\s+/, "")
来源：http://yh.chemitech.net.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ou.huixiangedu.cn

[E10] 左侧补零 / 定长填充
来源：http://rr.huixiangedu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yr.bookmarksfly.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qg.haigaiapp.cn

JS:   "7".padStart(3, "0")
来源：http://ld.muxihuayi.cn

TS:   "7".padStart(3, "0")
来源：http://iq.huixiangedu.cn

Java: String.format("%03d", 7)
来源：http://cj.wgjwhj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://am.jctech888.com.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wi.gzmigu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ow.wgjwhj.cn

[E11] 反转字符串
来源：http://ft.wgjwhj.cn

Py:   s[::-1]
来源：http://in.bookmarksfly.cn

PHP:  strrev($s);
来源：http://aq.colortex.cn

JS:   [...s].reverse().join("")
来源：http://cn.huixiangedu.cn

TS:   [...s].reverse().join("")
来源：http://tt.yuexingan06.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://xv.asd995.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qf.jctech888.com.cn

Ruby: s.reverse
来源：http://yh.panjiajie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://xk.panjiajie.cn

[E12] 统计某字符出现次数
来源：http://ai.shxzukj.cn

Py:   s.count("a")
来源：http://qp.panjiajie.cn

PHP:  substr_count($s, "a");
来源：http://gh.521024.cn

JS:   s.split("a").length - 1
来源：http://nr.newstarts.cn

TS:   s.split("a").length - 1
来源：http://ca.lnxyls.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gi.nszjky.cn

Go:   strings.Count(s, "a")
来源：http://ad.521024.cn

Ruby: s.count("a")
来源：http://lf.wgjwhj.cn

C#:   s.Count(c => c == 'a')
来源：http://gg.shtwfgs.cn

[E13] 逐字符遍历
来源：http://mh.nicolike.cn

Py:   for ch in s: print(ch)
来源：http://yp.hnjuh.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jl.bjjhwx.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://fv.jianghongdianzi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://lb.shtwfgs.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fb.muxihuayi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pn.jctech888.com.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://hy.asd995.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ti.yuntaijiaju.cn

[E14] URL 编码与 Base64
来源：http://go.newstarts.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fu.huixiangedu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://sw.asd995.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qc.newstarts.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ph.chemitech.net.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://er.huanxung.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zv.asd995.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fv.yuexingan06.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dh.chemitech.net.cn

[E15] HTML 转义 / 反转义
来源：http://vy.wgjwhj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://wr.szsharing.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hj.jctech888.com.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://uu.bookmarksfly.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://do.gzmigu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mb.gzmigu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://df.9csxet.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hn.521024.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fp.bookmarksfly.cn

[E16] 数字千分位
来源：http://mx.521024.cn

Py:   f"{1234567:,}"
来源：http://ad.jctech888.com.cn

PHP:  number_format(1234567);
来源：http://bf.colortex.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://nq.chemitech.net.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://bb.haigaiapp.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tw.lnxyls.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ud.shxzskj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bz.jianghongdianzi.cn

C#:   1234567.ToString("N0")
来源：http://sq.szsharing.cn

[E17] 首字母大写
来源：http://gu.shxzukj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cx.hahajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://jq.shtwfgs.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vb.521024.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nj.nicolike.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hg.yuexingan06.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zc.szsharing.cn

Ruby: s.capitalize
来源：http://cd.wgjwhj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ac.asd995.cn

[E18] 模板占位符替换
来源：http://op.521024.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://po.panjiajie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gl.colortex.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://qd.panjiajie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://vk.hnjuh.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ik.hnjuh.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rl.huixinmuqiang.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lp.nszjky.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bs.nicolike.cn

[E19] 多行文本按行拆分
来源：http://nt.bookmarksfly.cn

Py:   s.splitlines()
来源：http://pk.shxzskj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://iv.asd995.cn

JS:   s.split(/\r?\n/)
来源：http://de.521024.cn

TS:   s.split(/\r?\n/)
来源：http://mk.jctech888.com.cn

Java: s.lines().toList()
来源：http://af.nicolike.cn

Go:   strings.Split(s, "\n")
来源：http://dv.521024.cn

Ruby: s.lines
来源：http://xg.nszjky.cn

C#:   s.Split('\n')
来源：http://lb.jctech888.com.cn

[E20] 判断字符串是否为空
来源：http://yc.bookmarksfly.cn

Py:   if not s:
来源：http://go.shtwfgs.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ez.chemitech.net.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://go.muxihuayi.cn

TS:   if (s === "") {}
来源：http://kg.yuntaijiaju.cn

Java: if (s.isEmpty()) {}
来源：http://ul.yuntaijiaju.cn

Go:   if s == "" {}
来源：http://ky.huixiangedu.cn

Ruby: if s.empty?
来源：http://is.huixinmuqiang.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bn.shxzskj.cn

[E21] 超长截断加省略号
来源：http://ah.huixiangedu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ji.colortex.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ak.521024.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lv.newstarts.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tl.hnjuh.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qg.bookmarksfly.cn

Go:   // 按 rune 判断长度后截断
来源：http://dn.szxytkj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wu.muxihuayi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tq.jianghongdianzi.cn

[E22] 字节长度与字符长度
来源：http://sr.asd995.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://uo.bookmarksfly.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sq.muxihuayi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qb.hahajie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gn.yuexingan06.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mj.shtwfgs.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jo.hahajie.cn

Ruby: s.bytesize;  s.length
来源：http://pb.shxzskj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://oa.gzmigu.cn

================================================================================
来源：http://tj.newstarts.cn

F. 文件与目录
来源：http://er.nicolike.cn

================================================================================
来源：http://ek.bjjhwx.cn

[F01] 读取整个文件
来源：http://rc.szxytkj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mj.yuntaijiaju.cn

PHP:  file_get_contents("a.txt");
来源：http://jo.haigaiapp.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://it.nicolike.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sm.huixiangedu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://av.szsharing.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://em.nszjky.cn

Ruby: File.read("a.txt")
来源：http://em.jctech888.com.cn

C#:   File.ReadAllText("a.txt");
来源：http://zj.shtwfgs.cn

[F02] 逐行读取文件
来源：http://kd.asd995.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ht.shtwfgs.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://en.colortex.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pe.yuntaijiaju.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bd.521024.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gi.lnxyls.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tu.huixiangedu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dq.nszjky.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://iy.asd995.cn

[F03] 写入文件（覆盖）
来源：http://ax.szxytkj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xq.asd995.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://yp.jianghongdianzi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jp.gzmigu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ui.haigaiapp.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vj.bookmarksfly.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://de.panjiajie.cn

Ruby: File.write("a.txt", "hi")
来源：http://fm.huanxung.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ga.wgjwhj.cn

[F04] 追加写入文件
来源：http://tx.huixinmuqiang.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tv.shxzukj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bv.shxzskj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lr.bookmarksfly.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pe.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mq.szsharing.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zk.asd995.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pd.bookmarksfly.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wi.jctech888.com.cn

[F05] 判断文件或目录是否存在
来源：http://ol.gzmigu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ui.huanxung.cn

PHP:  file_exists("a.txt");
来源：http://sv.colortex.cn

JS:   fs.existsSync("a.txt")
来源：http://go.haigaiapp.cn

TS:   fs.existsSync("a.txt")
来源：http://sa.hahajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://pt.chemitech.net.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://eb.nicolike.cn

Ruby: File.exist?("a.txt")
来源：http://on.chemitech.net.cn

C#:   File.Exists("a.txt")
来源：http://hv.521024.cn

[F06] 删除文件
来源：http://dm.yuntaijiaju.cn

Py:   os.remove("a.txt")
来源：http://km.hahajie.cn

PHP:  unlink("a.txt");
来源：http://uv.haigaiapp.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ch.gzmigu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://qm.9csxet.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zx.szxytkj.cn

Go:   os.Remove("a.txt")
来源：http://xl.shxzskj.cn

Ruby: File.delete("a.txt")
来源：http://rf.haigaiapp.cn

C#:   File.Delete("a.txt");
来源：http://ui.shtwfgs.cn

[F07] 创建目录（含多级）
来源：http://vr.bookmarksfly.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vi.haigaiapp.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qr.nszjky.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ur.hahajie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yq.panjiajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://aj.yuntaijiaju.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hi.hahajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hg.yuexingan06.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gq.jctech888.com.cn

[F08] 遍历目录
来源：http://yv.bjjhwx.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ic.huanxung.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pa.wgjwhj.cn

JS:   fs.readdirSync("dir")
来源：http://qq.shxzukj.cn

TS:   fs.readdirSync("dir")
来源：http://xi.huanxung.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kk.nszjky.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ng.huanxung.cn

Ruby: Dir.children("dir")
来源：http://ia.szxytkj.cn

C#:   Directory.GetFiles("dir")
来源：http://uk.gzmigu.cn

[F09] 获取文件大小
来源：http://fl.bjjhwx.cn

Py:   os.path.getsize("a.txt")
来源：http://ov.gzmigu.cn

PHP:  filesize("a.txt");
来源：http://xp.muxihuayi.cn

JS:   fs.statSync("a.txt").size
来源：http://dr.haigaiapp.cn

TS:   fs.statSync("a.txt").size
来源：http://yk.wgjwhj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ul.panjiajie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ye.hahajie.cn

Ruby: File.size("a.txt")
来源：http://jq.huixiangedu.cn

C#:   new FileInfo("a.txt").Length
来源：http://ce.jianghongdianzi.cn

[F10] 取文件扩展名 / 文件名
来源：http://zv.szsharing.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://uo.colortex.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ot.panjiajie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vm.haigaiapp.cn

TS:   path.extname("a.txt")
来源：http://nx.panjiajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fm.gzmigu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://na.bookmarksfly.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yy.szsharing.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vm.huanxung.cn

[F11] 复制与移动文件
来源：http://kv.yuexingan06.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xw.newstarts.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kl.hnjuh.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ro.asd995.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hv.gzmigu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://sx.huixiangedu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zl.jianghongdianzi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bk.chemitech.net.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vv.shxzukj.cn

[F12] CSV 读写
来源：http://ac.yuntaijiaju.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://iw.huixinmuqiang.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pn.521024.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://sq.nszjky.cn

TS:   // 同上
来源：http://mh.lnxyls.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ct.newstarts.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://uq.huixinmuqiang.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gh.jianghongdianzi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://wr.newstarts.cn

================================================================================
来源：http://ht.hnjuh.cn

G. 面向对象
来源：http://ic.bjjhwx.cn

================================================================================
来源：http://fd.huixiangedu.cn

[G01] 定义类
来源：http://vd.nszjky.cn

Py:   class User: pass
来源：http://bq.jianghongdianzi.cn

PHP:  class User {}
来源：http://en.shxzukj.cn

JS:   class User {}
来源：http://tz.haigaiapp.cn

TS:   class User { name: string = ""; }
来源：http://xj.huanxung.cn

Java: class User {}
来源：http://cp.jianghongdianzi.cn

Go:   type User struct { Name string }
来源：http://et.521024.cn

Ruby: class User; end
来源：http://nq.asd995.cn

C#:   class User {}
来源：http://xe.wgjwhj.cn

[G02] 构造函数
来源：http://rz.gzmigu.cn

Py:   def __init__(self, name): self.name = name
来源：http://th.colortex.cn

PHP:  public function __construct(public string $name) {}
来源：http://vx.wgjwhj.cn

JS:   constructor(name) { this.name = name; }
来源：http://ti.nicolike.cn

TS:   constructor(public name: string) {}
来源：http://nd.jianghongdianzi.cn

Java: User(String name) { this.name = name; }
来源：http://im.haigaiapp.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cc.nicolike.cn

Ruby: def initialize(name); @name = name; end
来源：http://fl.colortex.cn

C#:   public User(string name) { Name = name; }
来源：http://wp.shtwfgs.cn

[G03] 实例属性
来源：http://iw.jianghongdianzi.cn

Py:   self.name = "x"
来源：http://wh.shxzukj.cn

PHP:  public string $name = "x";
来源：http://rd.szsharing.cn

JS:   this.name = "x";
来源：http://hf.yuntaijiaju.cn

TS:   name: string = "x";
来源：http://wg.szsharing.cn

Java: private String name;
来源：http://al.newstarts.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tu.colortex.cn

Ruby: @name = "x"
来源：http://rq.wgjwhj.cn

C#:   public string Name { get; set; } = "x";
来源：http://ks.colortex.cn

[G04] 定义方法
来源：http://lt.shxzukj.cn

Py:   def greet(self): return self.name
来源：http://vc.yuexingan06.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://py.haigaiapp.cn

JS:   greet() { return this.name; }
来源：http://he.nszjky.cn

TS:   greet(): string { return this.name; }
来源：http://vm.chemitech.net.cn

Java: String greet() { return name; }
来源：http://ue.nicolike.cn


<!-- 参考信息 -->