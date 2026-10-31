代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pi.szsharing.cn

[D24] 字典 / Map 基本操作
来源：http://bz.chemitech.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jz.szxytkj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ny.nszjky.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://is.nicolike.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cg.huixinmuqiang.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pv.gzmigu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://un.muxihuayi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bo.nicolike.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zs.shxzskj.cn

[D25] Set 集合去重与交并差
来源：http://uy.szxytkj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nk.yuexingan06.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://po.521024.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tv.jctech888.com.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fa.jianghongdianzi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ey.jianghongdianzi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ti.chemitech.net.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://he.521024.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ge.521024.cn

[D26] 数组转字符串
来源：http://ml.shxzskj.cn

Py:   ", ".join(map(str, arr))
来源：http://im.hnjuh.cn

PHP:  implode(", ", $arr);
来源：http://jc.bookmarksfly.cn

JS:   arr.join(", ")
来源：http://tz.colortex.cn

TS:   arr.join(", ")
来源：http://sr.chemitech.net.cn

Java: String.join(", ", list)
来源：http://ll.muxihuayi.cn

Go:   strings.Join(strs, ", ")
来源：http://rk.asd995.cn

Ruby: arr.join(", ")
来源：http://oj.hahajie.cn

C#:   string.Join(", ", list)
来源：http://xw.jianghongdianzi.cn

================================================================================
来源：http://pe.muxihuayi.cn

E. 字符串处理
来源：http://qa.hnjuh.cn

================================================================================
来源：http://we.yuntaijiaju.cn

[E01] 拼接字符串
来源：http://bi.szsharing.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lo.wgjwhj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yt.wgjwhj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vi.hnjuh.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ug.shxzskj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sc.szsharing.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://di.panjiajie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yb.bjjhwx.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fq.hnjuh.cn

[E02] 重复字符串
来源：http://mm.nicolike.cn

Py:   "ab" * 3
来源：http://hp.9csxet.cn

PHP:  str_repeat("ab", 3);
来源：http://qr.wgjwhj.cn

JS:   "ab".repeat(3)
来源：http://pc.asd995.cn

TS:   "ab".repeat(3)
来源：http://nk.muxihuayi.cn

Java: "ab".repeat(3)
来源：http://ks.shxzskj.cn

Go:   strings.Repeat("ab", 3)
来源：http://nu.bookmarksfly.cn

Ruby: "ab" * 3
来源：http://sg.lnxyls.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gv.huixiangedu.cn

[E03] 截取子串
来源：http://az.panjiajie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hg.shxzukj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hd.haigaiapp.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://it.nicolike.cn

TS:   s.slice(1, 4)
来源：http://ja.shxzukj.cn

Java: s.substring(1, 4)
来源：http://yf.huixiangedu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wm.colortex.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zx.jianghongdianzi.cn

C#:   s.Substring(1, 3)
来源：http://um.nszjky.cn

[E04] 查找子串位置
来源：http://az.newstarts.cn

Py:   s.find("x");  s.index("x")
来源：http://qj.gzmigu.cn

PHP:  strpos($s, "x");
来源：http://eo.jctech888.com.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zi.szxytkj.cn

TS:   s.indexOf("x")
来源：http://ko.szxytkj.cn

Java: s.indexOf("x")
来源：http://tt.colortex.cn

Go:   strings.Index(s, "x")
来源：http://sc.yuexingan06.cn

Ruby: s.index("x")
来源：http://ra.chemitech.net.cn

C#:   s.IndexOf("x")
来源：http://bd.newstarts.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ks.huanxung.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mq.huixiangedu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://om.newstarts.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yi.muxihuayi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qb.huixinmuqiang.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fn.yuexingan06.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rn.nicolike.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://uo.huixinmuqiang.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jy.wgjwhj.cn

[E06] 替换子串
来源：http://jd.hahajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://oj.huixiangedu.cn

PHP:  str_replace("a", "b", $s);
来源：http://bm.asd995.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nk.newstarts.cn

TS:   s.replaceAll("a", "b")
来源：http://pm.bjjhwx.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ck.lnxyls.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kz.muxihuayi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ws.chemitech.net.cn

C#:   s.Replace("a", "b")
来源：http://vy.bjjhwx.cn

[E07] 按分隔符拆分
来源：http://va.jctech888.com.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vo.szxytkj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wj.huanxung.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://pl.huanxung.cn

TS:   s.split(",")
来源：http://ut.huixiangedu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xy.huanxung.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fo.haigaiapp.cn

Ruby: s.split(",");  s.split
来源：http://vz.newstarts.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nv.gzmigu.cn

[E08] 数组按分隔符合并
来源：http://mt.huixinmuqiang.cn

Py:   ",".join(items)
来源：http://pb.shxzukj.cn

PHP:  implode(",", $items);
来源：http://dx.szxytkj.cn

JS:   items.join(",")
来源：http://ct.newstarts.cn

TS:   items.join(",")
来源：http://hn.jianghongdianzi.cn

Java: String.join(",", items)
来源：http://lo.chemitech.net.cn

Go:   strings.Join(items, ",")
来源：http://yx.yuexingan06.cn

Ruby: items.join(",")
来源：http://jn.521024.cn

C#:   string.Join(",", items)
来源：http://jk.huixinmuqiang.cn

[E09] 去除所有空白字符
来源：http://di.yuexingan06.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pf.yuntaijiaju.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://np.bjjhwx.cn

JS:   s.replace(/\s+/g, "")
来源：http://yk.shtwfgs.cn

TS:   s.replace(/\s+/g, "")
来源：http://yz.9csxet.cn

Java: s.replaceAll("\\s+", "")
来源：http://ey.hnjuh.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://fr.shxzskj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://vs.lnxyls.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yj.huanxung.cn

[E10] 左侧补零 / 定长填充
来源：http://cj.huixiangedu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vq.chemitech.net.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://uv.muxihuayi.cn

JS:   "7".padStart(3, "0")
来源：http://ej.hahajie.cn

TS:   "7".padStart(3, "0")
来源：http://rt.9csxet.cn

Java: String.format("%03d", 7)
来源：http://im.jianghongdianzi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://hx.huixinmuqiang.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ap.huixinmuqiang.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ul.asd995.cn

[E11] 反转字符串
来源：http://sf.chemitech.net.cn

Py:   s[::-1]
来源：http://zk.colortex.cn

PHP:  strrev($s);
来源：http://wi.nszjky.cn

JS:   [...s].reverse().join("")
来源：http://gm.huixiangedu.cn

TS:   [...s].reverse().join("")
来源：http://oa.jianghongdianzi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ox.panjiajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://sr.yuntaijiaju.cn

Ruby: s.reverse
来源：http://jl.9csxet.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ke.wgjwhj.cn

[E12] 统计某字符出现次数
来源：http://kq.huixiangedu.cn

Py:   s.count("a")
来源：http://tw.huixiangedu.cn

PHP:  substr_count($s, "a");
来源：http://yz.jianghongdianzi.cn

JS:   s.split("a").length - 1
来源：http://xf.lnxyls.cn

TS:   s.split("a").length - 1
来源：http://xn.521024.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://sr.chemitech.net.cn

Go:   strings.Count(s, "a")
来源：http://qe.colortex.cn

Ruby: s.count("a")
来源：http://ov.huixinmuqiang.cn

C#:   s.Count(c => c == 'a')
来源：http://tr.szsharing.cn

[E13] 逐字符遍历
来源：http://jf.szsharing.cn

Py:   for ch in s: print(ch)
来源：http://hd.lnxyls.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mv.muxihuayi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://uw.9csxet.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://zb.shxzukj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rl.521024.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pl.yuexingan06.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://uw.hnjuh.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://sk.colortex.cn

[E14] URL 编码与 Base64
来源：http://ku.colortex.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hq.shxzskj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://rl.hnjuh.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cw.szsharing.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hc.bookmarksfly.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ea.hahajie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qb.newstarts.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://sn.jctech888.com.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mq.huixinmuqiang.cn

[E15] HTML 转义 / 反转义
来源：http://qj.gzmigu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ir.panjiajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fl.huanxung.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rv.nszjky.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://jy.hahajie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xg.newstarts.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bn.huixiangedu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dg.hnjuh.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ga.szsharing.cn

[E16] 数字千分位
来源：http://vx.shxzukj.cn

Py:   f"{1234567:,}"
来源：http://eg.521024.cn

PHP:  number_format(1234567);
来源：http://zr.huanxung.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vq.yuntaijiaju.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ki.panjiajie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gd.bjjhwx.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hq.szsharing.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fz.shxzukj.cn

C#:   1234567.ToString("N0")
来源：http://bm.9csxet.cn

[E17] 首字母大写
来源：http://au.muxihuayi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xw.asd995.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://md.newstarts.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xt.gzmigu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ad.szxytkj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dy.9csxet.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://aa.hahajie.cn

Ruby: s.capitalize
来源：http://jw.szsharing.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hg.newstarts.cn

[E18] 模板占位符替换
来源：http://en.yuntaijiaju.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cl.jianghongdianzi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yf.huixinmuqiang.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://rs.newstarts.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://yn.shxzskj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qz.jianghongdianzi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ct.muxihuayi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://sx.panjiajie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bq.wgjwhj.cn

[E19] 多行文本按行拆分
来源：http://rv.szsharing.cn

Py:   s.splitlines()
来源：http://my.haigaiapp.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://za.hahajie.cn

JS:   s.split(/\r?\n/)
来源：http://ly.jianghongdianzi.cn

TS:   s.split(/\r?\n/)
来源：http://ok.shxzukj.cn

Java: s.lines().toList()
来源：http://pe.huanxung.cn

Go:   strings.Split(s, "\n")
来源：http://hx.lnxyls.cn

Ruby: s.lines
来源：http://wf.bookmarksfly.cn

C#:   s.Split('\n')
来源：http://vq.huixiangedu.cn

[E20] 判断字符串是否为空
来源：http://td.lnxyls.cn

Py:   if not s:
来源：http://ng.hnjuh.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nc.chemitech.net.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ja.nszjky.cn

TS:   if (s === "") {}
来源：http://xi.hahajie.cn

Java: if (s.isEmpty()) {}
来源：http://og.huixiangedu.cn

Go:   if s == "" {}
来源：http://ay.521024.cn

Ruby: if s.empty?
来源：http://xl.bjjhwx.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yy.huixiangedu.cn

[E21] 超长截断加省略号
来源：http://if.muxihuayi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qd.bookmarksfly.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dt.521024.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ya.newstarts.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kd.jctech888.com.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mn.9csxet.cn

Go:   // 按 rune 判断长度后截断
来源：http://ey.gzmigu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kh.szxytkj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ug.jianghongdianzi.cn

[E22] 字节长度与字符长度
来源：http://vt.hahajie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fj.shxzukj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://eb.muxihuayi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xl.jianghongdianzi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cs.szsharing.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yc.hnjuh.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tc.9csxet.cn

Ruby: s.bytesize;  s.length
来源：http://nb.lnxyls.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://iz.chemitech.net.cn

================================================================================
来源：http://dr.nszjky.cn

F. 文件与目录
来源：http://rt.jianghongdianzi.cn

================================================================================
来源：http://dw.huixiangedu.cn

[F01] 读取整个文件
来源：http://uw.huanxung.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xb.muxihuayi.cn

PHP:  file_get_contents("a.txt");
来源：http://vp.nicolike.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xn.shxzukj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wq.szxytkj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://by.newstarts.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jj.hahajie.cn

Ruby: File.read("a.txt")
来源：http://kj.colortex.cn

C#:   File.ReadAllText("a.txt");
来源：http://tv.gzmigu.cn

[F02] 逐行读取文件
来源：http://af.nszjky.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://da.bjjhwx.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gb.huixinmuqiang.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fh.yuntaijiaju.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nc.jctech888.com.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rp.huanxung.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vz.521024.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yj.newstarts.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rh.lnxyls.cn

[F03] 写入文件（覆盖）
来源：http://vh.huixinmuqiang.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sl.hahajie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ao.hnjuh.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lk.szxytkj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zu.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rd.yuntaijiaju.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bz.lnxyls.cn

Ruby: File.write("a.txt", "hi")
来源：http://ca.colortex.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://md.huanxung.cn

[F04] 追加写入文件
来源：http://ly.hahajie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zy.nicolike.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ad.nszjky.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hs.szxytkj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rk.jianghongdianzi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bj.521024.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ha.shtwfgs.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wu.newstarts.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fq.nicolike.cn

[F05] 判断文件或目录是否存在
来源：http://cs.gzmigu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kg.huixinmuqiang.cn

PHP:  file_exists("a.txt");
来源：http://yo.shxzskj.cn

JS:   fs.existsSync("a.txt")
来源：http://bf.colortex.cn

TS:   fs.existsSync("a.txt")
来源：http://ya.hnjuh.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://tv.nicolike.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wl.huanxung.cn

Ruby: File.exist?("a.txt")
来源：http://hz.bjjhwx.cn

C#:   File.Exists("a.txt")
来源：http://gl.haigaiapp.cn

[F06] 删除文件
来源：http://nz.yuexingan06.cn

Py:   os.remove("a.txt")
来源：http://gh.panjiajie.cn

PHP:  unlink("a.txt");
来源：http://dx.huixinmuqiang.cn

JS:   fs.unlinkSync("a.txt")
来源：http://iq.hahajie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://nx.jianghongdianzi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://du.huixiangedu.cn

Go:   os.Remove("a.txt")
来源：http://bt.huixiangedu.cn

Ruby: File.delete("a.txt")
来源：http://co.jianghongdianzi.cn

C#:   File.Delete("a.txt");
来源：http://zd.huanxung.cn

[F07] 创建目录（含多级）
来源：http://eb.lnxyls.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kd.shxzskj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bf.yuntaijiaju.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ei.hahajie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ee.bookmarksfly.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://et.panjiajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jd.hahajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://oe.shxzskj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ra.huixiangedu.cn

[F08] 遍历目录
来源：http://nc.521024.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://yy.haigaiapp.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://oo.jctech888.com.cn

JS:   fs.readdirSync("dir")
来源：http://jh.shtwfgs.cn

TS:   fs.readdirSync("dir")
来源：http://ok.wgjwhj.cn


<!-- 参考信息 -->