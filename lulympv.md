代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://hd.wgjwhj.cn

JS:   arr.includes(x)
来源：http://pt.huixiangedu.cn

TS:   arr.includes(x)
来源：http://kz.yuntaijiaju.cn

Java: list.contains(x)
来源：http://mv.chemitech.net.cn

Go:   slices.Contains(arr, x)
来源：http://hu.jianghongdianzi.cn

Ruby: arr.include?(x)
来源：http://sx.szsharing.cn

C#:   list.Contains(x)
来源：http://ud.hnjuh.cn

[D22] 复制数组（避免共享引用）
来源：http://aw.gzmigu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://aj.9csxet.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ht.wgjwhj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mp.jctech888.com.cn

TS:   [...arr];
来源：http://zb.nszjky.cn

Java: new ArrayList<>(list);
来源：http://ap.nicolike.cn

Go:   copied := append([]int(nil), arr...)
来源：http://tl.huixinmuqiang.cn

Ruby: arr.dup;  arr.clone
来源：http://zb.newstarts.cn

C#:   new List<int>(list);
来源：http://wo.newstarts.cn

[D23] reduce 累积计算
来源：http://ap.muxihuayi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qg.huixinmuqiang.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fm.gzmigu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yw.chemitech.net.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gm.shtwfgs.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://zg.521024.cn

Go:   // 手写循环
来源：http://iu.bookmarksfly.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rd.yuntaijiaju.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sd.haigaiapp.cn

[D24] 字典 / Map 基本操作
来源：http://tz.shxzskj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://se.jctech888.com.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ds.haigaiapp.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zu.huixinmuqiang.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ho.bjjhwx.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qj.newstarts.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dq.9csxet.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bf.huixiangedu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dc.szxytkj.cn

[D25] Set 集合去重与交并差
来源：http://nm.nicolike.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cg.hnjuh.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ty.521024.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://du.jctech888.com.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wu.panjiajie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://yw.shtwfgs.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bw.bookmarksfly.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ka.huixiangedu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ll.hahajie.cn

[D26] 数组转字符串
来源：http://rd.shtwfgs.cn

Py:   ", ".join(map(str, arr))
来源：http://vh.huixiangedu.cn

PHP:  implode(", ", $arr);
来源：http://bc.huanxung.cn

JS:   arr.join(", ")
来源：http://lp.haigaiapp.cn

TS:   arr.join(", ")
来源：http://vr.shxzukj.cn

Java: String.join(", ", list)
来源：http://fe.hnjuh.cn

Go:   strings.Join(strs, ", ")
来源：http://ad.bjjhwx.cn

Ruby: arr.join(", ")
来源：http://rr.huixinmuqiang.cn

C#:   string.Join(", ", list)
来源：http://yi.shxzukj.cn

================================================================================
来源：http://ul.gzmigu.cn

E. 字符串处理
来源：http://eb.newstarts.cn

================================================================================
来源：http://nx.yuexingan06.cn

[E01] 拼接字符串
来源：http://zd.bjjhwx.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nq.huixiangedu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://uv.huixinmuqiang.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gy.shxzskj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rx.lnxyls.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qq.hahajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bo.9csxet.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dc.wgjwhj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vj.9csxet.cn

[E02] 重复字符串
来源：http://vp.asd995.cn

Py:   "ab" * 3
来源：http://et.newstarts.cn

PHP:  str_repeat("ab", 3);
来源：http://kz.huanxung.cn

JS:   "ab".repeat(3)
来源：http://cr.bookmarksfly.cn

TS:   "ab".repeat(3)
来源：http://ao.colortex.cn

Java: "ab".repeat(3)
来源：http://kv.521024.cn

Go:   strings.Repeat("ab", 3)
来源：http://ug.nicolike.cn

Ruby: "ab" * 3
来源：http://qz.bjjhwx.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wn.wgjwhj.cn

[E03] 截取子串
来源：http://am.nicolike.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vy.shtwfgs.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ie.521024.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kr.chemitech.net.cn

TS:   s.slice(1, 4)
来源：http://ft.yuexingan06.cn

Java: s.substring(1, 4)
来源：http://qh.shxzukj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://if.jctech888.com.cn

Ruby: s[1, 3];  s[1..3]
来源：http://cz.szxytkj.cn

C#:   s.Substring(1, 3)
来源：http://cp.shxzskj.cn

[E04] 查找子串位置
来源：http://dq.hnjuh.cn

Py:   s.find("x");  s.index("x")
来源：http://sr.haigaiapp.cn

PHP:  strpos($s, "x");
来源：http://nk.9csxet.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ku.shtwfgs.cn

TS:   s.indexOf("x")
来源：http://cp.bookmarksfly.cn

Java: s.indexOf("x")
来源：http://ta.hahajie.cn

Go:   strings.Index(s, "x")
来源：http://yb.panjiajie.cn

Ruby: s.index("x")
来源：http://yi.chemitech.net.cn

C#:   s.IndexOf("x")
来源：http://ut.yuntaijiaju.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://vm.hahajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ay.521024.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bc.szxytkj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wv.shtwfgs.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://kz.wgjwhj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ot.shxzukj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ai.jianghongdianzi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vf.muxihuayi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sy.yuntaijiaju.cn

[E06] 替换子串
来源：http://pj.huixiangedu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ny.nicolike.cn

PHP:  str_replace("a", "b", $s);
来源：http://hg.panjiajie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tu.newstarts.cn

TS:   s.replaceAll("a", "b")
来源：http://bk.shxzskj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jp.shtwfgs.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bd.shtwfgs.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lh.chemitech.net.cn

C#:   s.Replace("a", "b")
来源：http://cw.panjiajie.cn

[E07] 按分隔符拆分
来源：http://tz.jianghongdianzi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://at.colortex.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://de.colortex.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://qz.shxzukj.cn

TS:   s.split(",")
来源：http://yx.shxzukj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ku.nszjky.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yx.shxzskj.cn

Ruby: s.split(",");  s.split
来源：http://pq.hahajie.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xx.huixinmuqiang.cn

[E08] 数组按分隔符合并
来源：http://bq.jctech888.com.cn

Py:   ",".join(items)
来源：http://jv.chemitech.net.cn

PHP:  implode(",", $items);
来源：http://ag.jctech888.com.cn

JS:   items.join(",")
来源：http://yi.haigaiapp.cn

TS:   items.join(",")
来源：http://tv.nszjky.cn

Java: String.join(",", items)
来源：http://ew.bjjhwx.cn

Go:   strings.Join(items, ",")
来源：http://mo.nszjky.cn

Ruby: items.join(",")
来源：http://al.szsharing.cn

C#:   string.Join(",", items)
来源：http://rb.jctech888.com.cn

[E09] 去除所有空白字符
来源：http://ty.shtwfgs.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ei.jianghongdianzi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cn.chemitech.net.cn

JS:   s.replace(/\s+/g, "")
来源：http://mq.colortex.cn

TS:   s.replace(/\s+/g, "")
来源：http://yc.hahajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://lw.jctech888.com.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ji.shxzukj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://rl.nszjky.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nr.jianghongdianzi.cn

[E10] 左侧补零 / 定长填充
来源：http://if.nszjky.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hn.wgjwhj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kp.nicolike.cn

JS:   "7".padStart(3, "0")
来源：http://sl.yuntaijiaju.cn

TS:   "7".padStart(3, "0")
来源：http://ej.jctech888.com.cn

Java: String.format("%03d", 7)
来源：http://kl.yuexingan06.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://be.bjjhwx.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fa.asd995.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kk.panjiajie.cn

[E11] 反转字符串
来源：http://aw.panjiajie.cn

Py:   s[::-1]
来源：http://ie.huanxung.cn

PHP:  strrev($s);
来源：http://no.huixiangedu.cn

JS:   [...s].reverse().join("")
来源：http://df.asd995.cn

TS:   [...s].reverse().join("")
来源：http://xi.9csxet.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://qn.nszjky.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://da.shtwfgs.cn

Ruby: s.reverse
来源：http://rw.521024.cn

C#:   new string(s.Reverse().ToArray())
来源：http://iu.hnjuh.cn

[E12] 统计某字符出现次数
来源：http://fg.hahajie.cn

Py:   s.count("a")
来源：http://bc.9csxet.cn

PHP:  substr_count($s, "a");
来源：http://py.9csxet.cn

JS:   s.split("a").length - 1
来源：http://md.panjiajie.cn

TS:   s.split("a").length - 1
来源：http://kd.asd995.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wk.jctech888.com.cn

Go:   strings.Count(s, "a")
来源：http://ez.nicolike.cn

Ruby: s.count("a")
来源：http://sx.gzmigu.cn

C#:   s.Count(c => c == 'a')
来源：http://tt.jctech888.com.cn

[E13] 逐字符遍历
来源：http://ey.huixiangedu.cn

Py:   for ch in s: print(ch)
来源：http://mh.colortex.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lv.shxzukj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://la.asd995.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ej.nicolike.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qw.szsharing.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mr.shtwfgs.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ly.huanxung.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zp.panjiajie.cn

[E14] URL 编码与 Base64
来源：http://hn.huanxung.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lr.hnjuh.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://xs.szsharing.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ep.yuntaijiaju.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://uh.muxihuayi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rn.bjjhwx.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vs.hahajie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cg.wgjwhj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://oc.lnxyls.cn

[E15] HTML 转义 / 反转义
来源：http://ra.muxihuayi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://hd.huixinmuqiang.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://je.huixinmuqiang.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ar.huixinmuqiang.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://zh.nicolike.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rf.yuexingan06.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mc.haigaiapp.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mt.lnxyls.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://om.haigaiapp.cn

[E16] 数字千分位
来源：http://jt.jctech888.com.cn

Py:   f"{1234567:,}"
来源：http://mo.9csxet.cn

PHP:  number_format(1234567);
来源：http://ym.muxihuayi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ll.521024.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://xn.panjiajie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ez.shxzukj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://iq.bookmarksfly.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://yg.asd995.cn

C#:   1234567.ToString("N0")
来源：http://mu.wgjwhj.cn

[E17] 首字母大写
来源：http://gn.haigaiapp.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zk.huixinmuqiang.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://na.hnjuh.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mf.shxzukj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://se.huixiangedu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://be.jctech888.com.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wr.szxytkj.cn

Ruby: s.capitalize
来源：http://ww.chemitech.net.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cx.yuexingan06.cn

[E18] 模板占位符替换
来源：http://qr.muxihuayi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://if.jctech888.com.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ru.jctech888.com.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://tv.9csxet.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://nh.gzmigu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lb.muxihuayi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wb.shtwfgs.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rx.colortex.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gz.huixinmuqiang.cn

[E19] 多行文本按行拆分
来源：http://dm.gzmigu.cn

Py:   s.splitlines()
来源：http://bm.shxzskj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://va.asd995.cn

JS:   s.split(/\r?\n/)
来源：http://py.shxzskj.cn

TS:   s.split(/\r?\n/)
来源：http://pe.nicolike.cn

Java: s.lines().toList()
来源：http://eh.jianghongdianzi.cn

Go:   strings.Split(s, "\n")
来源：http://jz.wgjwhj.cn

Ruby: s.lines
来源：http://zv.huixinmuqiang.cn

C#:   s.Split('\n')
来源：http://gf.newstarts.cn

[E20] 判断字符串是否为空
来源：http://jv.yuntaijiaju.cn

Py:   if not s:
来源：http://ds.huanxung.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sg.asd995.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fz.gzmigu.cn

TS:   if (s === "") {}
来源：http://un.colortex.cn

Java: if (s.isEmpty()) {}
来源：http://la.jianghongdianzi.cn

Go:   if s == "" {}
来源：http://yh.huixinmuqiang.cn

Ruby: if s.empty?
来源：http://sm.huixiangedu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gn.bookmarksfly.cn

[E21] 超长截断加省略号
来源：http://ep.wgjwhj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://iw.nicolike.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://oy.szsharing.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cr.lnxyls.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gd.chemitech.net.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fo.shxzukj.cn

Go:   // 按 rune 判断长度后截断
来源：http://bv.bjjhwx.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dv.lnxyls.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://na.lnxyls.cn

[E22] 字节长度与字符长度
来源：http://kc.nicolike.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ei.shxzukj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jd.9csxet.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://md.wgjwhj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dz.huixinmuqiang.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://md.szxytkj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ze.shxzskj.cn

Ruby: s.bytesize;  s.length
来源：http://gb.szxytkj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ma.jianghongdianzi.cn

================================================================================
来源：http://sw.shtwfgs.cn

F. 文件与目录
来源：http://pb.hahajie.cn

================================================================================
来源：http://vi.nszjky.cn

[F01] 读取整个文件
来源：http://pr.colortex.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vu.shxzukj.cn

PHP:  file_get_contents("a.txt");
来源：http://oz.nicolike.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wr.huixinmuqiang.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lu.chemitech.net.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ez.bjjhwx.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ux.newstarts.cn

Ruby: File.read("a.txt")
来源：http://fq.hnjuh.cn

C#:   File.ReadAllText("a.txt");
来源：http://rd.lnxyls.cn

[F02] 逐行读取文件
来源：http://yf.huixinmuqiang.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pd.yuntaijiaju.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vw.haigaiapp.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wh.shxzskj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uh.shxzukj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yp.9csxet.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mf.haigaiapp.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dj.hnjuh.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://np.nszjky.cn

[F03] 写入文件（覆盖）
来源：http://fd.yuntaijiaju.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gr.shxzskj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://mh.asd995.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vq.wgjwhj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tu.szxytkj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://iy.jianghongdianzi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dz.huixinmuqiang.cn

Ruby: File.write("a.txt", "hi")
来源：http://sw.521024.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ej.jctech888.com.cn

[F04] 追加写入文件
来源：http://dl.yuexingan06.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kb.chemitech.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fa.gzmigu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ji.asd995.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ze.nszjky.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vw.gzmigu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wv.nicolike.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://sw.bookmarksfly.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://un.yuexingan06.cn

[F05] 判断文件或目录是否存在
来源：http://jo.bjjhwx.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ck.wgjwhj.cn

PHP:  file_exists("a.txt");
来源：http://im.lnxyls.cn

JS:   fs.existsSync("a.txt")
来源：http://bf.bjjhwx.cn

TS:   fs.existsSync("a.txt")
来源：http://kz.wgjwhj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://px.chemitech.net.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wx.nicolike.cn

Ruby: File.exist?("a.txt")
来源：http://yg.shxzskj.cn


<!-- 参考信息 -->