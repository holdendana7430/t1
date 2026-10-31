代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qc.szsharing.cn

[D20] 统计每个元素出现次数
来源：http://dl.huixiangedu.cn

Py:   Counter(arr)
来源：http://zm.colortex.cn

PHP:  array_count_values($arr);
来源：http://ul.yuntaijiaju.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gb.haigaiapp.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ho.chemitech.net.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qk.huixinmuqiang.cn

Go:   // 手写 map[T]int
来源：http://yi.szsharing.cn

Ruby: arr.tally
来源：http://pf.haigaiapp.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yd.bjjhwx.cn

[D21] 判断是否包含某元素
来源：http://ek.nszjky.cn

Py:   x in arr
来源：http://ne.muxihuayi.cn

PHP:  in_array($x, $arr, true);
来源：http://hd.yuexingan06.cn

JS:   arr.includes(x)
来源：http://yv.lnxyls.cn

TS:   arr.includes(x)
来源：http://nr.panjiajie.cn

Java: list.contains(x)
来源：http://gw.521024.cn

Go:   slices.Contains(arr, x)
来源：http://hw.muxihuayi.cn

Ruby: arr.include?(x)
来源：http://vb.huixiangedu.cn

C#:   list.Contains(x)
来源：http://cp.shtwfgs.cn

[D22] 复制数组（避免共享引用）
来源：http://in.szsharing.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dc.huixinmuqiang.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zx.huixiangedu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qu.muxihuayi.cn

TS:   [...arr];
来源：http://vv.lnxyls.cn

Java: new ArrayList<>(list);
来源：http://lp.bjjhwx.cn

Go:   copied := append([]int(nil), arr...)
来源：http://td.muxihuayi.cn

Ruby: arr.dup;  arr.clone
来源：http://kp.hahajie.cn

C#:   new List<int>(list);
来源：http://tz.bookmarksfly.cn

[D23] reduce 累积计算
来源：http://ic.nszjky.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ns.wgjwhj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tg.9csxet.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lp.521024.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ak.chemitech.net.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://mq.nicolike.cn

Go:   // 手写循环
来源：http://ct.yuntaijiaju.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hh.hnjuh.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fy.lnxyls.cn

[D24] 字典 / Map 基本操作
来源：http://eu.chemitech.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kk.szsharing.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kh.lnxyls.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://yq.wgjwhj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dg.muxihuayi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://om.gzmigu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://no.gzmigu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://sh.shxzukj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qa.muxihuayi.cn

[D25] Set 集合去重与交并差
来源：http://df.shxzukj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vu.szsharing.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zz.yuexingan06.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yx.haigaiapp.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xu.panjiajie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ob.muxihuayi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ir.chemitech.net.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wo.bjjhwx.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mc.9csxet.cn

[D26] 数组转字符串
来源：http://ow.szsharing.cn

Py:   ", ".join(map(str, arr))
来源：http://ps.lnxyls.cn

PHP:  implode(", ", $arr);
来源：http://is.shtwfgs.cn

JS:   arr.join(", ")
来源：http://si.muxihuayi.cn

TS:   arr.join(", ")
来源：http://qc.521024.cn

Java: String.join(", ", list)
来源：http://hk.shtwfgs.cn

Go:   strings.Join(strs, ", ")
来源：http://aa.jianghongdianzi.cn

Ruby: arr.join(", ")
来源：http://ex.shtwfgs.cn

C#:   string.Join(", ", list)
来源：http://rj.bjjhwx.cn

================================================================================
来源：http://ht.9csxet.cn

E. 字符串处理
来源：http://oj.9csxet.cn

================================================================================
来源：http://yg.lnxyls.cn

[E01] 拼接字符串
来源：http://hc.hnjuh.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pf.szxytkj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://de.hnjuh.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gi.szxytkj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zs.shxzskj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wy.newstarts.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sp.muxihuayi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://at.huanxung.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qg.huixiangedu.cn

[E02] 重复字符串
来源：http://bc.yuntaijiaju.cn

Py:   "ab" * 3
来源：http://df.bookmarksfly.cn

PHP:  str_repeat("ab", 3);
来源：http://rw.jianghongdianzi.cn

JS:   "ab".repeat(3)
来源：http://zf.shtwfgs.cn

TS:   "ab".repeat(3)
来源：http://lo.bookmarksfly.cn

Java: "ab".repeat(3)
来源：http://hy.nszjky.cn

Go:   strings.Repeat("ab", 3)
来源：http://ij.lnxyls.cn

Ruby: "ab" * 3
来源：http://yz.huixiangedu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qo.huixinmuqiang.cn

[E03] 截取子串
来源：http://bk.bjjhwx.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ic.colortex.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cg.jianghongdianzi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ji.szsharing.cn

TS:   s.slice(1, 4)
来源：http://ss.szsharing.cn

Java: s.substring(1, 4)
来源：http://oa.szsharing.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gr.huixiangedu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ix.hahajie.cn

C#:   s.Substring(1, 3)
来源：http://gi.muxihuayi.cn

[E04] 查找子串位置
来源：http://aa.lnxyls.cn

Py:   s.find("x");  s.index("x")
来源：http://qh.muxihuayi.cn

PHP:  strpos($s, "x");
来源：http://xj.shxzskj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sz.shxzskj.cn

TS:   s.indexOf("x")
来源：http://uy.colortex.cn

Java: s.indexOf("x")
来源：http://uf.asd995.cn

Go:   strings.Index(s, "x")
来源：http://kp.521024.cn

Ruby: s.index("x")
来源：http://dv.colortex.cn

C#:   s.IndexOf("x")
来源：http://re.yuntaijiaju.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xu.yuntaijiaju.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pg.huixiangedu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lh.yuexingan06.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vt.521024.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://wu.gzmigu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://au.yuexingan06.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mz.yuntaijiaju.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lo.huixiangedu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cm.haigaiapp.cn

[E06] 替换子串
来源：http://ii.nszjky.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qy.hahajie.cn

PHP:  str_replace("a", "b", $s);
来源：http://xp.huixinmuqiang.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lj.chemitech.net.cn

TS:   s.replaceAll("a", "b")
来源：http://om.wgjwhj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://do.9csxet.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ct.haigaiapp.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wq.jianghongdianzi.cn

C#:   s.Replace("a", "b")
来源：http://po.shtwfgs.cn

[E07] 按分隔符拆分
来源：http://tt.hahajie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xt.nszjky.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://oz.huixiangedu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://wu.szsharing.cn

TS:   s.split(",")
来源：http://gv.huixinmuqiang.cn

Java: s.split(",");  s.split("\\s+")
来源：http://mn.jianghongdianzi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jm.shxzskj.cn

Ruby: s.split(",");  s.split
来源：http://nc.szxytkj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://az.gzmigu.cn

[E08] 数组按分隔符合并
来源：http://rk.yuexingan06.cn

Py:   ",".join(items)
来源：http://jp.bookmarksfly.cn

PHP:  implode(",", $items);
来源：http://eq.bjjhwx.cn

JS:   items.join(",")
来源：http://wx.9csxet.cn

TS:   items.join(",")
来源：http://fi.huanxung.cn

Java: String.join(",", items)
来源：http://qi.nszjky.cn

Go:   strings.Join(items, ",")
来源：http://un.521024.cn

Ruby: items.join(",")
来源：http://px.521024.cn

C#:   string.Join(",", items)
来源：http://dw.szxytkj.cn

[E09] 去除所有空白字符
来源：http://ld.nszjky.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nm.bjjhwx.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ik.huixinmuqiang.cn

JS:   s.replace(/\s+/g, "")
来源：http://ze.gzmigu.cn

TS:   s.replace(/\s+/g, "")
来源：http://bn.newstarts.cn

Java: s.replaceAll("\\s+", "")
来源：http://xm.gzmigu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://hy.jianghongdianzi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://vl.shxzukj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hv.wgjwhj.cn

[E10] 左侧补零 / 定长填充
来源：http://xj.chemitech.net.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ob.szxytkj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jk.haigaiapp.cn

JS:   "7".padStart(3, "0")
来源：http://eh.521024.cn

TS:   "7".padStart(3, "0")
来源：http://mk.hahajie.cn

Java: String.format("%03d", 7)
来源：http://gi.521024.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ox.jctech888.com.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fz.chemitech.net.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mf.haigaiapp.cn

[E11] 反转字符串
来源：http://za.nszjky.cn

Py:   s[::-1]
来源：http://rw.bjjhwx.cn

PHP:  strrev($s);
来源：http://cn.asd995.cn

JS:   [...s].reverse().join("")
来源：http://tl.jianghongdianzi.cn

TS:   [...s].reverse().join("")
来源：http://ln.shtwfgs.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://vg.nszjky.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://vi.jianghongdianzi.cn

Ruby: s.reverse
来源：http://ya.panjiajie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://zz.yuntaijiaju.cn

[E12] 统计某字符出现次数
来源：http://np.huixiangedu.cn

Py:   s.count("a")
来源：http://yt.huanxung.cn

PHP:  substr_count($s, "a");
来源：http://pe.shxzskj.cn

JS:   s.split("a").length - 1
来源：http://ep.szsharing.cn

TS:   s.split("a").length - 1
来源：http://jx.shxzskj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mo.muxihuayi.cn

Go:   strings.Count(s, "a")
来源：http://ns.chemitech.net.cn

Ruby: s.count("a")
来源：http://tm.nicolike.cn

C#:   s.Count(c => c == 'a')
来源：http://pp.panjiajie.cn

[E13] 逐字符遍历
来源：http://vv.bjjhwx.cn

Py:   for ch in s: print(ch)
来源：http://ow.huanxung.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qi.nicolike.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ph.yuexingan06.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://jz.shxzukj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qj.bjjhwx.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://or.jctech888.com.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://qc.jctech888.com.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://km.nszjky.cn

[E14] URL 编码与 Base64
来源：http://ac.huanxung.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fx.nicolike.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://we.haigaiapp.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://eb.chemitech.net.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pj.jianghongdianzi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bd.nicolike.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ms.huixinmuqiang.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cy.szsharing.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ds.shtwfgs.cn

[E15] HTML 转义 / 反转义
来源：http://fr.shtwfgs.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://be.gzmigu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yx.newstarts.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bx.huixinmuqiang.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://rv.jianghongdianzi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ho.bjjhwx.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://eg.gzmigu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jd.bookmarksfly.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ly.colortex.cn

[E16] 数字千分位
来源：http://ec.yuntaijiaju.cn

Py:   f"{1234567:,}"
来源：http://ee.bookmarksfly.cn

PHP:  number_format(1234567);
来源：http://yc.szxytkj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ae.lnxyls.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://le.bookmarksfly.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ga.yuntaijiaju.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qp.jctech888.com.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rx.szsharing.cn

C#:   1234567.ToString("N0")
来源：http://ge.nicolike.cn

[E17] 首字母大写
来源：http://hm.newstarts.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rn.colortex.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://da.huixinmuqiang.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gg.jianghongdianzi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jr.hnjuh.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fb.521024.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://si.bjjhwx.cn

Ruby: s.capitalize
来源：http://fk.bookmarksfly.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://di.shxzukj.cn

[E18] 模板占位符替换
来源：http://cz.newstarts.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hl.chemitech.net.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://oa.yuexingan06.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://wv.shxzukj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://zs.gzmigu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://sh.yuntaijiaju.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gs.szxytkj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mu.haigaiapp.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tf.szxytkj.cn

[E19] 多行文本按行拆分
来源：http://ai.yuntaijiaju.cn

Py:   s.splitlines()
来源：http://cb.521024.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cj.huixinmuqiang.cn

JS:   s.split(/\r?\n/)
来源：http://ca.newstarts.cn

TS:   s.split(/\r?\n/)
来源：http://tf.yuntaijiaju.cn

Java: s.lines().toList()
来源：http://op.521024.cn

Go:   strings.Split(s, "\n")
来源：http://iy.huixiangedu.cn

Ruby: s.lines
来源：http://ex.bjjhwx.cn

C#:   s.Split('\n')
来源：http://nw.9csxet.cn

[E20] 判断字符串是否为空
来源：http://hv.huanxung.cn

Py:   if not s:
来源：http://ir.panjiajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nn.panjiajie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bb.jctech888.com.cn

TS:   if (s === "") {}
来源：http://zb.szxytkj.cn

Java: if (s.isEmpty()) {}
来源：http://nf.szsharing.cn

Go:   if s == "" {}
来源：http://xd.yuntaijiaju.cn

Ruby: if s.empty?
来源：http://uq.521024.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ks.haigaiapp.cn

[E21] 超长截断加省略号
来源：http://xa.jctech888.com.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vr.jianghongdianzi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zv.huixiangedu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wb.jianghongdianzi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rg.yuexingan06.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gy.nszjky.cn

Go:   // 按 rune 判断长度后截断
来源：http://tj.shxzukj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jj.jianghongdianzi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://uc.colortex.cn

[E22] 字节长度与字符长度
来源：http://ug.panjiajie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://px.gzmigu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pb.nszjky.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dj.huixinmuqiang.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kg.bjjhwx.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sw.shtwfgs.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ko.9csxet.cn

Ruby: s.bytesize;  s.length
来源：http://ie.panjiajie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jf.newstarts.cn

================================================================================
来源：http://zl.haigaiapp.cn

F. 文件与目录
来源：http://lk.szxytkj.cn

================================================================================
来源：http://hx.bookmarksfly.cn

[F01] 读取整个文件
来源：http://xl.yuexingan06.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://za.hnjuh.cn

PHP:  file_get_contents("a.txt");
来源：http://ke.huanxung.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ck.nicolike.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ox.asd995.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ak.9csxet.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xj.huixiangedu.cn

Ruby: File.read("a.txt")
来源：http://gg.shxzskj.cn

C#:   File.ReadAllText("a.txt");
来源：http://vr.shtwfgs.cn

[F02] 逐行读取文件
来源：http://zi.gzmigu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wp.nszjky.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://di.haigaiapp.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xr.panjiajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mg.9csxet.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fs.gzmigu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qu.szxytkj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qb.jianghongdianzi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hu.wgjwhj.cn

[F03] 写入文件（覆盖）
来源：http://eh.panjiajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kx.521024.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://mv.muxihuayi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pe.jctech888.com.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yc.jctech888.com.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://py.bookmarksfly.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tv.9csxet.cn

Ruby: File.write("a.txt", "hi")
来源：http://nm.9csxet.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xb.jianghongdianzi.cn

[F04] 追加写入文件
来源：http://fs.gzmigu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://uh.newstarts.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yt.bjjhwx.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ba.shxzukj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ls.huixinmuqiang.cn


<!-- 参考信息 -->