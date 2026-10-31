代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yw.chemitech.net.cn

[D24] 字典 / Map 基本操作
来源：http://br.nicolike.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zf.jianghongdianzi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://db.hnjuh.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wx.panjiajie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wl.gzmigu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uv.hnjuh.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ox.jianghongdianzi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lv.newstarts.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ff.shtwfgs.cn

[D25] Set 集合去重与交并差
来源：http://pl.jctech888.com.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bu.haigaiapp.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jf.hahajie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bk.wgjwhj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ob.szsharing.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ah.shtwfgs.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ac.nicolike.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rf.szsharing.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ha.huixiangedu.cn

[D26] 数组转字符串
来源：http://sy.chemitech.net.cn

Py:   ", ".join(map(str, arr))
来源：http://aa.hnjuh.cn

PHP:  implode(", ", $arr);
来源：http://bp.huixiangedu.cn

JS:   arr.join(", ")
来源：http://og.nszjky.cn

TS:   arr.join(", ")
来源：http://ca.bjjhwx.cn

Java: String.join(", ", list)
来源：http://jt.huixiangedu.cn

Go:   strings.Join(strs, ", ")
来源：http://rm.shtwfgs.cn

Ruby: arr.join(", ")
来源：http://lz.huixiangedu.cn

C#:   string.Join(", ", list)
来源：http://ba.huanxung.cn

================================================================================
来源：http://ic.shxzskj.cn

E. 字符串处理
来源：http://js.nszjky.cn

================================================================================
来源：http://ga.newstarts.cn

[E01] 拼接字符串
来源：http://ap.jianghongdianzi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ea.hahajie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ci.wgjwhj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hy.shtwfgs.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nj.yuexingan06.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xq.bjjhwx.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ap.9csxet.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://aj.yuntaijiaju.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tn.chemitech.net.cn

[E02] 重复字符串
来源：http://tu.nszjky.cn

Py:   "ab" * 3
来源：http://kq.shxzskj.cn

PHP:  str_repeat("ab", 3);
来源：http://qi.yuntaijiaju.cn

JS:   "ab".repeat(3)
来源：http://ge.9csxet.cn

TS:   "ab".repeat(3)
来源：http://qe.asd995.cn

Java: "ab".repeat(3)
来源：http://ss.chemitech.net.cn

Go:   strings.Repeat("ab", 3)
来源：http://zo.shxzukj.cn

Ruby: "ab" * 3
来源：http://kq.huixinmuqiang.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hr.yuntaijiaju.cn

[E03] 截取子串
来源：http://ym.huixinmuqiang.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tm.muxihuayi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://so.asd995.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yx.yuntaijiaju.cn

TS:   s.slice(1, 4)
来源：http://jc.yuexingan06.cn

Java: s.substring(1, 4)
来源：http://gf.gzmigu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kw.shxzukj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ce.szxytkj.cn

C#:   s.Substring(1, 3)
来源：http://xy.yuexingan06.cn

[E04] 查找子串位置
来源：http://fj.panjiajie.cn

Py:   s.find("x");  s.index("x")
来源：http://mw.shxzukj.cn

PHP:  strpos($s, "x");
来源：http://qy.jctech888.com.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nc.nszjky.cn

TS:   s.indexOf("x")
来源：http://ev.newstarts.cn

Java: s.indexOf("x")
来源：http://qq.lnxyls.cn

Go:   strings.Index(s, "x")
来源：http://er.panjiajie.cn

Ruby: s.index("x")
来源：http://ci.colortex.cn

C#:   s.IndexOf("x")
来源：http://xj.gzmigu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://oa.haigaiapp.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://yj.yuntaijiaju.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pv.jctech888.com.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jk.huanxung.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://gw.szxytkj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ks.lnxyls.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bk.521024.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gg.9csxet.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ks.hnjuh.cn

[E06] 替换子串
来源：http://oj.yuntaijiaju.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ou.huanxung.cn

PHP:  str_replace("a", "b", $s);
来源：http://zv.hnjuh.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xj.521024.cn

TS:   s.replaceAll("a", "b")
来源：http://wa.jianghongdianzi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zu.shxzukj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://is.szxytkj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ee.jianghongdianzi.cn

C#:   s.Replace("a", "b")
来源：http://qn.colortex.cn

[E07] 按分隔符拆分
来源：http://bm.shtwfgs.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://az.chemitech.net.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ua.szsharing.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://vx.asd995.cn

TS:   s.split(",")
来源：http://dw.chemitech.net.cn

Java: s.split(",");  s.split("\\s+")
来源：http://dh.gzmigu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nu.nicolike.cn

Ruby: s.split(",");  s.split
来源：http://em.huixiangedu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tm.asd995.cn

[E08] 数组按分隔符合并
来源：http://wt.huanxung.cn

Py:   ",".join(items)
来源：http://dr.yuntaijiaju.cn

PHP:  implode(",", $items);
来源：http://iy.huixinmuqiang.cn

JS:   items.join(",")
来源：http://yz.haigaiapp.cn

TS:   items.join(",")
来源：http://hm.521024.cn

Java: String.join(",", items)
来源：http://th.hahajie.cn

Go:   strings.Join(items, ",")
来源：http://cv.huanxung.cn

Ruby: items.join(",")
来源：http://ak.shxzukj.cn

C#:   string.Join(",", items)
来源：http://gv.bjjhwx.cn

[E09] 去除所有空白字符
来源：http://qr.521024.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fi.chemitech.net.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cb.colortex.cn

JS:   s.replace(/\s+/g, "")
来源：http://qu.huixinmuqiang.cn

TS:   s.replace(/\s+/g, "")
来源：http://qf.huanxung.cn

Java: s.replaceAll("\\s+", "")
来源：http://zg.jctech888.com.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://bv.shxzskj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ae.bjjhwx.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mo.gzmigu.cn

[E10] 左侧补零 / 定长填充
来源：http://ih.huixinmuqiang.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://sd.huixinmuqiang.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://we.shtwfgs.cn

JS:   "7".padStart(3, "0")
来源：http://cy.hnjuh.cn

TS:   "7".padStart(3, "0")
来源：http://uo.hnjuh.cn

Java: String.format("%03d", 7)
来源：http://vn.shxzskj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://nr.yuexingan06.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kl.muxihuayi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dg.muxihuayi.cn

[E11] 反转字符串
来源：http://vz.muxihuayi.cn

Py:   s[::-1]
来源：http://rj.bjjhwx.cn

PHP:  strrev($s);
来源：http://um.yuntaijiaju.cn

JS:   [...s].reverse().join("")
来源：http://vy.hahajie.cn

TS:   [...s].reverse().join("")
来源：http://yr.szsharing.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://vs.gzmigu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ps.szxytkj.cn

Ruby: s.reverse
来源：http://qd.szxytkj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://lb.gzmigu.cn

[E12] 统计某字符出现次数
来源：http://aj.haigaiapp.cn

Py:   s.count("a")
来源：http://uc.hnjuh.cn

PHP:  substr_count($s, "a");
来源：http://ov.521024.cn

JS:   s.split("a").length - 1
来源：http://zz.yuntaijiaju.cn

TS:   s.split("a").length - 1
来源：http://ge.wgjwhj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hl.521024.cn

Go:   strings.Count(s, "a")
来源：http://sa.wgjwhj.cn

Ruby: s.count("a")
来源：http://xa.chemitech.net.cn

C#:   s.Count(c => c == 'a')
来源：http://yz.hnjuh.cn

[E13] 逐字符遍历
来源：http://wo.huixinmuqiang.cn

Py:   for ch in s: print(ch)
来源：http://wa.asd995.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yr.nszjky.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://gp.nszjky.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://yd.gzmigu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vj.wgjwhj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vg.huanxung.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://dk.newstarts.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kk.bookmarksfly.cn

[E14] URL 编码与 Base64
来源：http://re.yuntaijiaju.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://uc.muxihuayi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ac.huanxung.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://sb.wgjwhj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xu.shtwfgs.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xw.hnjuh.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ox.asd995.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://eu.bjjhwx.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ir.bjjhwx.cn

[E15] HTML 转义 / 反转义
来源：http://sp.nszjky.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://tc.gzmigu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gs.szsharing.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pb.huixinmuqiang.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://bz.lnxyls.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lh.huixiangedu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://za.jctech888.com.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ij.hnjuh.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vb.chemitech.net.cn

[E16] 数字千分位
来源：http://mz.9csxet.cn

Py:   f"{1234567:,}"
来源：http://ob.bjjhwx.cn

PHP:  number_format(1234567);
来源：http://xq.huixiangedu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://hg.lnxyls.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ze.huixiangedu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dd.shxzskj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://sx.panjiajie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mc.shxzukj.cn

C#:   1234567.ToString("N0")
来源：http://hz.szxytkj.cn

[E17] 首字母大写
来源：http://yo.muxihuayi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mv.gzmigu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://hs.muxihuayi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hs.hnjuh.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ly.szsharing.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dy.chemitech.net.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gp.asd995.cn

Ruby: s.capitalize
来源：http://pn.colortex.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zn.asd995.cn

[E18] 模板占位符替换
来源：http://hj.nicolike.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ew.szxytkj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ye.huixinmuqiang.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ds.yuexingan06.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ml.yuexingan06.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qv.gzmigu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gu.yuexingan06.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hk.hahajie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://sa.shxzukj.cn

[E19] 多行文本按行拆分
来源：http://vh.colortex.cn

Py:   s.splitlines()
来源：http://fx.gzmigu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ve.bjjhwx.cn

JS:   s.split(/\r?\n/)
来源：http://lu.521024.cn

TS:   s.split(/\r?\n/)
来源：http://yq.shxzskj.cn

Java: s.lines().toList()
来源：http://ny.shtwfgs.cn

Go:   strings.Split(s, "\n")
来源：http://bp.haigaiapp.cn

Ruby: s.lines
来源：http://mv.nszjky.cn

C#:   s.Split('\n')
来源：http://qb.newstarts.cn

[E20] 判断字符串是否为空
来源：http://bm.nszjky.cn

Py:   if not s:
来源：http://oy.jianghongdianzi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xc.szxytkj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lm.shxzskj.cn

TS:   if (s === "") {}
来源：http://pn.gzmigu.cn

Java: if (s.isEmpty()) {}
来源：http://yf.shxzukj.cn

Go:   if s == "" {}
来源：http://ge.hnjuh.cn

Ruby: if s.empty?
来源：http://jt.521024.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ep.chemitech.net.cn

[E21] 超长截断加省略号
来源：http://us.gzmigu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://oh.szxytkj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zi.chemitech.net.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ge.asd995.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ly.szxytkj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bj.521024.cn

Go:   // 按 rune 判断长度后截断
来源：http://lx.panjiajie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vj.yuntaijiaju.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://st.asd995.cn

[E22] 字节长度与字符长度
来源：http://fb.hahajie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zu.shxzukj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ve.szxytkj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://eb.szxytkj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xl.hnjuh.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://oy.szxytkj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://eg.huixiangedu.cn

Ruby: s.bytesize;  s.length
来源：http://vs.muxihuayi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cg.nszjky.cn

================================================================================
来源：http://dn.nicolike.cn

F. 文件与目录
来源：http://ox.asd995.cn

================================================================================
来源：http://kf.jianghongdianzi.cn

[F01] 读取整个文件
来源：http://na.colortex.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gw.shtwfgs.cn

PHP:  file_get_contents("a.txt");
来源：http://wd.9csxet.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zk.shtwfgs.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jk.hnjuh.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://wb.szsharing.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hv.chemitech.net.cn

Ruby: File.read("a.txt")
来源：http://yg.shxzskj.cn

C#:   File.ReadAllText("a.txt");
来源：http://rj.shxzskj.cn

[F02] 逐行读取文件
来源：http://ks.haigaiapp.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rr.shxzskj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pb.szxytkj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gl.szxytkj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jf.haigaiapp.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://va.jctech888.com.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hv.haigaiapp.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://uc.yuexingan06.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fk.9csxet.cn

[F03] 写入文件（覆盖）
来源：http://ha.chemitech.net.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ml.bjjhwx.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://fr.huixinmuqiang.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ot.hahajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sg.shxzukj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://eg.521024.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://es.nszjky.cn

Ruby: File.write("a.txt", "hi")
来源：http://og.panjiajie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vl.huixinmuqiang.cn

[F04] 追加写入文件
来源：http://nc.muxihuayi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dj.yuntaijiaju.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gy.shxzskj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qg.yuntaijiaju.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kq.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://es.hahajie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kr.jctech888.com.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wd.colortex.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cs.shxzukj.cn

[F05] 判断文件或目录是否存在
来源：http://xz.shxzukj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ap.panjiajie.cn

PHP:  file_exists("a.txt");
来源：http://sv.chemitech.net.cn

JS:   fs.existsSync("a.txt")
来源：http://yp.bookmarksfly.cn

TS:   fs.existsSync("a.txt")
来源：http://rg.bookmarksfly.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ba.jianghongdianzi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ty.huixiangedu.cn

Ruby: File.exist?("a.txt")
来源：http://zs.lnxyls.cn

C#:   File.Exists("a.txt")
来源：http://ru.huixinmuqiang.cn

[F06] 删除文件
来源：http://vx.521024.cn

Py:   os.remove("a.txt")
来源：http://pc.bookmarksfly.cn

PHP:  unlink("a.txt");
来源：http://xf.huanxung.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ad.newstarts.cn

TS:   fs.unlinkSync("a.txt")
来源：http://oc.haigaiapp.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ts.huixinmuqiang.cn

Go:   os.Remove("a.txt")
来源：http://sp.hahajie.cn

Ruby: File.delete("a.txt")
来源：http://wg.shtwfgs.cn

C#:   File.Delete("a.txt");
来源：http://jk.asd995.cn

[F07] 创建目录（含多级）
来源：http://ae.szsharing.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hf.szxytkj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cn.lnxyls.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ng.lnxyls.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cx.jctech888.com.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zo.asd995.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://np.lnxyls.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qd.panjiajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ec.newstarts.cn

[F08] 遍历目录
来源：http://nc.wgjwhj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://id.szxytkj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lw.shxzskj.cn

JS:   fs.readdirSync("dir")
来源：http://xz.bookmarksfly.cn

TS:   fs.readdirSync("dir")
来源：http://hq.hnjuh.cn


<!-- 参考信息 -->