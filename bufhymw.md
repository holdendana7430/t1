代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xj.jianghongdianzi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wi.huixinmuqiang.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qt.521024.cn

TS:   [...arr];
来源：http://ud.lnxyls.cn

Java: new ArrayList<>(list);
来源：http://od.yuntaijiaju.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ya.haigaiapp.cn

Ruby: arr.dup;  arr.clone
来源：http://xq.shxzskj.cn

C#:   new List<int>(list);
来源：http://yk.asd995.cn

[D23] reduce 累积计算
来源：http://yt.newstarts.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gr.huanxung.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bd.jctech888.com.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oh.newstarts.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nk.chemitech.net.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ey.gzmigu.cn

Go:   // 手写循环
来源：http://hp.haigaiapp.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hc.szxytkj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zd.huixiangedu.cn

[D24] 字典 / Map 基本操作
来源：http://mk.521024.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zj.huanxung.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yc.gzmigu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ym.hnjuh.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vv.huixinmuqiang.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mp.yuexingan06.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yr.jctech888.com.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fx.nszjky.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zf.shxzukj.cn

[D25] Set 集合去重与交并差
来源：http://kj.bookmarksfly.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vq.panjiajie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kn.szsharing.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wb.shtwfgs.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qh.shtwfgs.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sx.nicolike.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gg.wgjwhj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fm.521024.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yt.lnxyls.cn

[D26] 数组转字符串
来源：http://ys.shxzskj.cn

Py:   ", ".join(map(str, arr))
来源：http://rj.szsharing.cn

PHP:  implode(", ", $arr);
来源：http://ww.szxytkj.cn

JS:   arr.join(", ")
来源：http://rj.jctech888.com.cn

TS:   arr.join(", ")
来源：http://yo.shtwfgs.cn

Java: String.join(", ", list)
来源：http://xt.huixiangedu.cn

Go:   strings.Join(strs, ", ")
来源：http://cj.hnjuh.cn

Ruby: arr.join(", ")
来源：http://rq.bjjhwx.cn

C#:   string.Join(", ", list)
来源：http://je.gzmigu.cn

================================================================================
来源：http://cr.huixinmuqiang.cn

E. 字符串处理
来源：http://iw.yuexingan06.cn

================================================================================
来源：http://gs.newstarts.cn

[E01] 拼接字符串
来源：http://vy.huixinmuqiang.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jm.shxzskj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xo.hahajie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ks.bookmarksfly.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kx.hnjuh.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hy.huixiangedu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rj.521024.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ia.wgjwhj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ex.huixinmuqiang.cn

[E02] 重复字符串
来源：http://eq.521024.cn

Py:   "ab" * 3
来源：http://na.newstarts.cn

PHP:  str_repeat("ab", 3);
来源：http://tm.hnjuh.cn

JS:   "ab".repeat(3)
来源：http://ii.yuntaijiaju.cn

TS:   "ab".repeat(3)
来源：http://en.yuexingan06.cn

Java: "ab".repeat(3)
来源：http://ue.jianghongdianzi.cn

Go:   strings.Repeat("ab", 3)
来源：http://pj.shxzukj.cn

Ruby: "ab" * 3
来源：http://bd.huixinmuqiang.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://se.szxytkj.cn

[E03] 截取子串
来源：http://nt.yuexingan06.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fj.shtwfgs.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ap.bjjhwx.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ub.yuntaijiaju.cn

TS:   s.slice(1, 4)
来源：http://ck.hahajie.cn

Java: s.substring(1, 4)
来源：http://hz.shxzukj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://eb.asd995.cn

Ruby: s[1, 3];  s[1..3]
来源：http://sw.huanxung.cn

C#:   s.Substring(1, 3)
来源：http://uv.jianghongdianzi.cn

[E04] 查找子串位置
来源：http://xn.shtwfgs.cn

Py:   s.find("x");  s.index("x")
来源：http://vx.huanxung.cn

PHP:  strpos($s, "x");
来源：http://bk.bookmarksfly.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://li.wgjwhj.cn

TS:   s.indexOf("x")
来源：http://nh.shxzukj.cn

Java: s.indexOf("x")
来源：http://sd.haigaiapp.cn

Go:   strings.Index(s, "x")
来源：http://db.colortex.cn

Ruby: s.index("x")
来源：http://rv.huanxung.cn

C#:   s.IndexOf("x")
来源：http://mg.colortex.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ke.gzmigu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rz.nicolike.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://gr.chemitech.net.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yd.chemitech.net.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://yc.yuexingan06.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bw.521024.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ji.colortex.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lq.wgjwhj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ml.yuexingan06.cn

[E06] 替换子串
来源：http://sv.huixinmuqiang.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tb.9csxet.cn

PHP:  str_replace("a", "b", $s);
来源：http://zs.newstarts.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tq.szxytkj.cn

TS:   s.replaceAll("a", "b")
来源：http://lb.521024.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://po.huanxung.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gx.huixinmuqiang.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gm.jctech888.com.cn

C#:   s.Replace("a", "b")
来源：http://cb.panjiajie.cn

[E07] 按分隔符拆分
来源：http://ji.chemitech.net.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jn.hahajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jz.shtwfgs.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://sa.asd995.cn

TS:   s.split(",")
来源：http://lq.newstarts.cn

Java: s.split(",");  s.split("\\s+")
来源：http://kf.huanxung.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xv.chemitech.net.cn

Ruby: s.split(",");  s.split
来源：http://ot.nszjky.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qh.haigaiapp.cn

[E08] 数组按分隔符合并
来源：http://iw.szsharing.cn

Py:   ",".join(items)
来源：http://px.szxytkj.cn

PHP:  implode(",", $items);
来源：http://qh.huixiangedu.cn

JS:   items.join(",")
来源：http://za.asd995.cn

TS:   items.join(",")
来源：http://ay.muxihuayi.cn

Java: String.join(",", items)
来源：http://lj.asd995.cn

Go:   strings.Join(items, ",")
来源：http://yd.muxihuayi.cn

Ruby: items.join(",")
来源：http://bg.shtwfgs.cn

C#:   string.Join(",", items)
来源：http://ot.bookmarksfly.cn

[E09] 去除所有空白字符
来源：http://jf.hnjuh.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ol.shxzukj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tb.shxzskj.cn

JS:   s.replace(/\s+/g, "")
来源：http://kc.nicolike.cn

TS:   s.replace(/\s+/g, "")
来源：http://sj.hnjuh.cn

Java: s.replaceAll("\\s+", "")
来源：http://qg.newstarts.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://iy.yuntaijiaju.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ef.nicolike.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xd.521024.cn

[E10] 左侧补零 / 定长填充
来源：http://li.szsharing.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vv.shxzukj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qc.521024.cn

JS:   "7".padStart(3, "0")
来源：http://kc.9csxet.cn

TS:   "7".padStart(3, "0")
来源：http://sj.9csxet.cn

Java: String.format("%03d", 7)
来源：http://gm.jctech888.com.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://li.asd995.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zz.hahajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ru.lnxyls.cn

[E11] 反转字符串
来源：http://di.huanxung.cn

Py:   s[::-1]
来源：http://pn.haigaiapp.cn

PHP:  strrev($s);
来源：http://dn.jctech888.com.cn

JS:   [...s].reverse().join("")
来源：http://je.haigaiapp.cn

TS:   [...s].reverse().join("")
来源：http://ua.shtwfgs.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://kp.huixiangedu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ib.gzmigu.cn

Ruby: s.reverse
来源：http://tc.jianghongdianzi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://op.szxytkj.cn

[E12] 统计某字符出现次数
来源：http://vl.shxzukj.cn

Py:   s.count("a")
来源：http://aq.huixiangedu.cn

PHP:  substr_count($s, "a");
来源：http://fo.huixiangedu.cn

JS:   s.split("a").length - 1
来源：http://uh.colortex.cn

TS:   s.split("a").length - 1
来源：http://aj.panjiajie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ez.yuexingan06.cn

Go:   strings.Count(s, "a")
来源：http://fv.bjjhwx.cn

Ruby: s.count("a")
来源：http://ro.colortex.cn

C#:   s.Count(c => c == 'a')
来源：http://vo.nszjky.cn

[E13] 逐字符遍历
来源：http://vq.gzmigu.cn

Py:   for ch in s: print(ch)
来源：http://fw.hahajie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ev.yuntaijiaju.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ag.huixinmuqiang.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://he.shtwfgs.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://st.newstarts.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://eq.szsharing.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://qi.shxzukj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://at.yuexingan06.cn

[E14] URL 编码与 Base64
来源：http://kv.jianghongdianzi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zq.shxzskj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ch.9csxet.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fn.panjiajie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cg.muxihuayi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gd.nszjky.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mj.szxytkj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bm.chemitech.net.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gz.yuntaijiaju.cn

[E15] HTML 转义 / 反转义
来源：http://gm.jianghongdianzi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://sb.hahajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dy.521024.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ic.jianghongdianzi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://lu.lnxyls.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ku.521024.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zg.szxytkj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tx.muxihuayi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fm.9csxet.cn

[E16] 数字千分位
来源：http://sh.9csxet.cn

Py:   f"{1234567:,}"
来源：http://ps.shtwfgs.cn

PHP:  number_format(1234567);
来源：http://dh.521024.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://qt.hnjuh.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://uo.newstarts.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qn.muxihuayi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://aq.9csxet.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gs.bjjhwx.cn

C#:   1234567.ToString("N0")
来源：http://no.huixiangedu.cn

[E17] 首字母大写
来源：http://dp.jctech888.com.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://uw.9csxet.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://vz.yuexingan06.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vx.shxzskj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vy.szsharing.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zq.yuntaijiaju.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://uq.chemitech.net.cn

Ruby: s.capitalize
来源：http://kx.szxytkj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://md.hnjuh.cn

[E18] 模板占位符替换
来源：http://wm.bjjhwx.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ls.wgjwhj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://us.9csxet.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ds.yuntaijiaju.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ta.hahajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fz.szsharing.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gm.szxytkj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gu.chemitech.net.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://aa.shxzskj.cn

[E19] 多行文本按行拆分
来源：http://ls.hahajie.cn

Py:   s.splitlines()
来源：http://xe.nszjky.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://br.newstarts.cn

JS:   s.split(/\r?\n/)
来源：http://hb.bjjhwx.cn

TS:   s.split(/\r?\n/)
来源：http://hh.gzmigu.cn

Java: s.lines().toList()
来源：http://uu.bookmarksfly.cn

Go:   strings.Split(s, "\n")
来源：http://qt.jctech888.com.cn

Ruby: s.lines
来源：http://ep.yuexingan06.cn

C#:   s.Split('\n')
来源：http://wm.chemitech.net.cn

[E20] 判断字符串是否为空
来源：http://ym.lnxyls.cn

Py:   if not s:
来源：http://yb.colortex.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nb.jctech888.com.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vq.shxzukj.cn

TS:   if (s === "") {}
来源：http://as.colortex.cn

Java: if (s.isEmpty()) {}
来源：http://fu.gzmigu.cn

Go:   if s == "" {}
来源：http://ci.huixinmuqiang.cn

Ruby: if s.empty?
来源：http://vr.shxzukj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wy.nicolike.cn

[E21] 超长截断加省略号
来源：http://vq.huixinmuqiang.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hp.9csxet.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wg.lnxyls.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ru.yuntaijiaju.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pc.9csxet.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yy.szxytkj.cn

Go:   // 按 rune 判断长度后截断
来源：http://tl.gzmigu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ty.colortex.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://iv.newstarts.cn

[E22] 字节长度与字符长度
来源：http://zo.bookmarksfly.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nt.521024.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fq.nicolike.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fd.szxytkj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bc.nicolike.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nh.jctech888.com.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ip.chemitech.net.cn

Ruby: s.bytesize;  s.length
来源：http://jk.wgjwhj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uu.colortex.cn

================================================================================
来源：http://ot.wgjwhj.cn

F. 文件与目录
来源：http://rb.521024.cn

================================================================================
来源：http://dq.szxytkj.cn

[F01] 读取整个文件
来源：http://hn.hahajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yh.asd995.cn

PHP:  file_get_contents("a.txt");
来源：http://cx.lnxyls.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kn.huixinmuqiang.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hx.gzmigu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://yp.haigaiapp.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fa.shxzukj.cn

Ruby: File.read("a.txt")
来源：http://pf.panjiajie.cn

C#:   File.ReadAllText("a.txt");
来源：http://nd.jianghongdianzi.cn

[F02] 逐行读取文件
来源：http://ls.muxihuayi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jk.muxihuayi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nl.chemitech.net.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nh.gzmigu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ms.gzmigu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://az.nszjky.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pr.hnjuh.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cd.szxytkj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ug.chemitech.net.cn

[F03] 写入文件（覆盖）
来源：http://ll.lnxyls.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dy.huanxung.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://sb.lnxyls.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yp.colortex.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jc.asd995.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://sg.shxzukj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zt.nicolike.cn

Ruby: File.write("a.txt", "hi")
来源：http://nz.szxytkj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vr.shtwfgs.cn

[F04] 追加写入文件
来源：http://bx.szsharing.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jx.shxzukj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://sx.szxytkj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rj.huixiangedu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ns.yuntaijiaju.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uw.asd995.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ml.shxzukj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://px.yuntaijiaju.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ku.huixiangedu.cn

[F05] 判断文件或目录是否存在
来源：http://vs.haigaiapp.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://sr.jianghongdianzi.cn

PHP:  file_exists("a.txt");
来源：http://wd.shxzskj.cn

JS:   fs.existsSync("a.txt")
来源：http://zo.huixiangedu.cn

TS:   fs.existsSync("a.txt")
来源：http://ua.nszjky.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ci.shxzukj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ej.huixinmuqiang.cn

Ruby: File.exist?("a.txt")
来源：http://fc.yuntaijiaju.cn

C#:   File.Exists("a.txt")
来源：http://ch.colortex.cn

[F06] 删除文件
来源：http://tz.nicolike.cn

Py:   os.remove("a.txt")
来源：http://je.jianghongdianzi.cn

PHP:  unlink("a.txt");
来源：http://mh.szxytkj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://pl.wgjwhj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://od.wgjwhj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rt.wgjwhj.cn

Go:   os.Remove("a.txt")
来源：http://ae.szxytkj.cn


<!-- 参考信息 -->