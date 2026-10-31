代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zq.jctech888.com.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://oc.bjjhwx.cn

[D25] Set 集合去重与交并差
来源：http://mu.yuntaijiaju.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pj.huixinmuqiang.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rv.nicolike.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://am.szxytkj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nu.lnxyls.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ds.gzmigu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nt.nicolike.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nt.newstarts.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xe.gzmigu.cn

[D26] 数组转字符串
来源：http://ds.jctech888.com.cn

Py:   ", ".join(map(str, arr))
来源：http://xm.bookmarksfly.cn

PHP:  implode(", ", $arr);
来源：http://sx.hnjuh.cn

JS:   arr.join(", ")
来源：http://zl.szxytkj.cn

TS:   arr.join(", ")
来源：http://yb.jianghongdianzi.cn

Java: String.join(", ", list)
来源：http://gx.jctech888.com.cn

Go:   strings.Join(strs, ", ")
来源：http://xh.shxzukj.cn

Ruby: arr.join(", ")
来源：http://wm.yuexingan06.cn

C#:   string.Join(", ", list)
来源：http://ag.lnxyls.cn

================================================================================
来源：http://lc.huanxung.cn

E. 字符串处理
来源：http://hw.shxzukj.cn

================================================================================
来源：http://jt.newstarts.cn

[E01] 拼接字符串
来源：http://mg.hnjuh.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://iq.bjjhwx.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pk.jctech888.com.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kb.asd995.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dc.shxzskj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jt.yuntaijiaju.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gk.lnxyls.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sa.chemitech.net.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wa.huixiangedu.cn

[E02] 重复字符串
来源：http://mn.yuntaijiaju.cn

Py:   "ab" * 3
来源：http://bv.muxihuayi.cn

PHP:  str_repeat("ab", 3);
来源：http://hb.yuexingan06.cn

JS:   "ab".repeat(3)
来源：http://tj.521024.cn

TS:   "ab".repeat(3)
来源：http://hl.asd995.cn

Java: "ab".repeat(3)
来源：http://aw.yuexingan06.cn

Go:   strings.Repeat("ab", 3)
来源：http://vr.hahajie.cn

Ruby: "ab" * 3
来源：http://qp.huixiangedu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sk.521024.cn

[E03] 截取子串
来源：http://rp.hnjuh.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yo.yuntaijiaju.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kk.asd995.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gs.szxytkj.cn

TS:   s.slice(1, 4)
来源：http://rd.nszjky.cn

Java: s.substring(1, 4)
来源：http://jx.haigaiapp.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yo.szsharing.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ji.bjjhwx.cn

C#:   s.Substring(1, 3)
来源：http://mn.yuntaijiaju.cn

[E04] 查找子串位置
来源：http://tq.wgjwhj.cn

Py:   s.find("x");  s.index("x")
来源：http://zz.huanxung.cn

PHP:  strpos($s, "x");
来源：http://hg.gzmigu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pd.szxytkj.cn

TS:   s.indexOf("x")
来源：http://vf.asd995.cn

Java: s.indexOf("x")
来源：http://er.szsharing.cn

Go:   strings.Index(s, "x")
来源：http://hd.bookmarksfly.cn

Ruby: s.index("x")
来源：http://wj.hnjuh.cn

C#:   s.IndexOf("x")
来源：http://vs.gzmigu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://cx.shtwfgs.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gd.jianghongdianzi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://gl.gzmigu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ty.9csxet.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xy.hahajie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mm.hnjuh.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cc.wgjwhj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tk.9csxet.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://db.szxytkj.cn

[E06] 替换子串
来源：http://ps.szxytkj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vx.gzmigu.cn

PHP:  str_replace("a", "b", $s);
来源：http://yo.panjiajie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ll.hnjuh.cn

TS:   s.replaceAll("a", "b")
来源：http://lc.lnxyls.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fn.haigaiapp.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vm.9csxet.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kk.shxzskj.cn

C#:   s.Replace("a", "b")
来源：http://re.wgjwhj.cn

[E07] 按分隔符拆分
来源：http://ex.huixiangedu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nz.haigaiapp.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nx.panjiajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ir.9csxet.cn

TS:   s.split(",")
来源：http://hl.huixinmuqiang.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xu.yuexingan06.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://va.hahajie.cn

Ruby: s.split(",");  s.split
来源：http://rk.szxytkj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wf.huanxung.cn

[E08] 数组按分隔符合并
来源：http://la.gzmigu.cn

Py:   ",".join(items)
来源：http://ma.nicolike.cn

PHP:  implode(",", $items);
来源：http://xt.huixinmuqiang.cn

JS:   items.join(",")
来源：http://au.huixinmuqiang.cn

TS:   items.join(",")
来源：http://zr.yuexingan06.cn

Java: String.join(",", items)
来源：http://qu.muxihuayi.cn

Go:   strings.Join(items, ",")
来源：http://cx.muxihuayi.cn

Ruby: items.join(",")
来源：http://uf.lnxyls.cn

C#:   string.Join(",", items)
来源：http://ep.bjjhwx.cn

[E09] 去除所有空白字符
来源：http://vo.chemitech.net.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bo.jctech888.com.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gv.panjiajie.cn

JS:   s.replace(/\s+/g, "")
来源：http://rx.huixinmuqiang.cn

TS:   s.replace(/\s+/g, "")
来源：http://nx.colortex.cn

Java: s.replaceAll("\\s+", "")
来源：http://xk.hahajie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qt.huixiangedu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ti.huixiangedu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sb.huixinmuqiang.cn

[E10] 左侧补零 / 定长填充
来源：http://nw.521024.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gv.jctech888.com.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://sg.wgjwhj.cn

JS:   "7".padStart(3, "0")
来源：http://ss.huanxung.cn

TS:   "7".padStart(3, "0")
来源：http://dt.huixinmuqiang.cn

Java: String.format("%03d", 7)
来源：http://si.jianghongdianzi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://wv.shxzukj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cg.gzmigu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://td.bookmarksfly.cn

[E11] 反转字符串
来源：http://ni.lnxyls.cn

Py:   s[::-1]
来源：http://xh.yuntaijiaju.cn

PHP:  strrev($s);
来源：http://qd.nicolike.cn

JS:   [...s].reverse().join("")
来源：http://jy.jctech888.com.cn

TS:   [...s].reverse().join("")
来源：http://ox.shxzskj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://cl.gzmigu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://gj.huixiangedu.cn

Ruby: s.reverse
来源：http://xa.bookmarksfly.cn

C#:   new string(s.Reverse().ToArray())
来源：http://lh.huixiangedu.cn

[E12] 统计某字符出现次数
来源：http://wy.yuexingan06.cn

Py:   s.count("a")
来源：http://ui.bookmarksfly.cn

PHP:  substr_count($s, "a");
来源：http://zb.bookmarksfly.cn

JS:   s.split("a").length - 1
来源：http://qt.haigaiapp.cn

TS:   s.split("a").length - 1
来源：http://ms.yuexingan06.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yf.huanxung.cn

Go:   strings.Count(s, "a")
来源：http://ur.yuexingan06.cn

Ruby: s.count("a")
来源：http://uf.hahajie.cn

C#:   s.Count(c => c == 'a')
来源：http://lb.521024.cn

[E13] 逐字符遍历
来源：http://lr.huanxung.cn

Py:   for ch in s: print(ch)
来源：http://lr.panjiajie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zv.jctech888.com.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://it.hahajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://mi.wgjwhj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ih.521024.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rk.chemitech.net.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://xk.gzmigu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rl.bookmarksfly.cn

[E14] URL 编码与 Base64
来源：http://ab.colortex.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://re.nszjky.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://df.szxytkj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bh.shxzukj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jj.nicolike.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dp.newstarts.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kn.muxihuayi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://eb.hahajie.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fv.chemitech.net.cn

[E15] HTML 转义 / 反转义
来源：http://kp.jianghongdianzi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://rt.yuntaijiaju.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gh.nicolike.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://eg.szsharing.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://co.yuntaijiaju.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wp.jianghongdianzi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sf.hnjuh.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nd.nszjky.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ij.hahajie.cn

[E16] 数字千分位
来源：http://tw.szxytkj.cn

Py:   f"{1234567:,}"
来源：http://tt.asd995.cn

PHP:  number_format(1234567);
来源：http://ux.hnjuh.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://sq.lnxyls.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://xk.asd995.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rz.szsharing.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kd.jctech888.com.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://um.521024.cn

C#:   1234567.ToString("N0")
来源：http://dy.yuntaijiaju.cn

[E17] 首字母大写
来源：http://ea.chemitech.net.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sl.szxytkj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://qq.huixiangedu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fo.jianghongdianzi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kh.wgjwhj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ok.haigaiapp.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wn.yuntaijiaju.cn

Ruby: s.capitalize
来源：http://jo.hnjuh.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://sn.521024.cn

[E18] 模板占位符替换
来源：http://za.hahajie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wx.haigaiapp.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ol.szxytkj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://he.bookmarksfly.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ig.asd995.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nt.gzmigu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rw.lnxyls.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://os.bjjhwx.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tc.wgjwhj.cn

[E19] 多行文本按行拆分
来源：http://ok.gzmigu.cn

Py:   s.splitlines()
来源：http://vh.huixinmuqiang.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://np.huixinmuqiang.cn

JS:   s.split(/\r?\n/)
来源：http://bg.wgjwhj.cn

TS:   s.split(/\r?\n/)
来源：http://nb.chemitech.net.cn

Java: s.lines().toList()
来源：http://rv.shxzskj.cn

Go:   strings.Split(s, "\n")
来源：http://dq.huanxung.cn

Ruby: s.lines
来源：http://lu.huixiangedu.cn

C#:   s.Split('\n')
来源：http://yy.yuntaijiaju.cn

[E20] 判断字符串是否为空
来源：http://dx.yuexingan06.cn

Py:   if not s:
来源：http://xe.wgjwhj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dy.shxzskj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://js.asd995.cn

TS:   if (s === "") {}
来源：http://jf.bookmarksfly.cn

Java: if (s.isEmpty()) {}
来源：http://yt.gzmigu.cn

Go:   if s == "" {}
来源：http://qs.yuntaijiaju.cn

Ruby: if s.empty?
来源：http://yq.9csxet.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lb.yuexingan06.cn

[E21] 超长截断加省略号
来源：http://wb.bjjhwx.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tb.szsharing.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pz.shxzskj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qz.hahajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gf.szxytkj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qd.szxytkj.cn

Go:   // 按 rune 判断长度后截断
来源：http://yn.nicolike.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xv.yuntaijiaju.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wb.521024.cn

[E22] 字节长度与字符长度
来源：http://cc.yuntaijiaju.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ik.yuntaijiaju.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nh.bjjhwx.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ww.9csxet.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yw.yuexingan06.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bj.colortex.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ap.huanxung.cn

Ruby: s.bytesize;  s.length
来源：http://rm.szsharing.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vh.shtwfgs.cn

================================================================================
来源：http://vv.wgjwhj.cn

F. 文件与目录
来源：http://xj.newstarts.cn

================================================================================
来源：http://zu.huanxung.cn

[F01] 读取整个文件
来源：http://be.shxzukj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uh.lnxyls.cn

PHP:  file_get_contents("a.txt");
来源：http://te.hahajie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://uw.lnxyls.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vh.jianghongdianzi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ic.nszjky.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uv.colortex.cn

Ruby: File.read("a.txt")
来源：http://nq.huanxung.cn

C#:   File.ReadAllText("a.txt");
来源：http://jc.lnxyls.cn

[F02] 逐行读取文件
来源：http://zv.asd995.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xu.asd995.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nc.9csxet.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://is.nicolike.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kf.hahajie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tx.huixinmuqiang.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rc.yuexingan06.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hp.szsharing.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://un.hnjuh.cn

[F03] 写入文件（覆盖）
来源：http://zs.hahajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vu.jctech888.com.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://jn.gzmigu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uo.chemitech.net.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fk.shxzukj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hv.jianghongdianzi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ic.asd995.cn

Ruby: File.write("a.txt", "hi")
来源：http://fw.newstarts.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wc.wgjwhj.cn

[F04] 追加写入文件
来源：http://bl.szxytkj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hi.huixiangedu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zj.jianghongdianzi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rh.szsharing.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://up.jianghongdianzi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vl.bjjhwx.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gx.huixiangedu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xj.9csxet.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bh.jctech888.com.cn

[F05] 判断文件或目录是否存在
来源：http://pw.asd995.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fh.bjjhwx.cn

PHP:  file_exists("a.txt");
来源：http://hy.shtwfgs.cn

JS:   fs.existsSync("a.txt")
来源：http://fk.bjjhwx.cn

TS:   fs.existsSync("a.txt")
来源：http://ud.jianghongdianzi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://wi.nicolike.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zq.bookmarksfly.cn

Ruby: File.exist?("a.txt")
来源：http://oz.nszjky.cn

C#:   File.Exists("a.txt")
来源：http://wj.yuntaijiaju.cn

[F06] 删除文件
来源：http://be.muxihuayi.cn

Py:   os.remove("a.txt")
来源：http://is.shxzukj.cn

PHP:  unlink("a.txt");
来源：http://lm.hnjuh.cn

JS:   fs.unlinkSync("a.txt")
来源：http://tj.nicolike.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vt.asd995.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tf.huixinmuqiang.cn

Go:   os.Remove("a.txt")
来源：http://iy.huixinmuqiang.cn

Ruby: File.delete("a.txt")
来源：http://kf.gzmigu.cn

C#:   File.Delete("a.txt");
来源：http://ti.lnxyls.cn

[F07] 创建目录（含多级）
来源：http://we.colortex.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cz.jctech888.com.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ml.asd995.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ye.huixinmuqiang.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ub.asd995.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pa.szsharing.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qd.yuntaijiaju.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://il.huanxung.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ij.yuntaijiaju.cn

[F08] 遍历目录
来源：http://ro.hahajie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://wb.yuexingan06.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://if.huixiangedu.cn

JS:   fs.readdirSync("dir")
来源：http://gx.hnjuh.cn

TS:   fs.readdirSync("dir")
来源：http://ku.haigaiapp.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sk.jianghongdianzi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fq.gzmigu.cn

Ruby: Dir.children("dir")
来源：http://nf.9csxet.cn

C#:   Directory.GetFiles("dir")
来源：http://em.asd995.cn

[F09] 获取文件大小
来源：http://qp.lnxyls.cn

Py:   os.path.getsize("a.txt")
来源：http://rr.shtwfgs.cn

PHP:  filesize("a.txt");
来源：http://bf.wgjwhj.cn

JS:   fs.statSync("a.txt").size
来源：http://tf.wgjwhj.cn


<!-- 参考信息 -->