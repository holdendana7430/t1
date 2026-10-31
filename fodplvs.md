代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://sz.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yx.wgjwhj.cn

Go:   // 手写 map[string][]T
来源：http://ke.colortex.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://md.colortex.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bt.bookmarksfly.cn

[D20] 统计每个元素出现次数
来源：http://ur.nszjky.cn

Py:   Counter(arr)
来源：http://nh.muxihuayi.cn

PHP:  array_count_values($arr);
来源：http://gf.shxzskj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ea.hnjuh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qb.wgjwhj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fu.asd995.cn

Go:   // 手写 map[T]int
来源：http://cr.gzmigu.cn

Ruby: arr.tally
来源：http://ux.shxzukj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xn.9csxet.cn

[D21] 判断是否包含某元素
来源：http://gg.colortex.cn

Py:   x in arr
来源：http://pm.jianghongdianzi.cn

PHP:  in_array($x, $arr, true);
来源：http://oz.shxzukj.cn

JS:   arr.includes(x)
来源：http://hy.yuntaijiaju.cn

TS:   arr.includes(x)
来源：http://wf.huanxung.cn

Java: list.contains(x)
来源：http://ce.huixinmuqiang.cn

Go:   slices.Contains(arr, x)
来源：http://vp.chemitech.net.cn

Ruby: arr.include?(x)
来源：http://cm.lnxyls.cn

C#:   list.Contains(x)
来源：http://xu.gzmigu.cn

[D22] 复制数组（避免共享引用）
来源：http://ov.nicolike.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mr.panjiajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gu.shxzukj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mv.nicolike.cn

TS:   [...arr];
来源：http://jh.panjiajie.cn

Java: new ArrayList<>(list);
来源：http://qw.jctech888.com.cn

Go:   copied := append([]int(nil), arr...)
来源：http://wj.huixiangedu.cn

Ruby: arr.dup;  arr.clone
来源：http://qz.chemitech.net.cn

C#:   new List<int>(list);
来源：http://xq.szxytkj.cn

[D23] reduce 累积计算
来源：http://ce.bjjhwx.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mj.szxytkj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ky.huanxung.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://aa.asd995.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zu.nszjky.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://uh.szxytkj.cn

Go:   // 手写循环
来源：http://vd.nicolike.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tv.asd995.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pl.muxihuayi.cn

[D24] 字典 / Map 基本操作
来源：http://fx.chemitech.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ta.shtwfgs.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vs.yuntaijiaju.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nk.shxzskj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://so.bookmarksfly.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vv.muxihuayi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://oq.huanxung.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ih.haigaiapp.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kh.hahajie.cn

[D25] Set 集合去重与交并差
来源：http://im.nicolike.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ql.bjjhwx.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.shxzukj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ls.lnxyls.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bw.nszjky.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://yq.huixiangedu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xq.haigaiapp.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gf.wgjwhj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ks.lnxyls.cn

[D26] 数组转字符串
来源：http://ni.szxytkj.cn

Py:   ", ".join(map(str, arr))
来源：http://rq.asd995.cn

PHP:  implode(", ", $arr);
来源：http://si.nszjky.cn

JS:   arr.join(", ")
来源：http://il.9csxet.cn

TS:   arr.join(", ")
来源：http://fm.nszjky.cn

Java: String.join(", ", list)
来源：http://gw.szxytkj.cn

Go:   strings.Join(strs, ", ")
来源：http://fp.hahajie.cn

Ruby: arr.join(", ")
来源：http://vk.bookmarksfly.cn

C#:   string.Join(", ", list)
来源：http://pv.521024.cn

================================================================================
来源：http://ky.nszjky.cn

E. 字符串处理
来源：http://jy.szxytkj.cn

================================================================================
来源：http://fw.bookmarksfly.cn

[E01] 拼接字符串
来源：http://up.hnjuh.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bj.szxytkj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://us.9csxet.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vs.gzmigu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gw.gzmigu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://oz.huanxung.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://eu.yuexingan06.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cw.huixiangedu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xq.nszjky.cn

[E02] 重复字符串
来源：http://jn.chemitech.net.cn

Py:   "ab" * 3
来源：http://rr.newstarts.cn

PHP:  str_repeat("ab", 3);
来源：http://lp.hnjuh.cn

JS:   "ab".repeat(3)
来源：http://gf.jianghongdianzi.cn

TS:   "ab".repeat(3)
来源：http://gj.shxzskj.cn

Java: "ab".repeat(3)
来源：http://zu.jctech888.com.cn

Go:   strings.Repeat("ab", 3)
来源：http://zi.bookmarksfly.cn

Ruby: "ab" * 3
来源：http://kb.huixinmuqiang.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hg.szxytkj.cn

[E03] 截取子串
来源：http://vy.huanxung.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nk.hnjuh.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mf.haigaiapp.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nk.huanxung.cn

TS:   s.slice(1, 4)
来源：http://zg.bookmarksfly.cn

Java: s.substring(1, 4)
来源：http://pj.hahajie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sq.shxzukj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://yf.panjiajie.cn

C#:   s.Substring(1, 3)
来源：http://ez.asd995.cn

[E04] 查找子串位置
来源：http://um.colortex.cn

Py:   s.find("x");  s.index("x")
来源：http://ha.gzmigu.cn

PHP:  strpos($s, "x");
来源：http://zo.yuntaijiaju.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ao.nicolike.cn

TS:   s.indexOf("x")
来源：http://ki.yuntaijiaju.cn

Java: s.indexOf("x")
来源：http://og.asd995.cn

Go:   strings.Index(s, "x")
来源：http://gi.nszjky.cn

Ruby: s.index("x")
来源：http://vb.huixiangedu.cn

C#:   s.IndexOf("x")
来源：http://vl.9csxet.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://za.hnjuh.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://po.asd995.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cy.gzmigu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ia.muxihuayi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://jo.jctech888.com.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jr.colortex.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fz.hahajie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ut.nicolike.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hm.shxzukj.cn

[E06] 替换子串
来源：http://oc.jctech888.com.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://aq.lnxyls.cn

PHP:  str_replace("a", "b", $s);
来源：http://ot.szsharing.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pt.asd995.cn

TS:   s.replaceAll("a", "b")
来源：http://ds.panjiajie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yq.jctech888.com.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://na.shtwfgs.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://du.lnxyls.cn

C#:   s.Replace("a", "b")
来源：http://rs.521024.cn

[E07] 按分隔符拆分
来源：http://zr.colortex.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jw.newstarts.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hn.wgjwhj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://zl.bookmarksfly.cn

TS:   s.split(",")
来源：http://qv.huixinmuqiang.cn

Java: s.split(",");  s.split("\\s+")
来源：http://iv.shxzukj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xm.yuexingan06.cn

Ruby: s.split(",");  s.split
来源：http://vi.huanxung.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zh.huixiangedu.cn

[E08] 数组按分隔符合并
来源：http://mw.gzmigu.cn

Py:   ",".join(items)
来源：http://bg.huixinmuqiang.cn

PHP:  implode(",", $items);
来源：http://kk.9csxet.cn

JS:   items.join(",")
来源：http://qs.lnxyls.cn

TS:   items.join(",")
来源：http://dp.shtwfgs.cn

Java: String.join(",", items)
来源：http://gv.nszjky.cn

Go:   strings.Join(items, ",")
来源：http://is.9csxet.cn

Ruby: items.join(",")
来源：http://ew.bjjhwx.cn

C#:   string.Join(",", items)
来源：http://fj.bookmarksfly.cn

[E09] 去除所有空白字符
来源：http://he.colortex.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ar.hnjuh.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://uj.wgjwhj.cn

JS:   s.replace(/\s+/g, "")
来源：http://wz.jianghongdianzi.cn

TS:   s.replace(/\s+/g, "")
来源：http://za.yuexingan06.cn

Java: s.replaceAll("\\s+", "")
来源：http://hr.szsharing.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ct.huixinmuqiang.cn

Ruby: s.gsub(/\s+/, "")
来源：http://sw.yuexingan06.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bq.gzmigu.cn

[E10] 左侧补零 / 定长填充
来源：http://kh.shxzskj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kd.gzmigu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qq.panjiajie.cn

JS:   "7".padStart(3, "0")
来源：http://tu.muxihuayi.cn

TS:   "7".padStart(3, "0")
来源：http://vv.9csxet.cn

Java: String.format("%03d", 7)
来源：http://et.hahajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ft.newstarts.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cq.bookmarksfly.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zx.lnxyls.cn

[E11] 反转字符串
来源：http://yr.szsharing.cn

Py:   s[::-1]
来源：http://hn.yuntaijiaju.cn

PHP:  strrev($s);
来源：http://xg.jianghongdianzi.cn

JS:   [...s].reverse().join("")
来源：http://pd.yuexingan06.cn

TS:   [...s].reverse().join("")
来源：http://cv.hahajie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ii.szxytkj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://uc.shxzskj.cn

Ruby: s.reverse
来源：http://zq.huanxung.cn

C#:   new string(s.Reverse().ToArray())
来源：http://cp.521024.cn

[E12] 统计某字符出现次数
来源：http://cu.asd995.cn

Py:   s.count("a")
来源：http://yr.asd995.cn

PHP:  substr_count($s, "a");
来源：http://vt.newstarts.cn

JS:   s.split("a").length - 1
来源：http://ok.asd995.cn

TS:   s.split("a").length - 1
来源：http://pz.jctech888.com.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dc.chemitech.net.cn

Go:   strings.Count(s, "a")
来源：http://pn.wgjwhj.cn

Ruby: s.count("a")
来源：http://ir.9csxet.cn

C#:   s.Count(c => c == 'a')
来源：http://mg.haigaiapp.cn

[E13] 逐字符遍历
来源：http://xy.gzmigu.cn

Py:   for ch in s: print(ch)
来源：http://vr.bookmarksfly.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vi.bookmarksfly.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://cx.haigaiapp.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bl.panjiajie.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xs.yuexingan06.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rt.jctech888.com.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://in.shxzukj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yc.bjjhwx.cn

[E14] URL 编码与 Base64
来源：http://dx.chemitech.net.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ku.asd995.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://he.yuntaijiaju.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nb.521024.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zr.521024.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gk.yuexingan06.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fv.shtwfgs.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qy.jctech888.com.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ul.huixiangedu.cn

[E15] HTML 转义 / 反转义
来源：http://pc.haigaiapp.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://vd.shxzukj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://br.wgjwhj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rw.jianghongdianzi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wx.hahajie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pw.gzmigu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://eg.lnxyls.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vc.colortex.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ce.shxzskj.cn

[E16] 数字千分位
来源：http://jg.wgjwhj.cn

Py:   f"{1234567:,}"
来源：http://ga.colortex.cn

PHP:  number_format(1234567);
来源：http://hj.szxytkj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ez.asd995.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wo.9csxet.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cx.colortex.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wo.bjjhwx.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ez.huixiangedu.cn

C#:   1234567.ToString("N0")
来源：http://tq.huanxung.cn

[E17] 首字母大写
来源：http://aq.shxzukj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ap.nicolike.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://tw.hnjuh.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ai.szxytkj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gv.shtwfgs.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://im.jctech888.com.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ye.521024.cn

Ruby: s.capitalize
来源：http://ux.nicolike.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bk.chemitech.net.cn

[E18] 模板占位符替换
来源：http://ex.newstarts.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qz.asd995.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ko.hnjuh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://kl.gzmigu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://at.jctech888.com.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://am.gzmigu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jh.bjjhwx.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ds.bookmarksfly.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ha.colortex.cn

[E19] 多行文本按行拆分
来源：http://rf.szxytkj.cn

Py:   s.splitlines()
来源：http://zu.asd995.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kw.shxzukj.cn

JS:   s.split(/\r?\n/)
来源：http://io.newstarts.cn

TS:   s.split(/\r?\n/)
来源：http://es.szxytkj.cn

Java: s.lines().toList()
来源：http://le.bjjhwx.cn

Go:   strings.Split(s, "\n")
来源：http://cn.huixinmuqiang.cn

Ruby: s.lines
来源：http://vg.szsharing.cn

C#:   s.Split('\n')
来源：http://qq.gzmigu.cn

[E20] 判断字符串是否为空
来源：http://dz.huanxung.cn

Py:   if not s:
来源：http://iu.nicolike.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wb.hnjuh.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://og.9csxet.cn

TS:   if (s === "") {}
来源：http://nz.nszjky.cn

Java: if (s.isEmpty()) {}
来源：http://qf.jctech888.com.cn

Go:   if s == "" {}
来源：http://jg.huixinmuqiang.cn

Ruby: if s.empty?
来源：http://it.shxzukj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kd.colortex.cn

[E21] 超长截断加省略号
来源：http://oo.muxihuayi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://go.gzmigu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yk.hnjuh.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sj.hahajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://di.bjjhwx.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://uc.newstarts.cn

Go:   // 按 rune 判断长度后截断
来源：http://pv.szxytkj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yp.shxzukj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pn.huixinmuqiang.cn

[E22] 字节长度与字符长度
来源：http://ic.szsharing.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sz.huixiangedu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://go.newstarts.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vh.muxihuayi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://le.nicolike.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://iv.lnxyls.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qy.yuexingan06.cn

Ruby: s.bytesize;  s.length
来源：http://nl.521024.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cl.shtwfgs.cn

================================================================================
来源：http://bc.jianghongdianzi.cn

F. 文件与目录
来源：http://kx.jianghongdianzi.cn

================================================================================
来源：http://nl.bookmarksfly.cn

[F01] 读取整个文件
来源：http://rq.asd995.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gl.haigaiapp.cn

PHP:  file_get_contents("a.txt");
来源：http://rp.521024.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qq.wgjwhj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://km.huanxung.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://os.newstarts.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fu.huixinmuqiang.cn

Ruby: File.read("a.txt")
来源：http://ns.yuntaijiaju.cn

C#:   File.ReadAllText("a.txt");
来源：http://ak.lnxyls.cn

[F02] 逐行读取文件
来源：http://ih.colortex.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kb.colortex.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://as.yuexingan06.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hs.asd995.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ya.bookmarksfly.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://we.shtwfgs.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ko.szxytkj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bz.wgjwhj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kk.szxytkj.cn

[F03] 写入文件（覆盖）
来源：http://lp.panjiajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bd.jianghongdianzi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://lx.newstarts.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qd.nicolike.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zi.shtwfgs.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qb.huixinmuqiang.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gm.bjjhwx.cn

Ruby: File.write("a.txt", "hi")
来源：http://fk.yuntaijiaju.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dt.lnxyls.cn

[F04] 追加写入文件
来源：http://px.wgjwhj.cn


<!-- 参考信息 -->