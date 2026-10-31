代发 wailian999

Ruby: arr.tally
来源：http://qd.hahajie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ws.yuntaijiaju.cn

[D21] 判断是否包含某元素
来源：http://gd.szxytkj.cn

Py:   x in arr
来源：http://rn.newstarts.cn

PHP:  in_array($x, $arr, true);
来源：http://qf.huixinmuqiang.cn

JS:   arr.includes(x)
来源：http://yp.huanxung.cn

TS:   arr.includes(x)
来源：http://om.muxihuayi.cn

Java: list.contains(x)
来源：http://by.lnxyls.cn

Go:   slices.Contains(arr, x)
来源：http://kt.hnjuh.cn

Ruby: arr.include?(x)
来源：http://wk.yuntaijiaju.cn

C#:   list.Contains(x)
来源：http://no.bjjhwx.cn

[D22] 复制数组（避免共享引用）
来源：http://xs.gzmigu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qj.szxytkj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ee.huixinmuqiang.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gy.nicolike.cn

TS:   [...arr];
来源：http://hj.colortex.cn

Java: new ArrayList<>(list);
来源：http://si.chemitech.net.cn

Go:   copied := append([]int(nil), arr...)
来源：http://hl.panjiajie.cn

Ruby: arr.dup;  arr.clone
来源：http://eq.chemitech.net.cn

C#:   new List<int>(list);
来源：http://ww.shxzskj.cn

[D23] reduce 累积计算
来源：http://fb.huixinmuqiang.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bo.wgjwhj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yn.wgjwhj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ut.lnxyls.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mo.lnxyls.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xd.shxzskj.cn

Go:   // 手写循环
来源：http://gl.yuntaijiaju.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ej.bookmarksfly.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pw.gzmigu.cn

[D24] 字典 / Map 基本操作
来源：http://gc.szxytkj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rv.shxzukj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fr.huixiangedu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lk.szxytkj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vv.jianghongdianzi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zb.shxzskj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zf.521024.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qu.colortex.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zv.shtwfgs.cn

[D25] Set 集合去重与交并差
来源：http://ij.lnxyls.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ms.521024.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ik.nszjky.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mw.jctech888.com.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bg.shtwfgs.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dp.hnjuh.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://de.muxihuayi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zy.gzmigu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ef.9csxet.cn

[D26] 数组转字符串
来源：http://ju.bookmarksfly.cn

Py:   ", ".join(map(str, arr))
来源：http://rm.9csxet.cn

PHP:  implode(", ", $arr);
来源：http://mw.hahajie.cn

JS:   arr.join(", ")
来源：http://ck.newstarts.cn

TS:   arr.join(", ")
来源：http://wv.bjjhwx.cn

Java: String.join(", ", list)
来源：http://yl.jctech888.com.cn

Go:   strings.Join(strs, ", ")
来源：http://zs.huixiangedu.cn

Ruby: arr.join(", ")
来源：http://da.yuexingan06.cn

C#:   string.Join(", ", list)
来源：http://tg.nszjky.cn

================================================================================
来源：http://tm.huanxung.cn

E. 字符串处理
来源：http://pj.colortex.cn

================================================================================
来源：http://nx.colortex.cn

[E01] 拼接字符串
来源：http://jz.szsharing.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ob.panjiajie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://za.colortex.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hi.muxihuayi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ll.haigaiapp.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ag.hnjuh.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://te.jctech888.com.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sz.colortex.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kx.chemitech.net.cn

[E02] 重复字符串
来源：http://qe.yuntaijiaju.cn

Py:   "ab" * 3
来源：http://ug.jianghongdianzi.cn

PHP:  str_repeat("ab", 3);
来源：http://it.bjjhwx.cn

JS:   "ab".repeat(3)
来源：http://fe.shtwfgs.cn

TS:   "ab".repeat(3)
来源：http://qw.chemitech.net.cn

Java: "ab".repeat(3)
来源：http://pc.9csxet.cn

Go:   strings.Repeat("ab", 3)
来源：http://xj.9csxet.cn

Ruby: "ab" * 3
来源：http://sm.szsharing.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mr.shtwfgs.cn

[E03] 截取子串
来源：http://bw.chemitech.net.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lv.huanxung.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nc.9csxet.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wq.bookmarksfly.cn

TS:   s.slice(1, 4)
来源：http://vz.asd995.cn

Java: s.substring(1, 4)
来源：http://pw.huixiangedu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hq.chemitech.net.cn

Ruby: s[1, 3];  s[1..3]
来源：http://kz.nszjky.cn

C#:   s.Substring(1, 3)
来源：http://vh.hnjuh.cn

[E04] 查找子串位置
来源：http://td.chemitech.net.cn

Py:   s.find("x");  s.index("x")
来源：http://vj.bjjhwx.cn

PHP:  strpos($s, "x");
来源：http://ld.hahajie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://in.bjjhwx.cn

TS:   s.indexOf("x")
来源：http://vq.521024.cn

Java: s.indexOf("x")
来源：http://nd.hahajie.cn

Go:   strings.Index(s, "x")
来源：http://xf.nicolike.cn

Ruby: s.index("x")
来源：http://ue.jctech888.com.cn

C#:   s.IndexOf("x")
来源：http://hz.gzmigu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ar.asd995.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ym.szsharing.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xj.wgjwhj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://be.newstarts.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://kl.gzmigu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ie.jctech888.com.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://od.panjiajie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ar.shxzukj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ku.bjjhwx.cn

[E06] 替换子串
来源：http://hk.jianghongdianzi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://du.huixinmuqiang.cn

PHP:  str_replace("a", "b", $s);
来源：http://eh.muxihuayi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bo.yuntaijiaju.cn

TS:   s.replaceAll("a", "b")
来源：http://sc.bjjhwx.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://to.haigaiapp.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zu.haigaiapp.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gg.nicolike.cn

C#:   s.Replace("a", "b")
来源：http://fz.szsharing.cn

[E07] 按分隔符拆分
来源：http://kq.chemitech.net.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ng.shxzukj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ka.hnjuh.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ub.newstarts.cn

TS:   s.split(",")
来源：http://tv.lnxyls.cn

Java: s.split(",");  s.split("\\s+")
来源：http://af.521024.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xr.chemitech.net.cn

Ruby: s.split(",");  s.split
来源：http://bf.9csxet.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yp.chemitech.net.cn

[E08] 数组按分隔符合并
来源：http://dj.shxzskj.cn

Py:   ",".join(items)
来源：http://iu.521024.cn

PHP:  implode(",", $items);
来源：http://ap.jctech888.com.cn

JS:   items.join(",")
来源：http://zw.shxzukj.cn

TS:   items.join(",")
来源：http://ci.jctech888.com.cn

Java: String.join(",", items)
来源：http://vy.nicolike.cn

Go:   strings.Join(items, ",")
来源：http://mc.nicolike.cn

Ruby: items.join(",")
来源：http://um.nicolike.cn

C#:   string.Join(",", items)
来源：http://pj.asd995.cn

[E09] 去除所有空白字符
来源：http://ka.szsharing.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nc.shxzskj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ws.shtwfgs.cn

JS:   s.replace(/\s+/g, "")
来源：http://xm.newstarts.cn

TS:   s.replace(/\s+/g, "")
来源：http://gr.shxzukj.cn

Java: s.replaceAll("\\s+", "")
来源：http://br.lnxyls.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ed.asd995.cn

Ruby: s.gsub(/\s+/, "")
来源：http://hc.szsharing.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sz.newstarts.cn

[E10] 左侧补零 / 定长填充
来源：http://dv.haigaiapp.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dd.hnjuh.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ri.shtwfgs.cn

JS:   "7".padStart(3, "0")
来源：http://dy.nszjky.cn

TS:   "7".padStart(3, "0")
来源：http://sb.yuexingan06.cn

Java: String.format("%03d", 7)
来源：http://km.huixiangedu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://oy.lnxyls.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yc.hahajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://uh.yuntaijiaju.cn

[E11] 反转字符串
来源：http://gw.huixiangedu.cn

Py:   s[::-1]
来源：http://we.colortex.cn

PHP:  strrev($s);
来源：http://kh.hnjuh.cn

JS:   [...s].reverse().join("")
来源：http://vl.lnxyls.cn

TS:   [...s].reverse().join("")
来源：http://og.huixinmuqiang.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://es.colortex.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://cm.nicolike.cn

Ruby: s.reverse
来源：http://om.muxihuayi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://nn.szsharing.cn

[E12] 统计某字符出现次数
来源：http://hm.yuntaijiaju.cn

Py:   s.count("a")
来源：http://lx.nszjky.cn

PHP:  substr_count($s, "a");
来源：http://bg.szxytkj.cn

JS:   s.split("a").length - 1
来源：http://gc.chemitech.net.cn

TS:   s.split("a").length - 1
来源：http://qq.szxytkj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ow.jctech888.com.cn

Go:   strings.Count(s, "a")
来源：http://nl.gzmigu.cn

Ruby: s.count("a")
来源：http://xh.yuexingan06.cn

C#:   s.Count(c => c == 'a')
来源：http://cc.shxzskj.cn

[E13] 逐字符遍历
来源：http://hy.huixinmuqiang.cn

Py:   for ch in s: print(ch)
来源：http://lf.shxzskj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xm.bjjhwx.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://br.bjjhwx.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://mn.shxzukj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://au.hahajie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ne.asd995.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rd.bjjhwx.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ww.gzmigu.cn

[E14] URL 编码与 Base64
来源：http://ag.szxytkj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cg.bjjhwx.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://aw.asd995.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fu.shxzukj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://es.jctech888.com.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jz.shxzukj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gx.huanxung.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cm.muxihuayi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gs.lnxyls.cn

[E15] HTML 转义 / 反转义
来源：http://su.gzmigu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://yw.haigaiapp.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gr.haigaiapp.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nl.szxytkj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://tm.bjjhwx.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://oz.haigaiapp.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hr.huixiangedu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://di.panjiajie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hr.9csxet.cn

[E16] 数字千分位
来源：http://sg.wgjwhj.cn

Py:   f"{1234567:,}"
来源：http://xw.shxzskj.cn

PHP:  number_format(1234567);
来源：http://yf.newstarts.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ty.gzmigu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://qn.huixiangedu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ob.nicolike.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lw.asd995.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://od.huixinmuqiang.cn

C#:   1234567.ToString("N0")
来源：http://ql.huixinmuqiang.cn

[E17] 首字母大写
来源：http://vu.panjiajie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://na.9csxet.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://gf.bookmarksfly.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vv.lnxyls.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jr.jctech888.com.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zw.gzmigu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ia.jianghongdianzi.cn

Ruby: s.capitalize
来源：http://iq.yuexingan06.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jr.panjiajie.cn

[E18] 模板占位符替换
来源：http://er.szxytkj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kt.9csxet.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qs.haigaiapp.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://qq.haigaiapp.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://fk.asd995.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://eo.colortex.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ul.shxzukj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gx.521024.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zm.9csxet.cn

[E19] 多行文本按行拆分
来源：http://jd.szxytkj.cn

Py:   s.splitlines()
来源：http://ql.huixinmuqiang.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qj.newstarts.cn

JS:   s.split(/\r?\n/)
来源：http://gz.bjjhwx.cn

TS:   s.split(/\r?\n/)
来源：http://zh.jianghongdianzi.cn

Java: s.lines().toList()
来源：http://bo.huixinmuqiang.cn

Go:   strings.Split(s, "\n")
来源：http://xh.colortex.cn

Ruby: s.lines
来源：http://ry.bjjhwx.cn

C#:   s.Split('\n')
来源：http://vn.bookmarksfly.cn

[E20] 判断字符串是否为空
来源：http://bk.521024.cn

Py:   if not s:
来源：http://av.shxzskj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yr.nicolike.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cx.newstarts.cn

TS:   if (s === "") {}
来源：http://uq.nszjky.cn

Java: if (s.isEmpty()) {}
来源：http://qr.huanxung.cn

Go:   if s == "" {}
来源：http://md.colortex.cn

Ruby: if s.empty?
来源：http://kz.newstarts.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dq.shxzskj.cn

[E21] 超长截断加省略号
来源：http://eu.gzmigu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rp.9csxet.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vj.yuntaijiaju.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hn.shxzskj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bs.shxzskj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://em.bjjhwx.cn

Go:   // 按 rune 判断长度后截断
来源：http://im.chemitech.net.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lp.bjjhwx.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dg.szsharing.cn

[E22] 字节长度与字符长度
来源：http://id.gzmigu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zn.yuexingan06.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wq.shxzskj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xd.panjiajie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wb.huixinmuqiang.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vv.newstarts.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cu.lnxyls.cn

Ruby: s.bytesize;  s.length
来源：http://gv.jianghongdianzi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ko.huixiangedu.cn

================================================================================
来源：http://hc.nszjky.cn

F. 文件与目录
来源：http://kg.bookmarksfly.cn

================================================================================
来源：http://ft.jianghongdianzi.cn

[F01] 读取整个文件
来源：http://xs.yuntaijiaju.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mr.nicolike.cn

PHP:  file_get_contents("a.txt");
来源：http://jw.yuexingan06.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mg.gzmigu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://np.haigaiapp.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://uo.nicolike.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ql.bjjhwx.cn

Ruby: File.read("a.txt")
来源：http://ws.bookmarksfly.cn

C#:   File.ReadAllText("a.txt");
来源：http://rk.jctech888.com.cn

[F02] 逐行读取文件
来源：http://cq.lnxyls.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hg.haigaiapp.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dg.lnxyls.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bd.9csxet.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fi.bookmarksfly.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yd.jianghongdianzi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bs.panjiajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ph.chemitech.net.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pq.bjjhwx.cn

[F03] 写入文件（覆盖）
来源：http://rk.huixiangedu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zv.newstarts.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ps.bjjhwx.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://js.9csxet.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vx.bookmarksfly.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pv.9csxet.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ym.shtwfgs.cn

Ruby: File.write("a.txt", "hi")
来源：http://ah.szsharing.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cv.asd995.cn

[F04] 追加写入文件
来源：http://er.yuexingan06.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bb.jctech888.com.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cx.hnjuh.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hh.bookmarksfly.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oc.panjiajie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tp.nicolike.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ld.gzmigu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qk.shxzukj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qb.hahajie.cn

[F05] 判断文件或目录是否存在
来源：http://id.chemitech.net.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mv.yuexingan06.cn

PHP:  file_exists("a.txt");
来源：http://ow.newstarts.cn

JS:   fs.existsSync("a.txt")
来源：http://ka.9csxet.cn


<!-- 参考信息 -->