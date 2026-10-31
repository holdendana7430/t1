代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ld.nicolike.cn

[D24] 字典 / Map 基本操作
来源：http://gd.bookmarksfly.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ad.newstarts.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gc.szxytkj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qb.shtwfgs.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bw.hnjuh.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yp.bjjhwx.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yf.szxytkj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kl.bjjhwx.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zd.jianghongdianzi.cn

[D25] Set 集合去重与交并差
来源：http://tz.gzmigu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xm.haigaiapp.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zx.szxytkj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ml.shxzskj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wq.hahajie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nm.nszjky.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sh.lnxyls.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kv.chemitech.net.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://uc.lnxyls.cn

[D26] 数组转字符串
来源：http://ij.hnjuh.cn

Py:   ", ".join(map(str, arr))
来源：http://fm.huixinmuqiang.cn

PHP:  implode(", ", $arr);
来源：http://ac.521024.cn

JS:   arr.join(", ")
来源：http://va.hahajie.cn

TS:   arr.join(", ")
来源：http://op.szsharing.cn

Java: String.join(", ", list)
来源：http://fa.wgjwhj.cn

Go:   strings.Join(strs, ", ")
来源：http://xt.hahajie.cn

Ruby: arr.join(", ")
来源：http://ny.9csxet.cn

C#:   string.Join(", ", list)
来源：http://kj.bookmarksfly.cn

================================================================================
来源：http://cw.521024.cn

E. 字符串处理
来源：http://se.lnxyls.cn

================================================================================
来源：http://iq.lnxyls.cn

[E01] 拼接字符串
来源：http://nr.jctech888.com.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yj.asd995.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://up.9csxet.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tp.shxzskj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zf.bookmarksfly.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vv.huixiangedu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wa.yuexingan06.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nc.muxihuayi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gc.hnjuh.cn

[E02] 重复字符串
来源：http://wl.haigaiapp.cn

Py:   "ab" * 3
来源：http://uq.haigaiapp.cn

PHP:  str_repeat("ab", 3);
来源：http://mw.colortex.cn

JS:   "ab".repeat(3)
来源：http://ao.yuexingan06.cn

TS:   "ab".repeat(3)
来源：http://wy.huixiangedu.cn

Java: "ab".repeat(3)
来源：http://tt.yuntaijiaju.cn

Go:   strings.Repeat("ab", 3)
来源：http://lo.shxzukj.cn

Ruby: "ab" * 3
来源：http://jz.chemitech.net.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dm.szsharing.cn

[E03] 截取子串
来源：http://bb.gzmigu.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kg.bjjhwx.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rm.yuexingan06.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yj.wgjwhj.cn

TS:   s.slice(1, 4)
来源：http://ld.szsharing.cn

Java: s.substring(1, 4)
来源：http://gb.yuntaijiaju.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kq.521024.cn

Ruby: s[1, 3];  s[1..3]
来源：http://qr.hahajie.cn

C#:   s.Substring(1, 3)
来源：http://go.yuexingan06.cn

[E04] 查找子串位置
来源：http://kl.newstarts.cn

Py:   s.find("x");  s.index("x")
来源：http://ek.521024.cn

PHP:  strpos($s, "x");
来源：http://gc.lnxyls.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kx.shxzskj.cn

TS:   s.indexOf("x")
来源：http://dn.9csxet.cn

Java: s.indexOf("x")
来源：http://es.nszjky.cn

Go:   strings.Index(s, "x")
来源：http://gb.szsharing.cn

Ruby: s.index("x")
来源：http://zw.shxzukj.cn

C#:   s.IndexOf("x")
来源：http://oi.jianghongdianzi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://fu.bookmarksfly.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wc.hnjuh.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ci.huixinmuqiang.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hb.wgjwhj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://oi.haigaiapp.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wu.lnxyls.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hf.jianghongdianzi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vh.nszjky.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rx.chemitech.net.cn

[E06] 替换子串
来源：http://ka.haigaiapp.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://no.hnjuh.cn

PHP:  str_replace("a", "b", $s);
来源：http://fy.shxzukj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ns.muxihuayi.cn

TS:   s.replaceAll("a", "b")
来源：http://je.shxzukj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bl.yuexingan06.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sd.hahajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bx.lnxyls.cn

C#:   s.Replace("a", "b")
来源：http://fv.bjjhwx.cn

[E07] 按分隔符拆分
来源：http://ck.asd995.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cn.yuexingan06.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hk.huixinmuqiang.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://lh.haigaiapp.cn

TS:   s.split(",")
来源：http://lm.huanxung.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ob.hahajie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qp.nszjky.cn

Ruby: s.split(",");  s.split
来源：http://rr.nszjky.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cj.colortex.cn

[E08] 数组按分隔符合并
来源：http://hg.muxihuayi.cn

Py:   ",".join(items)
来源：http://id.yuntaijiaju.cn

PHP:  implode(",", $items);
来源：http://jk.huixiangedu.cn

JS:   items.join(",")
来源：http://am.hahajie.cn

TS:   items.join(",")
来源：http://za.szsharing.cn

Java: String.join(",", items)
来源：http://sa.shxzukj.cn

Go:   strings.Join(items, ",")
来源：http://cr.chemitech.net.cn

Ruby: items.join(",")
来源：http://xu.lnxyls.cn

C#:   string.Join(",", items)
来源：http://tl.shxzskj.cn

[E09] 去除所有空白字符
来源：http://ay.bookmarksfly.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qm.newstarts.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://py.shxzskj.cn

JS:   s.replace(/\s+/g, "")
来源：http://mz.bookmarksfly.cn

TS:   s.replace(/\s+/g, "")
来源：http://sr.huixiangedu.cn

Java: s.replaceAll("\\s+", "")
来源：http://um.huixiangedu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ld.shxzskj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://bw.szxytkj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ir.muxihuayi.cn

[E10] 左侧补零 / 定长填充
来源：http://of.shxzskj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://we.szsharing.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vu.wgjwhj.cn

JS:   "7".padStart(3, "0")
来源：http://xi.nicolike.cn

TS:   "7".padStart(3, "0")
来源：http://rq.shxzskj.cn

Java: String.format("%03d", 7)
来源：http://dl.jctech888.com.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://tw.jianghongdianzi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mz.bookmarksfly.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xn.lnxyls.cn

[E11] 反转字符串
来源：http://sy.haigaiapp.cn

Py:   s[::-1]
来源：http://en.gzmigu.cn

PHP:  strrev($s);
来源：http://bk.yuntaijiaju.cn

JS:   [...s].reverse().join("")
来源：http://sy.haigaiapp.cn

TS:   [...s].reverse().join("")
来源：http://gh.szxytkj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://pe.bjjhwx.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://wp.huanxung.cn

Ruby: s.reverse
来源：http://me.haigaiapp.cn

C#:   new string(s.Reverse().ToArray())
来源：http://dt.panjiajie.cn

[E12] 统计某字符出现次数
来源：http://ae.hnjuh.cn

Py:   s.count("a")
来源：http://lb.bookmarksfly.cn

PHP:  substr_count($s, "a");
来源：http://cn.wgjwhj.cn

JS:   s.split("a").length - 1
来源：http://pa.yuntaijiaju.cn

TS:   s.split("a").length - 1
来源：http://jo.shtwfgs.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wo.huixinmuqiang.cn

Go:   strings.Count(s, "a")
来源：http://ms.gzmigu.cn

Ruby: s.count("a")
来源：http://vk.lnxyls.cn

C#:   s.Count(c => c == 'a')
来源：http://zr.panjiajie.cn

[E13] 逐字符遍历
来源：http://cw.nicolike.cn

Py:   for ch in s: print(ch)
来源：http://tj.shxzskj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zd.huixinmuqiang.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://yf.hnjuh.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://eq.colortex.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rh.newstarts.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ii.9csxet.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://py.huanxung.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ut.newstarts.cn

[E14] URL 编码与 Base64
来源：http://di.shtwfgs.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ga.jctech888.com.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://lo.shxzskj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://no.shxzskj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qs.yuexingan06.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uz.shtwfgs.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vr.yuntaijiaju.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://np.shxzskj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bd.gzmigu.cn

[E15] HTML 转义 / 反转义
来源：http://sd.newstarts.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://zd.huixiangedu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jc.chemitech.net.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ky.521024.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://bg.nszjky.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qh.shxzukj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bj.nszjky.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jt.521024.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mz.muxihuayi.cn

[E16] 数字千分位
来源：http://ya.9csxet.cn

Py:   f"{1234567:,}"
来源：http://jl.colortex.cn

PHP:  number_format(1234567);
来源：http://ux.colortex.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://xu.shtwfgs.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://pe.gzmigu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hb.asd995.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xd.lnxyls.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dh.wgjwhj.cn

C#:   1234567.ToString("N0")
来源：http://uz.jianghongdianzi.cn

[E17] 首字母大写
来源：http://fx.huixiangedu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://de.9csxet.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://lr.shxzukj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xa.521024.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vj.jianghongdianzi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tk.lnxyls.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xc.yuntaijiaju.cn

Ruby: s.capitalize
来源：http://es.nszjky.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jg.9csxet.cn

[E18] 模板占位符替换
来源：http://dy.panjiajie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dn.yuexingan06.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://as.szsharing.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://tj.szsharing.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://sp.hahajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hw.shtwfgs.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://re.asd995.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fp.huixinmuqiang.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qi.wgjwhj.cn

[E19] 多行文本按行拆分
来源：http://pu.yuntaijiaju.cn

Py:   s.splitlines()
来源：http://rn.hnjuh.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fr.jianghongdianzi.cn

JS:   s.split(/\r?\n/)
来源：http://om.colortex.cn

TS:   s.split(/\r?\n/)
来源：http://mv.9csxet.cn

Java: s.lines().toList()
来源：http://oy.yuntaijiaju.cn

Go:   strings.Split(s, "\n")
来源：http://xs.hahajie.cn

Ruby: s.lines
来源：http://si.wgjwhj.cn

C#:   s.Split('\n')
来源：http://ja.yuexingan06.cn

[E20] 判断字符串是否为空
来源：http://fi.wgjwhj.cn

Py:   if not s:
来源：http://ra.yuntaijiaju.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hj.huixiangedu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hf.yuntaijiaju.cn

TS:   if (s === "") {}
来源：http://es.panjiajie.cn

Java: if (s.isEmpty()) {}
来源：http://wl.lnxyls.cn

Go:   if s == "" {}
来源：http://ll.szxytkj.cn

Ruby: if s.empty?
来源：http://ed.newstarts.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ov.jianghongdianzi.cn

[E21] 超长截断加省略号
来源：http://mq.haigaiapp.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rw.haigaiapp.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://df.shxzskj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ba.huanxung.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://og.gzmigu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://co.huixinmuqiang.cn

Go:   // 按 rune 判断长度后截断
来源：http://gc.huanxung.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dt.muxihuayi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pq.hnjuh.cn

[E22] 字节长度与字符长度
来源：http://gj.nszjky.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jj.shxzskj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://so.jctech888.com.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xr.9csxet.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://iv.jctech888.com.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kt.colortex.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ke.nicolike.cn

Ruby: s.bytesize;  s.length
来源：http://do.yuexingan06.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://co.colortex.cn

================================================================================
来源：http://qv.chemitech.net.cn

F. 文件与目录
来源：http://ok.hahajie.cn

================================================================================
来源：http://qf.panjiajie.cn

[F01] 读取整个文件
来源：http://ms.haigaiapp.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ro.hahajie.cn

PHP:  file_get_contents("a.txt");
来源：http://as.huixiangedu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ti.shxzukj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://up.wgjwhj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ig.gzmigu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sd.szxytkj.cn

Ruby: File.read("a.txt")
来源：http://qy.huixinmuqiang.cn

C#:   File.ReadAllText("a.txt");
来源：http://bs.colortex.cn

[F02] 逐行读取文件
来源：http://na.jctech888.com.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qz.gzmigu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://an.szxytkj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ew.lnxyls.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ba.szxytkj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qr.muxihuayi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://st.shxzukj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gb.shtwfgs.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ea.521024.cn

[F03] 写入文件（覆盖）
来源：http://sd.nicolike.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://da.jctech888.com.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xt.hahajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ct.nicolike.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oz.hahajie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lp.jianghongdianzi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ua.nicolike.cn

Ruby: File.write("a.txt", "hi")
来源：http://uc.muxihuayi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ux.szsharing.cn

[F04] 追加写入文件
来源：http://nf.bjjhwx.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ew.wgjwhj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rs.shxzukj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dv.colortex.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oh.9csxet.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://za.jianghongdianzi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jz.newstarts.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dl.newstarts.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jk.jctech888.com.cn

[F05] 判断文件或目录是否存在
来源：http://vw.yuntaijiaju.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ev.nszjky.cn

PHP:  file_exists("a.txt");
来源：http://mq.colortex.cn

JS:   fs.existsSync("a.txt")
来源：http://gf.newstarts.cn

TS:   fs.existsSync("a.txt")
来源：http://wl.haigaiapp.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gl.huanxung.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vs.jctech888.com.cn

Ruby: File.exist?("a.txt")
来源：http://fn.szsharing.cn

C#:   File.Exists("a.txt")
来源：http://mk.chemitech.net.cn

[F06] 删除文件
来源：http://oc.chemitech.net.cn

Py:   os.remove("a.txt")
来源：http://zx.panjiajie.cn

PHP:  unlink("a.txt");
来源：http://vf.yuexingan06.cn

JS:   fs.unlinkSync("a.txt")
来源：http://qs.colortex.cn

TS:   fs.unlinkSync("a.txt")
来源：http://yj.jianghongdianzi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ce.lnxyls.cn

Go:   os.Remove("a.txt")
来源：http://uf.muxihuayi.cn

Ruby: File.delete("a.txt")
来源：http://pd.newstarts.cn

C#:   File.Delete("a.txt");
来源：http://jf.nicolike.cn

[F07] 创建目录（含多级）
来源：http://yg.521024.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kj.jianghongdianzi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://os.bjjhwx.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ty.colortex.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oi.bjjhwx.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tj.asd995.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://oq.muxihuayi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ha.lnxyls.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vb.521024.cn

[F08] 遍历目录
来源：http://fa.haigaiapp.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://us.muxihuayi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gi.huixiangedu.cn

JS:   fs.readdirSync("dir")
来源：http://yh.huixinmuqiang.cn

TS:   fs.readdirSync("dir")
来源：http://ge.asd995.cn


<!-- 参考信息 -->