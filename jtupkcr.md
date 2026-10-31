代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://np.szxytkj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://im.asd995.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://db.nszjky.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://em.szxytkj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fu.szsharing.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tp.huanxung.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bi.haigaiapp.cn

[D26] 数组转字符串
来源：http://cf.colortex.cn

Py:   ", ".join(map(str, arr))
来源：http://wd.gzmigu.cn

PHP:  implode(", ", $arr);
来源：http://pv.wgjwhj.cn

JS:   arr.join(", ")
来源：http://wz.shxzskj.cn

TS:   arr.join(", ")
来源：http://dv.yuntaijiaju.cn

Java: String.join(", ", list)
来源：http://hh.huanxung.cn

Go:   strings.Join(strs, ", ")
来源：http://de.wgjwhj.cn

Ruby: arr.join(", ")
来源：http://ke.wgjwhj.cn

C#:   string.Join(", ", list)
来源：http://az.bookmarksfly.cn

================================================================================
来源：http://nt.szsharing.cn

E. 字符串处理
来源：http://aq.521024.cn

================================================================================
来源：http://jk.newstarts.cn

[E01] 拼接字符串
来源：http://tz.huixiangedu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ju.jianghongdianzi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jn.huixiangedu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pa.gzmigu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ky.hnjuh.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mo.bookmarksfly.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qd.newstarts.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xh.muxihuayi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zm.bookmarksfly.cn

[E02] 重复字符串
来源：http://wi.colortex.cn

Py:   "ab" * 3
来源：http://we.szxytkj.cn

PHP:  str_repeat("ab", 3);
来源：http://ft.nszjky.cn

JS:   "ab".repeat(3)
来源：http://kk.shxzukj.cn

TS:   "ab".repeat(3)
来源：http://ui.gzmigu.cn

Java: "ab".repeat(3)
来源：http://ia.hahajie.cn

Go:   strings.Repeat("ab", 3)
来源：http://pq.huixinmuqiang.cn

Ruby: "ab" * 3
来源：http://xc.szxytkj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pv.asd995.cn

[E03] 截取子串
来源：http://ok.yuexingan06.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cc.shtwfgs.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jb.newstarts.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ow.muxihuayi.cn

TS:   s.slice(1, 4)
来源：http://gp.huixinmuqiang.cn

Java: s.substring(1, 4)
来源：http://qh.panjiajie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://df.shtwfgs.cn

Ruby: s[1, 3];  s[1..3]
来源：http://vi.szsharing.cn

C#:   s.Substring(1, 3)
来源：http://vg.yuexingan06.cn

[E04] 查找子串位置
来源：http://wf.szsharing.cn

Py:   s.find("x");  s.index("x")
来源：http://lg.huanxung.cn

PHP:  strpos($s, "x");
来源：http://qv.jianghongdianzi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rp.shtwfgs.cn

TS:   s.indexOf("x")
来源：http://ch.shxzukj.cn

Java: s.indexOf("x")
来源：http://we.shxzskj.cn

Go:   strings.Index(s, "x")
来源：http://kt.nicolike.cn

Ruby: s.index("x")
来源：http://my.jctech888.com.cn

C#:   s.IndexOf("x")
来源：http://dy.muxihuayi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ov.hnjuh.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ak.nszjky.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ut.huixiangedu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cb.szsharing.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://kv.newstarts.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fp.shtwfgs.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wy.chemitech.net.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tu.panjiajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lj.bookmarksfly.cn

[E06] 替换子串
来源：http://gb.lnxyls.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rp.jctech888.com.cn

PHP:  str_replace("a", "b", $s);
来源：http://uz.wgjwhj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mw.yuntaijiaju.cn

TS:   s.replaceAll("a", "b")
来源：http://ky.haigaiapp.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sl.nicolike.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rc.hahajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fb.hnjuh.cn

C#:   s.Replace("a", "b")
来源：http://jp.yuntaijiaju.cn

[E07] 按分隔符拆分
来源：http://kv.colortex.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dt.haigaiapp.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qd.szsharing.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://du.szsharing.cn

TS:   s.split(",")
来源：http://zx.9csxet.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ij.newstarts.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xk.yuexingan06.cn

Ruby: s.split(",");  s.split
来源：http://bf.yuntaijiaju.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lx.jctech888.com.cn

[E08] 数组按分隔符合并
来源：http://yk.huanxung.cn

Py:   ",".join(items)
来源：http://pd.newstarts.cn

PHP:  implode(",", $items);
来源：http://cd.colortex.cn

JS:   items.join(",")
来源：http://lq.jianghongdianzi.cn

TS:   items.join(",")
来源：http://zp.nszjky.cn

Java: String.join(",", items)
来源：http://hy.newstarts.cn

Go:   strings.Join(items, ",")
来源：http://yk.nszjky.cn

Ruby: items.join(",")
来源：http://qj.szsharing.cn

C#:   string.Join(",", items)
来源：http://vq.newstarts.cn

[E09] 去除所有空白字符
来源：http://rd.huixiangedu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://na.bjjhwx.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zi.newstarts.cn

JS:   s.replace(/\s+/g, "")
来源：http://ly.nszjky.cn

TS:   s.replace(/\s+/g, "")
来源：http://fk.jctech888.com.cn

Java: s.replaceAll("\\s+", "")
来源：http://zf.bookmarksfly.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ed.jianghongdianzi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://er.szxytkj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xc.panjiajie.cn

[E10] 左侧补零 / 定长填充
来源：http://wh.shtwfgs.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ci.bjjhwx.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qz.nicolike.cn

JS:   "7".padStart(3, "0")
来源：http://aa.nicolike.cn

TS:   "7".padStart(3, "0")
来源：http://qg.bookmarksfly.cn

Java: String.format("%03d", 7)
来源：http://eb.nicolike.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://sh.panjiajie.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pl.shtwfgs.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://si.huanxung.cn

[E11] 反转字符串
来源：http://yw.panjiajie.cn

Py:   s[::-1]
来源：http://ar.huixinmuqiang.cn

PHP:  strrev($s);
来源：http://wy.bjjhwx.cn

JS:   [...s].reverse().join("")
来源：http://fk.hahajie.cn

TS:   [...s].reverse().join("")
来源：http://ut.bjjhwx.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://gq.huanxung.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://at.gzmigu.cn

Ruby: s.reverse
来源：http://bn.newstarts.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ot.huanxung.cn

[E12] 统计某字符出现次数
来源：http://fw.nicolike.cn

Py:   s.count("a")
来源：http://fp.jianghongdianzi.cn

PHP:  substr_count($s, "a");
来源：http://wb.asd995.cn

JS:   s.split("a").length - 1
来源：http://xd.muxihuayi.cn

TS:   s.split("a").length - 1
来源：http://rb.jctech888.com.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ae.bjjhwx.cn

Go:   strings.Count(s, "a")
来源：http://je.nszjky.cn

Ruby: s.count("a")
来源：http://zv.nicolike.cn

C#:   s.Count(c => c == 'a')
来源：http://vg.yuntaijiaju.cn

[E13] 逐字符遍历
来源：http://bd.jianghongdianzi.cn

Py:   for ch in s: print(ch)
来源：http://gu.huixinmuqiang.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gm.nszjky.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://sq.panjiajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://nx.muxihuayi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jf.bjjhwx.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fi.shxzukj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ip.colortex.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ox.gzmigu.cn

[E14] URL 编码与 Base64
来源：http://se.szsharing.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zh.shtwfgs.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://kz.jctech888.com.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://em.huanxung.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bl.haigaiapp.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uh.jianghongdianzi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fl.chemitech.net.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ke.lnxyls.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jx.shtwfgs.cn

[E15] HTML 转义 / 反转义
来源：http://af.jianghongdianzi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://zo.szsharing.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pd.huanxung.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mu.hahajie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://hd.szsharing.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://oi.bookmarksfly.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sp.asd995.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cu.huixiangedu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fi.jianghongdianzi.cn

[E16] 数字千分位
来源：http://rd.nicolike.cn

Py:   f"{1234567:,}"
来源：http://ud.yuexingan06.cn

PHP:  number_format(1234567);
来源：http://td.jctech888.com.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mn.nicolike.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://mp.colortex.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zy.wgjwhj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dj.chemitech.net.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xu.szsharing.cn

C#:   1234567.ToString("N0")
来源：http://gb.hahajie.cn

[E17] 首字母大写
来源：http://qr.shxzukj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://no.bookmarksfly.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://nd.nszjky.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xp.shxzskj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ib.hnjuh.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ld.yuntaijiaju.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hx.huixinmuqiang.cn

Ruby: s.capitalize
来源：http://al.wgjwhj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mb.bjjhwx.cn

[E18] 模板占位符替换
来源：http://ce.muxihuayi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xu.bjjhwx.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ia.panjiajie.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://un.shtwfgs.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://od.jianghongdianzi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ea.bookmarksfly.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gu.hahajie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qd.nicolike.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://km.jianghongdianzi.cn

[E19] 多行文本按行拆分
来源：http://cd.hahajie.cn

Py:   s.splitlines()
来源：http://hj.9csxet.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tb.huixinmuqiang.cn

JS:   s.split(/\r?\n/)
来源：http://xp.lnxyls.cn

TS:   s.split(/\r?\n/)
来源：http://nt.lnxyls.cn

Java: s.lines().toList()
来源：http://tc.huixinmuqiang.cn

Go:   strings.Split(s, "\n")
来源：http://cl.huixiangedu.cn

Ruby: s.lines
来源：http://jj.jctech888.com.cn

C#:   s.Split('\n')
来源：http://ko.hahajie.cn

[E20] 判断字符串是否为空
来源：http://wt.jctech888.com.cn

Py:   if not s:
来源：http://qa.bjjhwx.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yy.bookmarksfly.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pb.lnxyls.cn

TS:   if (s === "") {}
来源：http://or.chemitech.net.cn

Java: if (s.isEmpty()) {}
来源：http://rx.szsharing.cn

Go:   if s == "" {}
来源：http://ze.nszjky.cn

Ruby: if s.empty?
来源：http://cm.szxytkj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gc.jianghongdianzi.cn

[E21] 超长截断加省略号
来源：http://mb.bjjhwx.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://md.shtwfgs.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jk.newstarts.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dy.huixinmuqiang.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xz.huixinmuqiang.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cm.muxihuayi.cn

Go:   // 按 rune 判断长度后截断
来源：http://gm.huixinmuqiang.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wq.jctech888.com.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wv.asd995.cn

[E22] 字节长度与字符长度
来源：http://kg.shxzskj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hi.9csxet.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://du.haigaiapp.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tn.jianghongdianzi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lu.521024.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vs.gzmigu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fq.szsharing.cn

Ruby: s.bytesize;  s.length
来源：http://ct.shxzskj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sq.shxzukj.cn

================================================================================
来源：http://db.nszjky.cn

F. 文件与目录
来源：http://ls.chemitech.net.cn

================================================================================
来源：http://fz.muxihuayi.cn

[F01] 读取整个文件
来源：http://mw.haigaiapp.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://at.nszjky.cn

PHP:  file_get_contents("a.txt");
来源：http://in.huanxung.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cj.huanxung.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://er.huixinmuqiang.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://lm.hahajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rs.szxytkj.cn

Ruby: File.read("a.txt")
来源：http://ll.jianghongdianzi.cn

C#:   File.ReadAllText("a.txt");
来源：http://ac.colortex.cn

[F02] 逐行读取文件
来源：http://gd.nicolike.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ak.jianghongdianzi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ab.asd995.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ot.lnxyls.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sm.yuntaijiaju.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://if.nicolike.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vg.chemitech.net.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cd.huixinmuqiang.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bv.jctech888.com.cn

[F03] 写入文件（覆盖）
来源：http://cl.newstarts.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nr.nicolike.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://bs.yuntaijiaju.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tn.jianghongdianzi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ws.9csxet.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://uw.521024.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vb.chemitech.net.cn

Ruby: File.write("a.txt", "hi")
来源：http://sa.shtwfgs.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fe.bookmarksfly.cn

[F04] 追加写入文件
来源：http://xp.huanxung.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gb.colortex.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mc.wgjwhj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zr.chemitech.net.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fs.nszjky.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tk.yuexingan06.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://my.chemitech.net.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ab.521024.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zz.panjiajie.cn

[F05] 判断文件或目录是否存在
来源：http://zt.szxytkj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tg.panjiajie.cn

PHP:  file_exists("a.txt");
来源：http://ng.colortex.cn

JS:   fs.existsSync("a.txt")
来源：http://gd.hnjuh.cn

TS:   fs.existsSync("a.txt")
来源：http://fl.yuexingan06.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ah.bookmarksfly.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://av.jianghongdianzi.cn

Ruby: File.exist?("a.txt")
来源：http://wp.shxzskj.cn

C#:   File.Exists("a.txt")
来源：http://ll.shxzukj.cn

[F06] 删除文件
来源：http://pv.9csxet.cn

Py:   os.remove("a.txt")
来源：http://sc.huixinmuqiang.cn

PHP:  unlink("a.txt");
来源：http://ap.yuexingan06.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ft.nicolike.cn

TS:   fs.unlinkSync("a.txt")
来源：http://xm.nicolike.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://em.yuexingan06.cn

Go:   os.Remove("a.txt")
来源：http://td.szsharing.cn

Ruby: File.delete("a.txt")
来源：http://nb.9csxet.cn

C#:   File.Delete("a.txt");
来源：http://pe.colortex.cn

[F07] 创建目录（含多级）
来源：http://ol.szxytkj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cn.bookmarksfly.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://au.szsharing.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pm.shtwfgs.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mo.szsharing.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bn.9csxet.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ny.muxihuayi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dy.colortex.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ya.wgjwhj.cn

[F08] 遍历目录
来源：http://qx.haigaiapp.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ur.newstarts.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gc.huixinmuqiang.cn

JS:   fs.readdirSync("dir")
来源：http://mz.colortex.cn

TS:   fs.readdirSync("dir")
来源：http://sv.jianghongdianzi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wf.nicolike.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://qa.hnjuh.cn

Ruby: Dir.children("dir")
来源：http://yl.nszjky.cn

C#:   Directory.GetFiles("dir")
来源：http://as.lnxyls.cn

[F09] 获取文件大小
来源：http://xu.huixinmuqiang.cn

Py:   os.path.getsize("a.txt")
来源：http://qm.colortex.cn

PHP:  filesize("a.txt");
来源：http://ol.bookmarksfly.cn

JS:   fs.statSync("a.txt").size
来源：http://dl.asd995.cn

TS:   fs.statSync("a.txt").size
来源：http://nh.nicolike.cn

Java: Files.size(Path.of("a.txt"))
来源：http://op.shxzukj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://sb.nszjky.cn

Ruby: File.size("a.txt")
来源：http://wc.shxzukj.cn


<!-- 参考信息 -->