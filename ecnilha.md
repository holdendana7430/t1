代发 wailian999

[D19] 按字段分组
来源：http://lm.lnxyls.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qp.9csxet.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ge.nszjky.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xd.hahajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://rp.gzmigu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hs.chemitech.net.cn

Go:   // 手写 map[string][]T
来源：http://zz.huixiangedu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ph.hnjuh.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wj.hahajie.cn

[D20] 统计每个元素出现次数
来源：http://fm.yuntaijiaju.cn

Py:   Counter(arr)
来源：http://zd.huixiangedu.cn

PHP:  array_count_values($arr);
来源：http://md.hnjuh.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mk.colortex.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ui.521024.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://oo.muxihuayi.cn

Go:   // 手写 map[T]int
来源：http://po.yuexingan06.cn

Ruby: arr.tally
来源：http://gv.shxzskj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qm.nszjky.cn

[D21] 判断是否包含某元素
来源：http://eb.521024.cn

Py:   x in arr
来源：http://sz.521024.cn

PHP:  in_array($x, $arr, true);
来源：http://sp.muxihuayi.cn

JS:   arr.includes(x)
来源：http://xj.shxzukj.cn

TS:   arr.includes(x)
来源：http://bj.nszjky.cn

Java: list.contains(x)
来源：http://xc.shxzskj.cn

Go:   slices.Contains(arr, x)
来源：http://zd.panjiajie.cn

Ruby: arr.include?(x)
来源：http://zi.nszjky.cn

C#:   list.Contains(x)
来源：http://on.lnxyls.cn

[D22] 复制数组（避免共享引用）
来源：http://lx.jctech888.com.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yp.shxzskj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kx.nicolike.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gv.hahajie.cn

TS:   [...arr];
来源：http://ua.szxytkj.cn

Java: new ArrayList<>(list);
来源：http://xj.nszjky.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qz.lnxyls.cn

Ruby: arr.dup;  arr.clone
来源：http://pt.yuexingan06.cn

C#:   new List<int>(list);
来源：http://sg.hnjuh.cn

[D23] reduce 累积计算
来源：http://wz.yuexingan06.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rt.chemitech.net.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://br.bjjhwx.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ve.lnxyls.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yo.jctech888.com.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://wr.lnxyls.cn

Go:   // 手写循环
来源：http://mw.colortex.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cp.521024.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lb.hnjuh.cn

[D24] 字典 / Map 基本操作
来源：http://jn.hahajie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mp.gzmigu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xt.nszjky.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://uu.gzmigu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ic.chemitech.net.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hc.nszjky.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vc.lnxyls.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://oo.gzmigu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rq.huixinmuqiang.cn

[D25] Set 集合去重与交并差
来源：http://ht.gzmigu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xp.chemitech.net.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vv.9csxet.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://co.shtwfgs.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jl.yuntaijiaju.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qh.colortex.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://id.chemitech.net.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nx.lnxyls.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://oz.huixiangedu.cn

[D26] 数组转字符串
来源：http://ov.521024.cn

Py:   ", ".join(map(str, arr))
来源：http://mh.9csxet.cn

PHP:  implode(", ", $arr);
来源：http://yd.9csxet.cn

JS:   arr.join(", ")
来源：http://fh.shxzukj.cn

TS:   arr.join(", ")
来源：http://ec.bookmarksfly.cn

Java: String.join(", ", list)
来源：http://sf.jianghongdianzi.cn

Go:   strings.Join(strs, ", ")
来源：http://qd.colortex.cn

Ruby: arr.join(", ")
来源：http://kf.gzmigu.cn

C#:   string.Join(", ", list)
来源：http://hd.nicolike.cn

================================================================================
来源：http://sk.panjiajie.cn

E. 字符串处理
来源：http://yt.shxzukj.cn

================================================================================
来源：http://wz.yuexingan06.cn

[E01] 拼接字符串
来源：http://ds.huixinmuqiang.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yl.yuntaijiaju.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://da.huanxung.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bv.nicolike.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://op.nszjky.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ag.gzmigu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ev.shxzskj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ao.huixinmuqiang.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qa.huixiangedu.cn

[E02] 重复字符串
来源：http://xd.szsharing.cn

Py:   "ab" * 3
来源：http://mr.shtwfgs.cn

PHP:  str_repeat("ab", 3);
来源：http://au.wgjwhj.cn

JS:   "ab".repeat(3)
来源：http://oc.szxytkj.cn

TS:   "ab".repeat(3)
来源：http://fk.huixinmuqiang.cn

Java: "ab".repeat(3)
来源：http://ny.9csxet.cn

Go:   strings.Repeat("ab", 3)
来源：http://px.huixiangedu.cn

Ruby: "ab" * 3
来源：http://ev.huixiangedu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fy.9csxet.cn

[E03] 截取子串
来源：http://uf.lnxyls.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gw.gzmigu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gl.huanxung.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ga.nicolike.cn

TS:   s.slice(1, 4)
来源：http://eb.gzmigu.cn

Java: s.substring(1, 4)
来源：http://hr.9csxet.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zz.szsharing.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ry.shtwfgs.cn

C#:   s.Substring(1, 3)
来源：http://jb.haigaiapp.cn

[E04] 查找子串位置
来源：http://qn.hnjuh.cn

Py:   s.find("x");  s.index("x")
来源：http://ao.huanxung.cn

PHP:  strpos($s, "x");
来源：http://rj.huixiangedu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pb.huixiangedu.cn

TS:   s.indexOf("x")
来源：http://nw.shxzukj.cn

Java: s.indexOf("x")
来源：http://sl.panjiajie.cn

Go:   strings.Index(s, "x")
来源：http://wh.huixiangedu.cn

Ruby: s.index("x")
来源：http://oa.bjjhwx.cn

C#:   s.IndexOf("x")
来源：http://ks.huixiangedu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gq.gzmigu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jj.szxytkj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xz.asd995.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ng.huanxung.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://nu.newstarts.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://af.muxihuayi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dz.gzmigu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zl.shxzskj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xq.nicolike.cn

[E06] 替换子串
来源：http://qv.yuntaijiaju.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zm.bjjhwx.cn

PHP:  str_replace("a", "b", $s);
来源：http://vf.chemitech.net.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ro.nszjky.cn

TS:   s.replaceAll("a", "b")
来源：http://kt.huanxung.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jp.hnjuh.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ie.huixiangedu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xf.yuntaijiaju.cn

C#:   s.Replace("a", "b")
来源：http://as.gzmigu.cn

[E07] 按分隔符拆分
来源：http://ho.haigaiapp.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pv.shtwfgs.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://of.gzmigu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://qk.shtwfgs.cn

TS:   s.split(",")
来源：http://pz.hahajie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://pp.colortex.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fz.huixiangedu.cn

Ruby: s.split(",");  s.split
来源：http://yc.panjiajie.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vl.muxihuayi.cn

[E08] 数组按分隔符合并
来源：http://uc.9csxet.cn

Py:   ",".join(items)
来源：http://rv.szxytkj.cn

PHP:  implode(",", $items);
来源：http://da.hnjuh.cn

JS:   items.join(",")
来源：http://tw.shxzukj.cn

TS:   items.join(",")
来源：http://ir.jctech888.com.cn

Java: String.join(",", items)
来源：http://jb.nicolike.cn

Go:   strings.Join(items, ",")
来源：http://ea.jctech888.com.cn

Ruby: items.join(",")
来源：http://vh.shxzskj.cn

C#:   string.Join(",", items)
来源：http://ve.shtwfgs.cn

[E09] 去除所有空白字符
来源：http://zo.szsharing.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hw.yuexingan06.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zp.hahajie.cn

JS:   s.replace(/\s+/g, "")
来源：http://jn.shxzukj.cn

TS:   s.replace(/\s+/g, "")
来源：http://fw.shxzukj.cn

Java: s.replaceAll("\\s+", "")
来源：http://tk.muxihuayi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://la.hnjuh.cn

Ruby: s.gsub(/\s+/, "")
来源：http://tj.szsharing.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vy.hnjuh.cn

[E10] 左侧补零 / 定长填充
来源：http://qe.huixiangedu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hy.muxihuayi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qv.jctech888.com.cn

JS:   "7".padStart(3, "0")
来源：http://zi.colortex.cn

TS:   "7".padStart(3, "0")
来源：http://kk.huanxung.cn

Java: String.format("%03d", 7)
来源：http://uz.huanxung.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://bf.521024.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ul.huanxung.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qc.nszjky.cn

[E11] 反转字符串
来源：http://vy.gzmigu.cn

Py:   s[::-1]
来源：http://ns.wgjwhj.cn

PHP:  strrev($s);
来源：http://sa.huanxung.cn

JS:   [...s].reverse().join("")
来源：http://qz.hnjuh.cn

TS:   [...s].reverse().join("")
来源：http://js.wgjwhj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://hy.shtwfgs.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://fu.nszjky.cn

Ruby: s.reverse
来源：http://ai.yuexingan06.cn

C#:   new string(s.Reverse().ToArray())
来源：http://os.bookmarksfly.cn

[E12] 统计某字符出现次数
来源：http://qm.yuntaijiaju.cn

Py:   s.count("a")
来源：http://tn.shxzukj.cn

PHP:  substr_count($s, "a");
来源：http://xl.nicolike.cn

JS:   s.split("a").length - 1
来源：http://xk.shxzskj.cn

TS:   s.split("a").length - 1
来源：http://da.asd995.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ck.chemitech.net.cn

Go:   strings.Count(s, "a")
来源：http://tz.huanxung.cn

Ruby: s.count("a")
来源：http://gw.bookmarksfly.cn

C#:   s.Count(c => c == 'a')
来源：http://kp.colortex.cn

[E13] 逐字符遍历
来源：http://yx.szsharing.cn

Py:   for ch in s: print(ch)
来源：http://en.jianghongdianzi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qv.newstarts.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://bw.huixiangedu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://hd.szxytkj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://eg.shxzukj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ni.hnjuh.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://px.huixinmuqiang.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pn.shtwfgs.cn

[E14] URL 编码与 Base64
来源：http://jr.asd995.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zy.521024.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://xk.bjjhwx.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://em.bookmarksfly.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qu.shtwfgs.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dv.colortex.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fj.yuntaijiaju.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://no.lnxyls.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xr.asd995.cn

[E15] HTML 转义 / 反转义
来源：http://ht.hahajie.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://yb.hahajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yp.huixiangedu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jr.huixinmuqiang.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://nz.gzmigu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rd.szxytkj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xa.9csxet.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yf.colortex.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jd.chemitech.net.cn

[E16] 数字千分位
来源：http://yr.hahajie.cn

Py:   f"{1234567:,}"
来源：http://qo.colortex.cn

PHP:  number_format(1234567);
来源：http://kh.asd995.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://fe.wgjwhj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://mr.szxytkj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pu.shxzukj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://td.bjjhwx.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pc.szsharing.cn

C#:   1234567.ToString("N0")
来源：http://vv.asd995.cn

[E17] 首字母大写
来源：http://rv.asd995.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qv.shxzskj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://nk.szxytkj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ew.shtwfgs.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ax.jctech888.com.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jb.jctech888.com.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dc.bookmarksfly.cn

Ruby: s.capitalize
来源：http://pz.shtwfgs.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gh.hahajie.cn

[E18] 模板占位符替换
来源：http://zr.jianghongdianzi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tj.newstarts.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xg.shtwfgs.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xu.shxzskj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://xq.huixiangedu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ht.jianghongdianzi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ky.muxihuayi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://at.muxihuayi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xe.bjjhwx.cn

[E19] 多行文本按行拆分
来源：http://hg.huixinmuqiang.cn

Py:   s.splitlines()
来源：http://ll.lnxyls.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ga.wgjwhj.cn

JS:   s.split(/\r?\n/)
来源：http://gw.jctech888.com.cn

TS:   s.split(/\r?\n/)
来源：http://fe.gzmigu.cn

Java: s.lines().toList()
来源：http://iw.szxytkj.cn

Go:   strings.Split(s, "\n")
来源：http://pp.newstarts.cn

Ruby: s.lines
来源：http://er.jctech888.com.cn

C#:   s.Split('\n')
来源：http://dx.jctech888.com.cn

[E20] 判断字符串是否为空
来源：http://gr.nszjky.cn

Py:   if not s:
来源：http://lm.shxzskj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://no.shxzskj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ul.nicolike.cn

TS:   if (s === "") {}
来源：http://hn.shxzukj.cn

Java: if (s.isEmpty()) {}
来源：http://lu.shtwfgs.cn

Go:   if s == "" {}
来源：http://ot.haigaiapp.cn

Ruby: if s.empty?
来源：http://vl.jianghongdianzi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zq.chemitech.net.cn

[E21] 超长截断加省略号
来源：http://ms.chemitech.net.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rd.huixiangedu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mz.yuntaijiaju.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yu.huixinmuqiang.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uo.gzmigu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ya.huanxung.cn

Go:   // 按 rune 判断长度后截断
来源：http://fi.shtwfgs.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://et.szsharing.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nk.newstarts.cn

[E22] 字节长度与字符长度
来源：http://mr.nszjky.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://up.panjiajie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ll.jianghongdianzi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cd.lnxyls.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jt.hahajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://de.asd995.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zh.szxytkj.cn

Ruby: s.bytesize;  s.length
来源：http://xi.bookmarksfly.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rh.lnxyls.cn

================================================================================
来源：http://ho.newstarts.cn

F. 文件与目录
来源：http://qy.521024.cn

================================================================================
来源：http://ow.szsharing.cn

[F01] 读取整个文件
来源：http://kc.yuexingan06.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xe.nszjky.cn

PHP:  file_get_contents("a.txt");
来源：http://js.szsharing.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ac.panjiajie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nh.gzmigu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zz.huanxung.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zn.jianghongdianzi.cn

Ruby: File.read("a.txt")
来源：http://bp.huixiangedu.cn

C#:   File.ReadAllText("a.txt");
来源：http://ru.yuntaijiaju.cn

[F02] 逐行读取文件
来源：http://qk.bjjhwx.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ii.huanxung.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ov.shtwfgs.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://af.szsharing.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lh.hnjuh.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qp.hnjuh.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://sb.jctech888.com.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://el.shtwfgs.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ce.bjjhwx.cn

[F03] 写入文件（覆盖）
来源：http://ng.panjiajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cb.shxzskj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ka.shxzukj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mj.newstarts.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://om.huanxung.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rj.jctech888.com.cn


<!-- 参考信息 -->