代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ts.shxzskj.cn

[D24] 字典 / Map 基本操作
来源：http://bw.shxzskj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nm.yuntaijiaju.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gq.yuntaijiaju.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://if.nicolike.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://iq.huixiangedu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hy.shxzukj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ac.gzmigu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xo.shxzukj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zt.9csxet.cn

[D25] Set 集合去重与交并差
来源：http://sm.bookmarksfly.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gq.nszjky.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cd.hnjuh.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cp.nszjky.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ew.newstarts.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://yy.szxytkj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://eu.haigaiapp.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://iz.chemitech.net.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://iz.shxzukj.cn

[D26] 数组转字符串
来源：http://lx.muxihuayi.cn

Py:   ", ".join(map(str, arr))
来源：http://qr.521024.cn

PHP:  implode(", ", $arr);
来源：http://ql.newstarts.cn

JS:   arr.join(", ")
来源：http://sa.jianghongdianzi.cn

TS:   arr.join(", ")
来源：http://uj.jianghongdianzi.cn

Java: String.join(", ", list)
来源：http://fw.panjiajie.cn

Go:   strings.Join(strs, ", ")
来源：http://ky.nicolike.cn

Ruby: arr.join(", ")
来源：http://zm.huixiangedu.cn

C#:   string.Join(", ", list)
来源：http://jz.chemitech.net.cn

================================================================================
来源：http://lj.nszjky.cn

E. 字符串处理
来源：http://xi.panjiajie.cn

================================================================================
来源：http://kc.wgjwhj.cn

[E01] 拼接字符串
来源：http://vb.chemitech.net.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jd.panjiajie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dk.huixinmuqiang.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xe.yuexingan06.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ec.shxzukj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gd.yuexingan06.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cw.521024.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://uy.newstarts.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zo.szsharing.cn

[E02] 重复字符串
来源：http://zg.jianghongdianzi.cn

Py:   "ab" * 3
来源：http://qb.shxzukj.cn

PHP:  str_repeat("ab", 3);
来源：http://vn.szxytkj.cn

JS:   "ab".repeat(3)
来源：http://yv.yuexingan06.cn

TS:   "ab".repeat(3)
来源：http://xp.bjjhwx.cn

Java: "ab".repeat(3)
来源：http://uo.muxihuayi.cn

Go:   strings.Repeat("ab", 3)
来源：http://mv.huanxung.cn

Ruby: "ab" * 3
来源：http://hm.huixiangedu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zg.panjiajie.cn

[E03] 截取子串
来源：http://fn.yuntaijiaju.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fa.huixinmuqiang.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kz.bjjhwx.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ls.szsharing.cn

TS:   s.slice(1, 4)
来源：http://st.jianghongdianzi.cn

Java: s.substring(1, 4)
来源：http://rq.gzmigu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wy.shxzukj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://hm.wgjwhj.cn

C#:   s.Substring(1, 3)
来源：http://yj.jctech888.com.cn

[E04] 查找子串位置
来源：http://ef.shxzskj.cn

Py:   s.find("x");  s.index("x")
来源：http://ue.shxzskj.cn

PHP:  strpos($s, "x");
来源：http://qt.szsharing.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rv.panjiajie.cn

TS:   s.indexOf("x")
来源：http://go.haigaiapp.cn

Java: s.indexOf("x")
来源：http://my.muxihuayi.cn

Go:   strings.Index(s, "x")
来源：http://vs.yuntaijiaju.cn

Ruby: s.index("x")
来源：http://dn.huixinmuqiang.cn

C#:   s.IndexOf("x")
来源：http://ds.shxzskj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ub.huixiangedu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kx.panjiajie.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ki.lnxyls.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yo.szsharing.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://mi.nicolike.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lh.yuexingan06.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kj.lnxyls.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vr.haigaiapp.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gs.jianghongdianzi.cn

[E06] 替换子串
来源：http://jw.hahajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lg.szxytkj.cn

PHP:  str_replace("a", "b", $s);
来源：http://xe.lnxyls.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mm.szxytkj.cn

TS:   s.replaceAll("a", "b")
来源：http://np.nicolike.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sm.asd995.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ch.jctech888.com.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yd.lnxyls.cn

C#:   s.Replace("a", "b")
来源：http://hj.shxzukj.cn

[E07] 按分隔符拆分
来源：http://ne.hahajie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yw.bjjhwx.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nt.gzmigu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://az.szxytkj.cn

TS:   s.split(",")
来源：http://jk.yuexingan06.cn

Java: s.split(",");  s.split("\\s+")
来源：http://py.asd995.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fx.chemitech.net.cn

Ruby: s.split(",");  s.split
来源：http://rk.bookmarksfly.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jz.9csxet.cn

[E08] 数组按分隔符合并
来源：http://pe.huanxung.cn

Py:   ",".join(items)
来源：http://wl.muxihuayi.cn

PHP:  implode(",", $items);
来源：http://bk.muxihuayi.cn

JS:   items.join(",")
来源：http://ob.nicolike.cn

TS:   items.join(",")
来源：http://zx.9csxet.cn

Java: String.join(",", items)
来源：http://tf.huanxung.cn

Go:   strings.Join(items, ",")
来源：http://ix.huixinmuqiang.cn

Ruby: items.join(",")
来源：http://ay.shxzukj.cn

C#:   string.Join(",", items)
来源：http://ht.huanxung.cn

[E09] 去除所有空白字符
来源：http://rp.hahajie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kc.9csxet.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gp.bookmarksfly.cn

JS:   s.replace(/\s+/g, "")
来源：http://ld.newstarts.cn

TS:   s.replace(/\s+/g, "")
来源：http://xz.hahajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://zq.shxzukj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://fh.gzmigu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ol.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tf.jctech888.com.cn

[E10] 左侧补零 / 定长填充
来源：http://bi.colortex.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pk.panjiajie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tt.chemitech.net.cn

JS:   "7".padStart(3, "0")
来源：http://xf.yuntaijiaju.cn

TS:   "7".padStart(3, "0")
来源：http://qd.jctech888.com.cn

Java: String.format("%03d", 7)
来源：http://vw.muxihuayi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://za.nszjky.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yx.panjiajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hd.521024.cn

[E11] 反转字符串
来源：http://zi.huixinmuqiang.cn

Py:   s[::-1]
来源：http://fg.jianghongdianzi.cn

PHP:  strrev($s);
来源：http://sv.huixinmuqiang.cn

JS:   [...s].reverse().join("")
来源：http://eq.hnjuh.cn

TS:   [...s].reverse().join("")
来源：http://sr.haigaiapp.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ek.yuntaijiaju.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zf.nszjky.cn

Ruby: s.reverse
来源：http://sl.huanxung.cn

C#:   new string(s.Reverse().ToArray())
来源：http://db.jctech888.com.cn

[E12] 统计某字符出现次数
来源：http://dq.jctech888.com.cn

Py:   s.count("a")
来源：http://nj.hahajie.cn

PHP:  substr_count($s, "a");
来源：http://zb.szxytkj.cn

JS:   s.split("a").length - 1
来源：http://jh.szxytkj.cn

TS:   s.split("a").length - 1
来源：http://ou.lnxyls.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wt.muxihuayi.cn

Go:   strings.Count(s, "a")
来源：http://ce.chemitech.net.cn

Ruby: s.count("a")
来源：http://bz.shtwfgs.cn

C#:   s.Count(c => c == 'a')
来源：http://qr.jianghongdianzi.cn

[E13] 逐字符遍历
来源：http://qz.shxzukj.cn

Py:   for ch in s: print(ch)
来源：http://uo.shxzskj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fq.muxihuayi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://qw.panjiajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qn.nicolike.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://du.newstarts.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://do.yuntaijiaju.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://zq.haigaiapp.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cl.jctech888.com.cn

[E14] URL 编码与 Base64
来源：http://wr.panjiajie.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jd.huanxung.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://fk.muxihuayi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wg.wgjwhj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://iu.yuntaijiaju.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://as.szxytkj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xt.asd995.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rr.yuntaijiaju.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gu.jctech888.com.cn

[E15] HTML 转义 / 反转义
来源：http://pr.huixinmuqiang.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://dq.panjiajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vd.yuexingan06.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yf.huanxung.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://fn.colortex.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jq.huixinmuqiang.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fz.chemitech.net.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rz.wgjwhj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jc.huixinmuqiang.cn

[E16] 数字千分位
来源：http://qe.huanxung.cn

Py:   f"{1234567:,}"
来源：http://ho.newstarts.cn

PHP:  number_format(1234567);
来源：http://mr.bookmarksfly.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://aw.haigaiapp.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ho.huixinmuqiang.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tr.yuexingan06.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://aa.yuntaijiaju.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hy.jianghongdianzi.cn

C#:   1234567.ToString("N0")
来源：http://tt.colortex.cn

[E17] 首字母大写
来源：http://ua.chemitech.net.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jo.hnjuh.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ia.huixinmuqiang.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dx.hnjuh.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ny.gzmigu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jl.hnjuh.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lo.hahajie.cn

Ruby: s.capitalize
来源：http://pf.9csxet.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ou.lnxyls.cn

[E18] 模板占位符替换
来源：http://jt.huixinmuqiang.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bi.hahajie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pe.nszjky.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://jc.shtwfgs.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://uw.huixinmuqiang.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jp.huanxung.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cf.panjiajie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jj.hnjuh.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yh.chemitech.net.cn

[E19] 多行文本按行拆分
来源：http://od.lnxyls.cn

Py:   s.splitlines()
来源：http://sg.huixiangedu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jf.szsharing.cn

JS:   s.split(/\r?\n/)
来源：http://al.yuexingan06.cn

TS:   s.split(/\r?\n/)
来源：http://ma.gzmigu.cn

Java: s.lines().toList()
来源：http://ea.jctech888.com.cn

Go:   strings.Split(s, "\n")
来源：http://is.chemitech.net.cn

Ruby: s.lines
来源：http://ji.szsharing.cn

C#:   s.Split('\n')
来源：http://ed.jianghongdianzi.cn

[E20] 判断字符串是否为空
来源：http://dp.huixiangedu.cn

Py:   if not s:
来源：http://ev.newstarts.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tz.shxzukj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://te.lnxyls.cn

TS:   if (s === "") {}
来源：http://qy.hnjuh.cn

Java: if (s.isEmpty()) {}
来源：http://jj.gzmigu.cn

Go:   if s == "" {}
来源：http://ud.huixinmuqiang.cn

Ruby: if s.empty?
来源：http://jm.muxihuayi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lo.hahajie.cn

[E21] 超长截断加省略号
来源：http://sz.huanxung.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gn.nszjky.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ep.szxytkj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gb.asd995.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pl.shxzskj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ek.hnjuh.cn

Go:   // 按 rune 判断长度后截断
来源：http://lv.nszjky.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qn.shxzskj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vq.chemitech.net.cn

[E22] 字节长度与字符长度
来源：http://yv.muxihuayi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mw.bookmarksfly.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sd.newstarts.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kl.szsharing.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://oy.gzmigu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xo.jianghongdianzi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zq.lnxyls.cn

Ruby: s.bytesize;  s.length
来源：http://xu.nszjky.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nq.shtwfgs.cn

================================================================================
来源：http://fy.haigaiapp.cn

F. 文件与目录
来源：http://ay.9csxet.cn

================================================================================
来源：http://sr.shtwfgs.cn

[F01] 读取整个文件
来源：http://qd.nszjky.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yy.bjjhwx.cn

PHP:  file_get_contents("a.txt");
来源：http://df.newstarts.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ik.nicolike.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mr.yuexingan06.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://nd.shxzukj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lg.nszjky.cn

Ruby: File.read("a.txt")
来源：http://ea.hnjuh.cn

C#:   File.ReadAllText("a.txt");
来源：http://ab.huanxung.cn

[F02] 逐行读取文件
来源：http://rc.asd995.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vv.shxzskj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kg.chemitech.net.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nr.shtwfgs.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wa.jctech888.com.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xc.szxytkj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bn.jctech888.com.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ad.lnxyls.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kd.huixiangedu.cn

[F03] 写入文件（覆盖）
来源：http://ck.nicolike.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qv.nicolike.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://rh.nicolike.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hj.szxytkj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ec.asd995.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ly.muxihuayi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lj.colortex.cn

Ruby: File.write("a.txt", "hi")
来源：http://jo.hahajie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vy.huixinmuqiang.cn

[F04] 追加写入文件
来源：http://nq.jianghongdianzi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://le.bookmarksfly.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://oi.szsharing.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nf.panjiajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wi.shxzukj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vf.yuntaijiaju.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zy.huanxung.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gb.shxzukj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ti.yuntaijiaju.cn

[F05] 判断文件或目录是否存在
来源：http://ez.jianghongdianzi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xh.shxzskj.cn

PHP:  file_exists("a.txt");
来源：http://kb.jianghongdianzi.cn

JS:   fs.existsSync("a.txt")
来源：http://bu.521024.cn

TS:   fs.existsSync("a.txt")
来源：http://sm.szxytkj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://sv.gzmigu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fa.muxihuayi.cn

Ruby: File.exist?("a.txt")
来源：http://fu.hnjuh.cn

C#:   File.Exists("a.txt")
来源：http://mf.newstarts.cn

[F06] 删除文件
来源：http://mv.huixinmuqiang.cn

Py:   os.remove("a.txt")
来源：http://mt.newstarts.cn

PHP:  unlink("a.txt");
来源：http://cp.haigaiapp.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ad.asd995.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ut.hahajie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ry.bookmarksfly.cn

Go:   os.Remove("a.txt")
来源：http://iu.nszjky.cn

Ruby: File.delete("a.txt")
来源：http://gh.szsharing.cn

C#:   File.Delete("a.txt");
来源：http://iv.chemitech.net.cn

[F07] 创建目录（含多级）
来源：http://hm.huanxung.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bi.bookmarksfly.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zd.newstarts.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jd.colortex.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://om.hahajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ch.gzmigu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qp.chemitech.net.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nv.muxihuayi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ia.colortex.cn

[F08] 遍历目录
来源：http://kv.colortex.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://jw.nicolike.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ly.nszjky.cn

JS:   fs.readdirSync("dir")
来源：http://wm.haigaiapp.cn

TS:   fs.readdirSync("dir")
来源：http://pp.hnjuh.cn


<!-- 参考信息 -->