代发 wailian999

TS:   "ab".repeat(3)
来源：http://ut.521024.cn

Java: "ab".repeat(3)
来源：http://cv.colortex.cn

Go:   strings.Repeat("ab", 3)
来源：http://ic.jctech888.com.cn

Ruby: "ab" * 3
来源：http://qh.yuntaijiaju.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fw.panjiajie.cn

[E03] 截取子串
来源：http://fk.panjiajie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hy.jctech888.com.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pm.521024.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://si.huixinmuqiang.cn

TS:   s.slice(1, 4)
来源：http://cv.huanxung.cn

Java: s.substring(1, 4)
来源：http://ul.huixiangedu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nu.wgjwhj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zj.colortex.cn

C#:   s.Substring(1, 3)
来源：http://rb.bjjhwx.cn

[E04] 查找子串位置
来源：http://bc.9csxet.cn

Py:   s.find("x");  s.index("x")
来源：http://uf.bookmarksfly.cn

PHP:  strpos($s, "x");
来源：http://uq.huixinmuqiang.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jb.nicolike.cn

TS:   s.indexOf("x")
来源：http://kk.bjjhwx.cn

Java: s.indexOf("x")
来源：http://fe.521024.cn

Go:   strings.Index(s, "x")
来源：http://vw.yuntaijiaju.cn

Ruby: s.index("x")
来源：http://eo.chemitech.net.cn

C#:   s.IndexOf("x")
来源：http://ua.yuexingan06.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gq.bookmarksfly.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://sy.shxzskj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ys.asd995.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tt.chemitech.net.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hb.nszjky.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dl.shxzskj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zz.bjjhwx.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tm.panjiajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mo.asd995.cn

[E06] 替换子串
来源：http://vc.nicolike.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nr.lnxyls.cn

PHP:  str_replace("a", "b", $s);
来源：http://sb.jctech888.com.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gg.shxzskj.cn

TS:   s.replaceAll("a", "b")
来源：http://eo.hahajie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ev.hnjuh.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xp.yuntaijiaju.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://df.huixinmuqiang.cn

C#:   s.Replace("a", "b")
来源：http://ml.newstarts.cn

[E07] 按分隔符拆分
来源：http://sw.shtwfgs.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qa.jctech888.com.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qt.shtwfgs.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://mz.asd995.cn

TS:   s.split(",")
来源：http://xl.hnjuh.cn

Java: s.split(",");  s.split("\\s+")
来源：http://hh.huixinmuqiang.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tk.jctech888.com.cn

Ruby: s.split(",");  s.split
来源：http://qk.shxzskj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ru.wgjwhj.cn

[E08] 数组按分隔符合并
来源：http://lc.yuntaijiaju.cn

Py:   ",".join(items)
来源：http://np.bjjhwx.cn

PHP:  implode(",", $items);
来源：http://fi.szxytkj.cn

JS:   items.join(",")
来源：http://us.shxzskj.cn

TS:   items.join(",")
来源：http://ky.jianghongdianzi.cn

Java: String.join(",", items)
来源：http://xg.jianghongdianzi.cn

Go:   strings.Join(items, ",")
来源：http://ly.shxzskj.cn

Ruby: items.join(",")
来源：http://vd.huixinmuqiang.cn

C#:   string.Join(",", items)
来源：http://so.shxzukj.cn

[E09] 去除所有空白字符
来源：http://zu.chemitech.net.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ts.jianghongdianzi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://un.shtwfgs.cn

JS:   s.replace(/\s+/g, "")
来源：http://vg.lnxyls.cn

TS:   s.replace(/\s+/g, "")
来源：http://ds.newstarts.cn

Java: s.replaceAll("\\s+", "")
来源：http://ck.jianghongdianzi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://xl.jctech888.com.cn

Ruby: s.gsub(/\s+/, "")
来源：http://mi.gzmigu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zh.huixiangedu.cn

[E10] 左侧补零 / 定长填充
来源：http://il.nicolike.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hp.9csxet.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zv.jctech888.com.cn

JS:   "7".padStart(3, "0")
来源：http://mp.shxzukj.cn

TS:   "7".padStart(3, "0")
来源：http://zk.huixinmuqiang.cn

Java: String.format("%03d", 7)
来源：http://ur.bjjhwx.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://mx.szxytkj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jw.lnxyls.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dz.lnxyls.cn

[E11] 反转字符串
来源：http://ma.jianghongdianzi.cn

Py:   s[::-1]
来源：http://bt.wgjwhj.cn

PHP:  strrev($s);
来源：http://pn.wgjwhj.cn

JS:   [...s].reverse().join("")
来源：http://nf.newstarts.cn

TS:   [...s].reverse().join("")
来源：http://uk.yuntaijiaju.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://fb.bjjhwx.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://us.bookmarksfly.cn

Ruby: s.reverse
来源：http://gz.muxihuayi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ot.yuexingan06.cn

[E12] 统计某字符出现次数
来源：http://sn.colortex.cn

Py:   s.count("a")
来源：http://fg.shxzskj.cn

PHP:  substr_count($s, "a");
来源：http://lc.nszjky.cn

JS:   s.split("a").length - 1
来源：http://nj.szsharing.cn

TS:   s.split("a").length - 1
来源：http://qq.lnxyls.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hd.wgjwhj.cn

Go:   strings.Count(s, "a")
来源：http://bn.yuntaijiaju.cn

Ruby: s.count("a")
来源：http://cc.muxihuayi.cn

C#:   s.Count(c => c == 'a')
来源：http://jl.wgjwhj.cn

[E13] 逐字符遍历
来源：http://oa.chemitech.net.cn

Py:   for ch in s: print(ch)
来源：http://ce.shtwfgs.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ni.szxytkj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ly.huixiangedu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wu.bjjhwx.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bc.newstarts.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ic.gzmigu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rn.huanxung.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yw.huixiangedu.cn

[E14] URL 编码与 Base64
来源：http://yu.jctech888.com.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ge.huanxung.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qf.szxytkj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vj.chemitech.net.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yn.gzmigu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qu.newstarts.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ul.shxzukj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://na.lnxyls.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ws.newstarts.cn

[E15] HTML 转义 / 反转义
来源：http://iy.haigaiapp.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ig.shxzskj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ar.colortex.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pz.colortex.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ih.521024.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://th.bookmarksfly.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ci.haigaiapp.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ql.hnjuh.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wg.muxihuayi.cn

[E16] 数字千分位
来源：http://cf.wgjwhj.cn

Py:   f"{1234567:,}"
来源：http://om.newstarts.cn

PHP:  number_format(1234567);
来源：http://uh.newstarts.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ie.gzmigu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://jb.nszjky.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ps.asd995.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://eq.jianghongdianzi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://am.huixiangedu.cn

C#:   1234567.ToString("N0")
来源：http://jk.hahajie.cn

[E17] 首字母大写
来源：http://jj.lnxyls.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ep.bookmarksfly.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://mc.szsharing.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yq.szsharing.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rt.521024.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cb.huanxung.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mg.asd995.cn

Ruby: s.capitalize
来源：http://ck.shxzskj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tq.nszjky.cn

[E18] 模板占位符替换
来源：http://fp.huixiangedu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mq.yuntaijiaju.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nk.521024.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://vd.colortex.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://sz.shxzukj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rg.nszjky.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kt.asd995.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tk.haigaiapp.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xx.huanxung.cn

[E19] 多行文本按行拆分
来源：http://td.newstarts.cn

Py:   s.splitlines()
来源：http://qa.nicolike.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jp.colortex.cn

JS:   s.split(/\r?\n/)
来源：http://xy.colortex.cn

TS:   s.split(/\r?\n/)
来源：http://dn.shtwfgs.cn

Java: s.lines().toList()
来源：http://fu.panjiajie.cn

Go:   strings.Split(s, "\n")
来源：http://pz.colortex.cn

Ruby: s.lines
来源：http://xb.lnxyls.cn

C#:   s.Split('\n')
来源：http://jz.szxytkj.cn

[E20] 判断字符串是否为空
来源：http://lx.muxihuayi.cn

Py:   if not s:
来源：http://vg.wgjwhj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://om.asd995.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tj.nicolike.cn

TS:   if (s === "") {}
来源：http://rj.yuexingan06.cn

Java: if (s.isEmpty()) {}
来源：http://di.lnxyls.cn

Go:   if s == "" {}
来源：http://cg.newstarts.cn

Ruby: if s.empty?
来源：http://yv.lnxyls.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://km.9csxet.cn

[E21] 超长截断加省略号
来源：http://kb.shtwfgs.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ds.hnjuh.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ie.9csxet.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ly.nszjky.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sx.bjjhwx.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://un.huixiangedu.cn

Go:   // 按 rune 判断长度后截断
来源：http://au.szsharing.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cc.wgjwhj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://py.lnxyls.cn

[E22] 字节长度与字符长度
来源：http://hw.szxytkj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ad.chemitech.net.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nj.newstarts.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zn.asd995.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sk.521024.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ko.panjiajie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fq.szsharing.cn

Ruby: s.bytesize;  s.length
来源：http://js.muxihuayi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tz.bjjhwx.cn

================================================================================
来源：http://px.shxzskj.cn

F. 文件与目录
来源：http://qq.haigaiapp.cn

================================================================================
来源：http://sv.bjjhwx.cn

[F01] 读取整个文件
来源：http://gq.yuexingan06.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uv.gzmigu.cn

PHP:  file_get_contents("a.txt");
来源：http://vz.lnxyls.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fi.szxytkj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nl.huixiangedu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://au.bookmarksfly.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nh.shxzskj.cn

Ruby: File.read("a.txt")
来源：http://li.shtwfgs.cn

C#:   File.ReadAllText("a.txt");
来源：http://dm.nszjky.cn

[F02] 逐行读取文件
来源：http://rc.bjjhwx.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://iq.jctech888.com.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hb.muxihuayi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sf.yuexingan06.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://re.521024.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nx.shxzukj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zx.nszjky.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jp.jctech888.com.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pb.bookmarksfly.cn

[F03] 写入文件（覆盖）
来源：http://am.szsharing.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://up.colortex.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://jp.yuntaijiaju.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://aj.chemitech.net.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qi.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jh.huixinmuqiang.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wt.521024.cn

Ruby: File.write("a.txt", "hi")
来源：http://ad.nicolike.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pq.huixinmuqiang.cn

[F04] 追加写入文件
来源：http://ar.shxzskj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bu.bookmarksfly.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xf.jianghongdianzi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fz.chemitech.net.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cj.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://su.nszjky.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://un.yuexingan06.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yk.shtwfgs.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fr.haigaiapp.cn

[F05] 判断文件或目录是否存在
来源：http://gz.chemitech.net.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ul.gzmigu.cn

PHP:  file_exists("a.txt");
来源：http://bz.nicolike.cn

JS:   fs.existsSync("a.txt")
来源：http://ai.panjiajie.cn

TS:   fs.existsSync("a.txt")
来源：http://hv.haigaiapp.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://wk.asd995.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://su.muxihuayi.cn

Ruby: File.exist?("a.txt")
来源：http://vp.asd995.cn

C#:   File.Exists("a.txt")
来源：http://ij.huixinmuqiang.cn

[F06] 删除文件
来源：http://pd.521024.cn

Py:   os.remove("a.txt")
来源：http://js.chemitech.net.cn

PHP:  unlink("a.txt");
来源：http://kl.huixinmuqiang.cn

JS:   fs.unlinkSync("a.txt")
来源：http://jm.jctech888.com.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ao.huixinmuqiang.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ke.hahajie.cn

Go:   os.Remove("a.txt")
来源：http://wo.yuntaijiaju.cn

Ruby: File.delete("a.txt")
来源：http://am.szsharing.cn

C#:   File.Delete("a.txt");
来源：http://jp.bjjhwx.cn

[F07] 创建目录（含多级）
来源：http://rm.newstarts.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sk.colortex.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jt.shtwfgs.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hh.bookmarksfly.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mv.9csxet.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vc.bjjhwx.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pw.huanxung.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gc.panjiajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bg.hnjuh.cn

[F08] 遍历目录
来源：http://mt.yuexingan06.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://pi.shtwfgs.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zn.haigaiapp.cn

JS:   fs.readdirSync("dir")
来源：http://sv.jctech888.com.cn

TS:   fs.readdirSync("dir")
来源：http://zh.chemitech.net.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ri.bjjhwx.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://sn.shxzskj.cn

Ruby: Dir.children("dir")
来源：http://oz.colortex.cn

C#:   Directory.GetFiles("dir")
来源：http://lp.shxzukj.cn

[F09] 获取文件大小
来源：http://jn.hahajie.cn

Py:   os.path.getsize("a.txt")
来源：http://os.haigaiapp.cn

PHP:  filesize("a.txt");
来源：http://fg.jianghongdianzi.cn

JS:   fs.statSync("a.txt").size
来源：http://ea.nicolike.cn

TS:   fs.statSync("a.txt").size
来源：http://eq.nicolike.cn

Java: Files.size(Path.of("a.txt"))
来源：http://qj.asd995.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nw.bookmarksfly.cn

Ruby: File.size("a.txt")
来源：http://qc.colortex.cn

C#:   new FileInfo("a.txt").Length
来源：http://ij.shxzskj.cn

[F10] 取文件扩展名 / 文件名
来源：http://nt.hnjuh.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ca.shxzskj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nc.jctech888.com.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://py.asd995.cn

TS:   path.extname("a.txt")
来源：http://fg.bjjhwx.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hj.jianghongdianzi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ld.hnjuh.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://uk.gzmigu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://az.jctech888.com.cn

[F11] 复制与移动文件
来源：http://em.shxzukj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ql.szxytkj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cy.521024.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cg.wgjwhj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nq.huanxung.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bh.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fl.bookmarksfly.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pv.chemitech.net.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tm.szsharing.cn

[F12] CSV 读写
来源：http://ad.nszjky.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lv.newstarts.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vy.nszjky.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ig.szxytkj.cn

TS:   // 同上
来源：http://gu.jctech888.com.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ji.asd995.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sr.hnjuh.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ty.yuntaijiaju.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://by.muxihuayi.cn

================================================================================
来源：http://if.wgjwhj.cn

G. 面向对象
来源：http://jq.huanxung.cn

================================================================================
来源：http://lk.hahajie.cn

[G01] 定义类
来源：http://as.colortex.cn


<!-- 参考信息 -->