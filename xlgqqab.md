代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ps.chemitech.net.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cg.huanxung.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hl.newstarts.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://fg.hnjuh.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://aa.hnjuh.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ce.gzmigu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jk.szxytkj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://md.muxihuayi.cn

[E06] 替换子串
来源：http://mn.bookmarksfly.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vu.huixinmuqiang.cn

PHP:  str_replace("a", "b", $s);
来源：http://ax.colortex.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://in.szsharing.cn

TS:   s.replaceAll("a", "b")
来源：http://ay.bjjhwx.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ol.huanxung.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yl.muxihuayi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wj.shxzukj.cn

C#:   s.Replace("a", "b")
来源：http://np.colortex.cn

[E07] 按分隔符拆分
来源：http://ee.shtwfgs.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ma.lnxyls.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jr.huanxung.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://qu.lnxyls.cn

TS:   s.split(",")
来源：http://nl.colortex.cn

Java: s.split(",");  s.split("\\s+")
来源：http://fo.muxihuayi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ql.lnxyls.cn

Ruby: s.split(",");  s.split
来源：http://xx.huixinmuqiang.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://np.chemitech.net.cn

[E08] 数组按分隔符合并
来源：http://rd.wgjwhj.cn

Py:   ",".join(items)
来源：http://fm.newstarts.cn

PHP:  implode(",", $items);
来源：http://xa.huanxung.cn

JS:   items.join(",")
来源：http://dk.hahajie.cn

TS:   items.join(",")
来源：http://hs.szsharing.cn

Java: String.join(",", items)
来源：http://rv.huixinmuqiang.cn

Go:   strings.Join(items, ",")
来源：http://zq.gzmigu.cn

Ruby: items.join(",")
来源：http://lq.huixinmuqiang.cn

C#:   string.Join(",", items)
来源：http://iv.nicolike.cn

[E09] 去除所有空白字符
来源：http://ip.521024.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hj.chemitech.net.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hk.9csxet.cn

JS:   s.replace(/\s+/g, "")
来源：http://uu.asd995.cn

TS:   s.replace(/\s+/g, "")
来源：http://ns.colortex.cn

Java: s.replaceAll("\\s+", "")
来源：http://bc.asd995.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://fl.521024.cn

Ruby: s.gsub(/\s+/, "")
来源：http://pi.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fd.haigaiapp.cn

[E10] 左侧补零 / 定长填充
来源：http://hf.hnjuh.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hm.asd995.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://oo.nicolike.cn

JS:   "7".padStart(3, "0")
来源：http://uu.chemitech.net.cn

TS:   "7".padStart(3, "0")
来源：http://dy.jctech888.com.cn

Java: String.format("%03d", 7)
来源：http://rh.szxytkj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://va.huixiangedu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sf.huanxung.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yl.haigaiapp.cn

[E11] 反转字符串
来源：http://lh.hnjuh.cn

Py:   s[::-1]
来源：http://ha.colortex.cn

PHP:  strrev($s);
来源：http://gn.shxzskj.cn

JS:   [...s].reverse().join("")
来源：http://kp.bjjhwx.cn

TS:   [...s].reverse().join("")
来源：http://fs.newstarts.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://nt.yuntaijiaju.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://xn.shxzukj.cn

Ruby: s.reverse
来源：http://eu.bjjhwx.cn

C#:   new string(s.Reverse().ToArray())
来源：http://uv.gzmigu.cn

[E12] 统计某字符出现次数
来源：http://ma.yuexingan06.cn

Py:   s.count("a")
来源：http://hn.wgjwhj.cn

PHP:  substr_count($s, "a");
来源：http://pr.shxzskj.cn

JS:   s.split("a").length - 1
来源：http://fs.nicolike.cn

TS:   s.split("a").length - 1
来源：http://ob.chemitech.net.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hu.szxytkj.cn

Go:   strings.Count(s, "a")
来源：http://nj.hnjuh.cn

Ruby: s.count("a")
来源：http://na.shxzukj.cn

C#:   s.Count(c => c == 'a')
来源：http://my.shxzukj.cn

[E13] 逐字符遍历
来源：http://ho.chemitech.net.cn

Py:   for ch in s: print(ch)
来源：http://iw.nszjky.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://my.newstarts.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://zo.lnxyls.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bu.521024.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://it.lnxyls.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rm.wgjwhj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://gs.nszjky.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fn.chemitech.net.cn

[E14] URL 编码与 Base64
来源：http://et.bjjhwx.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ft.muxihuayi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://cu.bookmarksfly.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://em.shxzskj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lz.yuexingan06.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xt.huixinmuqiang.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rt.jctech888.com.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mg.huixinmuqiang.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vk.hahajie.cn

[E15] HTML 转义 / 反转义
来源：http://ev.huixinmuqiang.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://me.9csxet.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sq.haigaiapp.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sr.gzmigu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://zd.huixinmuqiang.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ag.colortex.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pd.szxytkj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nu.bjjhwx.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nf.jctech888.com.cn

[E16] 数字千分位
来源：http://cu.lnxyls.cn

Py:   f"{1234567:,}"
来源：http://au.panjiajie.cn

PHP:  number_format(1234567);
来源：http://sm.shxzskj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://yq.nicolike.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://yt.panjiajie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fj.jianghongdianzi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://su.shxzskj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vg.9csxet.cn

C#:   1234567.ToString("N0")
来源：http://bc.yuexingan06.cn

[E17] 首字母大写
来源：http://br.hnjuh.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://je.bookmarksfly.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://jy.colortex.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oz.gzmigu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://in.muxihuayi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pq.bookmarksfly.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pi.shtwfgs.cn

Ruby: s.capitalize
来源：http://vd.nicolike.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://sv.nicolike.cn

[E18] 模板占位符替换
来源：http://yc.haigaiapp.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gb.hnjuh.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yc.wgjwhj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://lf.colortex.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://sm.hahajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zg.muxihuayi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sm.shxzukj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gm.jianghongdianzi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vy.jianghongdianzi.cn

[E19] 多行文本按行拆分
来源：http://fk.shxzskj.cn

Py:   s.splitlines()
来源：http://kp.yuexingan06.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ry.newstarts.cn

JS:   s.split(/\r?\n/)
来源：http://il.hahajie.cn

TS:   s.split(/\r?\n/)
来源：http://un.hahajie.cn

Java: s.lines().toList()
来源：http://bc.muxihuayi.cn

Go:   strings.Split(s, "\n")
来源：http://dg.bjjhwx.cn

Ruby: s.lines
来源：http://jp.hahajie.cn

C#:   s.Split('\n')
来源：http://km.lnxyls.cn

[E20] 判断字符串是否为空
来源：http://ub.521024.cn

Py:   if not s:
来源：http://tp.jianghongdianzi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bj.yuexingan06.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qg.szxytkj.cn

TS:   if (s === "") {}
来源：http://km.nszjky.cn

Java: if (s.isEmpty()) {}
来源：http://kf.gzmigu.cn

Go:   if s == "" {}
来源：http://ez.9csxet.cn

Ruby: if s.empty?
来源：http://br.shxzskj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ys.hahajie.cn

[E21] 超长截断加省略号
来源：http://wn.bookmarksfly.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hi.shxzukj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lm.nicolike.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ss.szsharing.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://je.521024.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://al.panjiajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://jd.shxzskj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ei.jctech888.com.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://uu.yuexingan06.cn

[E22] 字节长度与字符长度
来源：http://ak.bookmarksfly.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kv.yuntaijiaju.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uo.jianghongdianzi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jn.wgjwhj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://eq.muxihuayi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://du.jctech888.com.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qv.9csxet.cn

Ruby: s.bytesize;  s.length
来源：http://yp.huanxung.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gy.9csxet.cn

================================================================================
来源：http://es.wgjwhj.cn

F. 文件与目录
来源：http://ni.muxihuayi.cn

================================================================================
来源：http://xq.shxzukj.cn

[F01] 读取整个文件
来源：http://uv.lnxyls.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://sd.hnjuh.cn

PHP:  file_get_contents("a.txt");
来源：http://gx.bookmarksfly.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bx.nicolike.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://eq.asd995.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://lg.gzmigu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jc.newstarts.cn

Ruby: File.read("a.txt")
来源：http://jb.nicolike.cn

C#:   File.ReadAllText("a.txt");
来源：http://rl.shxzukj.cn

[F02] 逐行读取文件
来源：http://dw.yuexingan06.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ck.panjiajie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pp.huanxung.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://na.huixinmuqiang.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zu.yuexingan06.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hk.chemitech.net.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tl.nicolike.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nl.huixiangedu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bp.asd995.cn

[F03] 写入文件（覆盖）
来源：http://cr.nszjky.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yx.bjjhwx.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://bp.panjiajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wf.chemitech.net.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jg.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://eb.chemitech.net.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ex.nicolike.cn

Ruby: File.write("a.txt", "hi")
来源：http://sy.newstarts.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://im.gzmigu.cn

[F04] 追加写入文件
来源：http://rj.gzmigu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wn.yuexingan06.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rg.lnxyls.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zt.hnjuh.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oi.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xj.shxzukj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://co.muxihuayi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yu.shxzukj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yt.shxzskj.cn

[F05] 判断文件或目录是否存在
来源：http://jf.muxihuayi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yx.chemitech.net.cn

PHP:  file_exists("a.txt");
来源：http://zh.asd995.cn

JS:   fs.existsSync("a.txt")
来源：http://ux.colortex.cn

TS:   fs.existsSync("a.txt")
来源：http://qn.521024.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://np.szsharing.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kg.521024.cn

Ruby: File.exist?("a.txt")
来源：http://qn.haigaiapp.cn

C#:   File.Exists("a.txt")
来源：http://vx.wgjwhj.cn

[F06] 删除文件
来源：http://kn.jianghongdianzi.cn

Py:   os.remove("a.txt")
来源：http://nr.huanxung.cn

PHP:  unlink("a.txt");
来源：http://pc.shxzukj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://bq.shxzskj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://gc.yuexingan06.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hv.gzmigu.cn

Go:   os.Remove("a.txt")
来源：http://eh.colortex.cn

Ruby: File.delete("a.txt")
来源：http://gf.haigaiapp.cn

C#:   File.Delete("a.txt");
来源：http://uy.huanxung.cn

[F07] 创建目录（含多级）
来源：http://cm.shtwfgs.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qs.bookmarksfly.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wg.jianghongdianzi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ef.gzmigu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ks.yuexingan06.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xd.shtwfgs.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://sv.bookmarksfly.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hw.colortex.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sj.bookmarksfly.cn

[F08] 遍历目录
来源：http://jt.gzmigu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://wm.bjjhwx.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fb.bjjhwx.cn

JS:   fs.readdirSync("dir")
来源：http://xz.chemitech.net.cn

TS:   fs.readdirSync("dir")
来源：http://rk.shtwfgs.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dw.bookmarksfly.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fn.jianghongdianzi.cn

Ruby: Dir.children("dir")
来源：http://bb.huanxung.cn

C#:   Directory.GetFiles("dir")
来源：http://wy.hnjuh.cn

[F09] 获取文件大小
来源：http://bg.gzmigu.cn

Py:   os.path.getsize("a.txt")
来源：http://zo.jianghongdianzi.cn

PHP:  filesize("a.txt");
来源：http://bc.521024.cn

JS:   fs.statSync("a.txt").size
来源：http://ha.jianghongdianzi.cn

TS:   fs.statSync("a.txt").size
来源：http://bs.nicolike.cn

Java: Files.size(Path.of("a.txt"))
来源：http://vw.shtwfgs.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ci.gzmigu.cn

Ruby: File.size("a.txt")
来源：http://mm.bjjhwx.cn

C#:   new FileInfo("a.txt").Length
来源：http://ga.huanxung.cn

[F10] 取文件扩展名 / 文件名
来源：http://jl.panjiajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://iw.szxytkj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gc.hahajie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dv.szsharing.cn

TS:   path.extname("a.txt")
来源：http://qs.bjjhwx.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qm.nszjky.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cn.yuntaijiaju.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ak.lnxyls.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mr.hahajie.cn

[F11] 复制与移动文件
来源：http://dg.newstarts.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://en.chemitech.net.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://av.jianghongdianzi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xf.huixinmuqiang.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mw.hahajie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vo.521024.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vp.nicolike.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sl.huixinmuqiang.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vj.szxytkj.cn

[F12] CSV 读写
来源：http://so.hahajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jw.haigaiapp.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wm.panjiajie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jw.hahajie.cn

TS:   // 同上
来源：http://yb.hnjuh.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cv.chemitech.net.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zv.bjjhwx.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qn.shxzskj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://tu.nicolike.cn

================================================================================
来源：http://ni.9csxet.cn

G. 面向对象
来源：http://xk.chemitech.net.cn

================================================================================
来源：http://ad.lnxyls.cn

[G01] 定义类
来源：http://qu.9csxet.cn

Py:   class User: pass
来源：http://zg.nicolike.cn

PHP:  class User {}
来源：http://xm.nicolike.cn

JS:   class User {}
来源：http://gh.huanxung.cn

TS:   class User { name: string = ""; }
来源：http://qi.wgjwhj.cn

Java: class User {}
来源：http://gu.521024.cn

Go:   type User struct { Name string }
来源：http://yx.hnjuh.cn

Ruby: class User; end
来源：http://qf.yuntaijiaju.cn

C#:   class User {}
来源：http://gg.nszjky.cn

[G02] 构造函数
来源：http://cf.colortex.cn

Py:   def __init__(self, name): self.name = name
来源：http://iz.9csxet.cn

PHP:  public function __construct(public string $name) {}
来源：http://pw.huanxung.cn

JS:   constructor(name) { this.name = name; }
来源：http://eh.lnxyls.cn

TS:   constructor(public name: string) {}
来源：http://ye.bookmarksfly.cn

Java: User(String name) { this.name = name; }
来源：http://rr.yuntaijiaju.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dz.chemitech.net.cn

Ruby: def initialize(name); @name = name; end
来源：http://ew.lnxyls.cn

C#:   public User(string name) { Name = name; }
来源：http://hj.hnjuh.cn

[G03] 实例属性
来源：http://xf.muxihuayi.cn

Py:   self.name = "x"
来源：http://jn.yuntaijiaju.cn

PHP:  public string $name = "x";
来源：http://vf.lnxyls.cn

JS:   this.name = "x";
来源：http://mk.huixiangedu.cn

TS:   name: string = "x";
来源：http://bu.huanxung.cn

Java: private String name;
来源：http://yd.nicolike.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nw.shxzukj.cn


<!-- 参考信息 -->