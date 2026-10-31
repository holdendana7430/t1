代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ka.jianghongdianzi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://uq.haigaiapp.cn

[D25] Set 集合去重与交并差
来源：http://lj.wgjwhj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ki.bjjhwx.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fn.panjiajie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wp.panjiajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://sq.bookmarksfly.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://eq.huanxung.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pv.jctech888.com.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xz.hahajie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://da.muxihuayi.cn

[D26] 数组转字符串
来源：http://pw.gzmigu.cn

Py:   ", ".join(map(str, arr))
来源：http://rc.muxihuayi.cn

PHP:  implode(", ", $arr);
来源：http://cj.szsharing.cn

JS:   arr.join(", ")
来源：http://ud.hahajie.cn

TS:   arr.join(", ")
来源：http://ue.yuexingan06.cn

Java: String.join(", ", list)
来源：http://da.wgjwhj.cn

Go:   strings.Join(strs, ", ")
来源：http://ve.huanxung.cn

Ruby: arr.join(", ")
来源：http://yo.shxzskj.cn

C#:   string.Join(", ", list)
来源：http://tp.huanxung.cn

================================================================================
来源：http://zl.nszjky.cn

E. 字符串处理
来源：http://uh.huanxung.cn

================================================================================
来源：http://xq.yuntaijiaju.cn

[E01] 拼接字符串
来源：http://ru.newstarts.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xj.chemitech.net.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kx.huixiangedu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pt.bookmarksfly.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mu.nszjky.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://en.jianghongdianzi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dv.chemitech.net.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mz.szsharing.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ep.lnxyls.cn

[E02] 重复字符串
来源：http://sj.lnxyls.cn

Py:   "ab" * 3
来源：http://gr.lnxyls.cn

PHP:  str_repeat("ab", 3);
来源：http://iy.shxzukj.cn

JS:   "ab".repeat(3)
来源：http://bq.muxihuayi.cn

TS:   "ab".repeat(3)
来源：http://hd.hahajie.cn

Java: "ab".repeat(3)
来源：http://gd.521024.cn

Go:   strings.Repeat("ab", 3)
来源：http://ol.yuexingan06.cn

Ruby: "ab" * 3
来源：http://di.colortex.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qz.bookmarksfly.cn

[E03] 截取子串
来源：http://bv.521024.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rv.yuexingan06.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xh.shxzskj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jk.jctech888.com.cn

TS:   s.slice(1, 4)
来源：http://or.yuntaijiaju.cn

Java: s.substring(1, 4)
来源：http://ot.yuntaijiaju.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mn.jianghongdianzi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ls.newstarts.cn

C#:   s.Substring(1, 3)
来源：http://il.szsharing.cn

[E04] 查找子串位置
来源：http://ba.yuntaijiaju.cn

Py:   s.find("x");  s.index("x")
来源：http://bb.huixiangedu.cn

PHP:  strpos($s, "x");
来源：http://qt.nicolike.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lr.shtwfgs.cn

TS:   s.indexOf("x")
来源：http://rz.panjiajie.cn

Java: s.indexOf("x")
来源：http://dw.jianghongdianzi.cn

Go:   strings.Index(s, "x")
来源：http://jv.jianghongdianzi.cn

Ruby: s.index("x")
来源：http://ex.lnxyls.cn

C#:   s.IndexOf("x")
来源：http://rj.bookmarksfly.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ew.hahajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ka.jctech888.com.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dz.shxzskj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kl.szxytkj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ap.nszjky.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sh.huixiangedu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uu.huixinmuqiang.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pa.muxihuayi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pv.yuntaijiaju.cn

[E06] 替换子串
来源：http://yw.shtwfgs.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qt.szsharing.cn

PHP:  str_replace("a", "b", $s);
来源：http://ab.shxzukj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nm.muxihuayi.cn

TS:   s.replaceAll("a", "b")
来源：http://cz.9csxet.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pa.shxzskj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jz.hahajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://sp.muxihuayi.cn

C#:   s.Replace("a", "b")
来源：http://yr.jianghongdianzi.cn

[E07] 按分隔符拆分
来源：http://lf.bjjhwx.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://se.shtwfgs.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tq.jianghongdianzi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://zr.lnxyls.cn

TS:   s.split(",")
来源：http://xm.nszjky.cn

Java: s.split(",");  s.split("\\s+")
来源：http://du.colortex.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fq.nicolike.cn

Ruby: s.split(",");  s.split
来源：http://bn.bookmarksfly.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cs.panjiajie.cn

[E08] 数组按分隔符合并
来源：http://pr.shtwfgs.cn

Py:   ",".join(items)
来源：http://cn.colortex.cn

PHP:  implode(",", $items);
来源：http://mx.9csxet.cn

JS:   items.join(",")
来源：http://wq.haigaiapp.cn

TS:   items.join(",")
来源：http://cb.jctech888.com.cn

Java: String.join(",", items)
来源：http://va.shxzskj.cn

Go:   strings.Join(items, ",")
来源：http://iw.shxzukj.cn

Ruby: items.join(",")
来源：http://qs.newstarts.cn

C#:   string.Join(",", items)
来源：http://gb.jctech888.com.cn

[E09] 去除所有空白字符
来源：http://un.hnjuh.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://sp.huanxung.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zp.wgjwhj.cn

JS:   s.replace(/\s+/g, "")
来源：http://zn.jianghongdianzi.cn

TS:   s.replace(/\s+/g, "")
来源：http://uo.nicolike.cn

Java: s.replaceAll("\\s+", "")
来源：http://fr.huanxung.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ol.bjjhwx.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ti.gzmigu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bc.panjiajie.cn

[E10] 左侧补零 / 定长填充
来源：http://zj.newstarts.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hm.huixinmuqiang.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://sj.yuntaijiaju.cn

JS:   "7".padStart(3, "0")
来源：http://cq.lnxyls.cn

TS:   "7".padStart(3, "0")
来源：http://dv.colortex.cn

Java: String.format("%03d", 7)
来源：http://ae.yuexingan06.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ho.chemitech.net.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fq.panjiajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nn.hahajie.cn

[E11] 反转字符串
来源：http://fl.shtwfgs.cn

Py:   s[::-1]
来源：http://ww.panjiajie.cn

PHP:  strrev($s);
来源：http://fv.szxytkj.cn

JS:   [...s].reverse().join("")
来源：http://jf.asd995.cn

TS:   [...s].reverse().join("")
来源：http://ci.bjjhwx.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://mb.nicolike.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.bjjhwx.cn

Ruby: s.reverse
来源：http://sm.huanxung.cn

C#:   new string(s.Reverse().ToArray())
来源：http://rr.asd995.cn

[E12] 统计某字符出现次数
来源：http://zh.shxzukj.cn

Py:   s.count("a")
来源：http://uj.huixiangedu.cn

PHP:  substr_count($s, "a");
来源：http://ri.huixiangedu.cn

JS:   s.split("a").length - 1
来源：http://hq.shtwfgs.cn

TS:   s.split("a").length - 1
来源：http://al.huanxung.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tr.szxytkj.cn

Go:   strings.Count(s, "a")
来源：http://nx.hahajie.cn

Ruby: s.count("a")
来源：http://qt.chemitech.net.cn

C#:   s.Count(c => c == 'a')
来源：http://ks.szxytkj.cn

[E13] 逐字符遍历
来源：http://re.521024.cn

Py:   for ch in s: print(ch)
来源：http://js.9csxet.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rh.bookmarksfly.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://el.huanxung.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://vv.shxzukj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wk.lnxyls.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://iw.shxzukj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://zq.jianghongdianzi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yx.shxzukj.cn

[E14] URL 编码与 Base64
来源：http://mc.nszjky.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ow.jctech888.com.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://lx.lnxyls.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://op.haigaiapp.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vw.jianghongdianzi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://sm.yuexingan06.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ua.szsharing.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nm.yuexingan06.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://db.shxzskj.cn

[E15] HTML 转义 / 反转义
来源：http://re.muxihuayi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://wb.jianghongdianzi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gz.huixinmuqiang.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lt.bookmarksfly.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://yp.nszjky.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://sd.asd995.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wi.chemitech.net.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xi.szxytkj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wv.bjjhwx.cn

[E16] 数字千分位
来源：http://uo.huixinmuqiang.cn

Py:   f"{1234567:,}"
来源：http://km.yuexingan06.cn

PHP:  number_format(1234567);
来源：http://jo.jianghongdianzi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://qt.yuexingan06.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wo.huixiangedu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://km.lnxyls.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ap.shxzskj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pt.szxytkj.cn

C#:   1234567.ToString("N0")
来源：http://rl.bookmarksfly.cn

[E17] 首字母大写
来源：http://av.shxzukj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lr.huanxung.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://eo.szxytkj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ux.gzmigu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hi.huanxung.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fc.shxzukj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vj.panjiajie.cn

Ruby: s.capitalize
来源：http://sx.huixiangedu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://os.lnxyls.cn

[E18] 模板占位符替换
来源：http://ve.gzmigu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qd.shxzukj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kv.szxytkj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://yb.muxihuayi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://fw.shxzskj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pd.shxzskj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gh.wgjwhj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lw.szsharing.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bz.nszjky.cn

[E19] 多行文本按行拆分
来源：http://aw.jctech888.com.cn

Py:   s.splitlines()
来源：http://lg.521024.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://oz.gzmigu.cn

JS:   s.split(/\r?\n/)
来源：http://lf.huanxung.cn

TS:   s.split(/\r?\n/)
来源：http://hu.521024.cn

Java: s.lines().toList()
来源：http://hl.yuntaijiaju.cn

Go:   strings.Split(s, "\n")
来源：http://mh.nicolike.cn

Ruby: s.lines
来源：http://im.haigaiapp.cn

C#:   s.Split('\n')
来源：http://ti.haigaiapp.cn

[E20] 判断字符串是否为空
来源：http://db.muxihuayi.cn

Py:   if not s:
来源：http://qk.huanxung.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://iq.shxzukj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pe.yuntaijiaju.cn

TS:   if (s === "") {}
来源：http://kq.wgjwhj.cn

Java: if (s.isEmpty()) {}
来源：http://tb.hnjuh.cn

Go:   if s == "" {}
来源：http://iu.huixinmuqiang.cn

Ruby: if s.empty?
来源：http://kd.huanxung.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ti.asd995.cn

[E21] 超长截断加省略号
来源：http://bh.shtwfgs.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://er.bookmarksfly.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pf.jctech888.com.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ns.huixinmuqiang.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://in.lnxyls.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://aq.yuexingan06.cn

Go:   // 按 rune 判断长度后截断
来源：http://st.bookmarksfly.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://db.huixiangedu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ss.colortex.cn

[E22] 字节长度与字符长度
来源：http://gu.huanxung.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bm.jctech888.com.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pz.chemitech.net.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ht.colortex.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://uf.hahajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lf.bjjhwx.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hi.szsharing.cn

Ruby: s.bytesize;  s.length
来源：http://ql.wgjwhj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fc.huixiangedu.cn

================================================================================
来源：http://so.gzmigu.cn

F. 文件与目录
来源：http://hl.jianghongdianzi.cn

================================================================================
来源：http://an.521024.cn

[F01] 读取整个文件
来源：http://xl.panjiajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vj.hahajie.cn

PHP:  file_get_contents("a.txt");
来源：http://bp.bookmarksfly.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tk.shxzskj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qr.lnxyls.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://gl.shxzukj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ew.hahajie.cn

Ruby: File.read("a.txt")
来源：http://ao.jianghongdianzi.cn

C#:   File.ReadAllText("a.txt");
来源：http://um.jianghongdianzi.cn

[F02] 逐行读取文件
来源：http://ct.yuexingan06.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cf.jianghongdianzi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://us.muxihuayi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vd.newstarts.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ar.gzmigu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fy.muxihuayi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rv.szsharing.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xp.shxzukj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mw.bookmarksfly.cn

[F03] 写入文件（覆盖）
来源：http://ob.hahajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mt.huixiangedu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://rt.shxzskj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fq.hnjuh.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ao.szsharing.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zi.gzmigu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://yn.bookmarksfly.cn

Ruby: File.write("a.txt", "hi")
来源：http://yc.nszjky.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bu.wgjwhj.cn

[F04] 追加写入文件
来源：http://jf.newstarts.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xd.hnjuh.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vc.szxytkj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lr.haigaiapp.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bc.lnxyls.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fn.haigaiapp.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ur.huixinmuqiang.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wm.huixiangedu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tj.szxytkj.cn

[F05] 判断文件或目录是否存在
来源：http://xc.521024.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lf.shtwfgs.cn

PHP:  file_exists("a.txt");
来源：http://xp.bookmarksfly.cn

JS:   fs.existsSync("a.txt")
来源：http://dn.huixiangedu.cn

TS:   fs.existsSync("a.txt")
来源：http://go.hahajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://pg.huanxung.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nr.9csxet.cn

Ruby: File.exist?("a.txt")
来源：http://fg.haigaiapp.cn

C#:   File.Exists("a.txt")
来源：http://ni.panjiajie.cn

[F06] 删除文件
来源：http://dj.gzmigu.cn

Py:   os.remove("a.txt")
来源：http://hd.9csxet.cn

PHP:  unlink("a.txt");
来源：http://ym.muxihuayi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://xw.huixinmuqiang.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ie.haigaiapp.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uc.jianghongdianzi.cn

Go:   os.Remove("a.txt")
来源：http://fm.muxihuayi.cn

Ruby: File.delete("a.txt")
来源：http://nj.bookmarksfly.cn

C#:   File.Delete("a.txt");
来源：http://mi.panjiajie.cn

[F07] 创建目录（含多级）
来源：http://be.bookmarksfly.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hy.jianghongdianzi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ee.gzmigu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nt.huixiangedu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dh.jianghongdianzi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://oy.bookmarksfly.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hp.huanxung.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gx.9csxet.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lj.9csxet.cn

[F08] 遍历目录
来源：http://bf.huanxung.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://uk.gzmigu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://oy.jctech888.com.cn

JS:   fs.readdirSync("dir")
来源：http://xg.bookmarksfly.cn

TS:   fs.readdirSync("dir")
来源：http://ti.shxzukj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qm.bookmarksfly.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://av.nszjky.cn

Ruby: Dir.children("dir")
来源：http://zf.huanxung.cn

C#:   Directory.GetFiles("dir")
来源：http://ej.muxihuayi.cn

[F09] 获取文件大小
来源：http://yb.newstarts.cn

Py:   os.path.getsize("a.txt")
来源：http://tw.shxzskj.cn

PHP:  filesize("a.txt");
来源：http://do.gzmigu.cn

JS:   fs.statSync("a.txt").size
来源：http://bo.newstarts.cn


<!-- 参考信息 -->