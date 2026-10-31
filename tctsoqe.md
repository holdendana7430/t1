代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://as.bookmarksfly.cn

JS:   arr.includes(x)
来源：http://nh.chemitech.net.cn

TS:   arr.includes(x)
来源：http://zz.haigaiapp.cn

Java: list.contains(x)
来源：http://fn.jctech888.com.cn

Go:   slices.Contains(arr, x)
来源：http://qd.yuntaijiaju.cn

Ruby: arr.include?(x)
来源：http://tw.newstarts.cn

C#:   list.Contains(x)
来源：http://ao.wgjwhj.cn

[D22] 复制数组（避免共享引用）
来源：http://ca.hahajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tj.yuexingan06.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lw.haigaiapp.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bp.bjjhwx.cn

TS:   [...arr];
来源：http://el.chemitech.net.cn

Java: new ArrayList<>(list);
来源：http://yf.huanxung.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ii.shxzskj.cn

Ruby: arr.dup;  arr.clone
来源：http://vt.nszjky.cn

C#:   new List<int>(list);
来源：http://eu.hahajie.cn

[D23] reduce 累积计算
来源：http://yh.shtwfgs.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kl.haigaiapp.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://np.chemitech.net.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jr.colortex.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zk.yuexingan06.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://hs.shxzukj.cn

Go:   // 手写循环
来源：http://dr.chemitech.net.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://as.yuexingan06.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ea.bookmarksfly.cn

[D24] 字典 / Map 基本操作
来源：http://nw.haigaiapp.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fd.yuexingan06.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dq.chemitech.net.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://eb.lnxyls.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jo.hahajie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vd.szsharing.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jw.shxzskj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://uv.jctech888.com.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ec.shtwfgs.cn

[D25] Set 集合去重与交并差
来源：http://ym.hnjuh.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wy.shxzukj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ph.huanxung.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vu.jianghongdianzi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yq.bjjhwx.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sx.szsharing.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ih.chemitech.net.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kk.nicolike.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ps.yuntaijiaju.cn

[D26] 数组转字符串
来源：http://dg.shtwfgs.cn

Py:   ", ".join(map(str, arr))
来源：http://ib.shtwfgs.cn

PHP:  implode(", ", $arr);
来源：http://pz.lnxyls.cn

JS:   arr.join(", ")
来源：http://nf.newstarts.cn

TS:   arr.join(", ")
来源：http://ww.nicolike.cn

Java: String.join(", ", list)
来源：http://hc.newstarts.cn

Go:   strings.Join(strs, ", ")
来源：http://fk.huixiangedu.cn

Ruby: arr.join(", ")
来源：http://zg.huixiangedu.cn

C#:   string.Join(", ", list)
来源：http://al.szsharing.cn

================================================================================
来源：http://pe.chemitech.net.cn

E. 字符串处理
来源：http://ou.bookmarksfly.cn

================================================================================
来源：http://qh.nicolike.cn

[E01] 拼接字符串
来源：http://cl.szxytkj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://on.muxihuayi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rq.asd995.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ek.szsharing.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bc.bjjhwx.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yn.521024.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sm.yuexingan06.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tk.9csxet.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ad.hnjuh.cn

[E02] 重复字符串
来源：http://zc.chemitech.net.cn

Py:   "ab" * 3
来源：http://yw.gzmigu.cn

PHP:  str_repeat("ab", 3);
来源：http://nw.lnxyls.cn

JS:   "ab".repeat(3)
来源：http://ii.shxzukj.cn

TS:   "ab".repeat(3)
来源：http://uw.jianghongdianzi.cn

Java: "ab".repeat(3)
来源：http://gd.lnxyls.cn

Go:   strings.Repeat("ab", 3)
来源：http://xe.muxihuayi.cn

Ruby: "ab" * 3
来源：http://do.9csxet.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lh.bookmarksfly.cn

[E03] 截取子串
来源：http://iq.521024.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ac.szxytkj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://un.huixinmuqiang.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ar.bookmarksfly.cn

TS:   s.slice(1, 4)
来源：http://rb.521024.cn

Java: s.substring(1, 4)
来源：http://oc.gzmigu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rd.asd995.cn

Ruby: s[1, 3];  s[1..3]
来源：http://en.huanxung.cn

C#:   s.Substring(1, 3)
来源：http://jy.521024.cn

[E04] 查找子串位置
来源：http://ng.hnjuh.cn

Py:   s.find("x");  s.index("x")
来源：http://ex.chemitech.net.cn

PHP:  strpos($s, "x");
来源：http://vz.muxihuayi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://an.jctech888.com.cn

TS:   s.indexOf("x")
来源：http://eu.haigaiapp.cn

Java: s.indexOf("x")
来源：http://es.shxzukj.cn

Go:   strings.Index(s, "x")
来源：http://qs.muxihuayi.cn

Ruby: s.index("x")
来源：http://fa.521024.cn

C#:   s.IndexOf("x")
来源：http://jx.shxzskj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://tf.panjiajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gi.shxzukj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pu.9csxet.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://eg.hnjuh.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://pj.hnjuh.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kw.shxzskj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qn.9csxet.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bz.haigaiapp.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vr.muxihuayi.cn

[E06] 替换子串
来源：http://wc.hahajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ev.asd995.cn

PHP:  str_replace("a", "b", $s);
来源：http://ed.szsharing.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://go.hahajie.cn

TS:   s.replaceAll("a", "b")
来源：http://vn.bookmarksfly.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vd.chemitech.net.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mb.huixiangedu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dx.newstarts.cn

C#:   s.Replace("a", "b")
来源：http://zu.szxytkj.cn

[E07] 按分隔符拆分
来源：http://nt.colortex.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gu.muxihuayi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yn.nszjky.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://nq.wgjwhj.cn

TS:   s.split(",")
来源：http://ni.hnjuh.cn

Java: s.split(",");  s.split("\\s+")
来源：http://kx.szxytkj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://uu.jianghongdianzi.cn

Ruby: s.split(",");  s.split
来源：http://pr.shxzukj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mz.yuexingan06.cn

[E08] 数组按分隔符合并
来源：http://nm.yuntaijiaju.cn

Py:   ",".join(items)
来源：http://dz.asd995.cn

PHP:  implode(",", $items);
来源：http://yf.bjjhwx.cn

JS:   items.join(",")
来源：http://to.yuexingan06.cn

TS:   items.join(",")
来源：http://be.lnxyls.cn

Java: String.join(",", items)
来源：http://ov.haigaiapp.cn

Go:   strings.Join(items, ",")
来源：http://wy.huixinmuqiang.cn

Ruby: items.join(",")
来源：http://nd.szsharing.cn

C#:   string.Join(",", items)
来源：http://ti.muxihuayi.cn

[E09] 去除所有空白字符
来源：http://sx.9csxet.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qj.colortex.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yy.gzmigu.cn

JS:   s.replace(/\s+/g, "")
来源：http://ri.chemitech.net.cn

TS:   s.replace(/\s+/g, "")
来源：http://ru.huanxung.cn

Java: s.replaceAll("\\s+", "")
来源：http://bj.hahajie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://sh.huixinmuqiang.cn

Ruby: s.gsub(/\s+/, "")
来源：http://gz.hahajie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ze.huixinmuqiang.cn

[E10] 左侧补零 / 定长填充
来源：http://ph.bjjhwx.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pq.huanxung.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vy.muxihuayi.cn

JS:   "7".padStart(3, "0")
来源：http://fl.huanxung.cn

TS:   "7".padStart(3, "0")
来源：http://ge.shxzskj.cn

Java: String.format("%03d", 7)
来源：http://vx.szsharing.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://mu.shxzukj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cu.yuexingan06.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fc.yuntaijiaju.cn

[E11] 反转字符串
来源：http://mw.shxzskj.cn

Py:   s[::-1]
来源：http://jl.chemitech.net.cn

PHP:  strrev($s);
来源：http://kl.newstarts.cn

JS:   [...s].reverse().join("")
来源：http://qn.wgjwhj.cn

TS:   [...s].reverse().join("")
来源：http://fo.jianghongdianzi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ok.colortex.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://eg.huixinmuqiang.cn

Ruby: s.reverse
来源：http://dc.jianghongdianzi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://fv.haigaiapp.cn

[E12] 统计某字符出现次数
来源：http://qw.gzmigu.cn

Py:   s.count("a")
来源：http://rs.jianghongdianzi.cn

PHP:  substr_count($s, "a");
来源：http://ym.muxihuayi.cn

JS:   s.split("a").length - 1
来源：http://el.jianghongdianzi.cn

TS:   s.split("a").length - 1
来源：http://an.lnxyls.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nf.hahajie.cn

Go:   strings.Count(s, "a")
来源：http://dj.panjiajie.cn

Ruby: s.count("a")
来源：http://mo.jianghongdianzi.cn

C#:   s.Count(c => c == 'a')
来源：http://no.wgjwhj.cn

[E13] 逐字符遍历
来源：http://cm.hnjuh.cn

Py:   for ch in s: print(ch)
来源：http://iu.hnjuh.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ax.yuntaijiaju.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://gs.jctech888.com.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://tg.hnjuh.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rz.newstarts.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://im.wgjwhj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://im.huixiangedu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zc.yuexingan06.cn

[E14] URL 编码与 Base64
来源：http://ny.lnxyls.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fu.wgjwhj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ph.huixinmuqiang.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xs.wgjwhj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lq.muxihuayi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://sy.szxytkj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lr.521024.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uh.huixinmuqiang.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dh.nszjky.cn

[E15] HTML 转义 / 反转义
来源：http://ke.colortex.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://gr.szxytkj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gs.hnjuh.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ys.chemitech.net.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ni.huixiangedu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tk.haigaiapp.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ot.huixiangedu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ew.bookmarksfly.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ew.asd995.cn

[E16] 数字千分位
来源：http://ho.nicolike.cn

Py:   f"{1234567:,}"
来源：http://cd.panjiajie.cn

PHP:  number_format(1234567);
来源：http://uw.jctech888.com.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vv.huixiangedu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://fg.wgjwhj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qh.newstarts.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ik.szxytkj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ri.chemitech.net.cn

C#:   1234567.ToString("N0")
来源：http://rl.panjiajie.cn

[E17] 首字母大写
来源：http://fd.asd995.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qs.shtwfgs.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://mx.chemitech.net.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zp.bjjhwx.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jy.bjjhwx.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zl.nszjky.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://my.nicolike.cn

Ruby: s.capitalize
来源：http://oq.jctech888.com.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tq.szxytkj.cn

[E18] 模板占位符替换
来源：http://xr.haigaiapp.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gf.jctech888.com.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kh.521024.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://li.huixiangedu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ua.jianghongdianzi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://db.yuntaijiaju.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ac.panjiajie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nl.yuntaijiaju.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wj.huixinmuqiang.cn

[E19] 多行文本按行拆分
来源：http://iy.panjiajie.cn

Py:   s.splitlines()
来源：http://ul.muxihuayi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yn.shxzskj.cn

JS:   s.split(/\r?\n/)
来源：http://er.jctech888.com.cn

TS:   s.split(/\r?\n/)
来源：http://zg.521024.cn

Java: s.lines().toList()
来源：http://eq.szxytkj.cn

Go:   strings.Split(s, "\n")
来源：http://jq.521024.cn

Ruby: s.lines
来源：http://dm.haigaiapp.cn

C#:   s.Split('\n')
来源：http://zu.huanxung.cn

[E20] 判断字符串是否为空
来源：http://wr.yuntaijiaju.cn

Py:   if not s:
来源：http://ba.hnjuh.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://oh.haigaiapp.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ah.gzmigu.cn

TS:   if (s === "") {}
来源：http://rv.9csxet.cn

Java: if (s.isEmpty()) {}
来源：http://mq.jianghongdianzi.cn

Go:   if s == "" {}
来源：http://pe.chemitech.net.cn

Ruby: if s.empty?
来源：http://mg.hahajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hr.521024.cn

[E21] 超长截断加省略号
来源：http://ur.jctech888.com.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pf.szsharing.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zw.9csxet.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://of.yuntaijiaju.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ko.yuexingan06.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://sw.gzmigu.cn

Go:   // 按 rune 判断长度后截断
来源：http://tr.nicolike.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vr.haigaiapp.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rs.521024.cn

[E22] 字节长度与字符长度
来源：http://wm.asd995.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lo.hahajie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dp.shtwfgs.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://np.hnjuh.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kg.521024.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nq.hnjuh.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vk.haigaiapp.cn

Ruby: s.bytesize;  s.length
来源：http://ty.521024.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xe.szxytkj.cn

================================================================================
来源：http://gb.haigaiapp.cn

F. 文件与目录
来源：http://zz.hahajie.cn

================================================================================
来源：http://oq.szxytkj.cn

[F01] 读取整个文件
来源：http://mn.jianghongdianzi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://iq.9csxet.cn

PHP:  file_get_contents("a.txt");
来源：http://zv.haigaiapp.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://np.yuexingan06.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ys.szxytkj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ut.hahajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qp.haigaiapp.cn

Ruby: File.read("a.txt")
来源：http://le.nszjky.cn

C#:   File.ReadAllText("a.txt");
来源：http://pp.szxytkj.cn

[F02] 逐行读取文件
来源：http://fl.jctech888.com.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ou.szsharing.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sy.szxytkj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jm.hahajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ry.9csxet.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sq.yuexingan06.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://uq.yuexingan06.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://td.wgjwhj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vv.huixiangedu.cn

[F03] 写入文件（覆盖）
来源：http://cz.hahajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zu.hahajie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://iq.newstarts.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vi.bjjhwx.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vz.bjjhwx.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://li.jctech888.com.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ab.hahajie.cn

Ruby: File.write("a.txt", "hi")
来源：http://ze.panjiajie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://av.lnxyls.cn

[F04] 追加写入文件
来源：http://qt.szsharing.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://oa.muxihuayi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hk.yuntaijiaju.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kg.panjiajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oq.nicolike.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://un.hnjuh.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wx.newstarts.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zq.shxzskj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pr.shtwfgs.cn

[F05] 判断文件或目录是否存在
来源：http://ve.521024.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://le.hahajie.cn

PHP:  file_exists("a.txt");
来源：http://uo.shtwfgs.cn

JS:   fs.existsSync("a.txt")
来源：http://zi.huixiangedu.cn

TS:   fs.existsSync("a.txt")
来源：http://wq.gzmigu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hu.gzmigu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qq.huixinmuqiang.cn

Ruby: File.exist?("a.txt")
来源：http://ij.jianghongdianzi.cn


<!-- 参考信息 -->