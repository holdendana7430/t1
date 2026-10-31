代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cm.shtwfgs.cn

[D20] 统计每个元素出现次数
来源：http://ry.szsharing.cn

Py:   Counter(arr)
来源：http://gt.yuntaijiaju.cn

PHP:  array_count_values($arr);
来源：http://at.nicolike.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ln.hnjuh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iq.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lg.gzmigu.cn

Go:   // 手写 map[T]int
来源：http://mr.shxzukj.cn

Ruby: arr.tally
来源：http://jp.haigaiapp.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ji.hnjuh.cn

[D21] 判断是否包含某元素
来源：http://ba.lnxyls.cn

Py:   x in arr
来源：http://tk.yuntaijiaju.cn

PHP:  in_array($x, $arr, true);
来源：http://ez.szsharing.cn

JS:   arr.includes(x)
来源：http://bg.asd995.cn

TS:   arr.includes(x)
来源：http://mj.9csxet.cn

Java: list.contains(x)
来源：http://kv.9csxet.cn

Go:   slices.Contains(arr, x)
来源：http://kd.muxihuayi.cn

Ruby: arr.include?(x)
来源：http://gq.nszjky.cn

C#:   list.Contains(x)
来源：http://to.colortex.cn

[D22] 复制数组（避免共享引用）
来源：http://jp.9csxet.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ti.muxihuayi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://td.chemitech.net.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://io.nicolike.cn

TS:   [...arr];
来源：http://ls.yuntaijiaju.cn

Java: new ArrayList<>(list);
来源：http://tp.9csxet.cn

Go:   copied := append([]int(nil), arr...)
来源：http://lr.9csxet.cn

Ruby: arr.dup;  arr.clone
来源：http://gi.newstarts.cn

C#:   new List<int>(list);
来源：http://zw.asd995.cn

[D23] reduce 累积计算
来源：http://nb.colortex.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sz.bjjhwx.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wf.jctech888.com.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://im.huanxung.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rj.szsharing.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://hd.shxzskj.cn

Go:   // 手写循环
来源：http://ug.szsharing.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yx.bookmarksfly.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://uf.521024.cn

[D24] 字典 / Map 基本操作
来源：http://fy.chemitech.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ur.muxihuayi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xi.asd995.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xz.shtwfgs.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ab.hnjuh.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mj.huixinmuqiang.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tz.lnxyls.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ml.521024.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pm.muxihuayi.cn

[D25] Set 集合去重与交并差
来源：http://tg.lnxyls.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://sz.bookmarksfly.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://am.bookmarksfly.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ls.newstarts.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dj.jctech888.com.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jf.huixiangedu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://th.asd995.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tj.shxzukj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cq.szsharing.cn

[D26] 数组转字符串
来源：http://cu.huanxung.cn

Py:   ", ".join(map(str, arr))
来源：http://ib.bjjhwx.cn

PHP:  implode(", ", $arr);
来源：http://ed.nicolike.cn

JS:   arr.join(", ")
来源：http://xe.jianghongdianzi.cn

TS:   arr.join(", ")
来源：http://ky.9csxet.cn

Java: String.join(", ", list)
来源：http://re.shtwfgs.cn

Go:   strings.Join(strs, ", ")
来源：http://tt.szxytkj.cn

Ruby: arr.join(", ")
来源：http://ri.colortex.cn

C#:   string.Join(", ", list)
来源：http://lj.shxzukj.cn

================================================================================
来源：http://yr.huixinmuqiang.cn

E. 字符串处理
来源：http://oe.yuntaijiaju.cn

================================================================================
来源：http://qt.hnjuh.cn

[E01] 拼接字符串
来源：http://do.521024.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cd.newstarts.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ay.shtwfgs.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kn.nicolike.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hi.newstarts.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vl.hnjuh.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sl.bjjhwx.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://me.nicolike.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zd.9csxet.cn

[E02] 重复字符串
来源：http://dn.huanxung.cn

Py:   "ab" * 3
来源：http://bb.hahajie.cn

PHP:  str_repeat("ab", 3);
来源：http://ca.newstarts.cn

JS:   "ab".repeat(3)
来源：http://bb.chemitech.net.cn

TS:   "ab".repeat(3)
来源：http://oj.muxihuayi.cn

Java: "ab".repeat(3)
来源：http://hr.bookmarksfly.cn

Go:   strings.Repeat("ab", 3)
来源：http://wn.wgjwhj.cn

Ruby: "ab" * 3
来源：http://gt.szsharing.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ru.szxytkj.cn

[E03] 截取子串
来源：http://fe.521024.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gh.hnjuh.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gb.muxihuayi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bb.521024.cn

TS:   s.slice(1, 4)
来源：http://xz.bjjhwx.cn

Java: s.substring(1, 4)
来源：http://vv.jctech888.com.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ow.asd995.cn

Ruby: s[1, 3];  s[1..3]
来源：http://eb.chemitech.net.cn

C#:   s.Substring(1, 3)
来源：http://wz.nicolike.cn

[E04] 查找子串位置
来源：http://vq.chemitech.net.cn

Py:   s.find("x");  s.index("x")
来源：http://fo.jianghongdianzi.cn

PHP:  strpos($s, "x");
来源：http://yr.shxzskj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wk.yuexingan06.cn

TS:   s.indexOf("x")
来源：http://yd.yuexingan06.cn

Java: s.indexOf("x")
来源：http://py.bookmarksfly.cn

Go:   strings.Index(s, "x")
来源：http://jl.huanxung.cn

Ruby: s.index("x")
来源：http://aw.521024.cn

C#:   s.IndexOf("x")
来源：http://ux.chemitech.net.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xb.huanxung.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://og.szsharing.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ex.521024.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ri.lnxyls.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://eh.nszjky.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oj.shtwfgs.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ui.chemitech.net.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yl.newstarts.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ly.yuexingan06.cn

[E06] 替换子串
来源：http://en.shtwfgs.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tb.nszjky.cn

PHP:  str_replace("a", "b", $s);
来源：http://do.yuntaijiaju.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dl.nszjky.cn

TS:   s.replaceAll("a", "b")
来源：http://zp.szxytkj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vf.chemitech.net.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://oy.szxytkj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tm.asd995.cn

C#:   s.Replace("a", "b")
来源：http://oa.asd995.cn

[E07] 按分隔符拆分
来源：http://il.szxytkj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qr.lnxyls.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kt.asd995.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://zh.asd995.cn

TS:   s.split(",")
来源：http://ey.9csxet.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ia.huixiangedu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xr.huixiangedu.cn

Ruby: s.split(",");  s.split
来源：http://ez.yuntaijiaju.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qw.colortex.cn

[E08] 数组按分隔符合并
来源：http://yu.jctech888.com.cn

Py:   ",".join(items)
来源：http://yy.shtwfgs.cn

PHP:  implode(",", $items);
来源：http://hu.szxytkj.cn

JS:   items.join(",")
来源：http://hl.jianghongdianzi.cn

TS:   items.join(",")
来源：http://if.shxzukj.cn

Java: String.join(",", items)
来源：http://mw.panjiajie.cn

Go:   strings.Join(items, ",")
来源：http://kk.yuexingan06.cn

Ruby: items.join(",")
来源：http://rn.hnjuh.cn

C#:   string.Join(",", items)
来源：http://ra.lnxyls.cn

[E09] 去除所有空白字符
来源：http://dw.bjjhwx.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xb.szxytkj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://py.wgjwhj.cn

JS:   s.replace(/\s+/g, "")
来源：http://cc.yuntaijiaju.cn

TS:   s.replace(/\s+/g, "")
来源：http://ww.panjiajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://dr.bjjhwx.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://hc.521024.cn

Ruby: s.gsub(/\s+/, "")
来源：http://lo.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lo.szxytkj.cn

[E10] 左侧补零 / 定长填充
来源：http://vu.muxihuayi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ps.huixiangedu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ux.huanxung.cn

JS:   "7".padStart(3, "0")
来源：http://oc.muxihuayi.cn

TS:   "7".padStart(3, "0")
来源：http://dn.haigaiapp.cn

Java: String.format("%03d", 7)
来源：http://bm.chemitech.net.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://bb.haigaiapp.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nh.521024.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kp.lnxyls.cn

[E11] 反转字符串
来源：http://ph.yuexingan06.cn

Py:   s[::-1]
来源：http://ve.gzmigu.cn

PHP:  strrev($s);
来源：http://uq.colortex.cn

JS:   [...s].reverse().join("")
来源：http://kk.asd995.cn

TS:   [...s].reverse().join("")
来源：http://fg.shxzukj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://gl.yuexingan06.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qa.bookmarksfly.cn

Ruby: s.reverse
来源：http://yb.jctech888.com.cn

C#:   new string(s.Reverse().ToArray())
来源：http://wj.szxytkj.cn

[E12] 统计某字符出现次数
来源：http://jz.muxihuayi.cn

Py:   s.count("a")
来源：http://lp.jctech888.com.cn

PHP:  substr_count($s, "a");
来源：http://fx.hnjuh.cn

JS:   s.split("a").length - 1
来源：http://im.hahajie.cn

TS:   s.split("a").length - 1
来源：http://fr.521024.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gg.shxzukj.cn

Go:   strings.Count(s, "a")
来源：http://fi.newstarts.cn

Ruby: s.count("a")
来源：http://jo.huanxung.cn

C#:   s.Count(c => c == 'a')
来源：http://re.huixiangedu.cn

[E13] 逐字符遍历
来源：http://xl.newstarts.cn

Py:   for ch in s: print(ch)
来源：http://kd.jianghongdianzi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://an.shtwfgs.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://mf.asd995.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ek.huixiangedu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sl.shxzukj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://eq.hnjuh.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://oz.jctech888.com.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://my.bookmarksfly.cn

[E14] URL 编码与 Base64
来源：http://jw.asd995.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://uj.shxzukj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qj.huanxung.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rw.yuexingan06.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qp.yuexingan06.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yy.nicolike.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qp.521024.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bp.colortex.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ia.nicolike.cn

[E15] HTML 转义 / 反转义
来源：http://uj.panjiajie.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://pi.huanxung.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://va.bookmarksfly.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ee.chemitech.net.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://si.colortex.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://sj.521024.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://et.jianghongdianzi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vf.jctech888.com.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ny.asd995.cn

[E16] 数字千分位
来源：http://jl.521024.cn

Py:   f"{1234567:,}"
来源：http://ub.hahajie.cn

PHP:  number_format(1234567);
来源：http://uc.wgjwhj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://kt.asd995.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://xz.szxytkj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zw.jianghongdianzi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hs.huixiangedu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xp.gzmigu.cn

C#:   1234567.ToString("N0")
来源：http://ui.jctech888.com.cn

[E17] 首字母大写
来源：http://bh.wgjwhj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xt.asd995.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://be.colortex.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rm.haigaiapp.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mm.huixinmuqiang.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fj.huixinmuqiang.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ui.szsharing.cn

Ruby: s.capitalize
来源：http://hj.newstarts.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ci.yuexingan06.cn

[E18] 模板占位符替换
来源：http://aq.jianghongdianzi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wf.nicolike.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rm.jianghongdianzi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://gn.huixiangedu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ic.newstarts.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ul.huixinmuqiang.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ef.colortex.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gj.shxzukj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vh.newstarts.cn

[E19] 多行文本按行拆分
来源：http://ib.huanxung.cn

Py:   s.splitlines()
来源：http://qz.jctech888.com.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bl.hnjuh.cn

JS:   s.split(/\r?\n/)
来源：http://ce.bjjhwx.cn

TS:   s.split(/\r?\n/)
来源：http://wc.gzmigu.cn

Java: s.lines().toList()
来源：http://ke.muxihuayi.cn

Go:   strings.Split(s, "\n")
来源：http://uv.newstarts.cn

Ruby: s.lines
来源：http://as.colortex.cn

C#:   s.Split('\n')
来源：http://dn.521024.cn

[E20] 判断字符串是否为空
来源：http://kb.asd995.cn

Py:   if not s:
来源：http://zt.hahajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ux.chemitech.net.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://is.wgjwhj.cn

TS:   if (s === "") {}
来源：http://ub.shxzukj.cn

Java: if (s.isEmpty()) {}
来源：http://ya.gzmigu.cn

Go:   if s == "" {}
来源：http://jw.huixinmuqiang.cn

Ruby: if s.empty?
来源：http://am.huixinmuqiang.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ty.shxzskj.cn

[E21] 超长截断加省略号
来源：http://co.muxihuayi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ew.wgjwhj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ju.szxytkj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ju.jctech888.com.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tj.shtwfgs.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ql.gzmigu.cn

Go:   // 按 rune 判断长度后截断
来源：http://ly.wgjwhj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ut.shxzukj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tv.asd995.cn

[E22] 字节长度与字符长度
来源：http://se.haigaiapp.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sg.bjjhwx.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vc.bookmarksfly.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fd.bookmarksfly.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://py.bjjhwx.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ca.chemitech.net.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ay.szxytkj.cn

Ruby: s.bytesize;  s.length
来源：http://nc.lnxyls.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fq.szxytkj.cn

================================================================================
来源：http://tu.9csxet.cn

F. 文件与目录
来源：http://ba.yuexingan06.cn

================================================================================
来源：http://ft.haigaiapp.cn

[F01] 读取整个文件
来源：http://nj.muxihuayi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fw.9csxet.cn

PHP:  file_get_contents("a.txt");
来源：http://wi.lnxyls.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mz.9csxet.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cm.521024.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://gs.bjjhwx.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nu.nszjky.cn

Ruby: File.read("a.txt")
来源：http://sx.wgjwhj.cn

C#:   File.ReadAllText("a.txt");
来源：http://jc.nszjky.cn

[F02] 逐行读取文件
来源：http://nk.shtwfgs.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jd.shtwfgs.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nw.hahajie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dc.shtwfgs.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rd.asd995.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jl.muxihuayi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jctech888.com.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://br.wgjwhj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tf.szxytkj.cn

[F03] 写入文件（覆盖）
来源：http://hn.bjjhwx.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bz.nicolike.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://pr.huanxung.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ag.nszjky.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ou.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xz.chemitech.net.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://my.haigaiapp.cn

Ruby: File.write("a.txt", "hi")
来源：http://cx.bjjhwx.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hp.hahajie.cn

[F04] 追加写入文件
来源：http://fl.jianghongdianzi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mt.nicolike.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ew.shxzskj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mb.nszjky.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ha.jianghongdianzi.cn


<!-- 参考信息 -->