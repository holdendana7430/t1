代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fa.szxytkj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fs.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xs.shxzskj.cn

Go:   // 手写 map[T]int
来源：http://mh.wgjwhj.cn

Ruby: arr.tally
来源：http://kk.hnjuh.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cq.shtwfgs.cn

[D21] 判断是否包含某元素
来源：http://wk.nszjky.cn

Py:   x in arr
来源：http://gq.yuexingan06.cn

PHP:  in_array($x, $arr, true);
来源：http://ap.colortex.cn

JS:   arr.includes(x)
来源：http://wb.huanxung.cn

TS:   arr.includes(x)
来源：http://mc.jctech888.com.cn

Java: list.contains(x)
来源：http://ra.panjiajie.cn

Go:   slices.Contains(arr, x)
来源：http://lf.jianghongdianzi.cn

Ruby: arr.include?(x)
来源：http://zc.szsharing.cn

C#:   list.Contains(x)
来源：http://ra.shxzukj.cn

[D22] 复制数组（避免共享引用）
来源：http://zd.yuexingan06.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bo.szxytkj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tn.yuntaijiaju.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bp.szsharing.cn

TS:   [...arr];
来源：http://bf.shxzukj.cn

Java: new ArrayList<>(list);
来源：http://sz.haigaiapp.cn

Go:   copied := append([]int(nil), arr...)
来源：http://nq.asd995.cn

Ruby: arr.dup;  arr.clone
来源：http://oy.asd995.cn

C#:   new List<int>(list);
来源：http://yi.huanxung.cn

[D23] reduce 累积计算
来源：http://ku.bookmarksfly.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cg.huanxung.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://sk.gzmigu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ty.hnjuh.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sm.chemitech.net.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://mm.shxzukj.cn

Go:   // 手写循环
来源：http://ey.shtwfgs.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jg.huanxung.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ua.wgjwhj.cn

[D24] 字典 / Map 基本操作
来源：http://ge.bookmarksfly.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://er.nszjky.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.shxzskj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wm.lnxyls.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hj.huixiangedu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://sa.521024.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gg.nicolike.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gv.jianghongdianzi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jd.szsharing.cn

[D25] Set 集合去重与交并差
来源：http://rw.szxytkj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bn.lnxyls.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://en.bookmarksfly.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://op.shtwfgs.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yd.yuntaijiaju.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ud.muxihuayi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hn.hnjuh.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zp.lnxyls.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cc.bookmarksfly.cn

[D26] 数组转字符串
来源：http://rq.colortex.cn

Py:   ", ".join(map(str, arr))
来源：http://jj.521024.cn

PHP:  implode(", ", $arr);
来源：http://al.nicolike.cn

JS:   arr.join(", ")
来源：http://aq.hahajie.cn

TS:   arr.join(", ")
来源：http://br.nicolike.cn

Java: String.join(", ", list)
来源：http://xz.gzmigu.cn

Go:   strings.Join(strs, ", ")
来源：http://yz.521024.cn

Ruby: arr.join(", ")
来源：http://uy.chemitech.net.cn

C#:   string.Join(", ", list)
来源：http://bu.newstarts.cn

================================================================================
来源：http://ci.gzmigu.cn

E. 字符串处理
来源：http://ut.newstarts.cn

================================================================================
来源：http://ap.chemitech.net.cn

[E01] 拼接字符串
来源：http://uj.muxihuayi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cy.jctech888.com.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rj.asd995.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zh.huixinmuqiang.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gc.szsharing.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qr.yuntaijiaju.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ut.chemitech.net.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kx.colortex.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lp.bjjhwx.cn

[E02] 重复字符串
来源：http://vg.huanxung.cn

Py:   "ab" * 3
来源：http://kw.shtwfgs.cn

PHP:  str_repeat("ab", 3);
来源：http://gv.muxihuayi.cn

JS:   "ab".repeat(3)
来源：http://zq.nszjky.cn

TS:   "ab".repeat(3)
来源：http://cq.chemitech.net.cn

Java: "ab".repeat(3)
来源：http://sn.colortex.cn

Go:   strings.Repeat("ab", 3)
来源：http://qj.shtwfgs.cn

Ruby: "ab" * 3
来源：http://hd.haigaiapp.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zn.shxzukj.cn

[E03] 截取子串
来源：http://nj.521024.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zp.haigaiapp.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nw.huanxung.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://br.lnxyls.cn

TS:   s.slice(1, 4)
来源：http://yy.bjjhwx.cn

Java: s.substring(1, 4)
来源：http://tz.hahajie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://we.shxzskj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zb.huixinmuqiang.cn

C#:   s.Substring(1, 3)
来源：http://xo.shxzukj.cn

[E04] 查找子串位置
来源：http://ed.chemitech.net.cn

Py:   s.find("x");  s.index("x")
来源：http://fi.szxytkj.cn

PHP:  strpos($s, "x");
来源：http://yl.haigaiapp.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yk.nicolike.cn

TS:   s.indexOf("x")
来源：http://qr.bjjhwx.cn

Java: s.indexOf("x")
来源：http://qt.gzmigu.cn

Go:   strings.Index(s, "x")
来源：http://ch.hahajie.cn

Ruby: s.index("x")
来源：http://rr.huixiangedu.cn

C#:   s.IndexOf("x")
来源：http://wz.nszjky.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://lo.bjjhwx.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fx.gzmigu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ha.huanxung.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rr.hnjuh.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://bc.bjjhwx.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lh.bookmarksfly.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vp.newstarts.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mh.szsharing.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xs.bookmarksfly.cn

[E06] 替换子串
来源：http://fn.huanxung.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dk.nszjky.cn

PHP:  str_replace("a", "b", $s);
来源：http://ba.nicolike.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fj.shxzskj.cn

TS:   s.replaceAll("a", "b")
来源：http://sc.nszjky.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hw.shtwfgs.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vl.colortex.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://eg.9csxet.cn

C#:   s.Replace("a", "b")
来源：http://wp.huanxung.cn

[E07] 按分隔符拆分
来源：http://rh.huixinmuqiang.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lx.hnjuh.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tq.lnxyls.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://at.shxzukj.cn

TS:   s.split(",")
来源：http://ro.hnjuh.cn

Java: s.split(",");  s.split("\\s+")
来源：http://nw.9csxet.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dx.lnxyls.cn

Ruby: s.split(",");  s.split
来源：http://qa.huixinmuqiang.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hd.huixiangedu.cn

[E08] 数组按分隔符合并
来源：http://mk.521024.cn

Py:   ",".join(items)
来源：http://mg.9csxet.cn

PHP:  implode(",", $items);
来源：http://zm.bjjhwx.cn

JS:   items.join(",")
来源：http://ic.gzmigu.cn

TS:   items.join(",")
来源：http://xz.wgjwhj.cn

Java: String.join(",", items)
来源：http://qm.shxzskj.cn

Go:   strings.Join(items, ",")
来源：http://cq.panjiajie.cn

Ruby: items.join(",")
来源：http://pr.yuntaijiaju.cn

C#:   string.Join(",", items)
来源：http://ah.huixiangedu.cn

[E09] 去除所有空白字符
来源：http://vi.hahajie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rq.colortex.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kf.nicolike.cn

JS:   s.replace(/\s+/g, "")
来源：http://pc.hnjuh.cn

TS:   s.replace(/\s+/g, "")
来源：http://xs.panjiajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://oe.panjiajie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://tg.9csxet.cn

Ruby: s.gsub(/\s+/, "")
来源：http://su.asd995.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wi.9csxet.cn

[E10] 左侧补零 / 定长填充
来源：http://df.shxzskj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gn.yuexingan06.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mg.nszjky.cn

JS:   "7".padStart(3, "0")
来源：http://nu.huixinmuqiang.cn

TS:   "7".padStart(3, "0")
来源：http://iw.wgjwhj.cn

Java: String.format("%03d", 7)
来源：http://gr.panjiajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://gf.hahajie.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mb.shxzskj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nf.jianghongdianzi.cn

[E11] 反转字符串
来源：http://xg.nicolike.cn

Py:   s[::-1]
来源：http://pd.hahajie.cn

PHP:  strrev($s);
来源：http://pk.521024.cn

JS:   [...s].reverse().join("")
来源：http://fy.nszjky.cn

TS:   [...s].reverse().join("")
来源：http://ar.asd995.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://fl.haigaiapp.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://dg.huixiangedu.cn

Ruby: s.reverse
来源：http://jl.gzmigu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://dk.gzmigu.cn

[E12] 统计某字符出现次数
来源：http://tm.wgjwhj.cn

Py:   s.count("a")
来源：http://lf.nszjky.cn

PHP:  substr_count($s, "a");
来源：http://gu.huixiangedu.cn

JS:   s.split("a").length - 1
来源：http://kl.9csxet.cn

TS:   s.split("a").length - 1
来源：http://ok.haigaiapp.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pn.huixiangedu.cn

Go:   strings.Count(s, "a")
来源：http://pm.szxytkj.cn

Ruby: s.count("a")
来源：http://xn.szsharing.cn

C#:   s.Count(c => c == 'a')
来源：http://no.szsharing.cn

[E13] 逐字符遍历
来源：http://km.bjjhwx.cn

Py:   for ch in s: print(ch)
来源：http://ov.shxzskj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xs.colortex.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://tp.huixinmuqiang.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://uz.chemitech.net.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cf.nicolike.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gx.muxihuayi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://sk.bjjhwx.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yw.gzmigu.cn

[E14] URL 编码与 Base64
来源：http://tq.yuexingan06.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qa.huanxung.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://oa.huixiangedu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yc.haigaiapp.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jz.jctech888.com.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qs.gzmigu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ks.bookmarksfly.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nj.jianghongdianzi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://it.szxytkj.cn

[E15] HTML 转义 / 反转义
来源：http://ql.newstarts.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ib.yuexingan06.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bo.521024.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://au.haigaiapp.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://eq.szxytkj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ph.panjiajie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nq.panjiajie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fg.asd995.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ph.huixinmuqiang.cn

[E16] 数字千分位
来源：http://dm.newstarts.cn

Py:   f"{1234567:,}"
来源：http://en.jctech888.com.cn

PHP:  number_format(1234567);
来源：http://pk.jianghongdianzi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://nv.huanxung.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://pi.muxihuayi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://uj.szxytkj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ke.shtwfgs.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://yl.lnxyls.cn

C#:   1234567.ToString("N0")
来源：http://aq.panjiajie.cn

[E17] 首字母大写
来源：http://xd.panjiajie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vn.nicolike.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xq.521024.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xf.521024.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ni.yuntaijiaju.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kv.jctech888.com.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hy.shtwfgs.cn

Ruby: s.capitalize
来源：http://da.9csxet.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dg.szsharing.cn

[E18] 模板占位符替换
来源：http://uz.wgjwhj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wj.jianghongdianzi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zp.asd995.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://pc.szsharing.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://aw.shxzukj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ek.yuexingan06.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fc.bookmarksfly.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://oh.szxytkj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://aq.muxihuayi.cn

[E19] 多行文本按行拆分
来源：http://qc.nicolike.cn

Py:   s.splitlines()
来源：http://br.gzmigu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pg.newstarts.cn

JS:   s.split(/\r?\n/)
来源：http://ft.shtwfgs.cn

TS:   s.split(/\r?\n/)
来源：http://mh.yuntaijiaju.cn

Java: s.lines().toList()
来源：http://xl.huixiangedu.cn

Go:   strings.Split(s, "\n")
来源：http://rz.yuntaijiaju.cn

Ruby: s.lines
来源：http://dw.jianghongdianzi.cn

C#:   s.Split('\n')
来源：http://za.521024.cn

[E20] 判断字符串是否为空
来源：http://uz.9csxet.cn

Py:   if not s:
来源：http://sg.gzmigu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yh.colortex.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yc.nicolike.cn

TS:   if (s === "") {}
来源：http://hg.bookmarksfly.cn

Java: if (s.isEmpty()) {}
来源：http://gd.lnxyls.cn

Go:   if s == "" {}
来源：http://tx.521024.cn

Ruby: if s.empty?
来源：http://ui.jianghongdianzi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gf.nszjky.cn

[E21] 超长截断加省略号
来源：http://bp.muxihuayi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dk.hnjuh.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://iy.yuntaijiaju.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wu.gzmigu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wa.hnjuh.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://eh.yuntaijiaju.cn

Go:   // 按 rune 判断长度后截断
来源：http://ht.wgjwhj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lk.bookmarksfly.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://yc.muxihuayi.cn

[E22] 字节长度与字符长度
来源：http://yp.huixiangedu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qo.lnxyls.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sf.asd995.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xy.shxzukj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ii.chemitech.net.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kd.jianghongdianzi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://az.yuntaijiaju.cn

Ruby: s.bytesize;  s.length
来源：http://kn.newstarts.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wd.shxzukj.cn

================================================================================
来源：http://oa.huanxung.cn

F. 文件与目录
来源：http://np.hahajie.cn

================================================================================
来源：http://vc.newstarts.cn

[F01] 读取整个文件
来源：http://ko.hnjuh.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://oa.chemitech.net.cn

PHP:  file_get_contents("a.txt");
来源：http://gz.hahajie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bt.gzmigu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jh.yuexingan06.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jl.panjiajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vh.szxytkj.cn

Ruby: File.read("a.txt")
来源：http://op.nicolike.cn

C#:   File.ReadAllText("a.txt");
来源：http://nq.9csxet.cn

[F02] 逐行读取文件
来源：http://oo.haigaiapp.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://id.haigaiapp.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ez.gzmigu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cw.shxzskj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://os.jctech888.com.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rp.wgjwhj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mo.hnjuh.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ys.jianghongdianzi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ww.lnxyls.cn

[F03] 写入文件（覆盖）
来源：http://kb.lnxyls.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gv.huanxung.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://lr.asd995.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ph.lnxyls.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://my.szxytkj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fc.gzmigu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dh.haigaiapp.cn

Ruby: File.write("a.txt", "hi")
来源：http://lh.haigaiapp.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qs.hnjuh.cn

[F04] 追加写入文件
来源：http://fc.szxytkj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zn.nszjky.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://oz.szsharing.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cl.shxzskj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ui.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hg.9csxet.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nu.haigaiapp.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cr.newstarts.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lx.9csxet.cn


<!-- 参考信息 -->