代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vm.muxihuayi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://eh.wgjwhj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cm.wgjwhj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vd.521024.cn

[E06] 替换子串
来源：http://ln.9csxet.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gl.szxytkj.cn

PHP:  str_replace("a", "b", $s);
来源：http://qq.panjiajie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hf.shxzukj.cn

TS:   s.replaceAll("a", "b")
来源：http://nk.szsharing.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xm.shtwfgs.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bx.szsharing.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ib.nszjky.cn

C#:   s.Replace("a", "b")
来源：http://wj.szxytkj.cn

[E07] 按分隔符拆分
来源：http://uo.chemitech.net.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jz.jctech888.com.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://or.panjiajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://an.521024.cn

TS:   s.split(",")
来源：http://de.panjiajie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://rt.bjjhwx.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dx.huixiangedu.cn

Ruby: s.split(",");  s.split
来源：http://ze.nicolike.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qo.gzmigu.cn

[E08] 数组按分隔符合并
来源：http://oo.chemitech.net.cn

Py:   ",".join(items)
来源：http://cw.huanxung.cn

PHP:  implode(",", $items);
来源：http://en.szsharing.cn

JS:   items.join(",")
来源：http://re.lnxyls.cn

TS:   items.join(",")
来源：http://xz.szsharing.cn

Java: String.join(",", items)
来源：http://ka.nszjky.cn

Go:   strings.Join(items, ",")
来源：http://ea.gzmigu.cn

Ruby: items.join(",")
来源：http://bp.huanxung.cn

C#:   string.Join(",", items)
来源：http://co.nicolike.cn

[E09] 去除所有空白字符
来源：http://by.9csxet.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://po.shxzskj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://da.szsharing.cn

JS:   s.replace(/\s+/g, "")
来源：http://cw.lnxyls.cn

TS:   s.replace(/\s+/g, "")
来源：http://wn.panjiajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://dr.wgjwhj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://js.szsharing.cn

Ruby: s.gsub(/\s+/, "")
来源：http://fb.haigaiapp.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jp.shxzukj.cn

[E10] 左侧补零 / 定长填充
来源：http://wm.haigaiapp.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zk.szsharing.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wa.hnjuh.cn

JS:   "7".padStart(3, "0")
来源：http://pz.panjiajie.cn

TS:   "7".padStart(3, "0")
来源：http://xr.szsharing.cn

Java: String.format("%03d", 7)
来源：http://er.newstarts.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xq.haigaiapp.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ee.nszjky.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rr.huanxung.cn

[E11] 反转字符串
来源：http://xy.szxytkj.cn

Py:   s[::-1]
来源：http://qq.yuexingan06.cn

PHP:  strrev($s);
来源：http://hr.wgjwhj.cn

JS:   [...s].reverse().join("")
来源：http://xd.nicolike.cn

TS:   [...s].reverse().join("")
来源：http://py.nicolike.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://fp.hnjuh.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zi.9csxet.cn

Ruby: s.reverse
来源：http://ss.panjiajie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://zy.huixiangedu.cn

[E12] 统计某字符出现次数
来源：http://ie.haigaiapp.cn

Py:   s.count("a")
来源：http://fs.panjiajie.cn

PHP:  substr_count($s, "a");
来源：http://sk.huixiangedu.cn

JS:   s.split("a").length - 1
来源：http://rc.shxzukj.cn

TS:   s.split("a").length - 1
来源：http://xh.asd995.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jn.lnxyls.cn

Go:   strings.Count(s, "a")
来源：http://wi.szxytkj.cn

Ruby: s.count("a")
来源：http://eh.chemitech.net.cn

C#:   s.Count(c => c == 'a')
来源：http://ml.nicolike.cn

[E13] 逐字符遍历
来源：http://li.lnxyls.cn

Py:   for ch in s: print(ch)
来源：http://hn.huanxung.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bl.shxzskj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://bu.panjiajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://xm.shtwfgs.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ps.lnxyls.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gy.nszjky.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://gi.muxihuayi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qh.newstarts.cn

[E14] URL 编码与 Base64
来源：http://kl.nszjky.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yg.hahajie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://pf.haigaiapp.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zn.521024.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://br.wgjwhj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tn.wgjwhj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cb.lnxyls.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ie.nicolike.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nx.chemitech.net.cn

[E15] HTML 转义 / 反转义
来源：http://wv.asd995.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://oy.huixinmuqiang.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ox.gzmigu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://co.szxytkj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://kg.hahajie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hi.huixinmuqiang.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xo.newstarts.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://do.hahajie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ts.gzmigu.cn

[E16] 数字千分位
来源：http://cf.nszjky.cn

Py:   f"{1234567:,}"
来源：http://yi.newstarts.cn

PHP:  number_format(1234567);
来源：http://tb.colortex.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://wy.huanxung.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://hr.szxytkj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nh.jianghongdianzi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://sj.gzmigu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bj.szxytkj.cn

C#:   1234567.ToString("N0")
来源：http://dq.newstarts.cn

[E17] 首字母大写
来源：http://gv.gzmigu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cn.szxytkj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://jg.nszjky.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ee.shxzskj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rf.colortex.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://yu.muxihuayi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cq.huanxung.cn

Ruby: s.capitalize
来源：http://dw.huanxung.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://az.shtwfgs.cn

[E18] 模板占位符替换
来源：http://fa.yuexingan06.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cg.bookmarksfly.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gu.colortex.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://rn.bjjhwx.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://tt.szsharing.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ll.bjjhwx.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ck.lnxyls.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://oh.hnjuh.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hj.nszjky.cn

[E19] 多行文本按行拆分
来源：http://ci.szxytkj.cn

Py:   s.splitlines()
来源：http://bo.bookmarksfly.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tw.asd995.cn

JS:   s.split(/\r?\n/)
来源：http://nv.yuntaijiaju.cn

TS:   s.split(/\r?\n/)
来源：http://yi.9csxet.cn

Java: s.lines().toList()
来源：http://ud.9csxet.cn

Go:   strings.Split(s, "\n")
来源：http://sg.huixinmuqiang.cn

Ruby: s.lines
来源：http://xg.hnjuh.cn

C#:   s.Split('\n')
来源：http://dw.wgjwhj.cn

[E20] 判断字符串是否为空
来源：http://wp.huixiangedu.cn

Py:   if not s:
来源：http://hf.jctech888.com.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yj.hnjuh.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yi.shxzskj.cn

TS:   if (s === "") {}
来源：http://lm.colortex.cn

Java: if (s.isEmpty()) {}
来源：http://jf.haigaiapp.cn

Go:   if s == "" {}
来源：http://ee.hahajie.cn

Ruby: if s.empty?
来源：http://ic.hnjuh.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://me.9csxet.cn

[E21] 超长截断加省略号
来源：http://ml.huixiangedu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wx.muxihuayi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kc.hnjuh.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ku.nicolike.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gg.colortex.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bs.yuexingan06.cn

Go:   // 按 rune 判断长度后截断
来源：http://mx.gzmigu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yt.bookmarksfly.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nu.nszjky.cn

[E22] 字节长度与字符长度
来源：http://ik.nicolike.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kj.huixinmuqiang.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://da.wgjwhj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qk.szsharing.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nk.szxytkj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hd.521024.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ck.panjiajie.cn

Ruby: s.bytesize;  s.length
来源：http://re.lnxyls.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tz.huixiangedu.cn

================================================================================
来源：http://tn.szxytkj.cn

F. 文件与目录
来源：http://tl.yuntaijiaju.cn

================================================================================
来源：http://rx.huixiangedu.cn

[F01] 读取整个文件
来源：http://vx.haigaiapp.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bg.chemitech.net.cn

PHP:  file_get_contents("a.txt");
来源：http://ew.9csxet.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://go.yuexingan06.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bc.panjiajie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://xm.yuntaijiaju.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ab.chemitech.net.cn

Ruby: File.read("a.txt")
来源：http://yk.lnxyls.cn

C#:   File.ReadAllText("a.txt");
来源：http://dd.9csxet.cn

[F02] 逐行读取文件
来源：http://nw.nszjky.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fk.haigaiapp.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sf.huixinmuqiang.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kv.lnxyls.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vk.colortex.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cu.jctech888.com.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xy.jctech888.com.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rr.wgjwhj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vn.yuntaijiaju.cn

[F03] 写入文件（覆盖）
来源：http://fe.panjiajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bl.huixiangedu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ej.asd995.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zm.shxzskj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kd.huanxung.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kv.jianghongdianzi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hf.asd995.cn

Ruby: File.write("a.txt", "hi")
来源：http://hw.hahajie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dk.nicolike.cn

[F04] 追加写入文件
来源：http://oy.newstarts.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dv.jctech888.com.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lr.haigaiapp.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tl.muxihuayi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ia.nicolike.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ok.chemitech.net.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xp.huixiangedu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://po.huanxung.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cc.huixiangedu.cn

[F05] 判断文件或目录是否存在
来源：http://pu.jianghongdianzi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ca.shtwfgs.cn

PHP:  file_exists("a.txt");
来源：http://gx.hahajie.cn

JS:   fs.existsSync("a.txt")
来源：http://aj.nicolike.cn

TS:   fs.existsSync("a.txt")
来源：http://oh.haigaiapp.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://pg.nszjky.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://em.shxzukj.cn

Ruby: File.exist?("a.txt")
来源：http://xa.hahajie.cn

C#:   File.Exists("a.txt")
来源：http://bg.colortex.cn

[F06] 删除文件
来源：http://tp.huixiangedu.cn

Py:   os.remove("a.txt")
来源：http://oj.bookmarksfly.cn

PHP:  unlink("a.txt");
来源：http://lv.jianghongdianzi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://fi.jctech888.com.cn

TS:   fs.unlinkSync("a.txt")
来源：http://el.lnxyls.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wt.yuntaijiaju.cn

Go:   os.Remove("a.txt")
来源：http://iz.9csxet.cn

Ruby: File.delete("a.txt")
来源：http://la.szsharing.cn

C#:   File.Delete("a.txt");
来源：http://za.hnjuh.cn

[F07] 创建目录（含多级）
来源：http://hm.shxzskj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bv.gzmigu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hp.gzmigu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fq.bookmarksfly.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nn.muxihuayi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mb.huixiangedu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gu.nicolike.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ao.wgjwhj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://st.nicolike.cn

[F08] 遍历目录
来源：http://jz.shxzukj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://op.asd995.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ur.szxytkj.cn

JS:   fs.readdirSync("dir")
来源：http://gf.gzmigu.cn

TS:   fs.readdirSync("dir")
来源：http://wq.gzmigu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yy.szsharing.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://qr.szsharing.cn

Ruby: Dir.children("dir")
来源：http://zv.shxzskj.cn

C#:   Directory.GetFiles("dir")
来源：http://it.nszjky.cn

[F09] 获取文件大小
来源：http://ra.9csxet.cn

Py:   os.path.getsize("a.txt")
来源：http://af.asd995.cn

PHP:  filesize("a.txt");
来源：http://ww.gzmigu.cn

JS:   fs.statSync("a.txt").size
来源：http://ey.shxzskj.cn

TS:   fs.statSync("a.txt").size
来源：http://az.jctech888.com.cn

Java: Files.size(Path.of("a.txt"))
来源：http://kn.shtwfgs.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zu.jctech888.com.cn

Ruby: File.size("a.txt")
来源：http://ol.shtwfgs.cn

C#:   new FileInfo("a.txt").Length
来源：http://nn.yuntaijiaju.cn

[F10] 取文件扩展名 / 文件名
来源：http://qw.panjiajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://op.szxytkj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pn.gzmigu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ag.yuexingan06.cn

TS:   path.extname("a.txt")
来源：http://fj.szsharing.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://oh.lnxyls.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qt.huanxung.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://uf.shxzskj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hv.szsharing.cn

[F11] 复制与移动文件
来源：http://wr.colortex.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ht.jctech888.com.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dm.521024.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wg.wgjwhj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ig.szxytkj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fs.521024.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gt.shxzskj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://by.huixinmuqiang.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cl.haigaiapp.cn

[F12] CSV 读写
来源：http://bb.newstarts.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pj.wgjwhj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://te.chemitech.net.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ir.panjiajie.cn

TS:   // 同上
来源：http://ez.szxytkj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wy.muxihuayi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jf.bookmarksfly.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gg.shtwfgs.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://zf.jianghongdianzi.cn

================================================================================
来源：http://qg.lnxyls.cn

G. 面向对象
来源：http://oe.panjiajie.cn

================================================================================
来源：http://zf.nicolike.cn

[G01] 定义类
来源：http://mq.9csxet.cn

Py:   class User: pass
来源：http://ra.huanxung.cn

PHP:  class User {}
来源：http://ya.hnjuh.cn

JS:   class User {}
来源：http://jl.gzmigu.cn

TS:   class User { name: string = ""; }
来源：http://yb.wgjwhj.cn

Java: class User {}
来源：http://hq.yuexingan06.cn

Go:   type User struct { Name string }
来源：http://he.colortex.cn

Ruby: class User; end
来源：http://df.newstarts.cn

C#:   class User {}
来源：http://vo.9csxet.cn

[G02] 构造函数
来源：http://vk.nicolike.cn

Py:   def __init__(self, name): self.name = name
来源：http://zl.shxzukj.cn

PHP:  public function __construct(public string $name) {}
来源：http://dw.yuexingan06.cn

JS:   constructor(name) { this.name = name; }
来源：http://qt.shxzukj.cn

TS:   constructor(public name: string) {}
来源：http://wf.bjjhwx.cn

Java: User(String name) { this.name = name; }
来源：http://po.huixiangedu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ek.huixiangedu.cn

Ruby: def initialize(name); @name = name; end
来源：http://at.asd995.cn

C#:   public User(string name) { Name = name; }
来源：http://vm.muxihuayi.cn

[G03] 实例属性
来源：http://du.szxytkj.cn

Py:   self.name = "x"
来源：http://qr.nszjky.cn

PHP:  public string $name = "x";
来源：http://xd.huanxung.cn

JS:   this.name = "x";
来源：http://zc.9csxet.cn

TS:   name: string = "x";
来源：http://zw.yuntaijiaju.cn

Java: private String name;
来源：http://ol.haigaiapp.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hy.colortex.cn

Ruby: @name = "x"
来源：http://hy.yuntaijiaju.cn

C#:   public string Name { get; set; } = "x";
来源：http://dd.bookmarksfly.cn

[G04] 定义方法
来源：http://ls.9csxet.cn

Py:   def greet(self): return self.name
来源：http://cw.yuexingan06.cn


<!-- 参考信息 -->