代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mc.nszjky.cn

[D20] 统计每个元素出现次数
来源：http://jj.muxihuayi.cn

Py:   Counter(arr)
来源：http://el.bookmarksfly.cn

PHP:  array_count_values($arr);
来源：http://al.huixiangedu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kj.gzmigu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bl.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nl.shtwfgs.cn

Go:   // 手写 map[T]int
来源：http://yk.nicolike.cn

Ruby: arr.tally
来源：http://jr.chemitech.net.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rq.jianghongdianzi.cn

[D21] 判断是否包含某元素
来源：http://jy.shxzskj.cn

Py:   x in arr
来源：http://cs.shxzukj.cn

PHP:  in_array($x, $arr, true);
来源：http://km.jctech888.com.cn

JS:   arr.includes(x)
来源：http://aw.shxzukj.cn

TS:   arr.includes(x)
来源：http://kc.jianghongdianzi.cn

Java: list.contains(x)
来源：http://ax.huanxung.cn

Go:   slices.Contains(arr, x)
来源：http://hg.shxzukj.cn

Ruby: arr.include?(x)
来源：http://hk.nicolike.cn

C#:   list.Contains(x)
来源：http://rc.asd995.cn

[D22] 复制数组（避免共享引用）
来源：http://il.panjiajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://sh.521024.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sf.shxzskj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ps.jianghongdianzi.cn

TS:   [...arr];
来源：http://uz.521024.cn

Java: new ArrayList<>(list);
来源：http://hm.colortex.cn

Go:   copied := append([]int(nil), arr...)
来源：http://lu.wgjwhj.cn

Ruby: arr.dup;  arr.clone
来源：http://mf.asd995.cn

C#:   new List<int>(list);
来源：http://cx.huixiangedu.cn

[D23] reduce 累积计算
来源：http://or.bjjhwx.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://eo.chemitech.net.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://eq.nszjky.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rr.hnjuh.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ye.asd995.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rq.huixinmuqiang.cn

Go:   // 手写循环
来源：http://rv.bookmarksfly.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bg.newstarts.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://py.newstarts.cn

[D24] 字典 / Map 基本操作
来源：http://qf.gzmigu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zv.colortex.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tk.hnjuh.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://go.szsharing.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ec.szsharing.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://sd.9csxet.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://oq.chemitech.net.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://uf.szsharing.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mk.muxihuayi.cn

[D25] Set 集合去重与交并差
来源：http://cm.shtwfgs.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vy.szxytkj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nu.huixiangedu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://oe.hahajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rt.huixinmuqiang.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qu.panjiajie.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sv.szsharing.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kg.gzmigu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xr.bookmarksfly.cn

[D26] 数组转字符串
来源：http://ss.gzmigu.cn

Py:   ", ".join(map(str, arr))
来源：http://yp.jianghongdianzi.cn

PHP:  implode(", ", $arr);
来源：http://sv.szxytkj.cn

JS:   arr.join(", ")
来源：http://de.yuntaijiaju.cn

TS:   arr.join(", ")
来源：http://uk.gzmigu.cn

Java: String.join(", ", list)
来源：http://py.yuexingan06.cn

Go:   strings.Join(strs, ", ")
来源：http://tb.yuexingan06.cn

Ruby: arr.join(", ")
来源：http://bh.huanxung.cn

C#:   string.Join(", ", list)
来源：http://th.hnjuh.cn

================================================================================
来源：http://gk.shxzskj.cn

E. 字符串处理
来源：http://sv.shtwfgs.cn

================================================================================
来源：http://mv.shxzukj.cn

[E01] 拼接字符串
来源：http://sb.chemitech.net.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://th.asd995.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jn.szxytkj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ga.colortex.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gb.newstarts.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ps.nszjky.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cf.huanxung.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cf.newstarts.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xa.shxzskj.cn

[E02] 重复字符串
来源：http://cp.jctech888.com.cn

Py:   "ab" * 3
来源：http://as.panjiajie.cn

PHP:  str_repeat("ab", 3);
来源：http://nh.muxihuayi.cn

JS:   "ab".repeat(3)
来源：http://kc.wgjwhj.cn

TS:   "ab".repeat(3)
来源：http://mi.hnjuh.cn

Java: "ab".repeat(3)
来源：http://yq.nszjky.cn

Go:   strings.Repeat("ab", 3)
来源：http://nn.hahajie.cn

Ruby: "ab" * 3
来源：http://xg.szsharing.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.huanxung.cn

[E03] 截取子串
来源：http://wd.huixiangedu.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://af.bookmarksfly.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ef.nicolike.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://by.shtwfgs.cn

TS:   s.slice(1, 4)
来源：http://vx.chemitech.net.cn

Java: s.substring(1, 4)
来源：http://zy.yuntaijiaju.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wx.bookmarksfly.cn

Ruby: s[1, 3];  s[1..3]
来源：http://vq.colortex.cn

C#:   s.Substring(1, 3)
来源：http://lh.huanxung.cn

[E04] 查找子串位置
来源：http://bu.yuntaijiaju.cn

Py:   s.find("x");  s.index("x")
来源：http://qp.muxihuayi.cn

PHP:  strpos($s, "x");
来源：http://mq.shxzskj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rs.colortex.cn

TS:   s.indexOf("x")
来源：http://wf.muxihuayi.cn

Java: s.indexOf("x")
来源：http://jd.colortex.cn

Go:   strings.Index(s, "x")
来源：http://xy.huixinmuqiang.cn

Ruby: s.index("x")
来源：http://hv.shxzukj.cn

C#:   s.IndexOf("x")
来源：http://je.jianghongdianzi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://px.521024.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fz.9csxet.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ig.bookmarksfly.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cp.muxihuayi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ok.yuexingan06.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zt.yuntaijiaju.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cy.huixiangedu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nm.yuntaijiaju.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ze.nicolike.cn

[E06] 替换子串
来源：http://qp.nszjky.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://md.bjjhwx.cn

PHP:  str_replace("a", "b", $s);
来源：http://bt.huanxung.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wc.nicolike.cn

TS:   s.replaceAll("a", "b")
来源：http://xr.521024.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ec.newstarts.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zy.colortex.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fq.9csxet.cn

C#:   s.Replace("a", "b")
来源：http://zl.huixinmuqiang.cn

[E07] 按分隔符拆分
来源：http://ey.bjjhwx.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nl.yuexingan06.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fg.jctech888.com.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://pv.yuexingan06.cn

TS:   s.split(",")
来源：http://rn.bookmarksfly.cn

Java: s.split(",");  s.split("\\s+")
来源：http://fb.huanxung.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ry.szsharing.cn

Ruby: s.split(",");  s.split
来源：http://fv.newstarts.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qr.shxzskj.cn

[E08] 数组按分隔符合并
来源：http://ci.huanxung.cn

Py:   ",".join(items)
来源：http://cr.colortex.cn

PHP:  implode(",", $items);
来源：http://fy.yuexingan06.cn

JS:   items.join(",")
来源：http://pr.shxzskj.cn

TS:   items.join(",")
来源：http://ut.muxihuayi.cn

Java: String.join(",", items)
来源：http://cv.gzmigu.cn

Go:   strings.Join(items, ",")
来源：http://ni.huixinmuqiang.cn

Ruby: items.join(",")
来源：http://nw.bjjhwx.cn

C#:   string.Join(",", items)
来源：http://fa.bjjhwx.cn

[E09] 去除所有空白字符
来源：http://cc.szsharing.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://en.lnxyls.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fc.huanxung.cn

JS:   s.replace(/\s+/g, "")
来源：http://ah.shxzukj.cn

TS:   s.replace(/\s+/g, "")
来源：http://bu.yuexingan06.cn

Java: s.replaceAll("\\s+", "")
来源：http://cq.bookmarksfly.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://rp.gzmigu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://jv.nicolike.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lp.shxzukj.cn

[E10] 左侧补零 / 定长填充
来源：http://ij.huixiangedu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gk.szxytkj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://il.wgjwhj.cn

JS:   "7".padStart(3, "0")
来源：http://by.wgjwhj.cn

TS:   "7".padStart(3, "0")
来源：http://mc.jianghongdianzi.cn

Java: String.format("%03d", 7)
来源：http://py.shtwfgs.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://yg.huanxung.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hy.lnxyls.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rf.521024.cn

[E11] 反转字符串
来源：http://yq.shxzukj.cn

Py:   s[::-1]
来源：http://ih.yuexingan06.cn

PHP:  strrev($s);
来源：http://wj.szsharing.cn

JS:   [...s].reverse().join("")
来源：http://wt.9csxet.cn

TS:   [...s].reverse().join("")
来源：http://kv.muxihuayi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://aj.szxytkj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ng.szxytkj.cn

Ruby: s.reverse
来源：http://rk.muxihuayi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ic.colortex.cn

[E12] 统计某字符出现次数
来源：http://ej.szsharing.cn

Py:   s.count("a")
来源：http://se.hahajie.cn

PHP:  substr_count($s, "a");
来源：http://qb.bookmarksfly.cn

JS:   s.split("a").length - 1
来源：http://qn.shxzukj.cn

TS:   s.split("a").length - 1
来源：http://ul.chemitech.net.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zs.muxihuayi.cn

Go:   strings.Count(s, "a")
来源：http://nf.hnjuh.cn

Ruby: s.count("a")
来源：http://yw.huixiangedu.cn

C#:   s.Count(c => c == 'a')
来源：http://oq.wgjwhj.cn

[E13] 逐字符遍历
来源：http://ac.panjiajie.cn

Py:   for ch in s: print(ch)
来源：http://he.9csxet.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rg.newstarts.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ux.panjiajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://rx.hahajie.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://iw.newstarts.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://aj.jctech888.com.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://xw.jianghongdianzi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xq.huanxung.cn

[E14] URL 编码与 Base64
来源：http://ab.nicolike.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tf.bookmarksfly.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://yq.lnxyls.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hg.wgjwhj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sb.jctech888.com.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mv.yuntaijiaju.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fx.muxihuayi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ev.shtwfgs.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tm.szxytkj.cn

[E15] HTML 转义 / 反转义
来源：http://hi.huixiangedu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://pj.chemitech.net.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ff.huanxung.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ea.muxihuayi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://vl.shxzskj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xk.shxzukj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://lu.hnjuh.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rl.panjiajie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://an.szsharing.cn

[E16] 数字千分位
来源：http://wh.shxzskj.cn

Py:   f"{1234567:,}"
来源：http://kz.shxzskj.cn

PHP:  number_format(1234567);
来源：http://nd.yuexingan06.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://qn.colortex.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://gg.shxzukj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gy.huixinmuqiang.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tq.yuexingan06.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ah.nszjky.cn

C#:   1234567.ToString("N0")
来源：http://oq.bookmarksfly.cn

[E17] 首字母大写
来源：http://xr.haigaiapp.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ak.yuexingan06.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://sb.shxzskj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pj.521024.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qk.huixiangedu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wq.lnxyls.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lw.9csxet.cn

Ruby: s.capitalize
来源：http://ms.huanxung.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ae.jctech888.com.cn

[E18] 模板占位符替换
来源：http://mi.jctech888.com.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ap.hahajie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nj.bjjhwx.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://nu.hahajie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://jg.panjiajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hj.szsharing.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jv.yuntaijiaju.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xp.shxzskj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ge.shxzukj.cn

[E19] 多行文本按行拆分
来源：http://ia.nszjky.cn

Py:   s.splitlines()
来源：http://dy.colortex.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dz.huixinmuqiang.cn

JS:   s.split(/\r?\n/)
来源：http://cg.huixinmuqiang.cn

TS:   s.split(/\r?\n/)
来源：http://cd.nicolike.cn

Java: s.lines().toList()
来源：http://nu.shxzukj.cn

Go:   strings.Split(s, "\n")
来源：http://bo.colortex.cn

Ruby: s.lines
来源：http://xq.szsharing.cn

C#:   s.Split('\n')
来源：http://hb.shxzskj.cn

[E20] 判断字符串是否为空
来源：http://mf.shtwfgs.cn

Py:   if not s:
来源：http://as.bjjhwx.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://iq.9csxet.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://br.asd995.cn

TS:   if (s === "") {}
来源：http://zr.hahajie.cn

Java: if (s.isEmpty()) {}
来源：http://is.newstarts.cn

Go:   if s == "" {}
来源：http://rh.muxihuayi.cn

Ruby: if s.empty?
来源：http://pj.shtwfgs.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fm.panjiajie.cn

[E21] 超长截断加省略号
来源：http://ed.hahajie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wx.gzmigu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jv.shtwfgs.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gf.haigaiapp.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://la.chemitech.net.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qx.shxzukj.cn

Go:   // 按 rune 判断长度后截断
来源：http://lg.huixinmuqiang.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pv.huanxung.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tu.jianghongdianzi.cn

[E22] 字节长度与字符长度
来源：http://nx.wgjwhj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xs.nszjky.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zn.nszjky.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lg.newstarts.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zk.lnxyls.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lz.lnxyls.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ti.huixiangedu.cn

Ruby: s.bytesize;  s.length
来源：http://cn.shtwfgs.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kw.shtwfgs.cn

================================================================================
来源：http://vw.chemitech.net.cn

F. 文件与目录
来源：http://pw.521024.cn

================================================================================
来源：http://cv.wgjwhj.cn

[F01] 读取整个文件
来源：http://uz.shtwfgs.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fg.huixinmuqiang.cn

PHP:  file_get_contents("a.txt");
来源：http://vg.hahajie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sx.muxihuayi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bv.shxzskj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://wg.muxihuayi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nk.szxytkj.cn

Ruby: File.read("a.txt")
来源：http://nn.wgjwhj.cn

C#:   File.ReadAllText("a.txt");
来源：http://pu.huanxung.cn

[F02] 逐行读取文件
来源：http://wi.nszjky.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rx.lnxyls.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bz.bjjhwx.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xc.panjiajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zd.huixiangedu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cu.wgjwhj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ye.hnjuh.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qt.hahajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ty.nicolike.cn

[F03] 写入文件（覆盖）
来源：http://il.huixinmuqiang.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jf.muxihuayi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://lg.wgjwhj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rq.shtwfgs.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fh.9csxet.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vz.yuexingan06.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rp.nszjky.cn

Ruby: File.write("a.txt", "hi")
来源：http://vv.wgjwhj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rw.shxzskj.cn

[F04] 追加写入文件
来源：http://gj.huixinmuqiang.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://my.hahajie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yh.szsharing.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bq.bjjhwx.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lk.jctech888.com.cn


<!-- 参考信息 -->