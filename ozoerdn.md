代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dh.shxzskj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fy.nicolike.cn

Go:   // 手写循环
来源：http://wx.shxzskj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xi.521024.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rv.chemitech.net.cn

[D24] 字典 / Map 基本操作
来源：http://vt.shxzukj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ov.newstarts.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dx.shxzukj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://po.hnjuh.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ka.panjiajie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://oz.bookmarksfly.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ph.szsharing.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://sw.yuntaijiaju.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gz.newstarts.cn

[D25] Set 集合去重与交并差
来源：http://ny.9csxet.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ep.gzmigu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kj.colortex.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fx.huanxung.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mx.jctech888.com.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ps.gzmigu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fn.yuexingan06.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://js.haigaiapp.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://so.huixiangedu.cn

[D26] 数组转字符串
来源：http://uq.szsharing.cn

Py:   ", ".join(map(str, arr))
来源：http://be.chemitech.net.cn

PHP:  implode(", ", $arr);
来源：http://tj.asd995.cn

JS:   arr.join(", ")
来源：http://ne.hahajie.cn

TS:   arr.join(", ")
来源：http://jw.szsharing.cn

Java: String.join(", ", list)
来源：http://gm.lnxyls.cn

Go:   strings.Join(strs, ", ")
来源：http://ew.lnxyls.cn

Ruby: arr.join(", ")
来源：http://aw.szsharing.cn

C#:   string.Join(", ", list)
来源：http://ov.asd995.cn

================================================================================
来源：http://oe.jctech888.com.cn

E. 字符串处理
来源：http://ev.muxihuayi.cn

================================================================================
来源：http://pe.huixiangedu.cn

[E01] 拼接字符串
来源：http://gi.wgjwhj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rg.huanxung.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zu.huanxung.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pp.huanxung.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://po.muxihuayi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mo.hnjuh.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cn.nszjky.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qp.chemitech.net.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cn.newstarts.cn

[E02] 重复字符串
来源：http://sg.szsharing.cn

Py:   "ab" * 3
来源：http://eq.nicolike.cn

PHP:  str_repeat("ab", 3);
来源：http://zs.szsharing.cn

JS:   "ab".repeat(3)
来源：http://ch.wgjwhj.cn

TS:   "ab".repeat(3)
来源：http://as.szxytkj.cn

Java: "ab".repeat(3)
来源：http://cp.asd995.cn

Go:   strings.Repeat("ab", 3)
来源：http://ag.asd995.cn

Ruby: "ab" * 3
来源：http://ah.shxzukj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ej.muxihuayi.cn

[E03] 截取子串
来源：http://vy.panjiajie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mw.chemitech.net.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dy.szsharing.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fy.haigaiapp.cn

TS:   s.slice(1, 4)
来源：http://lj.nicolike.cn

Java: s.substring(1, 4)
来源：http://ij.hnjuh.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tr.nszjky.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ry.hnjuh.cn

C#:   s.Substring(1, 3)
来源：http://co.nicolike.cn

[E04] 查找子串位置
来源：http://gz.hnjuh.cn

Py:   s.find("x");  s.index("x")
来源：http://lq.wgjwhj.cn

PHP:  strpos($s, "x");
来源：http://sb.shtwfgs.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mg.haigaiapp.cn

TS:   s.indexOf("x")
来源：http://tf.lnxyls.cn

Java: s.indexOf("x")
来源：http://oi.wgjwhj.cn

Go:   strings.Index(s, "x")
来源：http://vn.yuexingan06.cn

Ruby: s.index("x")
来源：http://ao.szsharing.cn

C#:   s.IndexOf("x")
来源：http://hp.huixinmuqiang.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://jf.yuexingan06.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://sm.nszjky.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qg.shxzskj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://us.szxytkj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://we.huanxung.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lb.9csxet.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xy.yuntaijiaju.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cs.huanxung.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://km.hahajie.cn

[E06] 替换子串
来源：http://ul.bjjhwx.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://eo.muxihuayi.cn

PHP:  str_replace("a", "b", $s);
来源：http://or.shxzukj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ix.gzmigu.cn

TS:   s.replaceAll("a", "b")
来源：http://jn.huixiangedu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lf.nicolike.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bp.szxytkj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ey.gzmigu.cn

C#:   s.Replace("a", "b")
来源：http://zr.panjiajie.cn

[E07] 按分隔符拆分
来源：http://mo.yuexingan06.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xc.hahajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ym.521024.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://hw.huanxung.cn

TS:   s.split(",")
来源：http://jd.yuntaijiaju.cn

Java: s.split(",");  s.split("\\s+")
来源：http://mm.haigaiapp.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rt.huanxung.cn

Ruby: s.split(",");  s.split
来源：http://tv.9csxet.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sg.bjjhwx.cn

[E08] 数组按分隔符合并
来源：http://cd.szxytkj.cn

Py:   ",".join(items)
来源：http://sc.szsharing.cn

PHP:  implode(",", $items);
来源：http://go.521024.cn

JS:   items.join(",")
来源：http://bj.huixiangedu.cn

TS:   items.join(",")
来源：http://vw.bookmarksfly.cn

Java: String.join(",", items)
来源：http://xr.jianghongdianzi.cn

Go:   strings.Join(items, ",")
来源：http://hx.lnxyls.cn

Ruby: items.join(",")
来源：http://vl.9csxet.cn

C#:   string.Join(",", items)
来源：http://ny.muxihuayi.cn

[E09] 去除所有空白字符
来源：http://kw.bjjhwx.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://uo.colortex.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://my.jianghongdianzi.cn

JS:   s.replace(/\s+/g, "")
来源：http://xd.huanxung.cn

TS:   s.replace(/\s+/g, "")
来源：http://sx.521024.cn

Java: s.replaceAll("\\s+", "")
来源：http://iu.asd995.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://gv.yuexingan06.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qk.jctech888.com.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qa.shxzukj.cn

[E10] 左侧补零 / 定长填充
来源：http://qf.wgjwhj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://or.jctech888.com.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qp.lnxyls.cn

JS:   "7".padStart(3, "0")
来源：http://ik.newstarts.cn

TS:   "7".padStart(3, "0")
来源：http://jc.shtwfgs.cn

Java: String.format("%03d", 7)
来源：http://qh.yuntaijiaju.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://av.nszjky.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mq.wgjwhj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lz.colortex.cn

[E11] 反转字符串
来源：http://dw.shxzskj.cn

Py:   s[::-1]
来源：http://uh.haigaiapp.cn

PHP:  strrev($s);
来源：http://la.shtwfgs.cn

JS:   [...s].reverse().join("")
来源：http://mr.shxzukj.cn

TS:   [...s].reverse().join("")
来源：http://xq.szxytkj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ov.shxzskj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://jb.hahajie.cn

Ruby: s.reverse
来源：http://ui.yuntaijiaju.cn

C#:   new string(s.Reverse().ToArray())
来源：http://xu.jctech888.com.cn

[E12] 统计某字符出现次数
来源：http://wr.nszjky.cn

Py:   s.count("a")
来源：http://hv.shxzskj.cn

PHP:  substr_count($s, "a");
来源：http://jq.9csxet.cn

JS:   s.split("a").length - 1
来源：http://kk.szxytkj.cn

TS:   s.split("a").length - 1
来源：http://ok.colortex.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vf.jctech888.com.cn

Go:   strings.Count(s, "a")
来源：http://gy.colortex.cn

Ruby: s.count("a")
来源：http://nh.huixinmuqiang.cn

C#:   s.Count(c => c == 'a')
来源：http://cu.yuntaijiaju.cn

[E13] 逐字符遍历
来源：http://ky.muxihuayi.cn

Py:   for ch in s: print(ch)
来源：http://un.shtwfgs.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ic.jctech888.com.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://iq.shxzskj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://zz.asd995.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wa.chemitech.net.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ao.lnxyls.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ki.bjjhwx.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yy.shtwfgs.cn

[E14] URL 编码与 Base64
来源：http://vf.colortex.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zu.nicolike.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://vl.jctech888.com.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rb.haigaiapp.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://za.jianghongdianzi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ow.9csxet.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ec.huanxung.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kf.wgjwhj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sq.nszjky.cn

[E15] HTML 转义 / 反转义
来源：http://gb.shxzskj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ts.huixiangedu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hr.yuntaijiaju.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jj.nicolike.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://si.shxzukj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ly.chemitech.net.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://oi.jianghongdianzi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xl.szsharing.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ps.hahajie.cn

[E16] 数字千分位
来源：http://zl.nszjky.cn

Py:   f"{1234567:,}"
来源：http://db.nszjky.cn

PHP:  number_format(1234567);
来源：http://og.nicolike.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://nn.nszjky.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ir.bjjhwx.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vo.haigaiapp.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://oy.muxihuayi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mf.panjiajie.cn

C#:   1234567.ToString("N0")
来源：http://hh.shxzukj.cn

[E17] 首字母大写
来源：http://ig.yuntaijiaju.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rk.jctech888.com.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://fa.panjiajie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mv.haigaiapp.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://no.newstarts.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hj.wgjwhj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://oi.gzmigu.cn

Ruby: s.capitalize
来源：http://ye.haigaiapp.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jc.haigaiapp.cn

[E18] 模板占位符替换
来源：http://vs.huixiangedu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sv.hnjuh.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ip.muxihuayi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://bd.shxzskj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ns.huanxung.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nz.bookmarksfly.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vz.9csxet.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kq.colortex.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://im.szxytkj.cn

[E19] 多行文本按行拆分
来源：http://zn.wgjwhj.cn

Py:   s.splitlines()
来源：http://zy.haigaiapp.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ac.shxzukj.cn

JS:   s.split(/\r?\n/)
来源：http://ot.wgjwhj.cn

TS:   s.split(/\r?\n/)
来源：http://jt.lnxyls.cn

Java: s.lines().toList()
来源：http://dv.nszjky.cn

Go:   strings.Split(s, "\n")
来源：http://mq.szsharing.cn

Ruby: s.lines
来源：http://hk.521024.cn

C#:   s.Split('\n')
来源：http://gm.szxytkj.cn

[E20] 判断字符串是否为空
来源：http://ve.huixiangedu.cn

Py:   if not s:
来源：http://yi.colortex.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rp.muxihuayi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jq.shtwfgs.cn

TS:   if (s === "") {}
来源：http://vc.yuntaijiaju.cn

Java: if (s.isEmpty()) {}
来源：http://gw.gzmigu.cn

Go:   if s == "" {}
来源：http://na.9csxet.cn

Ruby: if s.empty?
来源：http://vj.bookmarksfly.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fw.nszjky.cn

[E21] 超长截断加省略号
来源：http://si.huixinmuqiang.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ii.nszjky.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yl.521024.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yt.huanxung.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rb.hnjuh.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ze.gzmigu.cn

Go:   // 按 rune 判断长度后截断
来源：http://fn.huixiangedu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lg.newstarts.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jx.asd995.cn

[E22] 字节长度与字符长度
来源：http://zo.huixiangedu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dk.gzmigu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rv.wgjwhj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://or.nszjky.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jd.yuexingan06.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yl.panjiajie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://im.panjiajie.cn

Ruby: s.bytesize;  s.length
来源：http://si.lnxyls.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lo.lnxyls.cn

================================================================================
来源：http://gi.huanxung.cn

F. 文件与目录
来源：http://ai.nicolike.cn

================================================================================
来源：http://fv.hnjuh.cn

[F01] 读取整个文件
来源：http://ny.bookmarksfly.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ii.jianghongdianzi.cn

PHP:  file_get_contents("a.txt");
来源：http://bb.jianghongdianzi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ph.colortex.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bo.huixiangedu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://uw.yuntaijiaju.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tj.shxzskj.cn

Ruby: File.read("a.txt")
来源：http://yz.lnxyls.cn

C#:   File.ReadAllText("a.txt");
来源：http://vj.bjjhwx.cn

[F02] 逐行读取文件
来源：http://mk.shxzskj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://si.haigaiapp.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cg.asd995.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sj.szxytkj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://am.colortex.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ak.gzmigu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gt.jianghongdianzi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zh.hahajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hr.muxihuayi.cn

[F03] 写入文件（覆盖）
来源：http://hh.shxzukj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bx.hnjuh.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://if.yuntaijiaju.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mj.huixiangedu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ss.jctech888.com.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qd.9csxet.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lc.521024.cn

Ruby: File.write("a.txt", "hi")
来源：http://dr.bookmarksfly.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://al.9csxet.cn

[F04] 追加写入文件
来源：http://tm.jctech888.com.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ot.huixiangedu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vv.nszjky.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://if.9csxet.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://re.bjjhwx.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://be.shxzukj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yl.haigaiapp.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bf.wgjwhj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nz.chemitech.net.cn

[F05] 判断文件或目录是否存在
来源：http://jj.colortex.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xj.huixinmuqiang.cn

PHP:  file_exists("a.txt");
来源：http://hg.hnjuh.cn

JS:   fs.existsSync("a.txt")
来源：http://hf.lnxyls.cn

TS:   fs.existsSync("a.txt")
来源：http://nm.colortex.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://il.yuexingan06.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://et.9csxet.cn

Ruby: File.exist?("a.txt")
来源：http://wa.asd995.cn

C#:   File.Exists("a.txt")
来源：http://av.9csxet.cn

[F06] 删除文件
来源：http://xo.gzmigu.cn

Py:   os.remove("a.txt")
来源：http://iq.9csxet.cn

PHP:  unlink("a.txt");
来源：http://vv.shxzukj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://hm.yuexingan06.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ir.bjjhwx.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://os.hnjuh.cn

Go:   os.Remove("a.txt")
来源：http://de.shtwfgs.cn

Ruby: File.delete("a.txt")
来源：http://it.bookmarksfly.cn

C#:   File.Delete("a.txt");
来源：http://fs.panjiajie.cn

[F07] 创建目录（含多级）
来源：http://cn.szxytkj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zg.bjjhwx.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ux.yuexingan06.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ce.yuexingan06.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kp.shxzskj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kn.lnxyls.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://om.bookmarksfly.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xg.huixinmuqiang.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://va.jianghongdianzi.cn

[F08] 遍历目录
来源：http://ki.asd995.cn


<!-- 参考信息 -->