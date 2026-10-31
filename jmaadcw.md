代发 wailian999

TS:   "ab".repeat(3)
来源：http://gl.gzmigu.cn

Java: "ab".repeat(3)
来源：http://ad.bjjhwx.cn

Go:   strings.Repeat("ab", 3)
来源：http://mk.szsharing.cn

Ruby: "ab" * 3
来源：http://pe.hahajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rr.jctech888.com.cn

[E03] 截取子串
来源：http://lg.bjjhwx.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yp.huanxung.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ua.panjiajie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gm.asd995.cn

TS:   s.slice(1, 4)
来源：http://xh.huanxung.cn

Java: s.substring(1, 4)
来源：http://ee.huanxung.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gn.yuntaijiaju.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zz.szsharing.cn

C#:   s.Substring(1, 3)
来源：http://re.newstarts.cn

[E04] 查找子串位置
来源：http://sv.bjjhwx.cn

Py:   s.find("x");  s.index("x")
来源：http://vf.bjjhwx.cn

PHP:  strpos($s, "x");
来源：http://eo.nicolike.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bg.szsharing.cn

TS:   s.indexOf("x")
来源：http://vp.gzmigu.cn

Java: s.indexOf("x")
来源：http://bx.gzmigu.cn

Go:   strings.Index(s, "x")
来源：http://kc.shxzukj.cn

Ruby: s.index("x")
来源：http://yq.colortex.cn

C#:   s.IndexOf("x")
来源：http://mb.jianghongdianzi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ke.yuntaijiaju.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://oh.shtwfgs.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ai.haigaiapp.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rf.huanxung.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xy.bjjhwx.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ap.gzmigu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sa.yuntaijiaju.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rt.panjiajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qc.shxzskj.cn

[E06] 替换子串
来源：http://he.szsharing.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tn.jianghongdianzi.cn

PHP:  str_replace("a", "b", $s);
来源：http://cf.panjiajie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bc.jctech888.com.cn

TS:   s.replaceAll("a", "b")
来源：http://he.muxihuayi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://va.nszjky.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qb.newstarts.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jq.newstarts.cn

C#:   s.Replace("a", "b")
来源：http://xa.9csxet.cn

[E07] 按分隔符拆分
来源：http://lm.shtwfgs.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kn.haigaiapp.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pa.shxzukj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://gi.haigaiapp.cn

TS:   s.split(",")
来源：http://vt.jianghongdianzi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://bm.hnjuh.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ki.panjiajie.cn

Ruby: s.split(",");  s.split
来源：http://jo.nszjky.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xd.lnxyls.cn

[E08] 数组按分隔符合并
来源：http://jc.huixinmuqiang.cn

Py:   ",".join(items)
来源：http://ez.hahajie.cn

PHP:  implode(",", $items);
来源：http://rp.521024.cn

JS:   items.join(",")
来源：http://zi.521024.cn

TS:   items.join(",")
来源：http://vf.haigaiapp.cn

Java: String.join(",", items)
来源：http://zl.9csxet.cn

Go:   strings.Join(items, ",")
来源：http://jr.szsharing.cn

Ruby: items.join(",")
来源：http://rf.hnjuh.cn

C#:   string.Join(",", items)
来源：http://nh.521024.cn

[E09] 去除所有空白字符
来源：http://jp.gzmigu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rx.huixinmuqiang.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://oj.yuexingan06.cn

JS:   s.replace(/\s+/g, "")
来源：http://yo.szsharing.cn

TS:   s.replace(/\s+/g, "")
来源：http://ao.521024.cn

Java: s.replaceAll("\\s+", "")
来源：http://dh.shtwfgs.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://rl.lnxyls.cn

Ruby: s.gsub(/\s+/, "")
来源：http://re.hnjuh.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uf.hahajie.cn

[E10] 左侧补零 / 定长填充
来源：http://tw.muxihuayi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jn.panjiajie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://un.shxzskj.cn

JS:   "7".padStart(3, "0")
来源：http://vv.haigaiapp.cn

TS:   "7".padStart(3, "0")
来源：http://rj.wgjwhj.cn

Java: String.format("%03d", 7)
来源：http://mx.bookmarksfly.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://bm.panjiajie.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://us.shxzskj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://os.bjjhwx.cn

[E11] 反转字符串
来源：http://ms.huixinmuqiang.cn

Py:   s[::-1]
来源：http://no.newstarts.cn

PHP:  strrev($s);
来源：http://mn.gzmigu.cn

JS:   [...s].reverse().join("")
来源：http://qo.gzmigu.cn

TS:   [...s].reverse().join("")
来源：http://rm.9csxet.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://uu.yuexingan06.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://om.nszjky.cn

Ruby: s.reverse
来源：http://jn.9csxet.cn

C#:   new string(s.Reverse().ToArray())
来源：http://zm.haigaiapp.cn

[E12] 统计某字符出现次数
来源：http://zd.shxzukj.cn

Py:   s.count("a")
来源：http://et.colortex.cn

PHP:  substr_count($s, "a");
来源：http://gr.bookmarksfly.cn

JS:   s.split("a").length - 1
来源：http://tl.gzmigu.cn

TS:   s.split("a").length - 1
来源：http://rk.lnxyls.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ur.shxzskj.cn

Go:   strings.Count(s, "a")
来源：http://ki.yuntaijiaju.cn

Ruby: s.count("a")
来源：http://zl.9csxet.cn

C#:   s.Count(c => c == 'a')
来源：http://ew.huixiangedu.cn

[E13] 逐字符遍历
来源：http://db.muxihuayi.cn

Py:   for ch in s: print(ch)
来源：http://pd.colortex.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fj.521024.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://gt.asd995.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bb.szxytkj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://er.nszjky.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qz.huixiangedu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ws.panjiajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://oo.panjiajie.cn

[E14] URL 编码与 Base64
来源：http://jb.szsharing.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fy.huixiangedu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://jv.shxzukj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bz.bjjhwx.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://iz.szsharing.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yl.jctech888.com.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ya.jianghongdianzi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gu.muxihuayi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cm.yuexingan06.cn

[E15] HTML 转义 / 反转义
来源：http://dv.colortex.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://iu.huixiangedu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ja.huixinmuqiang.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://on.gzmigu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ey.hahajie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qg.yuexingan06.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ta.yuexingan06.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ev.asd995.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nk.shxzskj.cn

[E16] 数字千分位
来源：http://so.lnxyls.cn

Py:   f"{1234567:,}"
来源：http://ag.shxzukj.cn

PHP:  number_format(1234567);
来源：http://gs.gzmigu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mz.jctech888.com.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wh.huixiangedu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://oe.bjjhwx.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qo.shtwfgs.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xj.521024.cn

C#:   1234567.ToString("N0")
来源：http://so.huixiangedu.cn

[E17] 首字母大写
来源：http://ud.newstarts.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qy.nicolike.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://zk.panjiajie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lm.bookmarksfly.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gq.muxihuayi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ll.huixinmuqiang.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jo.newstarts.cn

Ruby: s.capitalize
来源：http://rx.521024.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vu.shxzskj.cn

[E18] 模板占位符替换
来源：http://kj.hahajie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zm.shxzukj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ia.bookmarksfly.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://rz.521024.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://sw.hahajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ln.shxzukj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sn.jctech888.com.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wh.nicolike.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ls.521024.cn

[E19] 多行文本按行拆分
来源：http://jx.newstarts.cn

Py:   s.splitlines()
来源：http://ky.panjiajie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vk.jctech888.com.cn

JS:   s.split(/\r?\n/)
来源：http://nd.szxytkj.cn

TS:   s.split(/\r?\n/)
来源：http://yv.9csxet.cn

Java: s.lines().toList()
来源：http://au.shtwfgs.cn

Go:   strings.Split(s, "\n")
来源：http://zv.yuexingan06.cn

Ruby: s.lines
来源：http://of.shxzskj.cn

C#:   s.Split('\n')
来源：http://lv.hnjuh.cn

[E20] 判断字符串是否为空
来源：http://fp.szsharing.cn

Py:   if not s:
来源：http://sp.huanxung.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://of.jctech888.com.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tm.yuexingan06.cn

TS:   if (s === "") {}
来源：http://dx.hnjuh.cn

Java: if (s.isEmpty()) {}
来源：http://eu.huanxung.cn

Go:   if s == "" {}
来源：http://lu.newstarts.cn

Ruby: if s.empty?
来源：http://cv.bookmarksfly.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://uv.yuexingan06.cn

[E21] 超长截断加省略号
来源：http://ja.szsharing.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://em.huixiangedu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://eu.gzmigu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yl.hahajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hf.yuntaijiaju.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rt.newstarts.cn

Go:   // 按 rune 判断长度后截断
来源：http://wj.szsharing.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pk.wgjwhj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sx.newstarts.cn

[E22] 字节长度与字符长度
来源：http://mh.bjjhwx.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yn.nszjky.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://aa.asd995.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tf.yuntaijiaju.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jy.shxzskj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://as.huixiangedu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vb.jctech888.com.cn

Ruby: s.bytesize;  s.length
来源：http://kc.panjiajie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mz.panjiajie.cn

================================================================================
来源：http://gj.szxytkj.cn

F. 文件与目录
来源：http://qg.shxzskj.cn

================================================================================
来源：http://wn.yuexingan06.cn

[F01] 读取整个文件
来源：http://qc.szxytkj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ws.hahajie.cn

PHP:  file_get_contents("a.txt");
来源：http://fz.shtwfgs.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kj.bookmarksfly.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xf.bookmarksfly.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vw.nicolike.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xz.bjjhwx.cn

Ruby: File.read("a.txt")
来源：http://fm.szxytkj.cn

C#:   File.ReadAllText("a.txt");
来源：http://yr.chemitech.net.cn

[F02] 逐行读取文件
来源：http://vl.gzmigu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ty.jianghongdianzi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vo.colortex.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ei.nszjky.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xz.haigaiapp.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qi.yuntaijiaju.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tm.muxihuayi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ve.shxzskj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wr.yuntaijiaju.cn

[F03] 写入文件（覆盖）
来源：http://ly.bjjhwx.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lt.shxzukj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vb.nszjky.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bu.jianghongdianzi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oq.lnxyls.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://uz.muxihuayi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hp.nicolike.cn

Ruby: File.write("a.txt", "hi")
来源：http://xp.bookmarksfly.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qv.huixiangedu.cn

[F04] 追加写入文件
来源：http://jk.yuntaijiaju.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://al.shxzskj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://aj.colortex.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qs.gzmigu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ac.huixinmuqiang.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tx.9csxet.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qw.yuexingan06.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ow.yuexingan06.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cn.hnjuh.cn

[F05] 判断文件或目录是否存在
来源：http://th.nszjky.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qu.jianghongdianzi.cn

PHP:  file_exists("a.txt");
来源：http://vi.nszjky.cn

JS:   fs.existsSync("a.txt")
来源：http://ik.shxzskj.cn

TS:   fs.existsSync("a.txt")
来源：http://xa.huixinmuqiang.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qv.shxzukj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://af.huanxung.cn

Ruby: File.exist?("a.txt")
来源：http://fa.haigaiapp.cn

C#:   File.Exists("a.txt")
来源：http://wo.haigaiapp.cn

[F06] 删除文件
来源：http://uq.lnxyls.cn

Py:   os.remove("a.txt")
来源：http://kz.asd995.cn

PHP:  unlink("a.txt");
来源：http://ue.shtwfgs.cn

JS:   fs.unlinkSync("a.txt")
来源：http://sy.hnjuh.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ah.nicolike.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ev.jctech888.com.cn

Go:   os.Remove("a.txt")
来源：http://cu.chemitech.net.cn

Ruby: File.delete("a.txt")
来源：http://ut.gzmigu.cn

C#:   File.Delete("a.txt");
来源：http://bd.colortex.cn

[F07] 创建目录（含多级）
来源：http://om.shxzukj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lx.newstarts.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sf.jianghongdianzi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fm.hnjuh.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vv.hnjuh.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hr.shxzukj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lt.bookmarksfly.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ds.shxzskj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hy.huixiangedu.cn

[F08] 遍历目录
来源：http://nt.huixiangedu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ig.521024.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://st.huanxung.cn

JS:   fs.readdirSync("dir")
来源：http://ir.bookmarksfly.cn

TS:   fs.readdirSync("dir")
来源：http://cg.nszjky.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://of.yuexingan06.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://qd.9csxet.cn

Ruby: Dir.children("dir")
来源：http://hb.hahajie.cn

C#:   Directory.GetFiles("dir")
来源：http://go.shxzskj.cn

[F09] 获取文件大小
来源：http://rr.chemitech.net.cn

Py:   os.path.getsize("a.txt")
来源：http://xn.nszjky.cn

PHP:  filesize("a.txt");
来源：http://ix.lnxyls.cn

JS:   fs.statSync("a.txt").size
来源：http://pu.bookmarksfly.cn

TS:   fs.statSync("a.txt").size
来源：http://bn.wgjwhj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://jv.asd995.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kq.jctech888.com.cn

Ruby: File.size("a.txt")
来源：http://sx.shxzukj.cn

C#:   new FileInfo("a.txt").Length
来源：http://sz.jianghongdianzi.cn

[F10] 取文件扩展名 / 文件名
来源：http://lk.huanxung.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fw.lnxyls.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yy.shtwfgs.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://es.gzmigu.cn

TS:   path.extname("a.txt")
来源：http://ku.szsharing.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qt.szsharing.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lx.colortex.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zw.colortex.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mf.newstarts.cn

[F11] 复制与移动文件
来源：http://cg.nicolike.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zm.huixiangedu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ub.wgjwhj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wh.shxzukj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wk.huixiangedu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mm.hahajie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ed.gzmigu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lo.chemitech.net.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vp.jianghongdianzi.cn

[F12] CSV 读写
来源：http://fz.wgjwhj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cj.shtwfgs.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rj.9csxet.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://am.jianghongdianzi.cn

TS:   // 同上
来源：http://sg.colortex.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wq.wgjwhj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ub.lnxyls.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://as.newstarts.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://kx.bookmarksfly.cn

================================================================================
来源：http://dy.haigaiapp.cn

G. 面向对象
来源：http://kq.asd995.cn

================================================================================
来源：http://yc.szxytkj.cn

[G01] 定义类
来源：http://zf.521024.cn


<!-- 参考信息 -->