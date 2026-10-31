代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zd.muxihuayi.cn

[D20] 统计每个元素出现次数
来源：http://no.bjjhwx.cn

Py:   Counter(arr)
来源：http://nh.haigaiapp.cn

PHP:  array_count_values($arr);
来源：http://js.panjiajie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gv.huixiangedu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iw.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kw.gzmigu.cn

Go:   // 手写 map[T]int
来源：http://vy.jianghongdianzi.cn

Ruby: arr.tally
来源：http://me.shxzskj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://js.yuexingan06.cn

[D21] 判断是否包含某元素
来源：http://dz.huixinmuqiang.cn

Py:   x in arr
来源：http://ky.haigaiapp.cn

PHP:  in_array($x, $arr, true);
来源：http://dq.bjjhwx.cn

JS:   arr.includes(x)
来源：http://ep.521024.cn

TS:   arr.includes(x)
来源：http://fe.shxzskj.cn

Java: list.contains(x)
来源：http://qg.panjiajie.cn

Go:   slices.Contains(arr, x)
来源：http://cf.szxytkj.cn

Ruby: arr.include?(x)
来源：http://uu.panjiajie.cn

C#:   list.Contains(x)
来源：http://iq.9csxet.cn

[D22] 复制数组（避免共享引用）
来源：http://ty.bjjhwx.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kp.szxytkj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ar.huixinmuqiang.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bp.panjiajie.cn

TS:   [...arr];
来源：http://vz.bjjhwx.cn

Java: new ArrayList<>(list);
来源：http://rj.asd995.cn

Go:   copied := append([]int(nil), arr...)
来源：http://sf.yuexingan06.cn

Ruby: arr.dup;  arr.clone
来源：http://hz.szxytkj.cn

C#:   new List<int>(list);
来源：http://ln.9csxet.cn

[D23] reduce 累积计算
来源：http://cw.jianghongdianzi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tb.wgjwhj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ci.panjiajie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pm.nszjky.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rp.shxzskj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://tm.huixiangedu.cn

Go:   // 手写循环
来源：http://yc.yuntaijiaju.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vn.bookmarksfly.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://uk.wgjwhj.cn

[D24] 字典 / Map 基本操作
来源：http://yo.521024.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mk.muxihuayi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yw.lnxyls.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fx.bookmarksfly.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yj.9csxet.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://sz.szxytkj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wk.colortex.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://df.lnxyls.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://sm.yuexingan06.cn

[D25] Set 集合去重与交并差
来源：http://ds.521024.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qs.521024.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fj.hahajie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rm.9csxet.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://sk.huixiangedu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://je.nicolike.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vb.yuexingan06.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qe.shxzskj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cl.shxzukj.cn

[D26] 数组转字符串
来源：http://im.haigaiapp.cn

Py:   ", ".join(map(str, arr))
来源：http://oe.huixiangedu.cn

PHP:  implode(", ", $arr);
来源：http://st.hnjuh.cn

JS:   arr.join(", ")
来源：http://ij.shxzskj.cn

TS:   arr.join(", ")
来源：http://ta.yuexingan06.cn

Java: String.join(", ", list)
来源：http://yt.nicolike.cn

Go:   strings.Join(strs, ", ")
来源：http://ho.hahajie.cn

Ruby: arr.join(", ")
来源：http://de.chemitech.net.cn

C#:   string.Join(", ", list)
来源：http://ve.huixiangedu.cn

================================================================================
来源：http://ae.lnxyls.cn

E. 字符串处理
来源：http://oc.huixiangedu.cn

================================================================================
来源：http://lh.wgjwhj.cn

[E01] 拼接字符串
来源：http://oo.szxytkj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rt.huixiangedu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kt.chemitech.net.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wv.huanxung.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://is.colortex.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zf.jctech888.com.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lv.hnjuh.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jl.panjiajie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://el.nszjky.cn

[E02] 重复字符串
来源：http://jy.shxzukj.cn

Py:   "ab" * 3
来源：http://zg.shxzukj.cn

PHP:  str_repeat("ab", 3);
来源：http://xc.yuexingan06.cn

JS:   "ab".repeat(3)
来源：http://ia.9csxet.cn

TS:   "ab".repeat(3)
来源：http://pv.huixinmuqiang.cn

Java: "ab".repeat(3)
来源：http://pa.yuntaijiaju.cn

Go:   strings.Repeat("ab", 3)
来源：http://xl.chemitech.net.cn

Ruby: "ab" * 3
来源：http://hh.bjjhwx.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ki.hahajie.cn

[E03] 截取子串
来源：http://cv.huixiangedu.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zp.gzmigu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xa.haigaiapp.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ni.panjiajie.cn

TS:   s.slice(1, 4)
来源：http://bt.521024.cn

Java: s.substring(1, 4)
来源：http://yv.lnxyls.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vf.lnxyls.cn

Ruby: s[1, 3];  s[1..3]
来源：http://eo.gzmigu.cn

C#:   s.Substring(1, 3)
来源：http://ru.huanxung.cn

[E04] 查找子串位置
来源：http://mu.shtwfgs.cn

Py:   s.find("x");  s.index("x")
来源：http://eq.yuntaijiaju.cn

PHP:  strpos($s, "x");
来源：http://yg.newstarts.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wi.huixinmuqiang.cn

TS:   s.indexOf("x")
来源：http://gd.jianghongdianzi.cn

Java: s.indexOf("x")
来源：http://uo.muxihuayi.cn

Go:   strings.Index(s, "x")
来源：http://te.wgjwhj.cn

Ruby: s.index("x")
来源：http://nj.haigaiapp.cn

C#:   s.IndexOf("x")
来源：http://dn.huixiangedu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://tv.bjjhwx.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jy.muxihuayi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sn.szsharing.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pq.nicolike.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xi.haigaiapp.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lf.shxzukj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pk.9csxet.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://am.hnjuh.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tn.huanxung.cn

[E06] 替换子串
来源：http://gz.shxzukj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cl.colortex.cn

PHP:  str_replace("a", "b", $s);
来源：http://ru.newstarts.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://am.shxzskj.cn

TS:   s.replaceAll("a", "b")
来源：http://qb.nicolike.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xt.szxytkj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://st.nicolike.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ga.shxzukj.cn

C#:   s.Replace("a", "b")
来源：http://pj.lnxyls.cn

[E07] 按分隔符拆分
来源：http://kl.jianghongdianzi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://os.lnxyls.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nd.jctech888.com.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://cf.colortex.cn

TS:   s.split(",")
来源：http://hr.huixiangedu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://md.wgjwhj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://au.nicolike.cn

Ruby: s.split(",");  s.split
来源：http://gx.jctech888.com.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://om.bookmarksfly.cn

[E08] 数组按分隔符合并
来源：http://cx.shtwfgs.cn

Py:   ",".join(items)
来源：http://ha.colortex.cn

PHP:  implode(",", $items);
来源：http://xa.chemitech.net.cn

JS:   items.join(",")
来源：http://ge.9csxet.cn

TS:   items.join(",")
来源：http://kc.shtwfgs.cn

Java: String.join(",", items)
来源：http://ce.521024.cn

Go:   strings.Join(items, ",")
来源：http://xv.yuntaijiaju.cn

Ruby: items.join(",")
来源：http://sb.yuntaijiaju.cn

C#:   string.Join(",", items)
来源：http://ln.szxytkj.cn

[E09] 去除所有空白字符
来源：http://lg.panjiajie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cp.yuexingan06.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lz.szxytkj.cn

JS:   s.replace(/\s+/g, "")
来源：http://od.szxytkj.cn

TS:   s.replace(/\s+/g, "")
来源：http://hw.bjjhwx.cn

Java: s.replaceAll("\\s+", "")
来源：http://ps.huixinmuqiang.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://hm.9csxet.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ms.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vx.gzmigu.cn

[E10] 左侧补零 / 定长填充
来源：http://zs.gzmigu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mt.lnxyls.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dt.shxzskj.cn

JS:   "7".padStart(3, "0")
来源：http://lj.nszjky.cn

TS:   "7".padStart(3, "0")
来源：http://tw.jianghongdianzi.cn

Java: String.format("%03d", 7)
来源：http://ib.shxzskj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://tx.asd995.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ua.asd995.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vh.bjjhwx.cn

[E11] 反转字符串
来源：http://wr.bookmarksfly.cn

Py:   s[::-1]
来源：http://oh.haigaiapp.cn

PHP:  strrev($s);
来源：http://au.szxytkj.cn

JS:   [...s].reverse().join("")
来源：http://vz.nszjky.cn

TS:   [...s].reverse().join("")
来源：http://rh.shxzukj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://gx.jctech888.com.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://yp.shxzskj.cn

Ruby: s.reverse
来源：http://ua.huixinmuqiang.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vg.szxytkj.cn

[E12] 统计某字符出现次数
来源：http://nl.9csxet.cn

Py:   s.count("a")
来源：http://mr.gzmigu.cn

PHP:  substr_count($s, "a");
来源：http://uo.haigaiapp.cn

JS:   s.split("a").length - 1
来源：http://nl.szxytkj.cn

TS:   s.split("a").length - 1
来源：http://gd.521024.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dr.yuntaijiaju.cn

Go:   strings.Count(s, "a")
来源：http://nk.asd995.cn

Ruby: s.count("a")
来源：http://or.jianghongdianzi.cn

C#:   s.Count(c => c == 'a')
来源：http://bq.huixinmuqiang.cn

[E13] 逐字符遍历
来源：http://fo.shxzskj.cn

Py:   for ch in s: print(ch)
来源：http://gb.gzmigu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://py.jianghongdianzi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://qs.shxzskj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.gzmigu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ax.yuexingan06.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dp.nicolike.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rl.huixinmuqiang.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kt.lnxyls.cn

[E14] URL 编码与 Base64
来源：http://zx.hahajie.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ce.newstarts.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://wf.huixinmuqiang.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dq.hnjuh.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qw.521024.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fs.bookmarksfly.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://en.nszjky.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://if.newstarts.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ry.bjjhwx.cn

[E15] HTML 转义 / 反转义
来源：http://ck.bookmarksfly.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://dw.asd995.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pl.9csxet.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://id.nicolike.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://yc.chemitech.net.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vf.yuntaijiaju.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pr.hnjuh.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://os.haigaiapp.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vu.gzmigu.cn

[E16] 数字千分位
来源：http://ed.colortex.cn

Py:   f"{1234567:,}"
来源：http://bo.gzmigu.cn

PHP:  number_format(1234567);
来源：http://jx.colortex.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://xk.szsharing.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://lb.hahajie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fk.shxzskj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tq.huixinmuqiang.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://li.hnjuh.cn

C#:   1234567.ToString("N0")
来源：http://xt.yuexingan06.cn

[E17] 首字母大写
来源：http://fw.chemitech.net.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://si.521024.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://hk.gzmigu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pv.asd995.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pc.521024.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://td.shxzskj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yl.szsharing.cn

Ruby: s.capitalize
来源：http://rf.521024.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qo.9csxet.cn

[E18] 模板占位符替换
来源：http://sz.9csxet.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://er.szsharing.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ce.lnxyls.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://cc.newstarts.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://qj.asd995.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://io.newstarts.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ww.hnjuh.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qq.huanxung.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yh.szsharing.cn

[E19] 多行文本按行拆分
来源：http://im.bookmarksfly.cn

Py:   s.splitlines()
来源：http://rr.muxihuayi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rg.shxzskj.cn

JS:   s.split(/\r?\n/)
来源：http://ww.haigaiapp.cn

TS:   s.split(/\r?\n/)
来源：http://vp.huixinmuqiang.cn

Java: s.lines().toList()
来源：http://cc.asd995.cn

Go:   strings.Split(s, "\n")
来源：http://sz.panjiajie.cn

Ruby: s.lines
来源：http://im.521024.cn

C#:   s.Split('\n')
来源：http://yj.lnxyls.cn

[E20] 判断字符串是否为空
来源：http://ds.szsharing.cn

Py:   if not s:
来源：http://ku.jctech888.com.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ex.hahajie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yq.521024.cn

TS:   if (s === "") {}
来源：http://vh.nicolike.cn

Java: if (s.isEmpty()) {}
来源：http://me.yuntaijiaju.cn

Go:   if s == "" {}
来源：http://jw.gzmigu.cn

Ruby: if s.empty?
来源：http://dt.haigaiapp.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lo.jianghongdianzi.cn

[E21] 超长截断加省略号
来源：http://he.9csxet.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wg.huixiangedu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xk.wgjwhj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ld.huixinmuqiang.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://aq.shxzukj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pk.shtwfgs.cn

Go:   // 按 rune 判断长度后截断
来源：http://tb.gzmigu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mt.lnxyls.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xj.9csxet.cn

[E22] 字节长度与字符长度
来源：http://mb.shxzskj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ac.colortex.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://aj.hahajie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://no.lnxyls.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gf.lnxyls.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dp.nszjky.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jf.yuntaijiaju.cn

Ruby: s.bytesize;  s.length
来源：http://bi.huanxung.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://iz.bjjhwx.cn

================================================================================
来源：http://mb.521024.cn

F. 文件与目录
来源：http://jh.521024.cn

================================================================================
来源：http://tm.shxzskj.cn

[F01] 读取整个文件
来源：http://id.newstarts.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tl.jctech888.com.cn

PHP:  file_get_contents("a.txt");
来源：http://ay.muxihuayi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xu.asd995.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lj.bookmarksfly.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://qe.521024.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vp.gzmigu.cn

Ruby: File.read("a.txt")
来源：http://vq.shtwfgs.cn

C#:   File.ReadAllText("a.txt");
来源：http://cb.hnjuh.cn

[F02] 逐行读取文件
来源：http://gv.nszjky.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://eq.chemitech.net.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jl.szxytkj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wl.huixiangedu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ua.yuntaijiaju.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jj.haigaiapp.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tq.shtwfgs.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vq.asd995.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xd.shxzukj.cn

[F03] 写入文件（覆盖）
来源：http://pd.colortex.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mc.shxzukj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://kw.shxzukj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wu.haigaiapp.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nw.hnjuh.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kf.hnjuh.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nb.colortex.cn

Ruby: File.write("a.txt", "hi")
来源：http://ja.bookmarksfly.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kq.colortex.cn

[F04] 追加写入文件
来源：http://zt.shxzskj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kr.shxzukj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nn.lnxyls.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ua.shxzskj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xx.haigaiapp.cn


<!-- 参考信息 -->