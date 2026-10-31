代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cq.colortex.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tj.9csxet.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rr.jianghongdianzi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://oc.hnjuh.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qm.9csxet.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pd.huanxung.cn

[D25] Set 集合去重与交并差
来源：http://ti.panjiajie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ju.newstarts.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rf.9csxet.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ul.panjiajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ea.szsharing.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fv.chemitech.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ep.9csxet.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fh.shxzskj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gf.hahajie.cn

[D26] 数组转字符串
来源：http://ad.wgjwhj.cn

Py:   ", ".join(map(str, arr))
来源：http://vv.huixiangedu.cn

PHP:  implode(", ", $arr);
来源：http://eg.nicolike.cn

JS:   arr.join(", ")
来源：http://nr.9csxet.cn

TS:   arr.join(", ")
来源：http://bp.9csxet.cn

Java: String.join(", ", list)
来源：http://oh.shxzskj.cn

Go:   strings.Join(strs, ", ")
来源：http://vz.huanxung.cn

Ruby: arr.join(", ")
来源：http://di.shxzukj.cn

C#:   string.Join(", ", list)
来源：http://px.jianghongdianzi.cn

================================================================================
来源：http://db.huanxung.cn

E. 字符串处理
来源：http://bv.bookmarksfly.cn

================================================================================
来源：http://ao.shxzukj.cn

[E01] 拼接字符串
来源：http://at.haigaiapp.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tb.shtwfgs.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ou.shxzskj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rc.jctech888.com.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yz.bookmarksfly.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lz.haigaiapp.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sz.huixiangedu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ok.gzmigu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wi.szxytkj.cn

[E02] 重复字符串
来源：http://pd.nszjky.cn

Py:   "ab" * 3
来源：http://bj.shxzskj.cn

PHP:  str_repeat("ab", 3);
来源：http://ne.muxihuayi.cn

JS:   "ab".repeat(3)
来源：http://mn.shxzskj.cn

TS:   "ab".repeat(3)
来源：http://vv.hnjuh.cn

Java: "ab".repeat(3)
来源：http://lu.muxihuayi.cn

Go:   strings.Repeat("ab", 3)
来源：http://rw.bjjhwx.cn

Ruby: "ab" * 3
来源：http://ur.huixiangedu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://li.szsharing.cn

[E03] 截取子串
来源：http://qr.colortex.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zj.yuntaijiaju.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fj.yuexingan06.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ly.asd995.cn

TS:   s.slice(1, 4)
来源：http://lx.colortex.cn

Java: s.substring(1, 4)
来源：http://rv.yuntaijiaju.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://uc.yuntaijiaju.cn

Ruby: s[1, 3];  s[1..3]
来源：http://iv.colortex.cn

C#:   s.Substring(1, 3)
来源：http://ek.bjjhwx.cn

[E04] 查找子串位置
来源：http://je.hahajie.cn

Py:   s.find("x");  s.index("x")
来源：http://er.chemitech.net.cn

PHP:  strpos($s, "x");
来源：http://dz.huixiangedu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kp.wgjwhj.cn

TS:   s.indexOf("x")
来源：http://bm.gzmigu.cn

Java: s.indexOf("x")
来源：http://gt.hahajie.cn

Go:   strings.Index(s, "x")
来源：http://cu.huixinmuqiang.cn

Ruby: s.index("x")
来源：http://mj.hnjuh.cn

C#:   s.IndexOf("x")
来源：http://rg.muxihuayi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://zo.panjiajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rc.huixiangedu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://um.huanxung.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://di.yuntaijiaju.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hr.jianghongdianzi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://re.nszjky.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nr.nszjky.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://sl.hahajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://id.szxytkj.cn

[E06] 替换子串
来源：http://cz.nszjky.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fo.jctech888.com.cn

PHP:  str_replace("a", "b", $s);
来源：http://ji.colortex.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ot.lnxyls.cn

TS:   s.replaceAll("a", "b")
来源：http://mr.gzmigu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mz.szsharing.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://aj.wgjwhj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ns.panjiajie.cn

C#:   s.Replace("a", "b")
来源：http://xf.shtwfgs.cn

[E07] 按分隔符拆分
来源：http://lg.chemitech.net.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dp.newstarts.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gx.haigaiapp.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://gq.nszjky.cn

TS:   s.split(",")
来源：http://yi.shtwfgs.cn

Java: s.split(",");  s.split("\\s+")
来源：http://sz.9csxet.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yy.bookmarksfly.cn

Ruby: s.split(",");  s.split
来源：http://yy.gzmigu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://st.jianghongdianzi.cn

[E08] 数组按分隔符合并
来源：http://kw.shtwfgs.cn

Py:   ",".join(items)
来源：http://hk.9csxet.cn

PHP:  implode(",", $items);
来源：http://aj.huanxung.cn

JS:   items.join(",")
来源：http://no.newstarts.cn

TS:   items.join(",")
来源：http://ca.bjjhwx.cn

Java: String.join(",", items)
来源：http://tz.huixinmuqiang.cn

Go:   strings.Join(items, ",")
来源：http://xv.jianghongdianzi.cn

Ruby: items.join(",")
来源：http://zs.9csxet.cn

C#:   string.Join(",", items)
来源：http://wk.wgjwhj.cn

[E09] 去除所有空白字符
来源：http://hg.szsharing.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rm.lnxyls.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ml.huixiangedu.cn

JS:   s.replace(/\s+/g, "")
来源：http://yl.newstarts.cn

TS:   s.replace(/\s+/g, "")
来源：http://sr.huanxung.cn

Java: s.replaceAll("\\s+", "")
来源：http://dn.521024.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://pa.hahajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://nn.lnxyls.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yp.huixinmuqiang.cn

[E10] 左侧补零 / 定长填充
来源：http://qk.shtwfgs.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qr.bookmarksfly.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hn.colortex.cn

JS:   "7".padStart(3, "0")
来源：http://ka.521024.cn

TS:   "7".padStart(3, "0")
来源：http://kn.yuexingan06.cn

Java: String.format("%03d", 7)
来源：http://jw.yuexingan06.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://gk.hnjuh.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bc.nicolike.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wp.huanxung.cn

[E11] 反转字符串
来源：http://sd.gzmigu.cn

Py:   s[::-1]
来源：http://re.jianghongdianzi.cn

PHP:  strrev($s);
来源：http://ow.panjiajie.cn

JS:   [...s].reverse().join("")
来源：http://ot.newstarts.cn

TS:   [...s].reverse().join("")
来源：http://rk.hahajie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://jz.colortex.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://nn.hahajie.cn

Ruby: s.reverse
来源：http://jf.yuexingan06.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ik.shxzukj.cn

[E12] 统计某字符出现次数
来源：http://oc.panjiajie.cn

Py:   s.count("a")
来源：http://gp.asd995.cn

PHP:  substr_count($s, "a");
来源：http://od.lnxyls.cn

JS:   s.split("a").length - 1
来源：http://xj.hahajie.cn

TS:   s.split("a").length - 1
来源：http://mi.asd995.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://eb.shtwfgs.cn

Go:   strings.Count(s, "a")
来源：http://kj.lnxyls.cn

Ruby: s.count("a")
来源：http://hf.huixinmuqiang.cn

C#:   s.Count(c => c == 'a')
来源：http://zh.gzmigu.cn

[E13] 逐字符遍历
来源：http://yx.9csxet.cn

Py:   for ch in s: print(ch)
来源：http://id.huanxung.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pg.yuntaijiaju.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xp.haigaiapp.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ey.colortex.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ds.9csxet.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yk.nszjky.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://zw.huixiangedu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gj.hnjuh.cn

[E14] URL 编码与 Base64
来源：http://mf.huanxung.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sp.hnjuh.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://vr.asd995.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://sd.jctech888.com.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sg.muxihuayi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://if.nicolike.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dt.nicolike.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://th.521024.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ur.lnxyls.cn

[E15] HTML 转义 / 反转义
来源：http://lh.hahajie.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://hv.jctech888.com.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ej.bookmarksfly.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yz.newstarts.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://kk.bjjhwx.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jn.bookmarksfly.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fh.yuexingan06.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zi.szxytkj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nu.shtwfgs.cn

[E16] 数字千分位
来源：http://wz.9csxet.cn

Py:   f"{1234567:,}"
来源：http://xa.muxihuayi.cn

PHP:  number_format(1234567);
来源：http://zy.chemitech.net.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://hj.gzmigu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ia.yuexingan06.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jm.szxytkj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fe.chemitech.net.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://le.yuntaijiaju.cn

C#:   1234567.ToString("N0")
来源：http://nl.shxzukj.cn

[E17] 首字母大写
来源：http://gd.nicolike.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zm.szxytkj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://mf.hnjuh.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fv.yuntaijiaju.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ki.panjiajie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://da.huanxung.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://op.panjiajie.cn

Ruby: s.capitalize
来源：http://uv.bookmarksfly.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xt.newstarts.cn

[E18] 模板占位符替换
来源：http://oq.colortex.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vu.nicolike.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ny.shxzukj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zy.yuntaijiaju.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://eq.nicolike.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gz.panjiajie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bg.nicolike.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fn.9csxet.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ku.huanxung.cn

[E19] 多行文本按行拆分
来源：http://nc.9csxet.cn

Py:   s.splitlines()
来源：http://we.huixiangedu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wq.colortex.cn

JS:   s.split(/\r?\n/)
来源：http://kf.9csxet.cn

TS:   s.split(/\r?\n/)
来源：http://bn.yuntaijiaju.cn

Java: s.lines().toList()
来源：http://ui.panjiajie.cn

Go:   strings.Split(s, "\n")
来源：http://ik.yuexingan06.cn

Ruby: s.lines
来源：http://dj.521024.cn

C#:   s.Split('\n')
来源：http://uw.asd995.cn

[E20] 判断字符串是否为空
来源：http://ha.chemitech.net.cn

Py:   if not s:
来源：http://ks.bookmarksfly.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hh.gzmigu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cb.huanxung.cn

TS:   if (s === "") {}
来源：http://uu.huixiangedu.cn

Java: if (s.isEmpty()) {}
来源：http://xj.colortex.cn

Go:   if s == "" {}
来源：http://wa.shxzskj.cn

Ruby: if s.empty?
来源：http://er.panjiajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qm.haigaiapp.cn

[E21] 超长截断加省略号
来源：http://rs.shxzskj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rf.panjiajie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://io.newstarts.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sl.bjjhwx.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ge.521024.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://do.haigaiapp.cn

Go:   // 按 rune 判断长度后截断
来源：http://zz.jctech888.com.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rz.wgjwhj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mu.huixiangedu.cn

[E22] 字节长度与字符长度
来源：http://fy.szxytkj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sc.huanxung.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jp.yuntaijiaju.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gp.huanxung.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yd.szxytkj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fi.bjjhwx.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hh.shxzskj.cn

Ruby: s.bytesize;  s.length
来源：http://it.shxzskj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kh.panjiajie.cn

================================================================================
来源：http://ph.yuntaijiaju.cn

F. 文件与目录
来源：http://nd.szxytkj.cn

================================================================================
来源：http://ow.colortex.cn

[F01] 读取整个文件
来源：http://xs.shxzukj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ty.gzmigu.cn

PHP:  file_get_contents("a.txt");
来源：http://yl.haigaiapp.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ab.nszjky.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qk.521024.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://pe.yuexingan06.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yb.bjjhwx.cn

Ruby: File.read("a.txt")
来源：http://fs.shtwfgs.cn

C#:   File.ReadAllText("a.txt");
来源：http://tv.nszjky.cn

[F02] 逐行读取文件
来源：http://ok.huixiangedu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dc.shxzskj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tv.lnxyls.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ug.bjjhwx.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qo.huixinmuqiang.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wu.yuexingan06.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ln.yuntaijiaju.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rj.szsharing.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hy.huixiangedu.cn

[F03] 写入文件（覆盖）
来源：http://lu.huanxung.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xc.shtwfgs.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://qr.shxzskj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gm.yuexingan06.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fv.huixinmuqiang.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hd.huixiangedu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://oa.muxihuayi.cn

Ruby: File.write("a.txt", "hi")
来源：http://vf.haigaiapp.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ix.shtwfgs.cn

[F04] 追加写入文件
来源：http://pf.shxzukj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bz.bjjhwx.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lb.hahajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nj.panjiajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://li.521024.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ak.bjjhwx.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ml.asd995.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zu.nicolike.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wk.shxzukj.cn

[F05] 判断文件或目录是否存在
来源：http://wz.9csxet.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bw.gzmigu.cn

PHP:  file_exists("a.txt");
来源：http://pu.panjiajie.cn

JS:   fs.existsSync("a.txt")
来源：http://uw.wgjwhj.cn

TS:   fs.existsSync("a.txt")
来源：http://pn.nszjky.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://pn.muxihuayi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qe.chemitech.net.cn

Ruby: File.exist?("a.txt")
来源：http://yl.asd995.cn

C#:   File.Exists("a.txt")
来源：http://pi.shtwfgs.cn

[F06] 删除文件
来源：http://lf.asd995.cn

Py:   os.remove("a.txt")
来源：http://ev.521024.cn

PHP:  unlink("a.txt");
来源：http://xf.bjjhwx.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ue.huanxung.cn

TS:   fs.unlinkSync("a.txt")
来源：http://bt.szsharing.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zh.huixiangedu.cn

Go:   os.Remove("a.txt")
来源：http://oa.hahajie.cn

Ruby: File.delete("a.txt")
来源：http://rp.asd995.cn

C#:   File.Delete("a.txt");
来源：http://wj.panjiajie.cn

[F07] 创建目录（含多级）
来源：http://jc.nicolike.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qt.bjjhwx.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vy.lnxyls.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fr.newstarts.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ai.yuexingan06.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ro.gzmigu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ye.colortex.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ku.9csxet.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://uc.huanxung.cn

[F08] 遍历目录
来源：http://fp.newstarts.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://fz.yuexingan06.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nc.muxihuayi.cn

JS:   fs.readdirSync("dir")
来源：http://nv.szxytkj.cn

TS:   fs.readdirSync("dir")
来源：http://re.asd995.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gh.shxzukj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ez.hnjuh.cn

Ruby: Dir.children("dir")
来源：http://iq.521024.cn

C#:   Directory.GetFiles("dir")
来源：http://ko.yuexingan06.cn


<!-- 参考信息 -->