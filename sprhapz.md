代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://es.haigaiapp.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kr.wgjwhj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ff.9csxet.cn

Go:   // 手写 map[T]int
来源：http://hq.gzmigu.cn

Ruby: arr.tally
来源：http://qb.asd995.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ec.newstarts.cn

[D21] 判断是否包含某元素
来源：http://jj.shxzskj.cn

Py:   x in arr
来源：http://yb.huanxung.cn

PHP:  in_array($x, $arr, true);
来源：http://hh.jianghongdianzi.cn

JS:   arr.includes(x)
来源：http://ok.haigaiapp.cn

TS:   arr.includes(x)
来源：http://da.szsharing.cn

Java: list.contains(x)
来源：http://ac.9csxet.cn

Go:   slices.Contains(arr, x)
来源：http://uy.chemitech.net.cn

Ruby: arr.include?(x)
来源：http://ov.haigaiapp.cn

C#:   list.Contains(x)
来源：http://ut.huixiangedu.cn

[D22] 复制数组（避免共享引用）
来源：http://kf.wgjwhj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ui.9csxet.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cb.yuexingan06.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://sl.yuntaijiaju.cn

TS:   [...arr];
来源：http://az.9csxet.cn

Java: new ArrayList<>(list);
来源：http://ut.wgjwhj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://vz.lnxyls.cn

Ruby: arr.dup;  arr.clone
来源：http://ns.hahajie.cn

C#:   new List<int>(list);
来源：http://pk.chemitech.net.cn

[D23] reduce 累积计算
来源：http://re.asd995.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://br.shtwfgs.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fw.szxytkj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wu.nicolike.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sz.shxzskj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://cd.nszjky.cn

Go:   // 手写循环
来源：http://re.nszjky.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ip.huixinmuqiang.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ea.lnxyls.cn

[D24] 字典 / Map 基本操作
来源：http://bj.bjjhwx.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cn.haigaiapp.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ln.newstarts.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hr.newstarts.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rn.nicolike.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gh.jianghongdianzi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lc.hnjuh.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xt.yuexingan06.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zi.nszjky.cn

[D25] Set 集合去重与交并差
来源：http://aj.shtwfgs.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://iz.jianghongdianzi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fj.yuntaijiaju.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://sv.jctech888.com.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://to.gzmigu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ka.yuexingan06.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kn.szsharing.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ne.panjiajie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fd.hnjuh.cn

[D26] 数组转字符串
来源：http://xo.panjiajie.cn

Py:   ", ".join(map(str, arr))
来源：http://qh.9csxet.cn

PHP:  implode(", ", $arr);
来源：http://qp.haigaiapp.cn

JS:   arr.join(", ")
来源：http://ao.huanxung.cn

TS:   arr.join(", ")
来源：http://tm.nszjky.cn

Java: String.join(", ", list)
来源：http://fn.lnxyls.cn

Go:   strings.Join(strs, ", ")
来源：http://de.colortex.cn

Ruby: arr.join(", ")
来源：http://hb.muxihuayi.cn

C#:   string.Join(", ", list)
来源：http://tr.9csxet.cn

================================================================================
来源：http://dn.asd995.cn

E. 字符串处理
来源：http://ai.panjiajie.cn

================================================================================
来源：http://tf.szxytkj.cn

[E01] 拼接字符串
来源：http://wp.bjjhwx.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ol.hnjuh.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://az.huixiangedu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qf.bookmarksfly.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tf.haigaiapp.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ht.bjjhwx.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wi.yuntaijiaju.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rh.nicolike.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://uj.jctech888.com.cn

[E02] 重复字符串
来源：http://ry.521024.cn

Py:   "ab" * 3
来源：http://sz.haigaiapp.cn

PHP:  str_repeat("ab", 3);
来源：http://te.yuntaijiaju.cn

JS:   "ab".repeat(3)
来源：http://wc.huixinmuqiang.cn

TS:   "ab".repeat(3)
来源：http://qv.nicolike.cn

Java: "ab".repeat(3)
来源：http://gi.newstarts.cn

Go:   strings.Repeat("ab", 3)
来源：http://gu.haigaiapp.cn

Ruby: "ab" * 3
来源：http://mw.muxihuayi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nv.hnjuh.cn

[E03] 截取子串
来源：http://ye.huanxung.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kv.huixiangedu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://db.bookmarksfly.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xn.bjjhwx.cn

TS:   s.slice(1, 4)
来源：http://np.chemitech.net.cn

Java: s.substring(1, 4)
来源：http://cr.jianghongdianzi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://or.hahajie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://uo.huanxung.cn

C#:   s.Substring(1, 3)
来源：http://mw.huixinmuqiang.cn

[E04] 查找子串位置
来源：http://sd.9csxet.cn

Py:   s.find("x");  s.index("x")
来源：http://iu.colortex.cn

PHP:  strpos($s, "x");
来源：http://zy.hnjuh.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sm.bookmarksfly.cn

TS:   s.indexOf("x")
来源：http://ew.huanxung.cn

Java: s.indexOf("x")
来源：http://rw.shxzukj.cn

Go:   strings.Index(s, "x")
来源：http://dw.bjjhwx.cn

Ruby: s.index("x")
来源：http://jl.szsharing.cn

C#:   s.IndexOf("x")
来源：http://qy.yuntaijiaju.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ep.9csxet.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rl.yuntaijiaju.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://og.nszjky.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://us.newstarts.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hp.lnxyls.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nh.shxzukj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yo.asd995.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qi.shtwfgs.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zv.haigaiapp.cn

[E06] 替换子串
来源：http://tg.jianghongdianzi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bj.shxzskj.cn

PHP:  str_replace("a", "b", $s);
来源：http://ld.huixiangedu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mx.shxzskj.cn

TS:   s.replaceAll("a", "b")
来源：http://ah.szxytkj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://im.huanxung.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jb.shxzskj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nb.nicolike.cn

C#:   s.Replace("a", "b")
来源：http://cb.yuntaijiaju.cn

[E07] 按分隔符拆分
来源：http://ut.9csxet.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tj.yuexingan06.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xn.huixinmuqiang.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://je.9csxet.cn

TS:   s.split(",")
来源：http://up.9csxet.cn

Java: s.split(",");  s.split("\\s+")
来源：http://db.wgjwhj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hb.huanxung.cn

Ruby: s.split(",");  s.split
来源：http://uh.nicolike.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://eu.hnjuh.cn

[E08] 数组按分隔符合并
来源：http://hb.jianghongdianzi.cn

Py:   ",".join(items)
来源：http://ff.shxzukj.cn

PHP:  implode(",", $items);
来源：http://yi.szxytkj.cn

JS:   items.join(",")
来源：http://yz.bjjhwx.cn

TS:   items.join(",")
来源：http://dg.gzmigu.cn

Java: String.join(",", items)
来源：http://xu.hnjuh.cn

Go:   strings.Join(items, ",")
来源：http://sc.hahajie.cn

Ruby: items.join(",")
来源：http://sl.shtwfgs.cn

C#:   string.Join(",", items)
来源：http://rn.gzmigu.cn

[E09] 去除所有空白字符
来源：http://ey.yuexingan06.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rq.wgjwhj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yp.gzmigu.cn

JS:   s.replace(/\s+/g, "")
来源：http://tz.yuexingan06.cn

TS:   s.replace(/\s+/g, "")
来源：http://jm.hnjuh.cn

Java: s.replaceAll("\\s+", "")
来源：http://to.wgjwhj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://xi.muxihuayi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://mt.shxzukj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ec.yuexingan06.cn

[E10] 左侧补零 / 定长填充
来源：http://rh.colortex.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tw.bookmarksfly.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qx.bookmarksfly.cn

JS:   "7".padStart(3, "0")
来源：http://oc.haigaiapp.cn

TS:   "7".padStart(3, "0")
来源：http://lc.gzmigu.cn

Java: String.format("%03d", 7)
来源：http://db.shtwfgs.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://vp.yuexingan06.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fd.haigaiapp.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pp.shxzskj.cn

[E11] 反转字符串
来源：http://uj.lnxyls.cn

Py:   s[::-1]
来源：http://rq.asd995.cn

PHP:  strrev($s);
来源：http://sm.521024.cn

JS:   [...s].reverse().join("")
来源：http://yt.hnjuh.cn

TS:   [...s].reverse().join("")
来源：http://ud.bjjhwx.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://jl.bjjhwx.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://pv.yuntaijiaju.cn

Ruby: s.reverse
来源：http://tc.lnxyls.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qz.521024.cn

[E12] 统计某字符出现次数
来源：http://tt.huanxung.cn

Py:   s.count("a")
来源：http://hf.gzmigu.cn

PHP:  substr_count($s, "a");
来源：http://en.huixiangedu.cn

JS:   s.split("a").length - 1
来源：http://tg.shxzskj.cn

TS:   s.split("a").length - 1
来源：http://ur.bookmarksfly.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yp.nszjky.cn

Go:   strings.Count(s, "a")
来源：http://xu.haigaiapp.cn

Ruby: s.count("a")
来源：http://ao.9csxet.cn

C#:   s.Count(c => c == 'a')
来源：http://qk.hahajie.cn

[E13] 逐字符遍历
来源：http://er.yuntaijiaju.cn

Py:   for ch in s: print(ch)
来源：http://hx.chemitech.net.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rv.9csxet.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ws.nszjky.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://az.bookmarksfly.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sq.szsharing.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xz.yuntaijiaju.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://hd.nicolike.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ng.haigaiapp.cn

[E14] URL 编码与 Base64
来源：http://wp.huanxung.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ak.shtwfgs.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ey.521024.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lc.hnjuh.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://re.huixiangedu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dx.yuexingan06.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bj.bookmarksfly.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gx.shxzskj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vo.shtwfgs.cn

[E15] HTML 转义 / 反转义
来源：http://rc.wgjwhj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://oq.muxihuayi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hv.huanxung.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gp.jianghongdianzi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ts.szxytkj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bv.asd995.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tr.nicolike.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qc.bjjhwx.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://br.9csxet.cn

[E16] 数字千分位
来源：http://me.bjjhwx.cn

Py:   f"{1234567:,}"
来源：http://lr.shxzskj.cn

PHP:  number_format(1234567);
来源：http://vq.hahajie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://eu.wgjwhj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ki.colortex.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bi.asd995.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bf.chemitech.net.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://yk.colortex.cn

C#:   1234567.ToString("N0")
来源：http://xh.haigaiapp.cn

[E17] 首字母大写
来源：http://gv.jctech888.com.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xx.chemitech.net.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://bt.haigaiapp.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ag.bjjhwx.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wg.szxytkj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ye.huanxung.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nc.jianghongdianzi.cn

Ruby: s.capitalize
来源：http://ve.newstarts.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://sm.huixinmuqiang.cn

[E18] 模板占位符替换
来源：http://fo.lnxyls.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ig.yuntaijiaju.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://oe.gzmigu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://yf.chemitech.net.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://cs.521024.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gv.bookmarksfly.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fe.shxzukj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bq.newstarts.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://oa.hahajie.cn

[E19] 多行文本按行拆分
来源：http://pz.asd995.cn

Py:   s.splitlines()
来源：http://fr.asd995.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://br.521024.cn

JS:   s.split(/\r?\n/)
来源：http://vf.nszjky.cn

TS:   s.split(/\r?\n/)
来源：http://bd.bjjhwx.cn

Java: s.lines().toList()
来源：http://fk.shxzskj.cn

Go:   strings.Split(s, "\n")
来源：http://sy.asd995.cn

Ruby: s.lines
来源：http://dm.shxzukj.cn

C#:   s.Split('\n')
来源：http://tq.huixiangedu.cn

[E20] 判断字符串是否为空
来源：http://vd.bookmarksfly.cn

Py:   if not s:
来源：http://qn.bookmarksfly.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sp.hahajie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://za.colortex.cn

TS:   if (s === "") {}
来源：http://sb.asd995.cn

Java: if (s.isEmpty()) {}
来源：http://id.nicolike.cn

Go:   if s == "" {}
来源：http://rs.wgjwhj.cn

Ruby: if s.empty?
来源：http://hb.gzmigu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ih.haigaiapp.cn

[E21] 超长截断加省略号
来源：http://gj.yuexingan06.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://oz.521024.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fy.yuntaijiaju.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gt.shxzskj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zf.haigaiapp.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cz.szsharing.cn

Go:   // 按 rune 判断长度后截断
来源：http://zu.huixiangedu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ry.nicolike.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fk.gzmigu.cn

[E22] 字节长度与字符长度
来源：http://fz.szsharing.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://eh.9csxet.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hc.yuntaijiaju.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xc.panjiajie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ya.hnjuh.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pj.9csxet.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rj.nicolike.cn

Ruby: s.bytesize;  s.length
来源：http://wj.yuntaijiaju.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://to.szsharing.cn

================================================================================
来源：http://zi.huanxung.cn

F. 文件与目录
来源：http://gv.jianghongdianzi.cn

================================================================================
来源：http://ha.jianghongdianzi.cn

[F01] 读取整个文件
来源：http://ir.9csxet.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tl.shtwfgs.cn

PHP:  file_get_contents("a.txt");
来源：http://dm.gzmigu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lk.yuexingan06.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pt.bookmarksfly.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://lf.newstarts.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sy.haigaiapp.cn

Ruby: File.read("a.txt")
来源：http://fg.huanxung.cn

C#:   File.ReadAllText("a.txt");
来源：http://nj.szsharing.cn

[F02] 逐行读取文件
来源：http://lr.nicolike.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hl.jctech888.com.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vf.yuntaijiaju.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oc.panjiajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pd.jianghongdianzi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bb.shxzukj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ha.hahajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ur.yuexingan06.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wt.szsharing.cn

[F03] 写入文件（覆盖）
来源：http://vr.bookmarksfly.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://na.lnxyls.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://pm.huanxung.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rf.newstarts.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cb.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ey.9csxet.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nx.colortex.cn

Ruby: File.write("a.txt", "hi")
来源：http://bq.yuexingan06.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gj.newstarts.cn

[F04] 追加写入文件
来源：http://jb.szxytkj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zf.nicolike.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kv.shtwfgs.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ny.szxytkj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ef.nicolike.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ka.nszjky.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yc.gzmigu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ea.gzmigu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kq.huixiangedu.cn


<!-- 参考信息 -->