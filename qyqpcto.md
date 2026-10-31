代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://tn.wgjwhj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ln.shxzukj.cn

Go:   // 手写 map[string][]T
来源：http://xd.huanxung.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://mg.521024.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pf.jctech888.com.cn

[D20] 统计每个元素出现次数
来源：http://aw.huixinmuqiang.cn

Py:   Counter(arr)
来源：http://lx.jianghongdianzi.cn

PHP:  array_count_values($arr);
来源：http://ee.bookmarksfly.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gl.muxihuayi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nf.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bg.lnxyls.cn

Go:   // 手写 map[T]int
来源：http://qj.wgjwhj.cn

Ruby: arr.tally
来源：http://ih.9csxet.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sf.nicolike.cn

[D21] 判断是否包含某元素
来源：http://vv.nszjky.cn

Py:   x in arr
来源：http://pm.panjiajie.cn

PHP:  in_array($x, $arr, true);
来源：http://yx.asd995.cn

JS:   arr.includes(x)
来源：http://nm.panjiajie.cn

TS:   arr.includes(x)
来源：http://xq.wgjwhj.cn

Java: list.contains(x)
来源：http://rz.huanxung.cn

Go:   slices.Contains(arr, x)
来源：http://nf.yuntaijiaju.cn

Ruby: arr.include?(x)
来源：http://kp.lnxyls.cn

C#:   list.Contains(x)
来源：http://bo.szxytkj.cn

[D22] 复制数组（避免共享引用）
来源：http://md.jctech888.com.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yq.huanxung.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gf.lnxyls.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jc.hnjuh.cn

TS:   [...arr];
来源：http://fm.gzmigu.cn

Java: new ArrayList<>(list);
来源：http://oy.nszjky.cn

Go:   copied := append([]int(nil), arr...)
来源：http://sj.szxytkj.cn

Ruby: arr.dup;  arr.clone
来源：http://ho.nszjky.cn

C#:   new List<int>(list);
来源：http://vy.newstarts.cn

[D23] reduce 累积计算
来源：http://qn.521024.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://im.jctech888.com.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dl.hahajie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oj.9csxet.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://se.jianghongdianzi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://kc.hahajie.cn

Go:   // 手写循环
来源：http://ed.huanxung.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://es.bjjhwx.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nw.hahajie.cn

[D24] 字典 / Map 基本操作
来源：http://db.hahajie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://iy.yuntaijiaju.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yv.haigaiapp.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ys.muxihuayi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zh.szsharing.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yj.hahajie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sb.bjjhwx.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rf.jctech888.com.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mq.szsharing.cn

[D25] Set 集合去重与交并差
来源：http://tu.newstarts.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ak.bookmarksfly.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qu.panjiajie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://sd.hahajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lr.nszjky.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pd.muxihuayi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zw.nszjky.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hf.shxzukj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ri.yuntaijiaju.cn

[D26] 数组转字符串
来源：http://rv.gzmigu.cn

Py:   ", ".join(map(str, arr))
来源：http://ve.jianghongdianzi.cn

PHP:  implode(", ", $arr);
来源：http://ar.asd995.cn

JS:   arr.join(", ")
来源：http://tk.chemitech.net.cn

TS:   arr.join(", ")
来源：http://nw.szxytkj.cn

Java: String.join(", ", list)
来源：http://gb.haigaiapp.cn

Go:   strings.Join(strs, ", ")
来源：http://pt.wgjwhj.cn

Ruby: arr.join(", ")
来源：http://ob.hnjuh.cn

C#:   string.Join(", ", list)
来源：http://ip.jianghongdianzi.cn

================================================================================
来源：http://nf.muxihuayi.cn

E. 字符串处理
来源：http://la.shtwfgs.cn

================================================================================
来源：http://da.asd995.cn

[E01] 拼接字符串
来源：http://wy.hnjuh.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pk.9csxet.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rt.huixinmuqiang.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ot.jianghongdianzi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zo.shxzskj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pm.huanxung.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vw.haigaiapp.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yq.huixinmuqiang.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ec.szsharing.cn

[E02] 重复字符串
来源：http://il.szxytkj.cn

Py:   "ab" * 3
来源：http://mf.colortex.cn

PHP:  str_repeat("ab", 3);
来源：http://lw.bjjhwx.cn

JS:   "ab".repeat(3)
来源：http://fs.haigaiapp.cn

TS:   "ab".repeat(3)
来源：http://vz.szsharing.cn

Java: "ab".repeat(3)
来源：http://kz.yuntaijiaju.cn

Go:   strings.Repeat("ab", 3)
来源：http://re.newstarts.cn

Ruby: "ab" * 3
来源：http://de.nicolike.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xh.huanxung.cn

[E03] 截取子串
来源：http://em.hahajie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fs.shxzukj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://da.yuntaijiaju.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yk.nszjky.cn

TS:   s.slice(1, 4)
来源：http://eg.huixiangedu.cn

Java: s.substring(1, 4)
来源：http://ba.szxytkj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rk.wgjwhj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zn.yuexingan06.cn

C#:   s.Substring(1, 3)
来源：http://zn.521024.cn

[E04] 查找子串位置
来源：http://rq.521024.cn

Py:   s.find("x");  s.index("x")
来源：http://hh.nszjky.cn

PHP:  strpos($s, "x");
来源：http://tl.bookmarksfly.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ig.szsharing.cn

TS:   s.indexOf("x")
来源：http://fy.yuexingan06.cn

Java: s.indexOf("x")
来源：http://hq.newstarts.cn

Go:   strings.Index(s, "x")
来源：http://du.colortex.cn

Ruby: s.index("x")
来源：http://wu.521024.cn

C#:   s.IndexOf("x")
来源：http://fx.bjjhwx.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://cl.chemitech.net.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://st.muxihuayi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sn.hnjuh.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ir.huanxung.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://nt.shxzskj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sp.huanxung.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fc.bjjhwx.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hq.huanxung.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mp.bjjhwx.cn

[E06] 替换子串
来源：http://xh.colortex.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cv.asd995.cn

PHP:  str_replace("a", "b", $s);
来源：http://po.szsharing.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wd.huixinmuqiang.cn

TS:   s.replaceAll("a", "b")
来源：http://yt.huanxung.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wy.lnxyls.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pp.shxzskj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dj.huixinmuqiang.cn

C#:   s.Replace("a", "b")
来源：http://sz.colortex.cn

[E07] 按分隔符拆分
来源：http://gc.wgjwhj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mu.nszjky.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ii.szsharing.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://jf.jctech888.com.cn

TS:   s.split(",")
来源：http://dj.yuexingan06.cn

Java: s.split(",");  s.split("\\s+")
来源：http://le.szsharing.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yb.bjjhwx.cn

Ruby: s.split(",");  s.split
来源：http://oi.newstarts.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fs.bjjhwx.cn

[E08] 数组按分隔符合并
来源：http://ss.nicolike.cn

Py:   ",".join(items)
来源：http://pe.huanxung.cn

PHP:  implode(",", $items);
来源：http://rm.huanxung.cn

JS:   items.join(",")
来源：http://fy.bjjhwx.cn

TS:   items.join(",")
来源：http://xf.shxzskj.cn

Java: String.join(",", items)
来源：http://wj.hahajie.cn

Go:   strings.Join(items, ",")
来源：http://fr.szsharing.cn

Ruby: items.join(",")
来源：http://fz.hnjuh.cn

C#:   string.Join(",", items)
来源：http://yp.nszjky.cn

[E09] 去除所有空白字符
来源：http://nh.shtwfgs.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hn.colortex.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hp.panjiajie.cn

JS:   s.replace(/\s+/g, "")
来源：http://ul.shtwfgs.cn

TS:   s.replace(/\s+/g, "")
来源：http://lj.wgjwhj.cn

Java: s.replaceAll("\\s+", "")
来源：http://bk.521024.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://nk.yuntaijiaju.cn

Ruby: s.gsub(/\s+/, "")
来源：http://vj.shtwfgs.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xg.haigaiapp.cn

[E10] 左侧补零 / 定长填充
来源：http://zj.newstarts.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mq.gzmigu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kj.shtwfgs.cn

JS:   "7".padStart(3, "0")
来源：http://ln.nicolike.cn

TS:   "7".padStart(3, "0")
来源：http://uf.yuntaijiaju.cn

Java: String.format("%03d", 7)
来源：http://kn.hahajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://oc.huixinmuqiang.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://za.yuntaijiaju.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ry.panjiajie.cn

[E11] 反转字符串
来源：http://oc.hnjuh.cn

Py:   s[::-1]
来源：http://xm.haigaiapp.cn

PHP:  strrev($s);
来源：http://hd.huixiangedu.cn

JS:   [...s].reverse().join("")
来源：http://wi.haigaiapp.cn

TS:   [...s].reverse().join("")
来源：http://wn.newstarts.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://da.nszjky.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ep.nicolike.cn

Ruby: s.reverse
来源：http://dc.panjiajie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ng.bookmarksfly.cn

[E12] 统计某字符出现次数
来源：http://tq.bjjhwx.cn

Py:   s.count("a")
来源：http://xz.nszjky.cn

PHP:  substr_count($s, "a");
来源：http://wy.huixiangedu.cn

JS:   s.split("a").length - 1
来源：http://ex.huixinmuqiang.cn

TS:   s.split("a").length - 1
来源：http://zb.shtwfgs.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tt.hahajie.cn

Go:   strings.Count(s, "a")
来源：http://mq.jianghongdianzi.cn

Ruby: s.count("a")
来源：http://sg.wgjwhj.cn

C#:   s.Count(c => c == 'a')
来源：http://jz.jianghongdianzi.cn

[E13] 逐字符遍历
来源：http://bg.szxytkj.cn

Py:   for ch in s: print(ch)
来源：http://ri.asd995.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ec.muxihuayi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://de.nicolike.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://sv.panjiajie.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yp.hnjuh.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://to.szsharing.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ya.yuexingan06.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jc.szxytkj.cn

[E14] URL 编码与 Base64
来源：http://sw.wgjwhj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bo.521024.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://mu.asd995.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xn.haigaiapp.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ln.521024.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://be.panjiajie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ot.chemitech.net.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vr.szsharing.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sn.wgjwhj.cn

[E15] HTML 转义 / 反转义
来源：http://nj.wgjwhj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://wq.huixiangedu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ml.huanxung.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pk.bookmarksfly.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://vw.jianghongdianzi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pj.shxzukj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ur.szxytkj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qf.chemitech.net.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ek.huixinmuqiang.cn

[E16] 数字千分位
来源：http://cj.shxzskj.cn

Py:   f"{1234567:,}"
来源：http://qc.huixinmuqiang.cn

PHP:  number_format(1234567);
来源：http://gs.shtwfgs.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://jw.jianghongdianzi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://lp.nszjky.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rb.bookmarksfly.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bp.asd995.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wx.muxihuayi.cn

C#:   1234567.ToString("N0")
来源：http://hd.huanxung.cn

[E17] 首字母大写
来源：http://vx.yuntaijiaju.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kq.jctech888.com.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://hq.haigaiapp.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ol.muxihuayi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ie.panjiajie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fl.muxihuayi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ii.yuexingan06.cn

Ruby: s.capitalize
来源：http://tc.newstarts.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jq.bookmarksfly.cn

[E18] 模板占位符替换
来源：http://tp.szsharing.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vs.panjiajie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nj.szxytkj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://hj.huixinmuqiang.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ts.nicolike.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gt.shxzskj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://he.nszjky.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rq.shxzukj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mp.haigaiapp.cn

[E19] 多行文本按行拆分
来源：http://nz.nicolike.cn

Py:   s.splitlines()
来源：http://xr.szxytkj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nv.newstarts.cn

JS:   s.split(/\r?\n/)
来源：http://kp.yuntaijiaju.cn

TS:   s.split(/\r?\n/)
来源：http://tc.shxzukj.cn

Java: s.lines().toList()
来源：http://aq.gzmigu.cn

Go:   strings.Split(s, "\n")
来源：http://kl.asd995.cn

Ruby: s.lines
来源：http://ro.haigaiapp.cn

C#:   s.Split('\n')
来源：http://mw.haigaiapp.cn

[E20] 判断字符串是否为空
来源：http://mt.szxytkj.cn

Py:   if not s:
来源：http://fd.panjiajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xo.huanxung.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xr.szsharing.cn

TS:   if (s === "") {}
来源：http://ql.nicolike.cn

Java: if (s.isEmpty()) {}
来源：http://dv.asd995.cn

Go:   if s == "" {}
来源：http://qs.nszjky.cn

Ruby: if s.empty?
来源：http://cc.chemitech.net.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://io.huixinmuqiang.cn

[E21] 超长截断加省略号
来源：http://hu.shtwfgs.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qe.lnxyls.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zb.panjiajie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hc.chemitech.net.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fq.chemitech.net.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ac.9csxet.cn

Go:   // 按 rune 判断长度后截断
来源：http://ln.lnxyls.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ey.9csxet.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://yu.chemitech.net.cn

[E22] 字节长度与字符长度
来源：http://lw.shxzskj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zr.huixinmuqiang.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ld.shxzukj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wa.huanxung.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rq.jianghongdianzi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ou.huixinmuqiang.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yl.jianghongdianzi.cn

Ruby: s.bytesize;  s.length
来源：http://gb.jianghongdianzi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rv.hnjuh.cn

================================================================================
来源：http://gz.hnjuh.cn

F. 文件与目录
来源：http://yq.szsharing.cn

================================================================================
来源：http://ds.yuexingan06.cn

[F01] 读取整个文件
来源：http://rh.huixinmuqiang.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wd.hahajie.cn

PHP:  file_get_contents("a.txt");
来源：http://ws.jianghongdianzi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rm.muxihuayi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ll.huixiangedu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ou.nicolike.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://su.szxytkj.cn

Ruby: File.read("a.txt")
来源：http://xe.huixinmuqiang.cn

C#:   File.ReadAllText("a.txt");
来源：http://ev.wgjwhj.cn

[F02] 逐行读取文件
来源：http://fh.hahajie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://iy.shxzukj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ba.jctech888.com.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xd.jctech888.com.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cl.haigaiapp.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hj.yuexingan06.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dc.huixiangedu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pk.huixinmuqiang.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ft.huixinmuqiang.cn

[F03] 写入文件（覆盖）
来源：http://dm.yuexingan06.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hn.panjiajie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://wi.521024.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://so.jianghongdianzi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xr.haigaiapp.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dr.hahajie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bc.szsharing.cn

Ruby: File.write("a.txt", "hi")
来源：http://mb.haigaiapp.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vs.jianghongdianzi.cn

[F04] 追加写入文件
来源：http://sk.haigaiapp.cn


<!-- 参考信息 -->