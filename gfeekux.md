代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://tz.huixinmuqiang.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ld.huanxung.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ig.521024.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jx.yuntaijiaju.cn

C#:   s.Replace("a", "b")
来源：http://bt.panjiajie.cn

[E07] 按分隔符拆分
来源：http://of.9csxet.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://oa.szsharing.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ic.huixinmuqiang.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://as.hahajie.cn

TS:   s.split(",")
来源：http://gt.panjiajie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://sx.huixinmuqiang.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vo.bookmarksfly.cn

Ruby: s.split(",");  s.split
来源：http://ly.muxihuayi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hr.asd995.cn

[E08] 数组按分隔符合并
来源：http://rb.chemitech.net.cn

Py:   ",".join(items)
来源：http://gi.gzmigu.cn

PHP:  implode(",", $items);
来源：http://ml.muxihuayi.cn

JS:   items.join(",")
来源：http://om.newstarts.cn

TS:   items.join(",")
来源：http://wk.huixiangedu.cn

Java: String.join(",", items)
来源：http://fj.hahajie.cn

Go:   strings.Join(items, ",")
来源：http://ft.nszjky.cn

Ruby: items.join(",")
来源：http://py.haigaiapp.cn

C#:   string.Join(",", items)
来源：http://bm.yuexingan06.cn

[E09] 去除所有空白字符
来源：http://qt.asd995.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qe.colortex.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ub.9csxet.cn

JS:   s.replace(/\s+/g, "")
来源：http://lg.huanxung.cn

TS:   s.replace(/\s+/g, "")
来源：http://lc.yuntaijiaju.cn

Java: s.replaceAll("\\s+", "")
来源：http://ho.colortex.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://al.colortex.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ll.haigaiapp.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rw.bookmarksfly.cn

[E10] 左侧补零 / 定长填充
来源：http://zo.shxzskj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jf.gzmigu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://br.shxzukj.cn

JS:   "7".padStart(3, "0")
来源：http://dc.gzmigu.cn

TS:   "7".padStart(3, "0")
来源：http://vt.wgjwhj.cn

Java: String.format("%03d", 7)
来源：http://mj.asd995.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ea.huixinmuqiang.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gg.9csxet.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ng.shxzskj.cn

[E11] 反转字符串
来源：http://hs.szsharing.cn

Py:   s[::-1]
来源：http://gk.jctech888.com.cn

PHP:  strrev($s);
来源：http://lg.shxzukj.cn

JS:   [...s].reverse().join("")
来源：http://ou.nicolike.cn

TS:   [...s].reverse().join("")
来源：http://nt.yuexingan06.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://vk.muxihuayi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://vm.jianghongdianzi.cn

Ruby: s.reverse
来源：http://ww.gzmigu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://nx.lnxyls.cn

[E12] 统计某字符出现次数
来源：http://if.panjiajie.cn

Py:   s.count("a")
来源：http://xq.9csxet.cn

PHP:  substr_count($s, "a");
来源：http://gi.lnxyls.cn

JS:   s.split("a").length - 1
来源：http://hx.newstarts.cn

TS:   s.split("a").length - 1
来源：http://kp.chemitech.net.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vc.bookmarksfly.cn

Go:   strings.Count(s, "a")
来源：http://rp.colortex.cn

Ruby: s.count("a")
来源：http://vz.huanxung.cn

C#:   s.Count(c => c == 'a')
来源：http://ck.nicolike.cn

[E13] 逐字符遍历
来源：http://rx.asd995.cn

Py:   for ch in s: print(ch)
来源：http://rd.shxzukj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tu.hahajie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://cq.panjiajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wb.bookmarksfly.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zs.huixinmuqiang.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ja.9csxet.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rv.szsharing.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qu.huixiangedu.cn

[E14] URL 编码与 Base64
来源：http://nb.shtwfgs.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xd.jianghongdianzi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bz.gzmigu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jb.lnxyls.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://oq.hnjuh.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://oz.shtwfgs.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xw.hahajie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fz.jctech888.com.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ib.yuntaijiaju.cn

[E15] HTML 转义 / 反转义
来源：http://qs.521024.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://qv.bookmarksfly.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sq.hnjuh.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://by.haigaiapp.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://rg.huixinmuqiang.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ar.jianghongdianzi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hc.hahajie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gi.shtwfgs.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vs.chemitech.net.cn

[E16] 数字千分位
来源：http://ne.jctech888.com.cn

Py:   f"{1234567:,}"
来源：http://po.muxihuayi.cn

PHP:  number_format(1234567);
来源：http://wv.huixinmuqiang.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://xz.haigaiapp.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://kc.colortex.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fp.bookmarksfly.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jb.newstarts.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tx.haigaiapp.cn

C#:   1234567.ToString("N0")
来源：http://sp.yuntaijiaju.cn

[E17] 首字母大写
来源：http://wy.szxytkj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gk.haigaiapp.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://gm.newstarts.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ve.jctech888.com.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mz.bookmarksfly.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://iq.haigaiapp.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dm.hnjuh.cn

Ruby: s.capitalize
来源：http://me.lnxyls.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://il.panjiajie.cn

[E18] 模板占位符替换
来源：http://ki.jctech888.com.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ms.wgjwhj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://eo.jctech888.com.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ym.bookmarksfly.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://tc.nszjky.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://im.newstarts.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xf.jianghongdianzi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tz.bookmarksfly.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wx.chemitech.net.cn

[E19] 多行文本按行拆分
来源：http://hi.huanxung.cn

Py:   s.splitlines()
来源：http://qk.nszjky.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hw.lnxyls.cn

JS:   s.split(/\r?\n/)
来源：http://fw.huixiangedu.cn

TS:   s.split(/\r?\n/)
来源：http://vf.hahajie.cn

Java: s.lines().toList()
来源：http://eh.gzmigu.cn

Go:   strings.Split(s, "\n")
来源：http://op.huanxung.cn

Ruby: s.lines
来源：http://gw.panjiajie.cn

C#:   s.Split('\n')
来源：http://gz.jianghongdianzi.cn

[E20] 判断字符串是否为空
来源：http://qf.huixinmuqiang.cn

Py:   if not s:
来源：http://yj.jctech888.com.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ut.huanxung.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vu.shxzukj.cn

TS:   if (s === "") {}
来源：http://cc.newstarts.cn

Java: if (s.isEmpty()) {}
来源：http://ee.huanxung.cn

Go:   if s == "" {}
来源：http://uv.shxzskj.cn

Ruby: if s.empty?
来源：http://rh.nicolike.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bo.szxytkj.cn

[E21] 超长截断加省略号
来源：http://ti.shxzukj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qt.huixiangedu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yp.wgjwhj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pd.haigaiapp.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://eq.nszjky.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://it.huixiangedu.cn

Go:   // 按 rune 判断长度后截断
来源：http://up.lnxyls.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ez.colortex.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://po.wgjwhj.cn

[E22] 字节长度与字符长度
来源：http://mz.huixiangedu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://uu.hahajie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://by.hahajie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ps.shxzukj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kw.chemitech.net.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://db.shxzukj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ox.521024.cn

Ruby: s.bytesize;  s.length
来源：http://ax.hahajie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vz.asd995.cn

================================================================================
来源：http://is.yuexingan06.cn

F. 文件与目录
来源：http://lv.yuexingan06.cn

================================================================================
来源：http://bj.haigaiapp.cn

[F01] 读取整个文件
来源：http://hd.lnxyls.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://sr.huanxung.cn

PHP:  file_get_contents("a.txt");
来源：http://xn.huixiangedu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ju.521024.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ff.nszjky.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zy.huixinmuqiang.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yq.huanxung.cn

Ruby: File.read("a.txt")
来源：http://vj.nicolike.cn

C#:   File.ReadAllText("a.txt");
来源：http://wy.gzmigu.cn

[F02] 逐行读取文件
来源：http://em.hahajie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xz.shtwfgs.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xq.lnxyls.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://le.nicolike.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jq.jctech888.com.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gk.chemitech.net.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qv.hahajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://za.huixinmuqiang.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tz.shxzskj.cn

[F03] 写入文件（覆盖）
来源：http://ub.muxihuayi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vd.szsharing.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://mt.chemitech.net.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://in.chemitech.net.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mb.nicolike.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://iv.nszjky.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ay.yuexingan06.cn

Ruby: File.write("a.txt", "hi")
来源：http://qr.wgjwhj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://er.nicolike.cn

[F04] 追加写入文件
来源：http://eh.huanxung.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tk.szsharing.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bn.jctech888.com.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rl.wgjwhj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ca.haigaiapp.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qo.gzmigu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yk.9csxet.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://li.haigaiapp.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qm.huixiangedu.cn

[F05] 判断文件或目录是否存在
来源：http://cc.bookmarksfly.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gc.shxzukj.cn

PHP:  file_exists("a.txt");
来源：http://np.jctech888.com.cn

JS:   fs.existsSync("a.txt")
来源：http://jn.huanxung.cn

TS:   fs.existsSync("a.txt")
来源：http://oa.yuexingan06.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://pu.panjiajie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rn.9csxet.cn

Ruby: File.exist?("a.txt")
来源：http://pc.gzmigu.cn

C#:   File.Exists("a.txt")
来源：http://rw.521024.cn

[F06] 删除文件
来源：http://un.lnxyls.cn

Py:   os.remove("a.txt")
来源：http://no.newstarts.cn

PHP:  unlink("a.txt");
来源：http://sr.lnxyls.cn

JS:   fs.unlinkSync("a.txt")
来源：http://xm.wgjwhj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://zi.yuntaijiaju.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hx.nszjky.cn

Go:   os.Remove("a.txt")
来源：http://fv.szxytkj.cn

Ruby: File.delete("a.txt")
来源：http://rj.asd995.cn

C#:   File.Delete("a.txt");
来源：http://el.szsharing.cn

[F07] 创建目录（含多级）
来源：http://qg.yuexingan06.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://la.colortex.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qm.chemitech.net.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tl.yuntaijiaju.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pe.newstarts.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mk.yuexingan06.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://de.hnjuh.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rr.hahajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qq.yuexingan06.cn

[F08] 遍历目录
来源：http://uz.newstarts.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ml.szxytkj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gk.panjiajie.cn

JS:   fs.readdirSync("dir")
来源：http://ah.gzmigu.cn

TS:   fs.readdirSync("dir")
来源：http://ka.gzmigu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ob.shtwfgs.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ut.lnxyls.cn

Ruby: Dir.children("dir")
来源：http://rs.huixinmuqiang.cn

C#:   Directory.GetFiles("dir")
来源：http://ih.wgjwhj.cn

[F09] 获取文件大小
来源：http://bv.szsharing.cn

Py:   os.path.getsize("a.txt")
来源：http://dn.yuntaijiaju.cn

PHP:  filesize("a.txt");
来源：http://nh.szxytkj.cn

JS:   fs.statSync("a.txt").size
来源：http://sq.panjiajie.cn

TS:   fs.statSync("a.txt").size
来源：http://tc.huanxung.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ov.wgjwhj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fp.panjiajie.cn

Ruby: File.size("a.txt")
来源：http://ut.bjjhwx.cn

C#:   new FileInfo("a.txt").Length
来源：http://td.hahajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://du.bjjhwx.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xk.huanxung.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ey.shxzskj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ht.huixinmuqiang.cn

TS:   path.extname("a.txt")
来源：http://og.lnxyls.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ev.newstarts.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ja.shxzskj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lr.huixiangedu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kr.nicolike.cn

[F11] 复制与移动文件
来源：http://es.gzmigu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kl.gzmigu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hf.nicolike.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sq.haigaiapp.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qe.haigaiapp.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uw.shxzskj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ip.jianghongdianzi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://iz.nszjky.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tk.yuntaijiaju.cn

[F12] CSV 读写
来源：http://ux.chemitech.net.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bz.hahajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://od.521024.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://um.jctech888.com.cn

TS:   // 同上
来源：http://lw.panjiajie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qb.muxihuayi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zq.lnxyls.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lb.szsharing.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ly.colortex.cn

================================================================================
来源：http://kq.haigaiapp.cn

G. 面向对象
来源：http://si.yuntaijiaju.cn

================================================================================
来源：http://rx.colortex.cn

[G01] 定义类
来源：http://ce.jianghongdianzi.cn

Py:   class User: pass
来源：http://er.haigaiapp.cn

PHP:  class User {}
来源：http://dl.huixinmuqiang.cn

JS:   class User {}
来源：http://ub.nszjky.cn

TS:   class User { name: string = ""; }
来源：http://ac.muxihuayi.cn

Java: class User {}
来源：http://kx.9csxet.cn

Go:   type User struct { Name string }
来源：http://ad.haigaiapp.cn

Ruby: class User; end
来源：http://jv.colortex.cn

C#:   class User {}
来源：http://jq.shxzskj.cn

[G02] 构造函数
来源：http://xw.jianghongdianzi.cn

Py:   def __init__(self, name): self.name = name
来源：http://lp.521024.cn

PHP:  public function __construct(public string $name) {}
来源：http://pz.bjjhwx.cn

JS:   constructor(name) { this.name = name; }
来源：http://pb.9csxet.cn

TS:   constructor(public name: string) {}
来源：http://mz.521024.cn

Java: User(String name) { this.name = name; }
来源：http://ud.bjjhwx.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dz.wgjwhj.cn

Ruby: def initialize(name); @name = name; end
来源：http://ze.9csxet.cn

C#:   public User(string name) { Name = name; }
来源：http://jg.521024.cn

[G03] 实例属性
来源：http://gh.muxihuayi.cn

Py:   self.name = "x"
来源：http://de.newstarts.cn

PHP:  public string $name = "x";
来源：http://rs.521024.cn

JS:   this.name = "x";
来源：http://jk.yuntaijiaju.cn

TS:   name: string = "x";
来源：http://hn.hnjuh.cn

Java: private String name;
来源：http://ne.gzmigu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ln.nicolike.cn

Ruby: @name = "x"
来源：http://ou.huixiangedu.cn

C#:   public string Name { get; set; } = "x";
来源：http://lt.hahajie.cn

[G04] 定义方法
来源：http://zi.shxzskj.cn

Py:   def greet(self): return self.name
来源：http://ec.szxytkj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://py.9csxet.cn

JS:   greet() { return this.name; }
来源：http://zx.hahajie.cn

TS:   greet(): string { return this.name; }
来源：http://wd.nicolike.cn

Java: String greet() { return name; }
来源：http://mg.huixinmuqiang.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ke.asd995.cn

Ruby: def greet; @name; end
来源：http://fm.nicolike.cn

C#:   public string Greet() => Name;
来源：http://qn.wgjwhj.cn

[G05] 继承
来源：http://nk.huixinmuqiang.cn


<!-- 参考信息 -->