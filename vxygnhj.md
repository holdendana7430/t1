代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://ra.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ip.shxzskj.cn

Go:   // 手写 map[string][]T
来源：http://hb.colortex.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://al.haigaiapp.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ii.haigaiapp.cn

[D20] 统计每个元素出现次数
来源：http://jg.huanxung.cn

Py:   Counter(arr)
来源：http://rv.huixiangedu.cn

PHP:  array_count_values($arr);
来源：http://ng.jianghongdianzi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rk.huixiangedu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mr.muxihuayi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lu.szsharing.cn

Go:   // 手写 map[T]int
来源：http://bb.chemitech.net.cn

Ruby: arr.tally
来源：http://tr.szxytkj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jc.shxzskj.cn

[D21] 判断是否包含某元素
来源：http://bq.chemitech.net.cn

Py:   x in arr
来源：http://fd.hnjuh.cn

PHP:  in_array($x, $arr, true);
来源：http://yv.bjjhwx.cn

JS:   arr.includes(x)
来源：http://nt.muxihuayi.cn

TS:   arr.includes(x)
来源：http://sn.newstarts.cn

Java: list.contains(x)
来源：http://so.asd995.cn

Go:   slices.Contains(arr, x)
来源：http://eu.shxzskj.cn

Ruby: arr.include?(x)
来源：http://oq.bookmarksfly.cn

C#:   list.Contains(x)
来源：http://ik.9csxet.cn

[D22] 复制数组（避免共享引用）
来源：http://fw.newstarts.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fe.asd995.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cl.szxytkj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lp.colortex.cn

TS:   [...arr];
来源：http://qq.bookmarksfly.cn

Java: new ArrayList<>(list);
来源：http://uk.gzmigu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ee.shtwfgs.cn

Ruby: arr.dup;  arr.clone
来源：http://le.jctech888.com.cn

C#:   new List<int>(list);
来源：http://zg.huixiangedu.cn

[D23] reduce 累积计算
来源：http://fl.wgjwhj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vn.huixiangedu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ca.szsharing.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cy.huixinmuqiang.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zg.gzmigu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ru.9csxet.cn

Go:   // 手写循环
来源：http://fc.hahajie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tc.shtwfgs.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xo.colortex.cn

[D24] 字典 / Map 基本操作
来源：http://iw.huanxung.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hg.panjiajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://so.9csxet.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://sg.gzmigu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://da.nszjky.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ma.szxytkj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lp.wgjwhj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://te.9csxet.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nh.huixinmuqiang.cn

[D25] Set 集合去重与交并差
来源：http://kq.huanxung.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gz.gzmigu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jy.jctech888.com.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ad.jctech888.com.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://us.chemitech.net.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hd.hahajie.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lj.colortex.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://go.shxzukj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kh.bookmarksfly.cn

[D26] 数组转字符串
来源：http://oz.newstarts.cn

Py:   ", ".join(map(str, arr))
来源：http://tr.9csxet.cn

PHP:  implode(", ", $arr);
来源：http://ri.huixiangedu.cn

JS:   arr.join(", ")
来源：http://zz.hahajie.cn

TS:   arr.join(", ")
来源：http://ba.521024.cn

Java: String.join(", ", list)
来源：http://sk.newstarts.cn

Go:   strings.Join(strs, ", ")
来源：http://op.muxihuayi.cn

Ruby: arr.join(", ")
来源：http://ig.huixinmuqiang.cn

C#:   string.Join(", ", list)
来源：http://dc.hahajie.cn

================================================================================
来源：http://vz.yuexingan06.cn

E. 字符串处理
来源：http://vr.huixinmuqiang.cn

================================================================================
来源：http://eg.panjiajie.cn

[E01] 拼接字符串
来源：http://yv.lnxyls.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xi.asd995.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zt.bjjhwx.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ns.wgjwhj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://df.colortex.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fb.shxzukj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wv.gzmigu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bo.jianghongdianzi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fz.521024.cn

[E02] 重复字符串
来源：http://tt.9csxet.cn

Py:   "ab" * 3
来源：http://up.nicolike.cn

PHP:  str_repeat("ab", 3);
来源：http://xf.hahajie.cn

JS:   "ab".repeat(3)
来源：http://rx.newstarts.cn

TS:   "ab".repeat(3)
来源：http://qv.panjiajie.cn

Java: "ab".repeat(3)
来源：http://ft.szxytkj.cn

Go:   strings.Repeat("ab", 3)
来源：http://gz.shxzskj.cn

Ruby: "ab" * 3
来源：http://sk.bjjhwx.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lx.szxytkj.cn

[E03] 截取子串
来源：http://wi.shxzskj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ql.hahajie.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nj.9csxet.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wu.wgjwhj.cn

TS:   s.slice(1, 4)
来源：http://ci.shxzskj.cn

Java: s.substring(1, 4)
来源：http://ap.huixiangedu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://az.haigaiapp.cn

Ruby: s[1, 3];  s[1..3]
来源：http://fx.szxytkj.cn

C#:   s.Substring(1, 3)
来源：http://gs.wgjwhj.cn

[E04] 查找子串位置
来源：http://is.colortex.cn

Py:   s.find("x");  s.index("x")
来源：http://nk.haigaiapp.cn

PHP:  strpos($s, "x");
来源：http://ke.shtwfgs.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xr.gzmigu.cn

TS:   s.indexOf("x")
来源：http://et.lnxyls.cn

Java: s.indexOf("x")
来源：http://ej.nicolike.cn

Go:   strings.Index(s, "x")
来源：http://dr.521024.cn

Ruby: s.index("x")
来源：http://cw.521024.cn

C#:   s.IndexOf("x")
来源：http://wb.bookmarksfly.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://mx.yuntaijiaju.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bo.yuntaijiaju.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://my.huixinmuqiang.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lq.shxzukj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xe.nszjky.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lr.521024.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rz.huanxung.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://oy.nicolike.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pd.hahajie.cn

[E06] 替换子串
来源：http://td.shtwfgs.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pr.bookmarksfly.cn

PHP:  str_replace("a", "b", $s);
来源：http://zw.shxzukj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ye.nicolike.cn

TS:   s.replaceAll("a", "b")
来源：http://sr.wgjwhj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dl.asd995.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ke.huanxung.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lk.shxzukj.cn

C#:   s.Replace("a", "b")
来源：http://hc.521024.cn

[E07] 按分隔符拆分
来源：http://at.jianghongdianzi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kt.bookmarksfly.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bo.haigaiapp.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ku.shxzskj.cn

TS:   s.split(",")
来源：http://fa.shxzskj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://pq.9csxet.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pk.huanxung.cn

Ruby: s.split(",");  s.split
来源：http://bt.hahajie.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xu.szsharing.cn

[E08] 数组按分隔符合并
来源：http://ko.hahajie.cn

Py:   ",".join(items)
来源：http://ec.colortex.cn

PHP:  implode(",", $items);
来源：http://wh.shtwfgs.cn

JS:   items.join(",")
来源：http://of.szxytkj.cn

TS:   items.join(",")
来源：http://kl.shxzskj.cn

Java: String.join(",", items)
来源：http://gf.huanxung.cn

Go:   strings.Join(items, ",")
来源：http://ox.hnjuh.cn

Ruby: items.join(",")
来源：http://cg.jctech888.com.cn

C#:   string.Join(",", items)
来源：http://ik.gzmigu.cn

[E09] 去除所有空白字符
来源：http://yu.jianghongdianzi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xv.asd995.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bf.huanxung.cn

JS:   s.replace(/\s+/g, "")
来源：http://cg.huixiangedu.cn

TS:   s.replace(/\s+/g, "")
来源：http://sd.shxzskj.cn

Java: s.replaceAll("\\s+", "")
来源：http://dl.panjiajie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://sq.jianghongdianzi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xd.521024.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rv.muxihuayi.cn

[E10] 左侧补零 / 定长填充
来源：http://sp.szsharing.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cm.yuexingan06.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mk.lnxyls.cn

JS:   "7".padStart(3, "0")
来源：http://vf.521024.cn

TS:   "7".padStart(3, "0")
来源：http://ka.panjiajie.cn

Java: String.format("%03d", 7)
来源：http://tu.wgjwhj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://gd.bookmarksfly.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ts.wgjwhj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rj.szxytkj.cn

[E11] 反转字符串
来源：http://ry.huixinmuqiang.cn

Py:   s[::-1]
来源：http://jx.hahajie.cn

PHP:  strrev($s);
来源：http://ru.jianghongdianzi.cn

JS:   [...s].reverse().join("")
来源：http://ad.nicolike.cn

TS:   [...s].reverse().join("")
来源：http://gy.nicolike.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ic.haigaiapp.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://td.jctech888.com.cn

Ruby: s.reverse
来源：http://zi.yuexingan06.cn

C#:   new string(s.Reverse().ToArray())
来源：http://dv.szxytkj.cn

[E12] 统计某字符出现次数
来源：http://lt.gzmigu.cn

Py:   s.count("a")
来源：http://hq.shxzukj.cn

PHP:  substr_count($s, "a");
来源：http://vg.shxzukj.cn

JS:   s.split("a").length - 1
来源：http://lq.asd995.cn

TS:   s.split("a").length - 1
来源：http://fu.gzmigu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ju.hnjuh.cn

Go:   strings.Count(s, "a")
来源：http://lj.nicolike.cn

Ruby: s.count("a")
来源：http://mv.nicolike.cn

C#:   s.Count(c => c == 'a')
来源：http://hd.lnxyls.cn

[E13] 逐字符遍历
来源：http://hc.yuntaijiaju.cn

Py:   for ch in s: print(ch)
来源：http://ve.nszjky.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ql.yuntaijiaju.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ty.gzmigu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://jh.huanxung.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sb.lnxyls.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ep.hahajie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://co.hnjuh.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qk.newstarts.cn

[E14] URL 编码与 Base64
来源：http://zk.jianghongdianzi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lz.jianghongdianzi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://re.shtwfgs.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cu.wgjwhj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xz.jianghongdianzi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://sb.huixinmuqiang.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pz.bookmarksfly.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kj.huixinmuqiang.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://op.asd995.cn

[E15] HTML 转义 / 反转义
来源：http://av.colortex.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ak.shxzukj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jr.chemitech.net.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rf.asd995.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://jj.jianghongdianzi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zt.wgjwhj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xe.huixiangedu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nk.wgjwhj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yt.jctech888.com.cn

[E16] 数字千分位
来源：http://pl.nszjky.cn

Py:   f"{1234567:,}"
来源：http://ja.huixinmuqiang.cn

PHP:  number_format(1234567);
来源：http://wh.shtwfgs.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ca.chemitech.net.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://kh.bjjhwx.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gp.lnxyls.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pq.bookmarksfly.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://uk.haigaiapp.cn

C#:   1234567.ToString("N0")
来源：http://hd.yuntaijiaju.cn

[E17] 首字母大写
来源：http://yb.panjiajie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sc.szxytkj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://tj.szxytkj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://br.hnjuh.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tp.muxihuayi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qu.yuexingan06.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dt.huanxung.cn

Ruby: s.capitalize
来源：http://vy.asd995.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ng.lnxyls.cn

[E18] 模板占位符替换
来源：http://sw.wgjwhj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ew.shxzukj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://op.chemitech.net.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://aq.jianghongdianzi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://pl.yuntaijiaju.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zs.jianghongdianzi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://le.bookmarksfly.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://at.shtwfgs.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://db.asd995.cn

[E19] 多行文本按行拆分
来源：http://jr.521024.cn

Py:   s.splitlines()
来源：http://kg.jctech888.com.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fr.nszjky.cn

JS:   s.split(/\r?\n/)
来源：http://bl.nszjky.cn

TS:   s.split(/\r?\n/)
来源：http://ss.huixiangedu.cn

Java: s.lines().toList()
来源：http://kt.asd995.cn

Go:   strings.Split(s, "\n")
来源：http://xu.yuntaijiaju.cn

Ruby: s.lines
来源：http://gw.panjiajie.cn

C#:   s.Split('\n')
来源：http://oz.panjiajie.cn

[E20] 判断字符串是否为空
来源：http://ud.colortex.cn

Py:   if not s:
来源：http://yg.bjjhwx.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zg.huanxung.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ow.szxytkj.cn

TS:   if (s === "") {}
来源：http://wq.haigaiapp.cn

Java: if (s.isEmpty()) {}
来源：http://du.muxihuayi.cn

Go:   if s == "" {}
来源：http://db.shxzukj.cn

Ruby: if s.empty?
来源：http://qy.huanxung.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cj.shxzukj.cn

[E21] 超长截断加省略号
来源：http://gr.yuexingan06.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xc.huixiangedu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rk.huanxung.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yk.muxihuayi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vt.shxzukj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ho.panjiajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://ba.szsharing.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ma.nicolike.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dy.shxzskj.cn

[E22] 字节长度与字符长度
来源：http://hd.yuexingan06.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ca.nicolike.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ai.shxzukj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mm.hahajie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ux.bjjhwx.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://al.newstarts.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lg.gzmigu.cn

Ruby: s.bytesize;  s.length
来源：http://mr.shxzskj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ma.newstarts.cn

================================================================================
来源：http://pl.nicolike.cn

F. 文件与目录
来源：http://uj.huanxung.cn

================================================================================
来源：http://tu.panjiajie.cn

[F01] 读取整个文件
来源：http://gv.hnjuh.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fz.shxzukj.cn

PHP:  file_get_contents("a.txt");
来源：http://xl.gzmigu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sq.jianghongdianzi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ss.gzmigu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://re.panjiajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wf.huixiangedu.cn

Ruby: File.read("a.txt")
来源：http://pg.hnjuh.cn

C#:   File.ReadAllText("a.txt");
来源：http://kk.gzmigu.cn

[F02] 逐行读取文件
来源：http://cv.shtwfgs.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nm.muxihuayi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://iv.colortex.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ie.shxzskj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ij.hnjuh.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ng.chemitech.net.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kv.huixinmuqiang.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pk.hahajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kf.yuexingan06.cn

[F03] 写入文件（覆盖）
来源：http://sa.jianghongdianzi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ux.huixiangedu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://bb.hahajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bg.shtwfgs.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vj.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yq.jctech888.com.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://eh.szxytkj.cn

Ruby: File.write("a.txt", "hi")
来源：http://sf.hahajie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ij.bookmarksfly.cn

[F04] 追加写入文件
来源：http://dh.shxzskj.cn


<!-- 参考信息 -->