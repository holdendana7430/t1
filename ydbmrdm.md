代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hx.hnjuh.cn

[D24] 字典 / Map 基本操作
来源：http://wt.huixiangedu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gk.newstarts.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nl.panjiajie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vz.gzmigu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pf.newstarts.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bd.shxzukj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hx.wgjwhj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tv.yuexingan06.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vb.shtwfgs.cn

[D25] Set 集合去重与交并差
来源：http://ty.huanxung.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mx.9csxet.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xu.szsharing.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zf.huixinmuqiang.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://oh.wgjwhj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://va.colortex.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://di.colortex.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tn.szxytkj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ie.hahajie.cn

[D26] 数组转字符串
来源：http://fs.gzmigu.cn

Py:   ", ".join(map(str, arr))
来源：http://is.chemitech.net.cn

PHP:  implode(", ", $arr);
来源：http://xg.szxytkj.cn

JS:   arr.join(", ")
来源：http://au.yuntaijiaju.cn

TS:   arr.join(", ")
来源：http://yz.asd995.cn

Java: String.join(", ", list)
来源：http://dn.521024.cn

Go:   strings.Join(strs, ", ")
来源：http://aw.jianghongdianzi.cn

Ruby: arr.join(", ")
来源：http://ea.muxihuayi.cn

C#:   string.Join(", ", list)
来源：http://yi.chemitech.net.cn

================================================================================
来源：http://wd.gzmigu.cn

E. 字符串处理
来源：http://bx.521024.cn

================================================================================
来源：http://dy.shtwfgs.cn

[E01] 拼接字符串
来源：http://dz.shtwfgs.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ea.nszjky.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xx.yuntaijiaju.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fk.yuntaijiaju.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sj.jctech888.com.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pl.chemitech.net.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gf.panjiajie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sz.panjiajie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://om.colortex.cn

[E02] 重复字符串
来源：http://zq.bjjhwx.cn

Py:   "ab" * 3
来源：http://ui.nszjky.cn

PHP:  str_repeat("ab", 3);
来源：http://yn.shxzskj.cn

JS:   "ab".repeat(3)
来源：http://ta.szsharing.cn

TS:   "ab".repeat(3)
来源：http://vf.szsharing.cn

Java: "ab".repeat(3)
来源：http://tc.521024.cn

Go:   strings.Repeat("ab", 3)
来源：http://tr.hahajie.cn

Ruby: "ab" * 3
来源：http://nd.shtwfgs.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://aj.huixinmuqiang.cn

[E03] 截取子串
来源：http://vt.jctech888.com.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qa.9csxet.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://il.nszjky.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yd.yuexingan06.cn

TS:   s.slice(1, 4)
来源：http://uy.9csxet.cn

Java: s.substring(1, 4)
来源：http://le.muxihuayi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zf.panjiajie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ep.huixiangedu.cn

C#:   s.Substring(1, 3)
来源：http://kr.szxytkj.cn

[E04] 查找子串位置
来源：http://rq.9csxet.cn

Py:   s.find("x");  s.index("x")
来源：http://eg.chemitech.net.cn

PHP:  strpos($s, "x");
来源：http://nz.wgjwhj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ju.chemitech.net.cn

TS:   s.indexOf("x")
来源：http://vm.szxytkj.cn

Java: s.indexOf("x")
来源：http://eo.asd995.cn

Go:   strings.Index(s, "x")
来源：http://hw.szxytkj.cn

Ruby: s.index("x")
来源：http://hl.nszjky.cn

C#:   s.IndexOf("x")
来源：http://ms.szxytkj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://of.szxytkj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xp.yuexingan06.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ic.hahajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ty.wgjwhj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ci.huanxung.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ij.panjiajie.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dv.bookmarksfly.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pk.yuexingan06.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xs.wgjwhj.cn

[E06] 替换子串
来源：http://xm.shxzukj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ns.yuntaijiaju.cn

PHP:  str_replace("a", "b", $s);
来源：http://ji.huixinmuqiang.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jh.shxzskj.cn

TS:   s.replaceAll("a", "b")
来源：http://wd.newstarts.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wj.nszjky.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ce.wgjwhj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yx.colortex.cn

C#:   s.Replace("a", "b")
来源：http://wy.nszjky.cn

[E07] 按分隔符拆分
来源：http://vf.shxzskj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hs.shxzukj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xy.huanxung.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://yr.yuexingan06.cn

TS:   s.split(",")
来源：http://mm.521024.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ho.nszjky.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://av.yuexingan06.cn

Ruby: s.split(",");  s.split
来源：http://ms.jctech888.com.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tu.yuntaijiaju.cn

[E08] 数组按分隔符合并
来源：http://qy.521024.cn

Py:   ",".join(items)
来源：http://mg.huanxung.cn

PHP:  implode(",", $items);
来源：http://uk.jctech888.com.cn

JS:   items.join(",")
来源：http://rc.wgjwhj.cn

TS:   items.join(",")
来源：http://sy.colortex.cn

Java: String.join(",", items)
来源：http://cb.lnxyls.cn

Go:   strings.Join(items, ",")
来源：http://ms.nszjky.cn

Ruby: items.join(",")
来源：http://ci.jctech888.com.cn

C#:   string.Join(",", items)
来源：http://os.yuntaijiaju.cn

[E09] 去除所有空白字符
来源：http://wq.muxihuayi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qr.jianghongdianzi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lr.jctech888.com.cn

JS:   s.replace(/\s+/g, "")
来源：http://sm.chemitech.net.cn

TS:   s.replace(/\s+/g, "")
来源：http://pn.huixiangedu.cn

Java: s.replaceAll("\\s+", "")
来源：http://da.gzmigu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://rc.shxzukj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://oj.szxytkj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://op.521024.cn

[E10] 左侧补零 / 定长填充
来源：http://kd.yuntaijiaju.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dy.jianghongdianzi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wn.lnxyls.cn

JS:   "7".padStart(3, "0")
来源：http://jp.huixiangedu.cn

TS:   "7".padStart(3, "0")
来源：http://ex.szsharing.cn

Java: String.format("%03d", 7)
来源：http://vt.shtwfgs.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ge.shtwfgs.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fn.chemitech.net.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vq.gzmigu.cn

[E11] 反转字符串
来源：http://cj.hnjuh.cn

Py:   s[::-1]
来源：http://sn.bjjhwx.cn

PHP:  strrev($s);
来源：http://cz.jctech888.com.cn

JS:   [...s].reverse().join("")
来源：http://cz.szsharing.cn

TS:   [...s].reverse().join("")
来源：http://gg.colortex.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://od.9csxet.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ev.huanxung.cn

Ruby: s.reverse
来源：http://bz.yuntaijiaju.cn

C#:   new string(s.Reverse().ToArray())
来源：http://df.jctech888.com.cn

[E12] 统计某字符出现次数
来源：http://wy.9csxet.cn

Py:   s.count("a")
来源：http://nn.shxzskj.cn

PHP:  substr_count($s, "a");
来源：http://er.wgjwhj.cn

JS:   s.split("a").length - 1
来源：http://zd.muxihuayi.cn

TS:   s.split("a").length - 1
来源：http://xr.9csxet.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xt.colortex.cn

Go:   strings.Count(s, "a")
来源：http://bj.colortex.cn

Ruby: s.count("a")
来源：http://vp.huanxung.cn

C#:   s.Count(c => c == 'a')
来源：http://wb.haigaiapp.cn

[E13] 逐字符遍历
来源：http://eq.yuntaijiaju.cn

Py:   for ch in s: print(ch)
来源：http://ya.huixiangedu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hc.nszjky.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://jn.9csxet.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://la.chemitech.net.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ce.szxytkj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fc.muxihuayi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ab.yuntaijiaju.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zo.jctech888.com.cn

[E14] URL 编码与 Base64
来源：http://zx.bjjhwx.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ab.huixiangedu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ox.nszjky.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ya.szxytkj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gt.wgjwhj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ty.bjjhwx.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gv.haigaiapp.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ki.lnxyls.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yz.nszjky.cn

[E15] HTML 转义 / 反转义
来源：http://qt.hnjuh.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://nf.lnxyls.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vm.bookmarksfly.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://on.jianghongdianzi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://at.lnxyls.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://uw.jianghongdianzi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vj.bjjhwx.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wy.shtwfgs.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ao.wgjwhj.cn

[E16] 数字千分位
来源：http://us.colortex.cn

Py:   f"{1234567:,}"
来源：http://wm.9csxet.cn

PHP:  number_format(1234567);
来源：http://cu.asd995.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://wm.newstarts.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zf.asd995.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://im.shxzskj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gt.szsharing.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://yx.yuexingan06.cn

C#:   1234567.ToString("N0")
来源：http://ed.gzmigu.cn

[E17] 首字母大写
来源：http://ap.huanxung.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rz.asd995.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://vl.nszjky.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lo.wgjwhj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yf.yuntaijiaju.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gn.bjjhwx.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ov.szsharing.cn

Ruby: s.capitalize
来源：http://ax.huixinmuqiang.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fd.gzmigu.cn

[E18] 模板占位符替换
来源：http://kc.yuexingan06.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sx.bookmarksfly.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ql.haigaiapp.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://fd.asd995.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://aj.huixiangedu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nd.wgjwhj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hg.asd995.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://js.huixiangedu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yj.jctech888.com.cn

[E19] 多行文本按行拆分
来源：http://bc.521024.cn

Py:   s.splitlines()
来源：http://zd.wgjwhj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ov.shxzskj.cn

JS:   s.split(/\r?\n/)
来源：http://jp.panjiajie.cn

TS:   s.split(/\r?\n/)
来源：http://gk.nszjky.cn

Java: s.lines().toList()
来源：http://uf.huanxung.cn

Go:   strings.Split(s, "\n")
来源：http://ex.gzmigu.cn

Ruby: s.lines
来源：http://fb.hnjuh.cn

C#:   s.Split('\n')
来源：http://aw.muxihuayi.cn

[E20] 判断字符串是否为空
来源：http://lz.jianghongdianzi.cn

Py:   if not s:
来源：http://xc.panjiajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ty.muxihuayi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lz.shxzskj.cn

TS:   if (s === "") {}
来源：http://oj.jianghongdianzi.cn

Java: if (s.isEmpty()) {}
来源：http://me.wgjwhj.cn

Go:   if s == "" {}
来源：http://vt.jianghongdianzi.cn

Ruby: if s.empty?
来源：http://of.shtwfgs.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nm.nszjky.cn

[E21] 超长截断加省略号
来源：http://fp.muxihuayi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wq.chemitech.net.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kj.szsharing.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://at.9csxet.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vn.yuntaijiaju.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tk.szxytkj.cn

Go:   // 按 rune 判断长度后截断
来源：http://bz.shxzukj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zz.panjiajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ck.szxytkj.cn

[E22] 字节长度与字符长度
来源：http://kc.muxihuayi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://iq.huanxung.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fr.nicolike.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jf.szsharing.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ud.haigaiapp.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cb.jctech888.com.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cq.huixiangedu.cn

Ruby: s.bytesize;  s.length
来源：http://yo.hnjuh.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ng.nszjky.cn

================================================================================
来源：http://rn.shtwfgs.cn

F. 文件与目录
来源：http://te.jianghongdianzi.cn

================================================================================
来源：http://xq.szxytkj.cn

[F01] 读取整个文件
来源：http://cp.yuntaijiaju.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ja.jctech888.com.cn

PHP:  file_get_contents("a.txt");
来源：http://md.jctech888.com.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ub.huixiangedu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ii.hnjuh.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://oa.szsharing.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wr.521024.cn

Ruby: File.read("a.txt")
来源：http://kc.newstarts.cn

C#:   File.ReadAllText("a.txt");
来源：http://zf.haigaiapp.cn

[F02] 逐行读取文件
来源：http://ka.wgjwhj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ku.yuntaijiaju.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fh.9csxet.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xg.szxytkj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kg.muxihuayi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ha.nszjky.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xs.huanxung.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://je.gzmigu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zq.chemitech.net.cn

[F03] 写入文件（覆盖）
来源：http://du.chemitech.net.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://iv.haigaiapp.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://zx.hahajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ki.521024.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nn.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ss.yuntaijiaju.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gw.jctech888.com.cn

Ruby: File.write("a.txt", "hi")
来源：http://tb.wgjwhj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://db.shxzskj.cn

[F04] 追加写入文件
来源：http://qr.9csxet.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rb.hahajie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ap.9csxet.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://db.szsharing.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wa.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ln.panjiajie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nf.bookmarksfly.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nw.newstarts.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ma.shtwfgs.cn

[F05] 判断文件或目录是否存在
来源：http://uw.huixinmuqiang.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gq.huanxung.cn

PHP:  file_exists("a.txt");
来源：http://fm.lnxyls.cn

JS:   fs.existsSync("a.txt")
来源：http://ju.jianghongdianzi.cn

TS:   fs.existsSync("a.txt")
来源：http://ob.wgjwhj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xd.colortex.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yp.bookmarksfly.cn

Ruby: File.exist?("a.txt")
来源：http://uo.szsharing.cn

C#:   File.Exists("a.txt")
来源：http://qw.hnjuh.cn

[F06] 删除文件
来源：http://sb.bookmarksfly.cn

Py:   os.remove("a.txt")
来源：http://wj.hahajie.cn

PHP:  unlink("a.txt");
来源：http://dz.wgjwhj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://xh.shxzskj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://tu.nicolike.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cd.hahajie.cn

Go:   os.Remove("a.txt")
来源：http://fm.bookmarksfly.cn

Ruby: File.delete("a.txt")
来源：http://be.asd995.cn

C#:   File.Delete("a.txt");
来源：http://vu.bjjhwx.cn

[F07] 创建目录（含多级）
来源：http://ev.jctech888.com.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://da.lnxyls.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bh.szsharing.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ic.shxzskj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ye.hnjuh.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hc.colortex.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mt.haigaiapp.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://op.shtwfgs.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://yu.shxzukj.cn

[F08] 遍历目录
来源：http://fh.hahajie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xw.asd995.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fq.bjjhwx.cn

JS:   fs.readdirSync("dir")
来源：http://is.gzmigu.cn

TS:   fs.readdirSync("dir")
来源：http://ed.colortex.cn


<!-- 参考信息 -->