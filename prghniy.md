代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://lz.asd995.cn

JS:   arr.includes(x)
来源：http://fh.nszjky.cn

TS:   arr.includes(x)
来源：http://fo.colortex.cn

Java: list.contains(x)
来源：http://zx.hahajie.cn

Go:   slices.Contains(arr, x)
来源：http://zo.panjiajie.cn

Ruby: arr.include?(x)
来源：http://hn.panjiajie.cn

C#:   list.Contains(x)
来源：http://ug.bookmarksfly.cn

[D22] 复制数组（避免共享引用）
来源：http://ut.huixinmuqiang.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pn.asd995.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ai.huixiangedu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://of.shxzukj.cn

TS:   [...arr];
来源：http://xb.shxzskj.cn

Java: new ArrayList<>(list);
来源：http://di.hahajie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://td.asd995.cn

Ruby: arr.dup;  arr.clone
来源：http://vy.haigaiapp.cn

C#:   new List<int>(list);
来源：http://qe.yuntaijiaju.cn

[D23] reduce 累积计算
来源：http://vr.yuexingan06.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ye.gzmigu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rd.haigaiapp.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://am.huixiangedu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lr.gzmigu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://as.yuntaijiaju.cn

Go:   // 手写循环
来源：http://ir.shtwfgs.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ce.yuexingan06.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jd.hnjuh.cn

[D24] 字典 / Map 基本操作
来源：http://dg.chemitech.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zl.hnjuh.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://df.nicolike.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tv.chemitech.net.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hh.nicolike.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://di.yuntaijiaju.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gn.huixiangedu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hp.huixiangedu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fi.gzmigu.cn

[D25] Set 集合去重与交并差
来源：http://xj.asd995.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xo.panjiajie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://of.jctech888.com.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gf.nicolike.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hv.yuexingan06.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kl.newstarts.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kb.colortex.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yy.huanxung.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xt.gzmigu.cn

[D26] 数组转字符串
来源：http://zz.gzmigu.cn

Py:   ", ".join(map(str, arr))
来源：http://tt.shtwfgs.cn

PHP:  implode(", ", $arr);
来源：http://sl.yuntaijiaju.cn

JS:   arr.join(", ")
来源：http://zu.nicolike.cn

TS:   arr.join(", ")
来源：http://zv.colortex.cn

Java: String.join(", ", list)
来源：http://zi.shxzskj.cn

Go:   strings.Join(strs, ", ")
来源：http://ed.szxytkj.cn

Ruby: arr.join(", ")
来源：http://xn.wgjwhj.cn

C#:   string.Join(", ", list)
来源：http://pk.hahajie.cn

================================================================================
来源：http://mw.haigaiapp.cn

E. 字符串处理
来源：http://ev.jianghongdianzi.cn

================================================================================
来源：http://zw.nszjky.cn

[E01] 拼接字符串
来源：http://th.huixinmuqiang.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jn.hahajie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rz.panjiajie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bn.nszjky.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zw.huixinmuqiang.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pe.newstarts.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fe.nicolike.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vk.lnxyls.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sy.huanxung.cn

[E02] 重复字符串
来源：http://wz.521024.cn

Py:   "ab" * 3
来源：http://yq.bookmarksfly.cn

PHP:  str_repeat("ab", 3);
来源：http://ty.muxihuayi.cn

JS:   "ab".repeat(3)
来源：http://ae.hnjuh.cn

TS:   "ab".repeat(3)
来源：http://qv.colortex.cn

Java: "ab".repeat(3)
来源：http://ss.chemitech.net.cn

Go:   strings.Repeat("ab", 3)
来源：http://mm.szxytkj.cn

Ruby: "ab" * 3
来源：http://mv.yuexingan06.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yf.hahajie.cn

[E03] 截取子串
来源：http://ws.chemitech.net.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ea.jianghongdianzi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lk.nicolike.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ev.huixiangedu.cn

TS:   s.slice(1, 4)
来源：http://dt.hnjuh.cn

Java: s.substring(1, 4)
来源：http://vi.wgjwhj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wh.521024.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ii.bjjhwx.cn

C#:   s.Substring(1, 3)
来源：http://ob.panjiajie.cn

[E04] 查找子串位置
来源：http://ju.panjiajie.cn

Py:   s.find("x");  s.index("x")
来源：http://ck.yuexingan06.cn

PHP:  strpos($s, "x");
来源：http://jh.muxihuayi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wx.nicolike.cn

TS:   s.indexOf("x")
来源：http://kz.newstarts.cn

Java: s.indexOf("x")
来源：http://im.haigaiapp.cn

Go:   strings.Index(s, "x")
来源：http://yq.asd995.cn

Ruby: s.index("x")
来源：http://hm.shtwfgs.cn

C#:   s.IndexOf("x")
来源：http://we.wgjwhj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://rn.jianghongdianzi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://sv.nszjky.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yq.lnxyls.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://em.jctech888.com.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ja.yuexingan06.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vg.jctech888.com.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pu.szsharing.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xz.hahajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://aj.haigaiapp.cn

[E06] 替换子串
来源：http://zl.hahajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ce.9csxet.cn

PHP:  str_replace("a", "b", $s);
来源：http://hu.nicolike.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qr.lnxyls.cn

TS:   s.replaceAll("a", "b")
来源：http://nw.colortex.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xw.huixinmuqiang.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vn.9csxet.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mv.wgjwhj.cn

C#:   s.Replace("a", "b")
来源：http://gp.shxzskj.cn

[E07] 按分隔符拆分
来源：http://tw.szsharing.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tp.9csxet.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qy.colortex.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://tt.jctech888.com.cn

TS:   s.split(",")
来源：http://rm.shxzukj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://aj.nicolike.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ke.newstarts.cn

Ruby: s.split(",");  s.split
来源：http://je.lnxyls.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nh.muxihuayi.cn

[E08] 数组按分隔符合并
来源：http://ac.nicolike.cn

Py:   ",".join(items)
来源：http://mg.haigaiapp.cn

PHP:  implode(",", $items);
来源：http://ac.hnjuh.cn

JS:   items.join(",")
来源：http://rs.asd995.cn

TS:   items.join(",")
来源：http://yj.wgjwhj.cn

Java: String.join(",", items)
来源：http://cl.lnxyls.cn

Go:   strings.Join(items, ",")
来源：http://gg.nszjky.cn

Ruby: items.join(",")
来源：http://li.yuntaijiaju.cn

C#:   string.Join(",", items)
来源：http://rd.huixiangedu.cn

[E09] 去除所有空白字符
来源：http://ay.521024.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ac.newstarts.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cx.hnjuh.cn

JS:   s.replace(/\s+/g, "")
来源：http://ll.muxihuayi.cn

TS:   s.replace(/\s+/g, "")
来源：http://af.bookmarksfly.cn

Java: s.replaceAll("\\s+", "")
来源：http://wp.huixiangedu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://we.jianghongdianzi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ar.yuntaijiaju.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nc.newstarts.cn

[E10] 左侧补零 / 定长填充
来源：http://mj.haigaiapp.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kf.shxzukj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://og.muxihuayi.cn

JS:   "7".padStart(3, "0")
来源：http://ai.shtwfgs.cn

TS:   "7".padStart(3, "0")
来源：http://er.yuntaijiaju.cn

Java: String.format("%03d", 7)
来源：http://tv.huixiangedu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://dh.shtwfgs.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://eb.bookmarksfly.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gh.shxzukj.cn

[E11] 反转字符串
来源：http://yg.9csxet.cn

Py:   s[::-1]
来源：http://xa.shxzskj.cn

PHP:  strrev($s);
来源：http://gf.yuexingan06.cn

JS:   [...s].reverse().join("")
来源：http://gh.huanxung.cn

TS:   [...s].reverse().join("")
来源：http://jm.haigaiapp.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://yi.wgjwhj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://hn.szsharing.cn

Ruby: s.reverse
来源：http://gb.shxzskj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://cl.huixinmuqiang.cn

[E12] 统计某字符出现次数
来源：http://aa.szsharing.cn

Py:   s.count("a")
来源：http://nw.muxihuayi.cn

PHP:  substr_count($s, "a");
来源：http://to.hnjuh.cn

JS:   s.split("a").length - 1
来源：http://vj.hnjuh.cn

TS:   s.split("a").length - 1
来源：http://os.chemitech.net.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ux.newstarts.cn

Go:   strings.Count(s, "a")
来源：http://lc.521024.cn

Ruby: s.count("a")
来源：http://cs.wgjwhj.cn

C#:   s.Count(c => c == 'a')
来源：http://jo.huanxung.cn

[E13] 逐字符遍历
来源：http://da.lnxyls.cn

Py:   for ch in s: print(ch)
来源：http://mr.asd995.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hy.newstarts.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://dx.muxihuayi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://gz.asd995.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dl.jctech888.com.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ov.hahajie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://nt.newstarts.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ov.colortex.cn

[E14] URL 编码与 Base64
来源：http://gt.shxzskj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yj.lnxyls.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://yz.wgjwhj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rj.shxzukj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zz.colortex.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mc.521024.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fs.jianghongdianzi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ay.bjjhwx.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kw.hnjuh.cn

[E15] HTML 转义 / 反转义
来源：http://cv.lnxyls.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://yc.panjiajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fh.nszjky.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jy.521024.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://yz.szsharing.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pk.shxzskj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jt.hnjuh.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://my.jianghongdianzi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rn.9csxet.cn

[E16] 数字千分位
来源：http://ul.jianghongdianzi.cn

Py:   f"{1234567:,}"
来源：http://ec.szxytkj.cn

PHP:  number_format(1234567);
来源：http://er.nicolike.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://xy.gzmigu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ss.hahajie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://si.shxzskj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qw.nszjky.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jl.yuexingan06.cn

C#:   1234567.ToString("N0")
来源：http://ji.9csxet.cn

[E17] 首字母大写
来源：http://lr.szsharing.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yf.huixinmuqiang.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://by.muxihuayi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qe.asd995.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://it.muxihuayi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mv.colortex.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fy.huixiangedu.cn

Ruby: s.capitalize
来源：http://og.9csxet.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rw.gzmigu.cn

[E18] 模板占位符替换
来源：http://yb.szxytkj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ni.jianghongdianzi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ei.chemitech.net.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ho.asd995.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://tj.shxzukj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vs.yuntaijiaju.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vp.gzmigu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ok.asd995.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vm.szsharing.cn

[E19] 多行文本按行拆分
来源：http://eq.jianghongdianzi.cn

Py:   s.splitlines()
来源：http://ra.521024.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kf.colortex.cn

JS:   s.split(/\r?\n/)
来源：http://zw.chemitech.net.cn

TS:   s.split(/\r?\n/)
来源：http://jd.hnjuh.cn

Java: s.lines().toList()
来源：http://cg.9csxet.cn

Go:   strings.Split(s, "\n")
来源：http://cc.521024.cn

Ruby: s.lines
来源：http://cw.shxzskj.cn

C#:   s.Split('\n')
来源：http://xb.nszjky.cn

[E20] 判断字符串是否为空
来源：http://gb.huixinmuqiang.cn

Py:   if not s:
来源：http://fn.yuexingan06.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wt.521024.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lk.panjiajie.cn

TS:   if (s === "") {}
来源：http://dp.huanxung.cn

Java: if (s.isEmpty()) {}
来源：http://lh.huixinmuqiang.cn

Go:   if s == "" {}
来源：http://ev.nicolike.cn

Ruby: if s.empty?
来源：http://pa.hahajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ak.hahajie.cn

[E21] 超长截断加省略号
来源：http://hx.szxytkj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ln.panjiajie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kc.huanxung.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ai.yuntaijiaju.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fc.hahajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zm.asd995.cn

Go:   // 按 rune 判断长度后截断
来源：http://hq.muxihuayi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ze.hahajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cz.jianghongdianzi.cn

[E22] 字节长度与字符长度
来源：http://hw.colortex.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mk.yuntaijiaju.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ka.haigaiapp.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gt.9csxet.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://al.jianghongdianzi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mj.gzmigu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lk.yuexingan06.cn

Ruby: s.bytesize;  s.length
来源：http://er.hahajie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pc.yuntaijiaju.cn

================================================================================
来源：http://hl.nicolike.cn

F. 文件与目录
来源：http://ce.bookmarksfly.cn

================================================================================
来源：http://aw.nszjky.cn

[F01] 读取整个文件
来源：http://dx.9csxet.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qv.haigaiapp.cn

PHP:  file_get_contents("a.txt");
来源：http://bo.jctech888.com.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jianghongdianzi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ma.asd995.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://st.jianghongdianzi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bo.yuntaijiaju.cn

Ruby: File.read("a.txt")
来源：http://ks.lnxyls.cn

C#:   File.ReadAllText("a.txt");
来源：http://xm.bjjhwx.cn

[F02] 逐行读取文件
来源：http://on.nszjky.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mh.521024.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lh.lnxyls.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zl.yuexingan06.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mf.colortex.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kt.gzmigu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cj.shtwfgs.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bk.hnjuh.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xs.newstarts.cn

[F03] 写入文件（覆盖）
来源：http://fq.huixinmuqiang.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fw.shtwfgs.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ch.wgjwhj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tb.panjiajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kt.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://sj.newstarts.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://oe.521024.cn

Ruby: File.write("a.txt", "hi")
来源：http://sx.521024.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nw.wgjwhj.cn

[F04] 追加写入文件
来源：http://nd.jianghongdianzi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zv.lnxyls.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pe.shxzukj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ok.newstarts.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://al.521024.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ju.szxytkj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ty.yuntaijiaju.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://im.shxzukj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://aq.shxzskj.cn

[F05] 判断文件或目录是否存在
来源：http://qr.jctech888.com.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://me.shxzskj.cn

PHP:  file_exists("a.txt");
来源：http://jy.bjjhwx.cn

JS:   fs.existsSync("a.txt")
来源：http://pf.hnjuh.cn

TS:   fs.existsSync("a.txt")
来源：http://az.bookmarksfly.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hx.haigaiapp.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lv.haigaiapp.cn

Ruby: File.exist?("a.txt")
来源：http://du.shtwfgs.cn


<!-- 参考信息 -->