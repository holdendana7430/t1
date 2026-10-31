代发 wailian999

[D19] 按字段分组
来源：http://au.hahajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yg.asd995.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wv.muxihuayi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yc.yuexingan06.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qh.shxzskj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kr.newstarts.cn

Go:   // 手写 map[string][]T
来源：http://sm.huixiangedu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://my.hahajie.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gi.gzmigu.cn

[D20] 统计每个元素出现次数
来源：http://vv.shtwfgs.cn

Py:   Counter(arr)
来源：http://mx.shxzukj.cn

PHP:  array_count_values($arr);
来源：http://il.hnjuh.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://me.newstarts.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bs.shxzskj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ky.hahajie.cn

Go:   // 手写 map[T]int
来源：http://xw.huixiangedu.cn

Ruby: arr.tally
来源：http://cf.jctech888.com.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zj.asd995.cn

[D21] 判断是否包含某元素
来源：http://na.jctech888.com.cn

Py:   x in arr
来源：http://zm.521024.cn

PHP:  in_array($x, $arr, true);
来源：http://ov.huanxung.cn

JS:   arr.includes(x)
来源：http://hd.nicolike.cn

TS:   arr.includes(x)
来源：http://po.wgjwhj.cn

Java: list.contains(x)
来源：http://dw.yuntaijiaju.cn

Go:   slices.Contains(arr, x)
来源：http://tk.shtwfgs.cn

Ruby: arr.include?(x)
来源：http://jd.shxzskj.cn

C#:   list.Contains(x)
来源：http://ki.yuexingan06.cn

[D22] 复制数组（避免共享引用）
来源：http://kn.521024.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cu.521024.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ln.asd995.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gn.bjjhwx.cn

TS:   [...arr];
来源：http://jw.wgjwhj.cn

Java: new ArrayList<>(list);
来源：http://kc.gzmigu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://yc.huixiangedu.cn

Ruby: arr.dup;  arr.clone
来源：http://kq.huixiangedu.cn

C#:   new List<int>(list);
来源：http://go.panjiajie.cn

[D23] reduce 累积计算
来源：http://qn.huixiangedu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jc.szsharing.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://oz.shtwfgs.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zn.haigaiapp.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ws.chemitech.net.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ze.huanxung.cn

Go:   // 手写循环
来源：http://yk.bjjhwx.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://io.wgjwhj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://uf.yuntaijiaju.cn

[D24] 字典 / Map 基本操作
来源：http://xb.hnjuh.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rc.nicolike.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yk.lnxyls.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://eu.asd995.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xa.szsharing.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ja.gzmigu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://by.jianghongdianzi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mg.haigaiapp.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://le.chemitech.net.cn

[D25] Set 集合去重与交并差
来源：http://nc.wgjwhj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jk.huixiangedu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mo.9csxet.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bn.huixiangedu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ti.huixinmuqiang.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qf.shxzukj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://yx.szsharing.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wn.gzmigu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://sf.colortex.cn

[D26] 数组转字符串
来源：http://fi.huixiangedu.cn

Py:   ", ".join(map(str, arr))
来源：http://os.bookmarksfly.cn

PHP:  implode(", ", $arr);
来源：http://lg.jctech888.com.cn

JS:   arr.join(", ")
来源：http://gf.colortex.cn

TS:   arr.join(", ")
来源：http://co.521024.cn

Java: String.join(", ", list)
来源：http://xs.hahajie.cn

Go:   strings.Join(strs, ", ")
来源：http://wr.yuntaijiaju.cn

Ruby: arr.join(", ")
来源：http://tk.bookmarksfly.cn

C#:   string.Join(", ", list)
来源：http://gm.huanxung.cn

================================================================================
来源：http://ve.shxzukj.cn

E. 字符串处理
来源：http://cy.nicolike.cn

================================================================================
来源：http://ix.hahajie.cn

[E01] 拼接字符串
来源：http://dm.colortex.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rp.chemitech.net.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pw.haigaiapp.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ix.hnjuh.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ev.muxihuayi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://om.wgjwhj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://or.shxzskj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tn.hnjuh.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hf.szsharing.cn

[E02] 重复字符串
来源：http://eb.panjiajie.cn

Py:   "ab" * 3
来源：http://ly.jctech888.com.cn

PHP:  str_repeat("ab", 3);
来源：http://cc.newstarts.cn

JS:   "ab".repeat(3)
来源：http://dn.newstarts.cn

TS:   "ab".repeat(3)
来源：http://ez.bookmarksfly.cn

Java: "ab".repeat(3)
来源：http://nj.szxytkj.cn

Go:   strings.Repeat("ab", 3)
来源：http://ct.wgjwhj.cn

Ruby: "ab" * 3
来源：http://du.gzmigu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zx.newstarts.cn

[E03] 截取子串
来源：http://su.huixiangedu.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://oy.hahajie.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xj.panjiajie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gs.hahajie.cn

TS:   s.slice(1, 4)
来源：http://bo.muxihuayi.cn

Java: s.substring(1, 4)
来源：http://ss.asd995.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mh.szxytkj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://so.muxihuayi.cn

C#:   s.Substring(1, 3)
来源：http://yt.wgjwhj.cn

[E04] 查找子串位置
来源：http://bm.hahajie.cn

Py:   s.find("x");  s.index("x")
来源：http://xn.9csxet.cn

PHP:  strpos($s, "x");
来源：http://ne.shtwfgs.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qq.colortex.cn

TS:   s.indexOf("x")
来源：http://in.huixinmuqiang.cn

Java: s.indexOf("x")
来源：http://xg.haigaiapp.cn

Go:   strings.Index(s, "x")
来源：http://kz.huanxung.cn

Ruby: s.index("x")
来源：http://vd.panjiajie.cn

C#:   s.IndexOf("x")
来源：http://ht.jianghongdianzi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gy.huixiangedu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://sp.asd995.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://gu.szsharing.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yn.jianghongdianzi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://wt.bjjhwx.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ql.hahajie.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://de.nszjky.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gp.huixiangedu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xv.bookmarksfly.cn

[E06] 替换子串
来源：http://ek.huixiangedu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fi.yuexingan06.cn

PHP:  str_replace("a", "b", $s);
来源：http://ht.muxihuayi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ca.colortex.cn

TS:   s.replaceAll("a", "b")
来源：http://yd.shtwfgs.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rz.nszjky.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://db.hnjuh.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://oh.colortex.cn

C#:   s.Replace("a", "b")
来源：http://qg.lnxyls.cn

[E07] 按分隔符拆分
来源：http://ef.jianghongdianzi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ak.asd995.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rb.hnjuh.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://si.panjiajie.cn

TS:   s.split(",")
来源：http://ze.9csxet.cn

Java: s.split(",");  s.split("\\s+")
来源：http://sy.shxzukj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pl.szsharing.cn

Ruby: s.split(",");  s.split
来源：http://fa.hahajie.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bq.colortex.cn

[E08] 数组按分隔符合并
来源：http://gy.huixinmuqiang.cn

Py:   ",".join(items)
来源：http://tx.newstarts.cn

PHP:  implode(",", $items);
来源：http://ye.shtwfgs.cn

JS:   items.join(",")
来源：http://vv.9csxet.cn

TS:   items.join(",")
来源：http://en.gzmigu.cn

Java: String.join(",", items)
来源：http://sx.521024.cn

Go:   strings.Join(items, ",")
来源：http://jf.hahajie.cn

Ruby: items.join(",")
来源：http://vr.bookmarksfly.cn

C#:   string.Join(",", items)
来源：http://jk.nszjky.cn

[E09] 去除所有空白字符
来源：http://gi.szxytkj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://iv.jianghongdianzi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://do.yuexingan06.cn

JS:   s.replace(/\s+/g, "")
来源：http://pv.szsharing.cn

TS:   s.replace(/\s+/g, "")
来源：http://uv.shxzskj.cn

Java: s.replaceAll("\\s+", "")
来源：http://ih.huanxung.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://iz.hnjuh.cn

Ruby: s.gsub(/\s+/, "")
来源：http://by.yuexingan06.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ij.shtwfgs.cn

[E10] 左侧补零 / 定长填充
来源：http://mw.wgjwhj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mk.521024.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zv.jctech888.com.cn

JS:   "7".padStart(3, "0")
来源：http://uy.jctech888.com.cn

TS:   "7".padStart(3, "0")
来源：http://nv.shxzukj.cn

Java: String.format("%03d", 7)
来源：http://id.newstarts.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://kz.hnjuh.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lu.wgjwhj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://uu.521024.cn

[E11] 反转字符串
来源：http://mm.shxzskj.cn

Py:   s[::-1]
来源：http://ty.asd995.cn

PHP:  strrev($s);
来源：http://gz.huixiangedu.cn

JS:   [...s].reverse().join("")
来源：http://ca.9csxet.cn

TS:   [...s].reverse().join("")
来源：http://qm.huixinmuqiang.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://xw.muxihuayi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://go.muxihuayi.cn

Ruby: s.reverse
来源：http://yc.bjjhwx.cn

C#:   new string(s.Reverse().ToArray())
来源：http://fs.gzmigu.cn

[E12] 统计某字符出现次数
来源：http://so.shtwfgs.cn

Py:   s.count("a")
来源：http://mw.jctech888.com.cn

PHP:  substr_count($s, "a");
来源：http://qa.nszjky.cn

JS:   s.split("a").length - 1
来源：http://ol.9csxet.cn

TS:   s.split("a").length - 1
来源：http://bh.huixiangedu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dl.9csxet.cn

Go:   strings.Count(s, "a")
来源：http://xh.panjiajie.cn

Ruby: s.count("a")
来源：http://nw.shxzskj.cn

C#:   s.Count(c => c == 'a')
来源：http://li.huixinmuqiang.cn

[E13] 逐字符遍历
来源：http://rt.huixinmuqiang.cn

Py:   for ch in s: print(ch)
来源：http://gl.jianghongdianzi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cs.shxzukj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://lg.colortex.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://sd.shxzukj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://up.szxytkj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kg.hnjuh.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ns.huixiangedu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ll.huixiangedu.cn

[E14] URL 编码与 Base64
来源：http://af.jianghongdianzi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xf.panjiajie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://df.jctech888.com.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qu.colortex.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nl.huixiangedu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bw.szsharing.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rx.jianghongdianzi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nw.muxihuayi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zt.hnjuh.cn

[E15] HTML 转义 / 反转义
来源：http://qd.szsharing.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://sz.gzmigu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uv.chemitech.net.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zb.huixinmuqiang.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://kg.hahajie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://co.nszjky.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ey.yuntaijiaju.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ii.nicolike.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bq.wgjwhj.cn

[E16] 数字千分位
来源：http://yu.jianghongdianzi.cn

Py:   f"{1234567:,}"
来源：http://dx.shtwfgs.cn

PHP:  number_format(1234567);
来源：http://gn.shtwfgs.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://cj.shtwfgs.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zp.gzmigu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kp.nszjky.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fv.asd995.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fd.panjiajie.cn

C#:   1234567.ToString("N0")
来源：http://oy.huixiangedu.cn

[E17] 首字母大写
来源：http://nk.hnjuh.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://im.9csxet.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://vs.bookmarksfly.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://or.panjiajie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ub.huixinmuqiang.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://su.muxihuayi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fe.szxytkj.cn

Ruby: s.capitalize
来源：http://ob.huixiangedu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://sv.bjjhwx.cn

[E18] 模板占位符替换
来源：http://so.huixinmuqiang.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jz.bookmarksfly.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ah.yuntaijiaju.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://dn.9csxet.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ro.szsharing.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ob.huixiangedu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bw.haigaiapp.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mm.yuntaijiaju.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://db.haigaiapp.cn

[E19] 多行文本按行拆分
来源：http://ah.yuntaijiaju.cn

Py:   s.splitlines()
来源：http://sc.shxzukj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hv.shtwfgs.cn

JS:   s.split(/\r?\n/)
来源：http://ho.nszjky.cn

TS:   s.split(/\r?\n/)
来源：http://zg.yuexingan06.cn

Java: s.lines().toList()
来源：http://pp.huanxung.cn

Go:   strings.Split(s, "\n")
来源：http://jh.panjiajie.cn

Ruby: s.lines
来源：http://hn.muxihuayi.cn

C#:   s.Split('\n')
来源：http://jd.huanxung.cn

[E20] 判断字符串是否为空
来源：http://kn.lnxyls.cn

Py:   if not s:
来源：http://md.huixinmuqiang.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lz.shxzskj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://uz.hnjuh.cn

TS:   if (s === "") {}
来源：http://zd.szsharing.cn

Java: if (s.isEmpty()) {}
来源：http://ks.huixiangedu.cn

Go:   if s == "" {}
来源：http://yj.gzmigu.cn

Ruby: if s.empty?
来源：http://vx.shxzskj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fs.huanxung.cn

[E21] 超长截断加省略号
来源：http://ng.yuexingan06.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dr.huanxung.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kn.shxzukj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fj.huixinmuqiang.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pn.shxzukj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wn.panjiajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://la.haigaiapp.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nw.asd995.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ey.9csxet.cn

[E22] 字节长度与字符长度
来源：http://sr.521024.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wh.colortex.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nb.bjjhwx.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lp.haigaiapp.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xk.szxytkj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kr.szxytkj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bp.hahajie.cn

Ruby: s.bytesize;  s.length
来源：http://ch.521024.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hi.jctech888.com.cn

================================================================================
来源：http://yc.szxytkj.cn

F. 文件与目录
来源：http://sz.newstarts.cn

================================================================================
来源：http://pq.9csxet.cn

[F01] 读取整个文件
来源：http://oo.nszjky.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mb.newstarts.cn

PHP:  file_get_contents("a.txt");
来源：http://gk.bookmarksfly.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fa.9csxet.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bf.huixinmuqiang.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ov.huixinmuqiang.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tl.jianghongdianzi.cn

Ruby: File.read("a.txt")
来源：http://uv.gzmigu.cn

C#:   File.ReadAllText("a.txt");
来源：http://qv.asd995.cn

[F02] 逐行读取文件
来源：http://xo.huixinmuqiang.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cw.colortex.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ww.jctech888.com.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yf.jianghongdianzi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yr.bookmarksfly.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://en.jctech888.com.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://va.chemitech.net.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://iu.haigaiapp.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kq.jctech888.com.cn

[F03] 写入文件（覆盖）
来源：http://qv.wgjwhj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qv.wgjwhj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ic.yuexingan06.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uy.bookmarksfly.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ex.huixiangedu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tg.huixinmuqiang.cn


<!-- 参考信息 -->