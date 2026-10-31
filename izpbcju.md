代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://uq.hahajie.cn

[D20] 统计每个元素出现次数
来源：http://dw.9csxet.cn

Py:   Counter(arr)
来源：http://hh.shxzukj.cn

PHP:  array_count_values($arr);
来源：http://hb.gzmigu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mu.gzmigu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://da.wgjwhj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://uj.shxzskj.cn

Go:   // 手写 map[T]int
来源：http://po.jctech888.com.cn

Ruby: arr.tally
来源：http://qj.haigaiapp.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cg.chemitech.net.cn

[D21] 判断是否包含某元素
来源：http://nk.shxzskj.cn

Py:   x in arr
来源：http://ls.huanxung.cn

PHP:  in_array($x, $arr, true);
来源：http://ss.hahajie.cn

JS:   arr.includes(x)
来源：http://uq.wgjwhj.cn

TS:   arr.includes(x)
来源：http://zo.huixinmuqiang.cn

Java: list.contains(x)
来源：http://se.shtwfgs.cn

Go:   slices.Contains(arr, x)
来源：http://oo.lnxyls.cn

Ruby: arr.include?(x)
来源：http://fs.yuntaijiaju.cn

C#:   list.Contains(x)
来源：http://hl.521024.cn

[D22] 复制数组（避免共享引用）
来源：http://xu.huixiangedu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://me.hahajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ys.szsharing.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hb.huixiangedu.cn

TS:   [...arr];
来源：http://re.gzmigu.cn

Java: new ArrayList<>(list);
来源：http://fn.colortex.cn

Go:   copied := append([]int(nil), arr...)
来源：http://lv.shtwfgs.cn

Ruby: arr.dup;  arr.clone
来源：http://ia.jianghongdianzi.cn

C#:   new List<int>(list);
来源：http://ig.shxzukj.cn

[D23] reduce 累积计算
来源：http://ud.szsharing.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hx.lnxyls.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wo.yuntaijiaju.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hy.gzmigu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iw.shtwfgs.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://il.haigaiapp.cn

Go:   // 手写循环
来源：http://jr.hahajie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zx.nicolike.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ya.newstarts.cn

[D24] 字典 / Map 基本操作
来源：http://wd.521024.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gm.9csxet.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kw.nszjky.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tq.jctech888.com.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xi.jianghongdianzi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kv.yuexingan06.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rm.szsharing.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://th.yuntaijiaju.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pv.shxzskj.cn

[D25] Set 集合去重与交并差
来源：http://qw.colortex.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bb.wgjwhj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ms.szxytkj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vq.shxzskj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ez.gzmigu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zb.lnxyls.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wt.panjiajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jd.hahajie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lu.wgjwhj.cn

[D26] 数组转字符串
来源：http://yn.521024.cn

Py:   ", ".join(map(str, arr))
来源：http://bt.gzmigu.cn

PHP:  implode(", ", $arr);
来源：http://fg.huixiangedu.cn

JS:   arr.join(", ")
来源：http://av.szsharing.cn

TS:   arr.join(", ")
来源：http://li.hahajie.cn

Java: String.join(", ", list)
来源：http://un.wgjwhj.cn

Go:   strings.Join(strs, ", ")
来源：http://vb.lnxyls.cn

Ruby: arr.join(", ")
来源：http://qo.szsharing.cn

C#:   string.Join(", ", list)
来源：http://db.chemitech.net.cn

================================================================================
来源：http://gw.shtwfgs.cn

E. 字符串处理
来源：http://ji.shxzskj.cn

================================================================================
来源：http://yr.shxzskj.cn

[E01] 拼接字符串
来源：http://cx.nicolike.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://so.shxzukj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ok.chemitech.net.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ao.hahajie.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dn.shtwfgs.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://au.newstarts.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://th.shxzukj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gr.wgjwhj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vs.hahajie.cn

[E02] 重复字符串
来源：http://jt.shxzukj.cn

Py:   "ab" * 3
来源：http://bd.wgjwhj.cn

PHP:  str_repeat("ab", 3);
来源：http://du.bookmarksfly.cn

JS:   "ab".repeat(3)
来源：http://sh.jianghongdianzi.cn

TS:   "ab".repeat(3)
来源：http://rd.chemitech.net.cn

Java: "ab".repeat(3)
来源：http://xc.hnjuh.cn

Go:   strings.Repeat("ab", 3)
来源：http://se.nszjky.cn

Ruby: "ab" * 3
来源：http://yi.hahajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zp.shtwfgs.cn

[E03] 截取子串
来源：http://fw.yuntaijiaju.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lp.huixinmuqiang.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pu.huixinmuqiang.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sk.shxzskj.cn

TS:   s.slice(1, 4)
来源：http://ec.muxihuayi.cn

Java: s.substring(1, 4)
来源：http://iz.bookmarksfly.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sw.bookmarksfly.cn

Ruby: s[1, 3];  s[1..3]
来源：http://pz.colortex.cn

C#:   s.Substring(1, 3)
来源：http://rd.asd995.cn

[E04] 查找子串位置
来源：http://ty.hnjuh.cn

Py:   s.find("x");  s.index("x")
来源：http://dw.panjiajie.cn

PHP:  strpos($s, "x");
来源：http://mq.nszjky.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hb.newstarts.cn

TS:   s.indexOf("x")
来源：http://yk.szsharing.cn

Java: s.indexOf("x")
来源：http://bv.nszjky.cn

Go:   strings.Index(s, "x")
来源：http://jn.bookmarksfly.cn

Ruby: s.index("x")
来源：http://xs.bookmarksfly.cn

C#:   s.IndexOf("x")
来源：http://uj.haigaiapp.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://rh.521024.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nr.colortex.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ss.asd995.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gq.yuexingan06.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://pc.gzmigu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ki.shxzukj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ph.nicolike.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://so.haigaiapp.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ri.hnjuh.cn

[E06] 替换子串
来源：http://bz.panjiajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yi.shxzskj.cn

PHP:  str_replace("a", "b", $s);
来源：http://lq.asd995.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yb.colortex.cn

TS:   s.replaceAll("a", "b")
来源：http://bu.yuntaijiaju.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://au.9csxet.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qe.jctech888.com.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vu.asd995.cn

C#:   s.Replace("a", "b")
来源：http://dh.521024.cn

[E07] 按分隔符拆分
来源：http://mz.shtwfgs.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rr.muxihuayi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gi.bookmarksfly.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://sn.shxzukj.cn

TS:   s.split(",")
来源：http://hz.hnjuh.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ih.wgjwhj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wb.lnxyls.cn

Ruby: s.split(",");  s.split
来源：http://zf.hahajie.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xf.nicolike.cn

[E08] 数组按分隔符合并
来源：http://ft.szxytkj.cn

Py:   ",".join(items)
来源：http://eb.szxytkj.cn

PHP:  implode(",", $items);
来源：http://lb.nszjky.cn

JS:   items.join(",")
来源：http://bb.9csxet.cn

TS:   items.join(",")
来源：http://dk.yuexingan06.cn

Java: String.join(",", items)
来源：http://sy.shtwfgs.cn

Go:   strings.Join(items, ",")
来源：http://uz.jianghongdianzi.cn

Ruby: items.join(",")
来源：http://qh.hnjuh.cn

C#:   string.Join(",", items)
来源：http://rn.panjiajie.cn

[E09] 去除所有空白字符
来源：http://kz.szxytkj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nz.jianghongdianzi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nr.yuexingan06.cn

JS:   s.replace(/\s+/g, "")
来源：http://rm.wgjwhj.cn

TS:   s.replace(/\s+/g, "")
来源：http://sv.bookmarksfly.cn

Java: s.replaceAll("\\s+", "")
来源：http://wi.521024.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ju.shtwfgs.cn

Ruby: s.gsub(/\s+/, "")
来源：http://cv.asd995.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gz.muxihuayi.cn

[E10] 左侧补零 / 定长填充
来源：http://ja.521024.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pj.panjiajie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ce.bjjhwx.cn

JS:   "7".padStart(3, "0")
来源：http://iy.huixinmuqiang.cn

TS:   "7".padStart(3, "0")
来源：http://qu.bjjhwx.cn

Java: String.format("%03d", 7)
来源：http://ku.wgjwhj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://hd.nicolike.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wh.nicolike.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ji.huixinmuqiang.cn

[E11] 反转字符串
来源：http://ju.huanxung.cn

Py:   s[::-1]
来源：http://fl.nicolike.cn

PHP:  strrev($s);
来源：http://vv.huixinmuqiang.cn

JS:   [...s].reverse().join("")
来源：http://nd.yuntaijiaju.cn

TS:   [...s].reverse().join("")
来源：http://wv.521024.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://mw.hahajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://sw.bjjhwx.cn

Ruby: s.reverse
来源：http://lf.bjjhwx.cn

C#:   new string(s.Reverse().ToArray())
来源：http://us.hahajie.cn

[E12] 统计某字符出现次数
来源：http://kw.nszjky.cn

Py:   s.count("a")
来源：http://st.haigaiapp.cn

PHP:  substr_count($s, "a");
来源：http://hr.asd995.cn

JS:   s.split("a").length - 1
来源：http://vo.huixiangedu.cn

TS:   s.split("a").length - 1
来源：http://gd.panjiajie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yb.muxihuayi.cn

Go:   strings.Count(s, "a")
来源：http://lk.huixiangedu.cn

Ruby: s.count("a")
来源：http://fm.asd995.cn

C#:   s.Count(c => c == 'a')
来源：http://wi.panjiajie.cn

[E13] 逐字符遍历
来源：http://zu.gzmigu.cn

Py:   for ch in s: print(ch)
来源：http://ae.9csxet.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cv.nicolike.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xc.huixinmuqiang.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://kc.haigaiapp.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://by.shtwfgs.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pg.shxzukj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://sp.hnjuh.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mk.szxytkj.cn

[E14] URL 编码与 Base64
来源：http://lw.bookmarksfly.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ho.nszjky.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://iv.jctech888.com.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tb.9csxet.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zf.hnjuh.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yr.521024.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cy.hnjuh.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://sh.colortex.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bg.haigaiapp.cn

[E15] HTML 转义 / 反转义
来源：http://xn.nszjky.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://vb.hnjuh.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zg.szxytkj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pj.asd995.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ww.hnjuh.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ki.521024.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vq.szxytkj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://np.yuntaijiaju.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xo.gzmigu.cn

[E16] 数字千分位
来源：http://au.colortex.cn

Py:   f"{1234567:,}"
来源：http://fx.szsharing.cn

PHP:  number_format(1234567);
来源：http://so.muxihuayi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ij.yuntaijiaju.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://dd.shxzukj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vh.wgjwhj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xc.szxytkj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nq.hnjuh.cn

C#:   1234567.ToString("N0")
来源：http://gs.jctech888.com.cn

[E17] 首字母大写
来源：http://sr.gzmigu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ep.jianghongdianzi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://dl.bookmarksfly.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fv.shxzukj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gw.wgjwhj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lt.chemitech.net.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ch.shxzukj.cn

Ruby: s.capitalize
来源：http://zu.asd995.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ue.shxzskj.cn

[E18] 模板占位符替换
来源：http://uy.muxihuayi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dt.nszjky.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fn.chemitech.net.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://en.wgjwhj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ti.colortex.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vq.gzmigu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sh.shxzukj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xw.9csxet.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nf.colortex.cn

[E19] 多行文本按行拆分
来源：http://tz.hnjuh.cn

Py:   s.splitlines()
来源：http://ed.jctech888.com.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ni.panjiajie.cn

JS:   s.split(/\r?\n/)
来源：http://hc.chemitech.net.cn

TS:   s.split(/\r?\n/)
来源：http://an.lnxyls.cn

Java: s.lines().toList()
来源：http://ar.szsharing.cn

Go:   strings.Split(s, "\n")
来源：http://yo.hahajie.cn

Ruby: s.lines
来源：http://vi.muxihuayi.cn

C#:   s.Split('\n')
来源：http://fr.haigaiapp.cn

[E20] 判断字符串是否为空
来源：http://xd.nicolike.cn

Py:   if not s:
来源：http://bh.haigaiapp.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qy.nicolike.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ep.hahajie.cn

TS:   if (s === "") {}
来源：http://kq.jianghongdianzi.cn

Java: if (s.isEmpty()) {}
来源：http://ou.shtwfgs.cn

Go:   if s == "" {}
来源：http://ti.yuexingan06.cn

Ruby: if s.empty?
来源：http://zp.shtwfgs.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hi.hnjuh.cn

[E21] 超长截断加省略号
来源：http://zt.muxihuayi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pc.szsharing.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pm.lnxyls.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yn.shxzukj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fi.asd995.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jr.jianghongdianzi.cn

Go:   // 按 rune 判断长度后截断
来源：http://di.huixinmuqiang.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gs.jianghongdianzi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rr.wgjwhj.cn

[E22] 字节长度与字符长度
来源：http://of.yuexingan06.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mx.521024.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fy.wgjwhj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rb.shxzskj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ep.shtwfgs.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://va.huixinmuqiang.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dz.asd995.cn

Ruby: s.bytesize;  s.length
来源：http://yt.yuexingan06.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gn.bjjhwx.cn

================================================================================
来源：http://cc.nszjky.cn

F. 文件与目录
来源：http://wz.szxytkj.cn

================================================================================
来源：http://qu.panjiajie.cn

[F01] 读取整个文件
来源：http://ga.nicolike.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://et.hahajie.cn

PHP:  file_get_contents("a.txt");
来源：http://gl.jctech888.com.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://an.huanxung.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sg.hahajie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jx.nszjky.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gq.muxihuayi.cn

Ruby: File.read("a.txt")
来源：http://ni.shxzskj.cn

C#:   File.ReadAllText("a.txt");
来源：http://ox.jianghongdianzi.cn

[F02] 逐行读取文件
来源：http://wy.chemitech.net.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xt.shtwfgs.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://oq.9csxet.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vh.huixinmuqiang.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sw.huixiangedu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fe.szsharing.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vq.szxytkj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hd.wgjwhj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gp.huanxung.cn

[F03] 写入文件（覆盖）
来源：http://jy.szsharing.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pu.chemitech.net.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://lm.shxzskj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://if.asd995.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qz.hahajie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wd.nicolike.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wv.521024.cn

Ruby: File.write("a.txt", "hi")
来源：http://lm.jctech888.com.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bf.jianghongdianzi.cn

[F04] 追加写入文件
来源：http://nm.bjjhwx.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://oy.nszjky.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://he.asd995.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uc.9csxet.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fy.wgjwhj.cn


<!-- 参考信息 -->