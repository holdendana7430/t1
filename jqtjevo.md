代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cb.newstarts.cn

[D20] 统计每个元素出现次数
来源：http://fv.bjjhwx.cn

Py:   Counter(arr)
来源：http://go.panjiajie.cn

PHP:  array_count_values($arr);
来源：http://ny.bookmarksfly.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bk.shtwfgs.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eb.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nh.wgjwhj.cn

Go:   // 手写 map[T]int
来源：http://mz.bjjhwx.cn

Ruby: arr.tally
来源：http://qt.bookmarksfly.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wi.jctech888.com.cn

[D21] 判断是否包含某元素
来源：http://ob.szsharing.cn

Py:   x in arr
来源：http://pv.muxihuayi.cn

PHP:  in_array($x, $arr, true);
来源：http://xm.bookmarksfly.cn

JS:   arr.includes(x)
来源：http://by.lnxyls.cn

TS:   arr.includes(x)
来源：http://kf.yuntaijiaju.cn

Java: list.contains(x)
来源：http://lr.muxihuayi.cn

Go:   slices.Contains(arr, x)
来源：http://py.shtwfgs.cn

Ruby: arr.include?(x)
来源：http://yg.haigaiapp.cn

C#:   list.Contains(x)
来源：http://cg.shxzukj.cn

[D22] 复制数组（避免共享引用）
来源：http://nw.szxytkj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fs.nszjky.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lw.haigaiapp.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ru.nszjky.cn

TS:   [...arr];
来源：http://wu.huixinmuqiang.cn

Java: new ArrayList<>(list);
来源：http://ye.521024.cn

Go:   copied := append([]int(nil), arr...)
来源：http://au.haigaiapp.cn

Ruby: arr.dup;  arr.clone
来源：http://bi.jianghongdianzi.cn

C#:   new List<int>(list);
来源：http://jq.colortex.cn

[D23] reduce 累积计算
来源：http://px.shtwfgs.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yb.hahajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pe.bjjhwx.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eo.panjiajie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rm.nicolike.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rf.hnjuh.cn

Go:   // 手写循环
来源：http://ge.szsharing.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zn.huanxung.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vj.gzmigu.cn

[D24] 字典 / Map 基本操作
来源：http://gy.haigaiapp.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wq.nicolike.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qk.jianghongdianzi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jn.yuntaijiaju.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wh.huixiangedu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://on.asd995.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qw.chemitech.net.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://yr.muxihuayi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://at.nszjky.cn

[D25] Set 集合去重与交并差
来源：http://xm.hnjuh.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lo.nszjky.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wv.newstarts.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fv.huixiangedu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bm.huanxung.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dm.szxytkj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fu.colortex.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://df.asd995.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fv.haigaiapp.cn

[D26] 数组转字符串
来源：http://cs.shxzukj.cn

Py:   ", ".join(map(str, arr))
来源：http://of.newstarts.cn

PHP:  implode(", ", $arr);
来源：http://km.huixinmuqiang.cn

JS:   arr.join(", ")
来源：http://ve.szsharing.cn

TS:   arr.join(", ")
来源：http://zw.huixiangedu.cn

Java: String.join(", ", list)
来源：http://uz.lnxyls.cn

Go:   strings.Join(strs, ", ")
来源：http://bw.colortex.cn

Ruby: arr.join(", ")
来源：http://ib.jctech888.com.cn

C#:   string.Join(", ", list)
来源：http://if.chemitech.net.cn

================================================================================
来源：http://xg.jianghongdianzi.cn

E. 字符串处理
来源：http://yp.shxzskj.cn

================================================================================
来源：http://iq.gzmigu.cn

[E01] 拼接字符串
来源：http://tn.chemitech.net.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cn.521024.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yv.jctech888.com.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wf.panjiajie.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rx.newstarts.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ay.szsharing.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ii.hnjuh.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dk.asd995.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vj.shtwfgs.cn

[E02] 重复字符串
来源：http://vt.huanxung.cn

Py:   "ab" * 3
来源：http://ru.gzmigu.cn

PHP:  str_repeat("ab", 3);
来源：http://km.bjjhwx.cn

JS:   "ab".repeat(3)
来源：http://ii.asd995.cn

TS:   "ab".repeat(3)
来源：http://jo.huixinmuqiang.cn

Java: "ab".repeat(3)
来源：http://zm.521024.cn

Go:   strings.Repeat("ab", 3)
来源：http://sb.panjiajie.cn

Ruby: "ab" * 3
来源：http://cr.wgjwhj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xr.shxzukj.cn

[E03] 截取子串
来源：http://eb.szsharing.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mk.shxzukj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ki.wgjwhj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sr.szsharing.cn

TS:   s.slice(1, 4)
来源：http://tw.szxytkj.cn

Java: s.substring(1, 4)
来源：http://fj.szxytkj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ey.shxzskj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://cv.hnjuh.cn

C#:   s.Substring(1, 3)
来源：http://qr.panjiajie.cn

[E04] 查找子串位置
来源：http://ly.jianghongdianzi.cn

Py:   s.find("x");  s.index("x")
来源：http://wb.chemitech.net.cn

PHP:  strpos($s, "x");
来源：http://tl.szxytkj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sm.colortex.cn

TS:   s.indexOf("x")
来源：http://wp.szxytkj.cn

Java: s.indexOf("x")
来源：http://sj.yuntaijiaju.cn

Go:   strings.Index(s, "x")
来源：http://vx.shtwfgs.cn

Ruby: s.index("x")
来源：http://ww.szxytkj.cn

C#:   s.IndexOf("x")
来源：http://ij.szsharing.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://jk.nszjky.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zr.lnxyls.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cb.bjjhwx.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qf.jctech888.com.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://jl.asd995.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wt.bjjhwx.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ba.shxzskj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bb.9csxet.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cm.yuntaijiaju.cn

[E06] 替换子串
来源：http://xo.chemitech.net.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://uj.huanxung.cn

PHP:  str_replace("a", "b", $s);
来源：http://bn.shxzukj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sf.shtwfgs.cn

TS:   s.replaceAll("a", "b")
来源：http://wv.yuntaijiaju.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tz.yuntaijiaju.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fj.nszjky.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qr.chemitech.net.cn

C#:   s.Replace("a", "b")
来源：http://cb.newstarts.cn

[E07] 按分隔符拆分
来源：http://hz.huixinmuqiang.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vk.521024.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wk.shxzukj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://yc.nicolike.cn

TS:   s.split(",")
来源：http://wu.nicolike.cn

Java: s.split(",");  s.split("\\s+")
来源：http://eh.asd995.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jw.muxihuayi.cn

Ruby: s.split(",");  s.split
来源：http://wj.huixiangedu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://au.szsharing.cn

[E08] 数组按分隔符合并
来源：http://qb.huixinmuqiang.cn

Py:   ",".join(items)
来源：http://mr.muxihuayi.cn

PHP:  implode(",", $items);
来源：http://yu.chemitech.net.cn

JS:   items.join(",")
来源：http://gk.shxzukj.cn

TS:   items.join(",")
来源：http://kw.yuexingan06.cn

Java: String.join(",", items)
来源：http://vi.colortex.cn

Go:   strings.Join(items, ",")
来源：http://iq.wgjwhj.cn

Ruby: items.join(",")
来源：http://gh.huanxung.cn

C#:   string.Join(",", items)
来源：http://zb.nszjky.cn

[E09] 去除所有空白字符
来源：http://xh.szxytkj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xf.9csxet.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://is.gzmigu.cn

JS:   s.replace(/\s+/g, "")
来源：http://cx.yuntaijiaju.cn

TS:   s.replace(/\s+/g, "")
来源：http://jp.newstarts.cn

Java: s.replaceAll("\\s+", "")
来源：http://oi.haigaiapp.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://vr.hahajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://vx.haigaiapp.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ms.panjiajie.cn

[E10] 左侧补零 / 定长填充
来源：http://ax.yuexingan06.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://uv.yuexingan06.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tx.yuexingan06.cn

JS:   "7".padStart(3, "0")
来源：http://gs.huixinmuqiang.cn

TS:   "7".padStart(3, "0")
来源：http://pb.szsharing.cn

Java: String.format("%03d", 7)
来源：http://yz.9csxet.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://dh.huixinmuqiang.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cx.huanxung.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qb.haigaiapp.cn

[E11] 反转字符串
来源：http://wa.chemitech.net.cn

Py:   s[::-1]
来源：http://iv.szxytkj.cn

PHP:  strrev($s);
来源：http://kx.9csxet.cn

JS:   [...s].reverse().join("")
来源：http://qe.huixiangedu.cn

TS:   [...s].reverse().join("")
来源：http://gq.chemitech.net.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://yx.panjiajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zj.panjiajie.cn

Ruby: s.reverse
来源：http://gv.gzmigu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://nx.colortex.cn

[E12] 统计某字符出现次数
来源：http://hu.colortex.cn

Py:   s.count("a")
来源：http://th.panjiajie.cn

PHP:  substr_count($s, "a");
来源：http://zt.wgjwhj.cn

JS:   s.split("a").length - 1
来源：http://gz.shxzukj.cn

TS:   s.split("a").length - 1
来源：http://xe.huixinmuqiang.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ne.newstarts.cn

Go:   strings.Count(s, "a")
来源：http://hm.shxzukj.cn

Ruby: s.count("a")
来源：http://ta.szxytkj.cn

C#:   s.Count(c => c == 'a')
来源：http://zl.shxzukj.cn

[E13] 逐字符遍历
来源：http://ci.newstarts.cn

Py:   for ch in s: print(ch)
来源：http://tx.newstarts.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bl.panjiajie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://up.hahajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://io.szsharing.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fa.wgjwhj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zl.hahajie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://zt.huixinmuqiang.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xa.szxytkj.cn

[E14] URL 编码与 Base64
来源：http://rr.nszjky.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vx.bookmarksfly.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://tk.bookmarksfly.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cr.bjjhwx.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zw.muxihuayi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ly.huixinmuqiang.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dr.huixiangedu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xs.shxzskj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ij.huixiangedu.cn

[E15] HTML 转义 / 反转义
来源：http://qu.colortex.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://iy.huixiangedu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rn.newstarts.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jb.hahajie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://mo.bjjhwx.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fp.shtwfgs.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vv.chemitech.net.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qt.bjjhwx.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://we.newstarts.cn

[E16] 数字千分位
来源：http://re.9csxet.cn

Py:   f"{1234567:,}"
来源：http://gj.chemitech.net.cn

PHP:  number_format(1234567);
来源：http://hd.jianghongdianzi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://si.szxytkj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://qh.gzmigu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tk.jianghongdianzi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ud.lnxyls.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://oe.shtwfgs.cn

C#:   1234567.ToString("N0")
来源：http://fy.shxzukj.cn

[E17] 首字母大写
来源：http://dm.yuexingan06.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sz.nszjky.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://kc.shxzskj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dj.huixiangedu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://km.chemitech.net.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cv.haigaiapp.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ty.newstarts.cn

Ruby: s.capitalize
来源：http://im.9csxet.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rv.hahajie.cn

[E18] 模板占位符替换
来源：http://ju.shxzukj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xo.huixiangedu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mn.521024.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://af.chemitech.net.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://eo.huixinmuqiang.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mv.muxihuayi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xc.huanxung.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wm.lnxyls.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ju.gzmigu.cn

[E19] 多行文本按行拆分
来源：http://pe.bjjhwx.cn

Py:   s.splitlines()
来源：http://yj.hnjuh.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zo.9csxet.cn

JS:   s.split(/\r?\n/)
来源：http://xq.asd995.cn

TS:   s.split(/\r?\n/)
来源：http://ti.521024.cn

Java: s.lines().toList()
来源：http://tn.jctech888.com.cn

Go:   strings.Split(s, "\n")
来源：http://sk.chemitech.net.cn

Ruby: s.lines
来源：http://bg.haigaiapp.cn

C#:   s.Split('\n')
来源：http://mm.haigaiapp.cn

[E20] 判断字符串是否为空
来源：http://fw.chemitech.net.cn

Py:   if not s:
来源：http://ti.haigaiapp.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gd.haigaiapp.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://id.hnjuh.cn

TS:   if (s === "") {}
来源：http://yd.nszjky.cn

Java: if (s.isEmpty()) {}
来源：http://az.jctech888.com.cn

Go:   if s == "" {}
来源：http://su.jctech888.com.cn

Ruby: if s.empty?
来源：http://sd.shtwfgs.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qk.wgjwhj.cn

[E21] 超长截断加省略号
来源：http://on.panjiajie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://py.muxihuayi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bd.szsharing.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://op.muxihuayi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ly.hahajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ho.nszjky.cn

Go:   // 按 rune 判断长度后截断
来源：http://kr.hahajie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://le.shtwfgs.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sh.yuexingan06.cn

[E22] 字节长度与字符长度
来源：http://ux.jianghongdianzi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zd.jctech888.com.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cq.shxzskj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pk.gzmigu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hs.asd995.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://oi.yuntaijiaju.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ng.hnjuh.cn

Ruby: s.bytesize;  s.length
来源：http://kt.shxzukj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hq.muxihuayi.cn

================================================================================
来源：http://dz.hnjuh.cn

F. 文件与目录
来源：http://lk.colortex.cn

================================================================================
来源：http://lk.asd995.cn

[F01] 读取整个文件
来源：http://ed.shxzukj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jd.shxzukj.cn

PHP:  file_get_contents("a.txt");
来源：http://er.shxzukj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sn.shxzukj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mq.shtwfgs.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://kv.jianghongdianzi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uf.newstarts.cn

Ruby: File.read("a.txt")
来源：http://iy.asd995.cn

C#:   File.ReadAllText("a.txt");
来源：http://ph.haigaiapp.cn

[F02] 逐行读取文件
来源：http://mm.panjiajie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bv.yuexingan06.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dw.haigaiapp.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sn.gzmigu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rh.haigaiapp.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qi.colortex.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lx.wgjwhj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cs.haigaiapp.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ku.wgjwhj.cn

[F03] 写入文件（覆盖）
来源：http://zn.chemitech.net.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pb.colortex.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://hb.haigaiapp.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://it.yuexingan06.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ul.huanxung.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fb.lnxyls.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://aa.hahajie.cn

Ruby: File.write("a.txt", "hi")
来源：http://bx.bookmarksfly.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mr.lnxyls.cn

[F04] 追加写入文件
来源：http://rb.haigaiapp.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kt.hnjuh.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kg.nszjky.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jx.9csxet.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yi.chemitech.net.cn


<!-- 参考信息 -->