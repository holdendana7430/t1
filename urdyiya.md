代发 wailian999

TS:   "ab".repeat(3)
来源：http://nv.panjiajie.cn

Java: "ab".repeat(3)
来源：http://rn.lnxyls.cn

Go:   strings.Repeat("ab", 3)
来源：http://bo.521024.cn

Ruby: "ab" * 3
来源：http://qk.panjiajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ss.panjiajie.cn

[E03] 截取子串
来源：http://fa.huixinmuqiang.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pw.jianghongdianzi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://uc.panjiajie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yg.panjiajie.cn

TS:   s.slice(1, 4)
来源：http://qe.9csxet.cn

Java: s.substring(1, 4)
来源：http://cd.yuntaijiaju.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://aw.wgjwhj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://pn.huanxung.cn

C#:   s.Substring(1, 3)
来源：http://my.shxzukj.cn

[E04] 查找子串位置
来源：http://qk.jianghongdianzi.cn

Py:   s.find("x");  s.index("x")
来源：http://pk.hahajie.cn

PHP:  strpos($s, "x");
来源：http://mr.wgjwhj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wb.newstarts.cn

TS:   s.indexOf("x")
来源：http://no.asd995.cn

Java: s.indexOf("x")
来源：http://fa.huanxung.cn

Go:   strings.Index(s, "x")
来源：http://yb.asd995.cn

Ruby: s.index("x")
来源：http://ha.szsharing.cn

C#:   s.IndexOf("x")
来源：http://nx.szsharing.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://hc.szsharing.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tv.shxzskj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xh.hnjuh.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sc.muxihuayi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://wd.szsharing.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lq.shtwfgs.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://iv.shtwfgs.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mp.muxihuayi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ic.bookmarksfly.cn

[E06] 替换子串
来源：http://zy.hahajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ip.yuexingan06.cn

PHP:  str_replace("a", "b", $s);
来源：http://uv.521024.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jb.haigaiapp.cn

TS:   s.replaceAll("a", "b")
来源：http://fj.muxihuayi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://um.bjjhwx.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yc.lnxyls.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://eb.haigaiapp.cn

C#:   s.Replace("a", "b")
来源：http://ie.colortex.cn

[E07] 按分隔符拆分
来源：http://la.jianghongdianzi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://us.nszjky.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kw.gzmigu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://zb.shxzukj.cn

TS:   s.split(",")
来源：http://rf.asd995.cn

Java: s.split(",");  s.split("\\s+")
来源：http://hp.huixiangedu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qb.shxzukj.cn

Ruby: s.split(",");  s.split
来源：http://pu.huanxung.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ww.9csxet.cn

[E08] 数组按分隔符合并
来源：http://li.bookmarksfly.cn

Py:   ",".join(items)
来源：http://es.nszjky.cn

PHP:  implode(",", $items);
来源：http://nz.haigaiapp.cn

JS:   items.join(",")
来源：http://xs.yuexingan06.cn

TS:   items.join(",")
来源：http://qo.huanxung.cn

Java: String.join(",", items)
来源：http://ml.shtwfgs.cn

Go:   strings.Join(items, ",")
来源：http://sz.szsharing.cn

Ruby: items.join(",")
来源：http://nj.9csxet.cn

C#:   string.Join(",", items)
来源：http://bo.shtwfgs.cn

[E09] 去除所有空白字符
来源：http://dm.szxytkj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zh.haigaiapp.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ux.haigaiapp.cn

JS:   s.replace(/\s+/g, "")
来源：http://nl.szxytkj.cn

TS:   s.replace(/\s+/g, "")
来源：http://se.newstarts.cn

Java: s.replaceAll("\\s+", "")
来源：http://oc.hahajie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://fu.shxzukj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://yk.szsharing.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rj.newstarts.cn

[E10] 左侧补零 / 定长填充
来源：http://gm.newstarts.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gs.521024.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fu.haigaiapp.cn

JS:   "7".padStart(3, "0")
来源：http://wm.szxytkj.cn

TS:   "7".padStart(3, "0")
来源：http://ro.bjjhwx.cn

Java: String.format("%03d", 7)
来源：http://nr.asd995.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ez.wgjwhj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://eb.muxihuayi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dh.yuexingan06.cn

[E11] 反转字符串
来源：http://rb.nszjky.cn

Py:   s[::-1]
来源：http://ut.huixiangedu.cn

PHP:  strrev($s);
来源：http://ye.hahajie.cn

JS:   [...s].reverse().join("")
来源：http://qr.9csxet.cn

TS:   [...s].reverse().join("")
来源：http://fv.jianghongdianzi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://sm.muxihuayi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zd.huixinmuqiang.cn

Ruby: s.reverse
来源：http://qd.hahajie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://mq.jctech888.com.cn

[E12] 统计某字符出现次数
来源：http://vg.bjjhwx.cn

Py:   s.count("a")
来源：http://ua.hahajie.cn

PHP:  substr_count($s, "a");
来源：http://lz.shxzskj.cn

JS:   s.split("a").length - 1
来源：http://kl.chemitech.net.cn

TS:   s.split("a").length - 1
来源：http://zr.wgjwhj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gs.gzmigu.cn

Go:   strings.Count(s, "a")
来源：http://jj.huanxung.cn

Ruby: s.count("a")
来源：http://ry.chemitech.net.cn

C#:   s.Count(c => c == 'a')
来源：http://xy.panjiajie.cn

[E13] 逐字符遍历
来源：http://il.hahajie.cn

Py:   for ch in s: print(ch)
来源：http://tp.nicolike.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fk.huanxung.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://hi.hnjuh.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://eb.521024.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://me.szxytkj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ax.bookmarksfly.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://sg.nszjky.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qg.szxytkj.cn

[E14] URL 编码与 Base64
来源：http://li.yuntaijiaju.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sd.bjjhwx.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://wa.shxzskj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wl.szxytkj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qv.asd995.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://es.huixiangedu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pd.lnxyls.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://sj.yuexingan06.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sw.huixiangedu.cn

[E15] HTML 转义 / 反转义
来源：http://jv.yuntaijiaju.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://gc.haigaiapp.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ee.nszjky.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vk.panjiajie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wf.colortex.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ti.haigaiapp.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pu.lnxyls.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fe.hnjuh.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yl.shtwfgs.cn

[E16] 数字千分位
来源：http://pw.muxihuayi.cn

Py:   f"{1234567:,}"
来源：http://qz.shxzukj.cn

PHP:  number_format(1234567);
来源：http://nz.huixiangedu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://dk.shxzukj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://gd.lnxyls.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xi.521024.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nq.shtwfgs.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://sz.lnxyls.cn

C#:   1234567.ToString("N0")
来源：http://fg.nszjky.cn

[E17] 首字母大写
来源：http://kt.hahajie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xg.bjjhwx.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://tq.yuexingan06.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ym.huixinmuqiang.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ww.9csxet.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://km.nicolike.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://je.bjjhwx.cn

Ruby: s.capitalize
来源：http://fq.muxihuayi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ds.bjjhwx.cn

[E18] 模板占位符替换
来源：http://yi.lnxyls.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nh.wgjwhj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lz.yuntaijiaju.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ed.szxytkj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://or.yuntaijiaju.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ah.gzmigu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cu.colortex.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ht.haigaiapp.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tv.bjjhwx.cn

[E19] 多行文本按行拆分
来源：http://rp.bjjhwx.cn

Py:   s.splitlines()
来源：http://st.panjiajie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://oc.huixinmuqiang.cn

JS:   s.split(/\r?\n/)
来源：http://lt.nicolike.cn

TS:   s.split(/\r?\n/)
来源：http://oi.huanxung.cn

Java: s.lines().toList()
来源：http://le.9csxet.cn

Go:   strings.Split(s, "\n")
来源：http://kg.521024.cn

Ruby: s.lines
来源：http://ie.hahajie.cn

C#:   s.Split('\n')
来源：http://xo.chemitech.net.cn

[E20] 判断字符串是否为空
来源：http://fr.huanxung.cn

Py:   if not s:
来源：http://xd.muxihuayi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ns.521024.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mr.muxihuayi.cn

TS:   if (s === "") {}
来源：http://hc.shxzukj.cn

Java: if (s.isEmpty()) {}
来源：http://yg.bookmarksfly.cn

Go:   if s == "" {}
来源：http://bs.wgjwhj.cn

Ruby: if s.empty?
来源：http://po.asd995.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dk.shxzukj.cn

[E21] 超长截断加省略号
来源：http://gk.shxzukj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jq.huixiangedu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ei.muxihuayi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://in.szsharing.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yw.jianghongdianzi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cl.shxzskj.cn

Go:   // 按 rune 判断长度后截断
来源：http://xx.shxzskj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://be.bookmarksfly.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://og.hnjuh.cn

[E22] 字节长度与字符长度
来源：http://cq.bjjhwx.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sl.yuexingan06.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ob.newstarts.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ru.9csxet.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pj.lnxyls.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://he.shxzskj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ce.nicolike.cn

Ruby: s.bytesize;  s.length
来源：http://kg.jianghongdianzi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dk.yuntaijiaju.cn

================================================================================
来源：http://bm.bookmarksfly.cn

F. 文件与目录
来源：http://yq.shxzukj.cn

================================================================================
来源：http://fr.muxihuayi.cn

[F01] 读取整个文件
来源：http://qj.bookmarksfly.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nl.yuexingan06.cn

PHP:  file_get_contents("a.txt");
来源：http://aw.521024.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bi.9csxet.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yo.huanxung.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://mg.9csxet.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.huixiangedu.cn

Ruby: File.read("a.txt")
来源：http://li.521024.cn

C#:   File.ReadAllText("a.txt");
来源：http://xt.szsharing.cn

[F02] 逐行读取文件
来源：http://jt.521024.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bs.lnxyls.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jd.shxzskj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tb.hahajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ps.gzmigu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pz.shxzskj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jk.muxihuayi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ua.bjjhwx.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lg.newstarts.cn

[F03] 写入文件（覆盖）
来源：http://xh.nicolike.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ed.yuexingan06.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ls.muxihuayi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ao.bookmarksfly.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pm.huanxung.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cq.panjiajie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pa.wgjwhj.cn

Ruby: File.write("a.txt", "hi")
来源：http://fz.521024.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ng.nszjky.cn

[F04] 追加写入文件
来源：http://od.shxzskj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ar.lnxyls.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://oo.jctech888.com.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://na.asd995.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mc.jianghongdianzi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ms.szxytkj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qu.hnjuh.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jg.nicolike.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wu.szxytkj.cn

[F05] 判断文件或目录是否存在
来源：http://gs.wgjwhj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mk.nicolike.cn

PHP:  file_exists("a.txt");
来源：http://ax.huixiangedu.cn

JS:   fs.existsSync("a.txt")
来源：http://mk.bjjhwx.cn

TS:   fs.existsSync("a.txt")
来源：http://mh.panjiajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://in.521024.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ga.jctech888.com.cn

Ruby: File.exist?("a.txt")
来源：http://zu.hnjuh.cn

C#:   File.Exists("a.txt")
来源：http://fp.szsharing.cn

[F06] 删除文件
来源：http://sb.bookmarksfly.cn

Py:   os.remove("a.txt")
来源：http://wv.newstarts.cn

PHP:  unlink("a.txt");
来源：http://jy.shxzskj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vk.huixinmuqiang.cn

TS:   fs.unlinkSync("a.txt")
来源：http://qc.jianghongdianzi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://aa.szsharing.cn

Go:   os.Remove("a.txt")
来源：http://cq.szsharing.cn

Ruby: File.delete("a.txt")
来源：http://oc.nicolike.cn

C#:   File.Delete("a.txt");
来源：http://ps.nszjky.cn

[F07] 创建目录（含多级）
来源：http://ng.panjiajie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nb.jianghongdianzi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fw.newstarts.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bt.lnxyls.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zk.muxihuayi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bh.panjiajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://io.shxzskj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xz.chemitech.net.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zm.huixinmuqiang.cn

[F08] 遍历目录
来源：http://pa.haigaiapp.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zu.newstarts.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kl.bjjhwx.cn

JS:   fs.readdirSync("dir")
来源：http://co.colortex.cn

TS:   fs.readdirSync("dir")
来源：http://mz.nicolike.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gk.shxzukj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://eo.jctech888.com.cn

Ruby: Dir.children("dir")
来源：http://vy.newstarts.cn

C#:   Directory.GetFiles("dir")
来源：http://bu.yuntaijiaju.cn

[F09] 获取文件大小
来源：http://jw.huanxung.cn

Py:   os.path.getsize("a.txt")
来源：http://em.panjiajie.cn

PHP:  filesize("a.txt");
来源：http://px.chemitech.net.cn

JS:   fs.statSync("a.txt").size
来源：http://dc.szxytkj.cn

TS:   fs.statSync("a.txt").size
来源：http://hc.newstarts.cn

Java: Files.size(Path.of("a.txt"))
来源：http://dj.9csxet.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fj.huixinmuqiang.cn

Ruby: File.size("a.txt")
来源：http://qg.wgjwhj.cn

C#:   new FileInfo("a.txt").Length
来源：http://zg.jctech888.com.cn

[F10] 取文件扩展名 / 文件名
来源：http://lr.huixinmuqiang.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://sc.bookmarksfly.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vl.haigaiapp.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yg.9csxet.cn

TS:   path.extname("a.txt")
来源：http://xu.shxzukj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jo.newstarts.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pt.haigaiapp.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://py.bjjhwx.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zo.panjiajie.cn

[F11] 复制与移动文件
来源：http://ip.jctech888.com.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://sa.muxihuayi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mp.521024.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gs.nszjky.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lf.huanxung.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://px.shxzskj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wd.shtwfgs.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zl.szxytkj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rh.chemitech.net.cn

[F12] CSV 读写
来源：http://dv.gzmigu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ax.jctech888.com.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dd.haigaiapp.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xn.newstarts.cn

TS:   // 同上
来源：http://eg.wgjwhj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qu.muxihuayi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kb.wgjwhj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vv.bjjhwx.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://um.nicolike.cn

================================================================================
来源：http://qg.szxytkj.cn

G. 面向对象
来源：http://ew.521024.cn

================================================================================
来源：http://sy.wgjwhj.cn

[G01] 定义类
来源：http://wj.huixinmuqiang.cn


<!-- 参考信息 -->