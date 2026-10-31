代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://iv.9csxet.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zl.nszjky.cn

[D25] Set 集合去重与交并差
来源：http://wq.asd995.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tx.szsharing.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sv.colortex.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xg.bjjhwx.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ao.muxihuayi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qg.wgjwhj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mu.huixinmuqiang.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uq.shxzskj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hv.chemitech.net.cn

[D26] 数组转字符串
来源：http://ca.lnxyls.cn

Py:   ", ".join(map(str, arr))
来源：http://gl.huanxung.cn

PHP:  implode(", ", $arr);
来源：http://er.lnxyls.cn

JS:   arr.join(", ")
来源：http://cy.newstarts.cn

TS:   arr.join(", ")
来源：http://wd.yuntaijiaju.cn

Java: String.join(", ", list)
来源：http://bp.huanxung.cn

Go:   strings.Join(strs, ", ")
来源：http://fq.jianghongdianzi.cn

Ruby: arr.join(", ")
来源：http://ah.9csxet.cn

C#:   string.Join(", ", list)
来源：http://uo.colortex.cn

================================================================================
来源：http://ft.shxzskj.cn

E. 字符串处理
来源：http://im.huanxung.cn

================================================================================
来源：http://fd.wgjwhj.cn

[E01] 拼接字符串
来源：http://lh.521024.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://oi.muxihuayi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rs.huanxung.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gp.shxzukj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ft.jctech888.com.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dl.chemitech.net.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ar.hnjuh.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fw.nicolike.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ni.nicolike.cn

[E02] 重复字符串
来源：http://rh.huanxung.cn

Py:   "ab" * 3
来源：http://tu.wgjwhj.cn

PHP:  str_repeat("ab", 3);
来源：http://nh.colortex.cn

JS:   "ab".repeat(3)
来源：http://xh.gzmigu.cn

TS:   "ab".repeat(3)
来源：http://df.asd995.cn

Java: "ab".repeat(3)
来源：http://ls.asd995.cn

Go:   strings.Repeat("ab", 3)
来源：http://uu.huixiangedu.cn

Ruby: "ab" * 3
来源：http://pd.shxzskj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ps.shxzukj.cn

[E03] 截取子串
来源：http://ue.jianghongdianzi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jc.nicolike.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ef.jctech888.com.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rp.panjiajie.cn

TS:   s.slice(1, 4)
来源：http://ah.wgjwhj.cn

Java: s.substring(1, 4)
来源：http://ff.shxzukj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://oi.lnxyls.cn

Ruby: s[1, 3];  s[1..3]
来源：http://qo.bookmarksfly.cn

C#:   s.Substring(1, 3)
来源：http://ro.shtwfgs.cn

[E04] 查找子串位置
来源：http://fs.yuexingan06.cn

Py:   s.find("x");  s.index("x")
来源：http://nc.szsharing.cn

PHP:  strpos($s, "x");
来源：http://wv.hahajie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ue.szxytkj.cn

TS:   s.indexOf("x")
来源：http://fo.hahajie.cn

Java: s.indexOf("x")
来源：http://by.wgjwhj.cn

Go:   strings.Index(s, "x")
来源：http://aj.wgjwhj.cn

Ruby: s.index("x")
来源：http://vp.nicolike.cn

C#:   s.IndexOf("x")
来源：http://nk.szxytkj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://pb.9csxet.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://oj.wgjwhj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xl.huixinmuqiang.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fr.jianghongdianzi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://of.huixinmuqiang.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qa.yuexingan06.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zy.panjiajie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ww.haigaiapp.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ib.huixinmuqiang.cn

[E06] 替换子串
来源：http://pr.shxzukj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bb.9csxet.cn

PHP:  str_replace("a", "b", $s);
来源：http://pp.shxzskj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qk.huanxung.cn

TS:   s.replaceAll("a", "b")
来源：http://ds.gzmigu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pl.9csxet.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gu.jianghongdianzi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ap.hnjuh.cn

C#:   s.Replace("a", "b")
来源：http://ho.bookmarksfly.cn

[E07] 按分隔符拆分
来源：http://kl.huanxung.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://se.jianghongdianzi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yg.521024.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ln.szsharing.cn

TS:   s.split(",")
来源：http://xm.yuexingan06.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xs.hahajie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ti.haigaiapp.cn

Ruby: s.split(",");  s.split
来源：http://op.gzmigu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wq.chemitech.net.cn

[E08] 数组按分隔符合并
来源：http://rz.newstarts.cn

Py:   ",".join(items)
来源：http://cv.szxytkj.cn

PHP:  implode(",", $items);
来源：http://rz.huixinmuqiang.cn

JS:   items.join(",")
来源：http://wa.huixiangedu.cn

TS:   items.join(",")
来源：http://rw.shtwfgs.cn

Java: String.join(",", items)
来源：http://ii.9csxet.cn

Go:   strings.Join(items, ",")
来源：http://xe.hnjuh.cn

Ruby: items.join(",")
来源：http://qy.szsharing.cn

C#:   string.Join(",", items)
来源：http://ok.shtwfgs.cn

[E09] 去除所有空白字符
来源：http://iz.lnxyls.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hh.lnxyls.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dl.yuexingan06.cn

JS:   s.replace(/\s+/g, "")
来源：http://fq.yuntaijiaju.cn

TS:   s.replace(/\s+/g, "")
来源：http://zm.hahajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://dy.szsharing.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://nm.lnxyls.cn

Ruby: s.gsub(/\s+/, "")
来源：http://wm.yuexingan06.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lx.wgjwhj.cn

[E10] 左侧补零 / 定长填充
来源：http://aa.chemitech.net.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pb.colortex.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vg.yuntaijiaju.cn

JS:   "7".padStart(3, "0")
来源：http://ah.szsharing.cn

TS:   "7".padStart(3, "0")
来源：http://ve.yuexingan06.cn

Java: String.format("%03d", 7)
来源：http://ek.hahajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://te.muxihuayi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://oy.jianghongdianzi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://px.yuntaijiaju.cn

[E11] 反转字符串
来源：http://ne.bookmarksfly.cn

Py:   s[::-1]
来源：http://bq.lnxyls.cn

PHP:  strrev($s);
来源：http://er.colortex.cn

JS:   [...s].reverse().join("")
来源：http://gn.bookmarksfly.cn

TS:   [...s].reverse().join("")
来源：http://zf.lnxyls.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://vs.jctech888.com.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ex.hahajie.cn

Ruby: s.reverse
来源：http://oc.bjjhwx.cn

C#:   new string(s.Reverse().ToArray())
来源：http://kr.wgjwhj.cn

[E12] 统计某字符出现次数
来源：http://cu.panjiajie.cn

Py:   s.count("a")
来源：http://kb.chemitech.net.cn

PHP:  substr_count($s, "a");
来源：http://iw.bjjhwx.cn

JS:   s.split("a").length - 1
来源：http://dd.jianghongdianzi.cn

TS:   s.split("a").length - 1
来源：http://nj.newstarts.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hr.gzmigu.cn

Go:   strings.Count(s, "a")
来源：http://pm.nicolike.cn

Ruby: s.count("a")
来源：http://lt.panjiajie.cn

C#:   s.Count(c => c == 'a')
来源：http://ji.muxihuayi.cn

[E13] 逐字符遍历
来源：http://uo.chemitech.net.cn

Py:   for ch in s: print(ch)
来源：http://ga.muxihuayi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fg.hahajie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://oy.shtwfgs.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://kj.huanxung.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://of.shxzukj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wi.9csxet.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ds.chemitech.net.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vp.521024.cn

[E14] URL 编码与 Base64
来源：http://lj.muxihuayi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jm.wgjwhj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bh.bjjhwx.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gr.hahajie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sk.haigaiapp.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kr.szxytkj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kh.chemitech.net.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fk.newstarts.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ny.wgjwhj.cn

[E15] HTML 转义 / 反转义
来源：http://de.huanxung.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://rk.shxzskj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ip.nszjky.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ek.jctech888.com.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ro.wgjwhj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://se.haigaiapp.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vf.chemitech.net.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ef.shxzskj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qo.haigaiapp.cn

[E16] 数字千分位
来源：http://qe.asd995.cn

Py:   f"{1234567:,}"
来源：http://zy.szsharing.cn

PHP:  number_format(1234567);
来源：http://bp.lnxyls.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://rg.bjjhwx.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://aa.panjiajie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nx.yuexingan06.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lj.newstarts.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gx.9csxet.cn

C#:   1234567.ToString("N0")
来源：http://ql.asd995.cn

[E17] 首字母大写
来源：http://xx.lnxyls.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cu.shtwfgs.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://uv.panjiajie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hh.huixinmuqiang.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://va.huixiangedu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://yd.yuntaijiaju.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://el.wgjwhj.cn

Ruby: s.capitalize
来源：http://nc.huanxung.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://im.muxihuayi.cn

[E18] 模板占位符替换
来源：http://yy.szxytkj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://we.szsharing.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yf.nicolike.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://vl.yuntaijiaju.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://tk.yuexingan06.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rd.nszjky.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fo.szxytkj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fy.521024.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://un.nicolike.cn

[E19] 多行文本按行拆分
来源：http://ie.wgjwhj.cn

Py:   s.splitlines()
来源：http://et.colortex.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cj.hnjuh.cn

JS:   s.split(/\r?\n/)
来源：http://ej.muxihuayi.cn

TS:   s.split(/\r?\n/)
来源：http://ob.szxytkj.cn

Java: s.lines().toList()
来源：http://yn.hahajie.cn

Go:   strings.Split(s, "\n")
来源：http://lj.521024.cn

Ruby: s.lines
来源：http://sx.hahajie.cn

C#:   s.Split('\n')
来源：http://uv.chemitech.net.cn

[E20] 判断字符串是否为空
来源：http://jw.wgjwhj.cn

Py:   if not s:
来源：http://fi.lnxyls.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lw.yuexingan06.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qk.wgjwhj.cn

TS:   if (s === "") {}
来源：http://nq.yuexingan06.cn

Java: if (s.isEmpty()) {}
来源：http://np.colortex.cn

Go:   if s == "" {}
来源：http://kc.jctech888.com.cn

Ruby: if s.empty?
来源：http://jr.huixinmuqiang.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://na.nicolike.cn

[E21] 超长截断加省略号
来源：http://ex.521024.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://oc.yuntaijiaju.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ix.bookmarksfly.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jo.bjjhwx.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mj.jctech888.com.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vk.shxzukj.cn

Go:   // 按 rune 判断长度后截断
来源：http://pe.bjjhwx.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fo.yuexingan06.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://aa.wgjwhj.cn

[E22] 字节长度与字符长度
来源：http://xx.chemitech.net.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kx.newstarts.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kt.jctech888.com.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ny.521024.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zc.szxytkj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vx.shxzukj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dd.panjiajie.cn

Ruby: s.bytesize;  s.length
来源：http://hl.hahajie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ez.gzmigu.cn

================================================================================
来源：http://oj.asd995.cn

F. 文件与目录
来源：http://bk.521024.cn

================================================================================
来源：http://ow.panjiajie.cn

[F01] 读取整个文件
来源：http://pe.gzmigu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://sm.hnjuh.cn

PHP:  file_get_contents("a.txt");
来源：http://ar.jianghongdianzi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xv.wgjwhj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://db.hahajie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://co.asd995.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kc.yuntaijiaju.cn

Ruby: File.read("a.txt")
来源：http://ca.yuexingan06.cn

C#:   File.ReadAllText("a.txt");
来源：http://fq.huixiangedu.cn

[F02] 逐行读取文件
来源：http://ca.huanxung.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ha.colortex.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pe.colortex.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://iz.newstarts.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fr.szsharing.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://md.shtwfgs.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lq.colortex.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://um.hnjuh.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jr.hnjuh.cn

[F03] 写入文件（覆盖）
来源：http://oc.szsharing.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zr.wgjwhj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://oo.szsharing.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uz.hnjuh.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vd.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zo.nszjky.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wp.shxzskj.cn

Ruby: File.write("a.txt", "hi")
来源：http://yk.colortex.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://oq.shxzukj.cn

[F04] 追加写入文件
来源：http://jm.muxihuayi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xd.colortex.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kn.jctech888.com.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://op.asd995.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ej.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yb.hahajie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lo.hahajie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://uz.nicolike.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://is.bookmarksfly.cn

[F05] 判断文件或目录是否存在
来源：http://xl.huixiangedu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vx.szxytkj.cn

PHP:  file_exists("a.txt");
来源：http://bs.yuexingan06.cn

JS:   fs.existsSync("a.txt")
来源：http://wb.jianghongdianzi.cn

TS:   fs.existsSync("a.txt")
来源：http://jx.szxytkj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://er.nszjky.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://uw.yuntaijiaju.cn

Ruby: File.exist?("a.txt")
来源：http://xs.chemitech.net.cn

C#:   File.Exists("a.txt")
来源：http://om.lnxyls.cn

[F06] 删除文件
来源：http://lv.9csxet.cn

Py:   os.remove("a.txt")
来源：http://ep.shxzukj.cn

PHP:  unlink("a.txt");
来源：http://lf.yuexingan06.cn

JS:   fs.unlinkSync("a.txt")
来源：http://bd.jctech888.com.cn

TS:   fs.unlinkSync("a.txt")
来源：http://xv.shxzukj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zn.haigaiapp.cn

Go:   os.Remove("a.txt")
来源：http://dk.nszjky.cn

Ruby: File.delete("a.txt")
来源：http://sz.haigaiapp.cn

C#:   File.Delete("a.txt");
来源：http://ib.chemitech.net.cn

[F07] 创建目录（含多级）
来源：http://mf.lnxyls.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ty.chemitech.net.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qw.wgjwhj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gh.panjiajie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yi.nszjky.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fg.szxytkj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://eg.jianghongdianzi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://eg.shxzukj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mp.shtwfgs.cn

[F08] 遍历目录
来源：http://tq.bookmarksfly.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://kc.asd995.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lp.colortex.cn

JS:   fs.readdirSync("dir")
来源：http://ae.szsharing.cn

TS:   fs.readdirSync("dir")
来源：http://ho.newstarts.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ww.panjiajie.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://pq.hnjuh.cn

Ruby: Dir.children("dir")
来源：http://uk.nicolike.cn

C#:   Directory.GetFiles("dir")
来源：http://zz.bjjhwx.cn

[F09] 获取文件大小
来源：http://vo.shtwfgs.cn

Py:   os.path.getsize("a.txt")
来源：http://gy.yuexingan06.cn

PHP:  filesize("a.txt");
来源：http://et.shtwfgs.cn

JS:   fs.statSync("a.txt").size
来源：http://wg.shxzskj.cn


<!-- 参考信息 -->