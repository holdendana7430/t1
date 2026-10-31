代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://el.newstarts.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://st.jctech888.com.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cx.szsharing.cn

TS:   [...arr];
来源：http://wk.bookmarksfly.cn

Java: new ArrayList<>(list);
来源：http://qr.9csxet.cn

Go:   copied := append([]int(nil), arr...)
来源：http://kp.nicolike.cn

Ruby: arr.dup;  arr.clone
来源：http://lh.bjjhwx.cn

C#:   new List<int>(list);
来源：http://od.szxytkj.cn

[D23] reduce 累积计算
来源：http://xs.shtwfgs.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tb.bookmarksfly.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ie.colortex.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xn.wgjwhj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wf.muxihuayi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ca.jctech888.com.cn

Go:   // 手写循环
来源：http://cz.521024.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xb.yuntaijiaju.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yz.haigaiapp.cn

[D24] 字典 / Map 基本操作
来源：http://ua.huixinmuqiang.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ca.hnjuh.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://uu.wgjwhj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xr.nszjky.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wz.szsharing.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zw.lnxyls.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://uv.hahajie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gs.jianghongdianzi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rx.szsharing.cn

[D25] Set 集合去重与交并差
来源：http://yw.haigaiapp.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://iw.lnxyls.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qm.hnjuh.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://js.wgjwhj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xa.szxytkj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jg.chemitech.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kc.bjjhwx.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qj.nicolike.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cd.szsharing.cn

[D26] 数组转字符串
来源：http://sd.nszjky.cn

Py:   ", ".join(map(str, arr))
来源：http://xk.wgjwhj.cn

PHP:  implode(", ", $arr);
来源：http://gf.haigaiapp.cn

JS:   arr.join(", ")
来源：http://km.panjiajie.cn

TS:   arr.join(", ")
来源：http://aa.panjiajie.cn

Java: String.join(", ", list)
来源：http://ex.9csxet.cn

Go:   strings.Join(strs, ", ")
来源：http://yh.szxytkj.cn

Ruby: arr.join(", ")
来源：http://ol.shxzukj.cn

C#:   string.Join(", ", list)
来源：http://pv.szsharing.cn

================================================================================
来源：http://hr.colortex.cn

E. 字符串处理
来源：http://ru.9csxet.cn

================================================================================
来源：http://bi.haigaiapp.cn

[E01] 拼接字符串
来源：http://ks.hnjuh.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ex.newstarts.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ji.lnxyls.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xy.newstarts.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qr.szsharing.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tf.shxzskj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fs.shxzskj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zh.hahajie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zu.szxytkj.cn

[E02] 重复字符串
来源：http://sd.bjjhwx.cn

Py:   "ab" * 3
来源：http://ap.jctech888.com.cn

PHP:  str_repeat("ab", 3);
来源：http://yx.lnxyls.cn

JS:   "ab".repeat(3)
来源：http://jg.huanxung.cn

TS:   "ab".repeat(3)
来源：http://as.newstarts.cn

Java: "ab".repeat(3)
来源：http://ku.bookmarksfly.cn

Go:   strings.Repeat("ab", 3)
来源：http://uj.haigaiapp.cn

Ruby: "ab" * 3
来源：http://fn.newstarts.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fa.szxytkj.cn

[E03] 截取子串
来源：http://xh.nicolike.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://na.nicolike.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dl.huixiangedu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ws.newstarts.cn

TS:   s.slice(1, 4)
来源：http://io.huixiangedu.cn

Java: s.substring(1, 4)
来源：http://wu.nicolike.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wf.muxihuayi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://rk.521024.cn

C#:   s.Substring(1, 3)
来源：http://nh.hnjuh.cn

[E04] 查找子串位置
来源：http://ug.colortex.cn

Py:   s.find("x");  s.index("x")
来源：http://rf.gzmigu.cn

PHP:  strpos($s, "x");
来源：http://ji.panjiajie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://im.colortex.cn

TS:   s.indexOf("x")
来源：http://zw.huixiangedu.cn

Java: s.indexOf("x")
来源：http://bd.jctech888.com.cn

Go:   strings.Index(s, "x")
来源：http://xq.colortex.cn

Ruby: s.index("x")
来源：http://ag.shtwfgs.cn

C#:   s.IndexOf("x")
来源：http://xa.szxytkj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://fc.hahajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gx.muxihuayi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://iq.gzmigu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ry.colortex.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ds.nicolike.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mh.haigaiapp.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ia.shxzukj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ng.newstarts.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qo.bjjhwx.cn

[E06] 替换子串
来源：http://jj.colortex.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qb.521024.cn

PHP:  str_replace("a", "b", $s);
来源：http://kk.hnjuh.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pg.hnjuh.cn

TS:   s.replaceAll("a", "b")
来源：http://lt.nicolike.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rl.bookmarksfly.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vu.szxytkj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fd.szxytkj.cn

C#:   s.Replace("a", "b")
来源：http://xq.yuntaijiaju.cn

[E07] 按分隔符拆分
来源：http://rn.shtwfgs.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tt.asd995.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gm.panjiajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://it.hnjuh.cn

TS:   s.split(",")
来源：http://zd.hahajie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ak.muxihuayi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zz.panjiajie.cn

Ruby: s.split(",");  s.split
来源：http://yz.shxzskj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ki.muxihuayi.cn

[E08] 数组按分隔符合并
来源：http://id.newstarts.cn

Py:   ",".join(items)
来源：http://sb.jianghongdianzi.cn

PHP:  implode(",", $items);
来源：http://xa.9csxet.cn

JS:   items.join(",")
来源：http://uf.chemitech.net.cn

TS:   items.join(",")
来源：http://od.shtwfgs.cn

Java: String.join(",", items)
来源：http://ef.hahajie.cn

Go:   strings.Join(items, ",")
来源：http://wa.lnxyls.cn

Ruby: items.join(",")
来源：http://jw.chemitech.net.cn

C#:   string.Join(",", items)
来源：http://qn.yuntaijiaju.cn

[E09] 去除所有空白字符
来源：http://cm.9csxet.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bi.huixiangedu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vw.9csxet.cn

JS:   s.replace(/\s+/g, "")
来源：http://vz.bookmarksfly.cn

TS:   s.replace(/\s+/g, "")
来源：http://oq.jctech888.com.cn

Java: s.replaceAll("\\s+", "")
来源：http://kg.haigaiapp.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ic.szxytkj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ud.lnxyls.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vr.jctech888.com.cn

[E10] 左侧补零 / 定长填充
来源：http://jh.gzmigu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nk.asd995.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hj.panjiajie.cn

JS:   "7".padStart(3, "0")
来源：http://wd.nszjky.cn

TS:   "7".padStart(3, "0")
来源：http://qv.colortex.cn

Java: String.format("%03d", 7)
来源：http://jw.yuexingan06.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://vw.hnjuh.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://of.hahajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pk.szxytkj.cn

[E11] 反转字符串
来源：http://mu.shxzskj.cn

Py:   s[::-1]
来源：http://tf.9csxet.cn

PHP:  strrev($s);
来源：http://th.yuexingan06.cn

JS:   [...s].reverse().join("")
来源：http://rg.hnjuh.cn

TS:   [...s].reverse().join("")
来源：http://sl.szxytkj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ty.haigaiapp.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://hr.huanxung.cn

Ruby: s.reverse
来源：http://rh.chemitech.net.cn

C#:   new string(s.Reverse().ToArray())
来源：http://rv.newstarts.cn

[E12] 统计某字符出现次数
来源：http://oo.haigaiapp.cn

Py:   s.count("a")
来源：http://mc.haigaiapp.cn

PHP:  substr_count($s, "a");
来源：http://ea.9csxet.cn

JS:   s.split("a").length - 1
来源：http://im.jctech888.com.cn

TS:   s.split("a").length - 1
来源：http://jf.yuntaijiaju.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xo.panjiajie.cn

Go:   strings.Count(s, "a")
来源：http://gk.9csxet.cn

Ruby: s.count("a")
来源：http://aa.shxzskj.cn

C#:   s.Count(c => c == 'a')
来源：http://pr.shxzskj.cn

[E13] 逐字符遍历
来源：http://ou.nicolike.cn

Py:   for ch in s: print(ch)
来源：http://xr.szsharing.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fm.hnjuh.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://oa.newstarts.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://po.lnxyls.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ov.jctech888.com.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bk.nszjky.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://im.asd995.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kf.panjiajie.cn

[E14] URL 编码与 Base64
来源：http://di.szxytkj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qw.asd995.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qe.szsharing.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ig.yuntaijiaju.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ou.yuexingan06.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://by.colortex.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zg.shtwfgs.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://so.chemitech.net.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wc.521024.cn

[E15] HTML 转义 / 反转义
来源：http://or.hnjuh.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://go.521024.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wm.szsharing.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wp.szxytkj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ti.szxytkj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ut.szxytkj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jj.hnjuh.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vg.huanxung.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bl.jctech888.com.cn

[E16] 数字千分位
来源：http://do.chemitech.net.cn

Py:   f"{1234567:,}"
来源：http://is.bjjhwx.cn

PHP:  number_format(1234567);
来源：http://ox.haigaiapp.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://qq.521024.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://fh.nicolike.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tw.huixiangedu.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yy.yuexingan06.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xz.shxzukj.cn

C#:   1234567.ToString("N0")
来源：http://yv.wgjwhj.cn

[E17] 首字母大写
来源：http://jp.huanxung.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ft.bookmarksfly.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://pv.nszjky.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uv.shxzukj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vt.muxihuayi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zs.lnxyls.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vi.szxytkj.cn

Ruby: s.capitalize
来源：http://fc.huixiangedu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ah.haigaiapp.cn

[E18] 模板占位符替换
来源：http://ym.huanxung.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lw.colortex.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ru.muxihuayi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://po.jianghongdianzi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://sd.shtwfgs.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://an.shxzskj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ni.chemitech.net.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fl.colortex.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zq.huixinmuqiang.cn

[E19] 多行文本按行拆分
来源：http://rh.muxihuayi.cn

Py:   s.splitlines()
来源：http://ql.jctech888.com.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mt.jianghongdianzi.cn

JS:   s.split(/\r?\n/)
来源：http://ri.lnxyls.cn

TS:   s.split(/\r?\n/)
来源：http://ei.hahajie.cn

Java: s.lines().toList()
来源：http://yo.nszjky.cn

Go:   strings.Split(s, "\n")
来源：http://rs.haigaiapp.cn

Ruby: s.lines
来源：http://yf.panjiajie.cn

C#:   s.Split('\n')
来源：http://oc.asd995.cn

[E20] 判断字符串是否为空
来源：http://xg.wgjwhj.cn

Py:   if not s:
来源：http://kx.szxytkj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xn.yuexingan06.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xd.wgjwhj.cn

TS:   if (s === "") {}
来源：http://qb.9csxet.cn

Java: if (s.isEmpty()) {}
来源：http://gh.huixinmuqiang.cn

Go:   if s == "" {}
来源：http://lm.colortex.cn

Ruby: if s.empty?
来源：http://kk.colortex.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://be.nicolike.cn

[E21] 超长截断加省略号
来源：http://be.bjjhwx.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kj.chemitech.net.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vb.shxzukj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bn.huixiangedu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://to.huixiangedu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zv.panjiajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://ww.huixinmuqiang.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lp.hahajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cp.yuexingan06.cn

[E22] 字节长度与字符长度
来源：http://dk.huixinmuqiang.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qj.szsharing.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hb.nicolike.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lw.yuexingan06.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lc.chemitech.net.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ll.bookmarksfly.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rs.shxzskj.cn

Ruby: s.bytesize;  s.length
来源：http://xm.haigaiapp.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://os.hnjuh.cn

================================================================================
来源：http://vu.szsharing.cn

F. 文件与目录
来源：http://yy.huanxung.cn

================================================================================
来源：http://ea.muxihuayi.cn

[F01] 读取整个文件
来源：http://fp.szsharing.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://br.shtwfgs.cn

PHP:  file_get_contents("a.txt");
来源：http://ub.yuexingan06.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pr.gzmigu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lb.newstarts.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://kv.muxihuayi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ur.muxihuayi.cn

Ruby: File.read("a.txt")
来源：http://es.nicolike.cn

C#:   File.ReadAllText("a.txt");
来源：http://de.chemitech.net.cn

[F02] 逐行读取文件
来源：http://eg.chemitech.net.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lz.szxytkj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ru.szsharing.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oe.asd995.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ex.huixinmuqiang.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ba.colortex.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nn.shxzukj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bj.haigaiapp.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xp.shxzukj.cn

[F03] 写入文件（覆盖）
来源：http://mh.newstarts.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ar.nicolike.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ll.huixiangedu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ys.jctech888.com.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lb.huanxung.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wd.szsharing.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hw.jctech888.com.cn

Ruby: File.write("a.txt", "hi")
来源：http://ux.huanxung.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tr.bjjhwx.cn

[F04] 追加写入文件
来源：http://oi.haigaiapp.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sh.jctech888.com.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zm.newstarts.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sg.jianghongdianzi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ca.lnxyls.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sj.jianghongdianzi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nv.gzmigu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://sp.huixinmuqiang.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dm.nszjky.cn

[F05] 判断文件或目录是否存在
来源：http://yf.yuntaijiaju.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bs.bjjhwx.cn

PHP:  file_exists("a.txt");
来源：http://oe.jctech888.com.cn

JS:   fs.existsSync("a.txt")
来源：http://hh.shtwfgs.cn

TS:   fs.existsSync("a.txt")
来源：http://dt.shxzskj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://no.bookmarksfly.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://af.huixiangedu.cn

Ruby: File.exist?("a.txt")
来源：http://jz.colortex.cn

C#:   File.Exists("a.txt")
来源：http://hx.szsharing.cn

[F06] 删除文件
来源：http://um.9csxet.cn

Py:   os.remove("a.txt")
来源：http://rj.asd995.cn

PHP:  unlink("a.txt");
来源：http://uy.shxzukj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://kh.yuntaijiaju.cn

TS:   fs.unlinkSync("a.txt")
来源：http://eh.shtwfgs.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ib.haigaiapp.cn

Go:   os.Remove("a.txt")
来源：http://ke.shxzskj.cn


<!-- 参考信息 -->