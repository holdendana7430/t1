代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vp.hnjuh.cn

[E03] 截取子串
来源：http://pw.panjiajie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gn.shxzskj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kc.szsharing.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yo.huixiangedu.cn

TS:   s.slice(1, 4)
来源：http://as.9csxet.cn

Java: s.substring(1, 4)
来源：http://bw.521024.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ng.chemitech.net.cn

Ruby: s[1, 3];  s[1..3]
来源：http://pj.hahajie.cn

C#:   s.Substring(1, 3)
来源：http://dh.huixiangedu.cn

[E04] 查找子串位置
来源：http://bw.szxytkj.cn

Py:   s.find("x");  s.index("x")
来源：http://pq.szsharing.cn

PHP:  strpos($s, "x");
来源：http://lj.huixiangedu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ps.yuntaijiaju.cn

TS:   s.indexOf("x")
来源：http://pz.jctech888.com.cn

Java: s.indexOf("x")
来源：http://vd.jctech888.com.cn

Go:   strings.Index(s, "x")
来源：http://fk.haigaiapp.cn

Ruby: s.index("x")
来源：http://aw.nicolike.cn

C#:   s.IndexOf("x")
来源：http://oa.gzmigu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://bk.jctech888.com.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bc.haigaiapp.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rs.szsharing.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fb.colortex.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://jf.yuexingan06.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rd.haigaiapp.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ct.szxytkj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zy.jianghongdianzi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lp.huixinmuqiang.cn

[E06] 替换子串
来源：http://nh.asd995.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://eb.521024.cn

PHP:  str_replace("a", "b", $s);
来源：http://js.asd995.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dj.jctech888.com.cn

TS:   s.replaceAll("a", "b")
来源：http://nx.jianghongdianzi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kg.jctech888.com.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wp.9csxet.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fn.colortex.cn

C#:   s.Replace("a", "b")
来源：http://au.yuexingan06.cn

[E07] 按分隔符拆分
来源：http://yw.lnxyls.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://eg.wgjwhj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://of.jianghongdianzi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://va.9csxet.cn

TS:   s.split(",")
来源：http://lv.lnxyls.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ia.9csxet.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xy.huixiangedu.cn

Ruby: s.split(",");  s.split
来源：http://pe.shxzukj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tx.hnjuh.cn

[E08] 数组按分隔符合并
来源：http://zh.jianghongdianzi.cn

Py:   ",".join(items)
来源：http://qz.szxytkj.cn

PHP:  implode(",", $items);
来源：http://uo.yuntaijiaju.cn

JS:   items.join(",")
来源：http://kf.asd995.cn

TS:   items.join(",")
来源：http://eh.yuntaijiaju.cn

Java: String.join(",", items)
来源：http://it.chemitech.net.cn

Go:   strings.Join(items, ",")
来源：http://nq.szxytkj.cn

Ruby: items.join(",")
来源：http://wz.newstarts.cn

C#:   string.Join(",", items)
来源：http://zd.colortex.cn

[E09] 去除所有空白字符
来源：http://rt.nszjky.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://uy.colortex.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://co.jianghongdianzi.cn

JS:   s.replace(/\s+/g, "")
来源：http://ku.hahajie.cn

TS:   s.replace(/\s+/g, "")
来源：http://hf.jctech888.com.cn

Java: s.replaceAll("\\s+", "")
来源：http://vk.muxihuayi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ij.nszjky.cn

Ruby: s.gsub(/\s+/, "")
来源：http://jb.bookmarksfly.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fk.jctech888.com.cn

[E10] 左侧补零 / 定长填充
来源：http://jv.gzmigu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://oo.bjjhwx.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qz.colortex.cn

JS:   "7".padStart(3, "0")
来源：http://rr.szxytkj.cn

TS:   "7".padStart(3, "0")
来源：http://ru.yuntaijiaju.cn

Java: String.format("%03d", 7)
来源：http://mm.521024.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ob.bookmarksfly.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://oq.haigaiapp.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hk.haigaiapp.cn

[E11] 反转字符串
来源：http://gv.nicolike.cn

Py:   s[::-1]
来源：http://gl.shxzskj.cn

PHP:  strrev($s);
来源：http://it.bjjhwx.cn

JS:   [...s].reverse().join("")
来源：http://cb.shtwfgs.cn

TS:   [...s].reverse().join("")
来源：http://ck.szxytkj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://nc.wgjwhj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://hq.muxihuayi.cn

Ruby: s.reverse
来源：http://de.huixinmuqiang.cn

C#:   new string(s.Reverse().ToArray())
来源：http://sn.colortex.cn

[E12] 统计某字符出现次数
来源：http://cw.yuntaijiaju.cn

Py:   s.count("a")
来源：http://cz.colortex.cn

PHP:  substr_count($s, "a");
来源：http://br.szsharing.cn

JS:   s.split("a").length - 1
来源：http://jc.bjjhwx.cn

TS:   s.split("a").length - 1
来源：http://fd.jianghongdianzi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fe.gzmigu.cn

Go:   strings.Count(s, "a")
来源：http://gi.shxzskj.cn

Ruby: s.count("a")
来源：http://oj.szxytkj.cn

C#:   s.Count(c => c == 'a')
来源：http://to.asd995.cn

[E13] 逐字符遍历
来源：http://mz.muxihuayi.cn

Py:   for ch in s: print(ch)
来源：http://mb.lnxyls.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zk.jianghongdianzi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ez.gzmigu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://an.huixiangedu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jy.nicolike.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rx.nicolike.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://hi.wgjwhj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kq.yuntaijiaju.cn

[E14] URL 编码与 Base64
来源：http://mn.bookmarksfly.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sa.huanxung.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ls.huixinmuqiang.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://sh.szsharing.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fw.jianghongdianzi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pu.hnjuh.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fr.huixiangedu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://iq.jianghongdianzi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pq.bookmarksfly.cn

[E15] HTML 转义 / 反转义
来源：http://yu.jianghongdianzi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://kj.yuntaijiaju.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://px.shxzukj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zm.shtwfgs.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://kx.panjiajie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gy.huixinmuqiang.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yz.asd995.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fo.shxzskj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://um.nicolike.cn

[E16] 数字千分位
来源：http://xh.haigaiapp.cn

Py:   f"{1234567:,}"
来源：http://zj.bjjhwx.cn

PHP:  number_format(1234567);
来源：http://sw.nszjky.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ls.huixiangedu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ig.huixinmuqiang.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hs.shxzukj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xh.shtwfgs.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dv.szxytkj.cn

C#:   1234567.ToString("N0")
来源：http://ab.panjiajie.cn

[E17] 首字母大写
来源：http://do.szsharing.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cz.yuexingan06.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://jp.jianghongdianzi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ho.nicolike.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tu.huanxung.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://if.nicolike.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nn.521024.cn

Ruby: s.capitalize
来源：http://bd.haigaiapp.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://oa.yuntaijiaju.cn

[E18] 模板占位符替换
来源：http://ry.jctech888.com.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qe.jctech888.com.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ne.shtwfgs.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://yw.huanxung.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://bv.huixiangedu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wk.szsharing.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sm.haigaiapp.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://so.gzmigu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://oc.chemitech.net.cn

[E19] 多行文本按行拆分
来源：http://fo.asd995.cn

Py:   s.splitlines()
来源：http://hi.jctech888.com.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yq.bookmarksfly.cn

JS:   s.split(/\r?\n/)
来源：http://do.asd995.cn

TS:   s.split(/\r?\n/)
来源：http://kg.shxzukj.cn

Java: s.lines().toList()
来源：http://sz.bjjhwx.cn

Go:   strings.Split(s, "\n")
来源：http://wa.521024.cn

Ruby: s.lines
来源：http://xo.huanxung.cn

C#:   s.Split('\n')
来源：http://zv.huixiangedu.cn

[E20] 判断字符串是否为空
来源：http://ht.huixiangedu.cn

Py:   if not s:
来源：http://mo.jianghongdianzi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tb.521024.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pd.huixiangedu.cn

TS:   if (s === "") {}
来源：http://jf.shtwfgs.cn

Java: if (s.isEmpty()) {}
来源：http://ws.huixiangedu.cn

Go:   if s == "" {}
来源：http://wt.jctech888.com.cn

Ruby: if s.empty?
来源：http://au.panjiajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ut.huixiangedu.cn

[E21] 超长截断加省略号
来源：http://ju.jianghongdianzi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lg.yuntaijiaju.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bn.shtwfgs.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://te.bookmarksfly.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nq.gzmigu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bj.521024.cn

Go:   // 按 rune 判断长度后截断
来源：http://ri.lnxyls.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://id.haigaiapp.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hu.jianghongdianzi.cn

[E22] 字节长度与字符长度
来源：http://yh.jianghongdianzi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://te.bookmarksfly.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sq.colortex.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ig.nszjky.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wa.shxzskj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fa.huixiangedu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://td.nicolike.cn

Ruby: s.bytesize;  s.length
来源：http://rd.shtwfgs.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nu.asd995.cn

================================================================================
来源：http://aa.jctech888.com.cn

F. 文件与目录
来源：http://vb.shxzskj.cn

================================================================================
来源：http://pt.jianghongdianzi.cn

[F01] 读取整个文件
来源：http://gq.lnxyls.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zz.nicolike.cn

PHP:  file_get_contents("a.txt");
来源：http://gp.yuexingan06.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lw.nszjky.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xy.panjiajie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://cp.yuntaijiaju.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cg.shxzskj.cn

Ruby: File.read("a.txt")
来源：http://dm.lnxyls.cn

C#:   File.ReadAllText("a.txt");
来源：http://ax.szsharing.cn

[F02] 逐行读取文件
来源：http://ev.muxihuayi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mm.huanxung.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qb.hahajie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fi.bjjhwx.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aj.colortex.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://oh.szxytkj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xk.panjiajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ly.lnxyls.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jd.hahajie.cn

[F03] 写入文件（覆盖）
来源：http://be.asd995.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fv.bookmarksfly.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://bz.lnxyls.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rq.huixinmuqiang.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cd.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pc.muxihuayi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://iw.bookmarksfly.cn

Ruby: File.write("a.txt", "hi")
来源：http://nq.yuexingan06.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://to.szsharing.cn

[F04] 追加写入文件
来源：http://jw.szxytkj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dv.hahajie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://sq.521024.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://aa.huixinmuqiang.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tb.9csxet.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fe.yuexingan06.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ln.jctech888.com.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://in.hahajie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ho.huanxung.cn

[F05] 判断文件或目录是否存在
来源：http://hr.yuntaijiaju.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wt.hahajie.cn

PHP:  file_exists("a.txt");
来源：http://ot.jctech888.com.cn

JS:   fs.existsSync("a.txt")
来源：http://tm.lnxyls.cn

TS:   fs.existsSync("a.txt")
来源：http://wt.jianghongdianzi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://cb.szsharing.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ew.shxzukj.cn

Ruby: File.exist?("a.txt")
来源：http://ft.jianghongdianzi.cn

C#:   File.Exists("a.txt")
来源：http://te.9csxet.cn

[F06] 删除文件
来源：http://bl.szxytkj.cn

Py:   os.remove("a.txt")
来源：http://rc.chemitech.net.cn

PHP:  unlink("a.txt");
来源：http://bb.muxihuayi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://cm.gzmigu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://om.huixiangedu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cs.chemitech.net.cn

Go:   os.Remove("a.txt")
来源：http://hh.huixiangedu.cn

Ruby: File.delete("a.txt")
来源：http://ze.huixiangedu.cn

C#:   File.Delete("a.txt");
来源：http://vf.bjjhwx.cn

[F07] 创建目录（含多级）
来源：http://ln.nicolike.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lw.jctech888.com.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://oy.9csxet.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wi.yuntaijiaju.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fu.colortex.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cq.huanxung.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dj.yuexingan06.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://oi.chemitech.net.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ha.chemitech.net.cn

[F08] 遍历目录
来源：http://wn.521024.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ck.szxytkj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://al.lnxyls.cn

JS:   fs.readdirSync("dir")
来源：http://ib.nszjky.cn

TS:   fs.readdirSync("dir")
来源：http://iw.szsharing.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hu.huixinmuqiang.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ha.jctech888.com.cn

Ruby: Dir.children("dir")
来源：http://rv.wgjwhj.cn

C#:   Directory.GetFiles("dir")
来源：http://vm.asd995.cn

[F09] 获取文件大小
来源：http://bd.muxihuayi.cn

Py:   os.path.getsize("a.txt")
来源：http://kt.yuntaijiaju.cn

PHP:  filesize("a.txt");
来源：http://zl.bjjhwx.cn

JS:   fs.statSync("a.txt").size
来源：http://cs.shtwfgs.cn

TS:   fs.statSync("a.txt").size
来源：http://uh.jctech888.com.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ag.wgjwhj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yd.chemitech.net.cn

Ruby: File.size("a.txt")
来源：http://bf.jianghongdianzi.cn

C#:   new FileInfo("a.txt").Length
来源：http://ia.shtwfgs.cn

[F10] 取文件扩展名 / 文件名
来源：http://xz.newstarts.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://eh.newstarts.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://sv.jianghongdianzi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://za.nszjky.cn

TS:   path.extname("a.txt")
来源：http://so.shxzukj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zw.gzmigu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ae.shxzukj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dw.panjiajie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pf.haigaiapp.cn

[F11] 复制与移动文件
来源：http://lo.bjjhwx.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nf.colortex.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hp.lnxyls.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pq.lnxyls.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cj.wgjwhj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vj.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wy.huixinmuqiang.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kv.muxihuayi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://uo.shxzukj.cn

[F12] CSV 读写
来源：http://ds.yuntaijiaju.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xp.hahajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tq.yuntaijiaju.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fn.panjiajie.cn

TS:   // 同上
来源：http://pk.521024.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kc.nszjky.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yu.9csxet.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nm.gzmigu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://os.szxytkj.cn

================================================================================
来源：http://fc.szsharing.cn

G. 面向对象
来源：http://xm.shxzukj.cn

================================================================================
来源：http://gh.huixiangedu.cn

[G01] 定义类
来源：http://ni.chemitech.net.cn

Py:   class User: pass
来源：http://rp.huixinmuqiang.cn

PHP:  class User {}
来源：http://kv.nicolike.cn

JS:   class User {}
来源：http://od.haigaiapp.cn

TS:   class User { name: string = ""; }
来源：http://nm.lnxyls.cn


<!-- 参考信息 -->