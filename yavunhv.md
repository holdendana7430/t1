代发 wailian999

[D19] 按字段分组
来源：http://ax.chemitech.net.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bx.colortex.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lu.gzmigu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ne.haigaiapp.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://wv.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tt.521024.cn

Go:   // 手写 map[string][]T
来源：http://ad.shxzskj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://db.huixinmuqiang.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mo.shxzukj.cn

[D20] 统计每个元素出现次数
来源：http://yl.shxzskj.cn

Py:   Counter(arr)
来源：http://qp.bookmarksfly.cn

PHP:  array_count_values($arr);
来源：http://qs.szsharing.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tx.huanxung.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wm.shtwfgs.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tc.asd995.cn

Go:   // 手写 map[T]int
来源：http://ma.nicolike.cn

Ruby: arr.tally
来源：http://gc.huixiangedu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://aj.yuexingan06.cn

[D21] 判断是否包含某元素
来源：http://vy.nicolike.cn

Py:   x in arr
来源：http://ca.muxihuayi.cn

PHP:  in_array($x, $arr, true);
来源：http://gm.huanxung.cn

JS:   arr.includes(x)
来源：http://vj.panjiajie.cn

TS:   arr.includes(x)
来源：http://xc.jianghongdianzi.cn

Java: list.contains(x)
来源：http://lp.szsharing.cn

Go:   slices.Contains(arr, x)
来源：http://pt.chemitech.net.cn

Ruby: arr.include?(x)
来源：http://tv.yuexingan06.cn

C#:   list.Contains(x)
来源：http://uo.9csxet.cn

[D22] 复制数组（避免共享引用）
来源：http://kq.wgjwhj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yk.yuexingan06.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fb.nszjky.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ks.yuntaijiaju.cn

TS:   [...arr];
来源：http://ph.wgjwhj.cn

Java: new ArrayList<>(list);
来源：http://vu.muxihuayi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ia.chemitech.net.cn

Ruby: arr.dup;  arr.clone
来源：http://rh.jctech888.com.cn

C#:   new List<int>(list);
来源：http://rh.nicolike.cn

[D23] reduce 累积计算
来源：http://mk.huixinmuqiang.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nl.newstarts.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yu.shxzskj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mf.szxytkj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wh.hnjuh.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xd.nszjky.cn

Go:   // 手写循环
来源：http://ri.hnjuh.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wg.521024.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pg.yuntaijiaju.cn

[D24] 字典 / Map 基本操作
来源：http://kk.shxzukj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vs.bjjhwx.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ie.521024.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mb.bjjhwx.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wx.bjjhwx.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kw.huixinmuqiang.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nd.bjjhwx.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ju.chemitech.net.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nj.gzmigu.cn

[D25] Set 集合去重与交并差
来源：http://th.shxzskj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://td.shxzskj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://np.nicolike.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wc.newstarts.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qu.9csxet.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ga.bookmarksfly.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mt.hnjuh.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yl.colortex.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rn.hahajie.cn

[D26] 数组转字符串
来源：http://rn.colortex.cn

Py:   ", ".join(map(str, arr))
来源：http://qf.szxytkj.cn

PHP:  implode(", ", $arr);
来源：http://hq.jianghongdianzi.cn

JS:   arr.join(", ")
来源：http://oc.panjiajie.cn

TS:   arr.join(", ")
来源：http://qu.jianghongdianzi.cn

Java: String.join(", ", list)
来源：http://vh.wgjwhj.cn

Go:   strings.Join(strs, ", ")
来源：http://ug.chemitech.net.cn

Ruby: arr.join(", ")
来源：http://wm.jctech888.com.cn

C#:   string.Join(", ", list)
来源：http://ff.asd995.cn

================================================================================
来源：http://rs.huixiangedu.cn

E. 字符串处理
来源：http://jp.jianghongdianzi.cn

================================================================================
来源：http://jq.jctech888.com.cn

[E01] 拼接字符串
来源：http://cj.chemitech.net.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dr.asd995.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cb.wgjwhj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wj.shxzukj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qi.panjiajie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://so.wgjwhj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cn.chemitech.net.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yk.jctech888.com.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ic.yuntaijiaju.cn

[E02] 重复字符串
来源：http://dq.shxzukj.cn

Py:   "ab" * 3
来源：http://yt.yuntaijiaju.cn

PHP:  str_repeat("ab", 3);
来源：http://yc.huixinmuqiang.cn

JS:   "ab".repeat(3)
来源：http://fo.nicolike.cn

TS:   "ab".repeat(3)
来源：http://hn.huanxung.cn

Java: "ab".repeat(3)
来源：http://zp.nszjky.cn

Go:   strings.Repeat("ab", 3)
来源：http://hz.yuexingan06.cn

Ruby: "ab" * 3
来源：http://yw.muxihuayi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ni.jctech888.com.cn

[E03] 截取子串
来源：http://ef.wgjwhj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kz.bjjhwx.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vo.shxzskj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://py.asd995.cn

TS:   s.slice(1, 4)
来源：http://pd.yuntaijiaju.cn

Java: s.substring(1, 4)
来源：http://gp.newstarts.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sn.huixiangedu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://oo.yuntaijiaju.cn

C#:   s.Substring(1, 3)
来源：http://nu.nicolike.cn

[E04] 查找子串位置
来源：http://il.asd995.cn

Py:   s.find("x");  s.index("x")
来源：http://gt.haigaiapp.cn

PHP:  strpos($s, "x");
来源：http://nb.muxihuayi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cw.nszjky.cn

TS:   s.indexOf("x")
来源：http://fr.huixinmuqiang.cn

Java: s.indexOf("x")
来源：http://sh.gzmigu.cn

Go:   strings.Index(s, "x")
来源：http://ta.9csxet.cn

Ruby: s.index("x")
来源：http://zq.shtwfgs.cn

C#:   s.IndexOf("x")
来源：http://ba.huixiangedu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://uk.shxzskj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fy.gzmigu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rj.chemitech.net.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bu.lnxyls.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zc.yuexingan06.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ws.muxihuayi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jm.asd995.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fu.wgjwhj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wl.shxzskj.cn

[E06] 替换子串
来源：http://sr.wgjwhj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gs.asd995.cn

PHP:  str_replace("a", "b", $s);
来源：http://ia.haigaiapp.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bx.521024.cn

TS:   s.replaceAll("a", "b")
来源：http://zn.wgjwhj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dd.nicolike.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rq.haigaiapp.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gs.hahajie.cn

C#:   s.Replace("a", "b")
来源：http://fq.gzmigu.cn

[E07] 按分隔符拆分
来源：http://np.szxytkj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gw.colortex.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zf.521024.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://tr.hahajie.cn

TS:   s.split(",")
来源：http://xk.nicolike.cn

Java: s.split(",");  s.split("\\s+")
来源：http://nt.wgjwhj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ke.9csxet.cn

Ruby: s.split(",");  s.split
来源：http://az.hahajie.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tz.huixinmuqiang.cn

[E08] 数组按分隔符合并
来源：http://fi.yuntaijiaju.cn

Py:   ",".join(items)
来源：http://tb.bookmarksfly.cn

PHP:  implode(",", $items);
来源：http://kr.gzmigu.cn

JS:   items.join(",")
来源：http://gw.lnxyls.cn

TS:   items.join(",")
来源：http://ao.521024.cn

Java: String.join(",", items)
来源：http://op.bookmarksfly.cn

Go:   strings.Join(items, ",")
来源：http://pb.colortex.cn

Ruby: items.join(",")
来源：http://al.huanxung.cn

C#:   string.Join(",", items)
来源：http://nm.shxzukj.cn

[E09] 去除所有空白字符
来源：http://gu.yuexingan06.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://uz.jctech888.com.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yn.huixinmuqiang.cn

JS:   s.replace(/\s+/g, "")
来源：http://xs.muxihuayi.cn

TS:   s.replace(/\s+/g, "")
来源：http://uu.jianghongdianzi.cn

Java: s.replaceAll("\\s+", "")
来源：http://pl.haigaiapp.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://be.newstarts.cn

Ruby: s.gsub(/\s+/, "")
来源：http://th.nszjky.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vo.huixinmuqiang.cn

[E10] 左侧补零 / 定长填充
来源：http://wy.9csxet.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ni.wgjwhj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mt.chemitech.net.cn

JS:   "7".padStart(3, "0")
来源：http://ug.bookmarksfly.cn

TS:   "7".padStart(3, "0")
来源：http://lx.nicolike.cn

Java: String.format("%03d", 7)
来源：http://yp.gzmigu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ym.panjiajie.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wv.yuntaijiaju.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bx.bookmarksfly.cn

[E11] 反转字符串
来源：http://jt.bookmarksfly.cn

Py:   s[::-1]
来源：http://ew.huanxung.cn

PHP:  strrev($s);
来源：http://lc.szsharing.cn

JS:   [...s].reverse().join("")
来源：http://kt.haigaiapp.cn

TS:   [...s].reverse().join("")
来源：http://sy.asd995.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://fr.huanxung.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://oo.bjjhwx.cn

Ruby: s.reverse
来源：http://sd.asd995.cn

C#:   new string(s.Reverse().ToArray())
来源：http://rb.szxytkj.cn

[E12] 统计某字符出现次数
来源：http://yr.9csxet.cn

Py:   s.count("a")
来源：http://fm.lnxyls.cn

PHP:  substr_count($s, "a");
来源：http://te.asd995.cn

JS:   s.split("a").length - 1
来源：http://yl.huixiangedu.cn

TS:   s.split("a").length - 1
来源：http://ai.nszjky.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://iz.yuexingan06.cn

Go:   strings.Count(s, "a")
来源：http://ba.hnjuh.cn

Ruby: s.count("a")
来源：http://bg.hahajie.cn

C#:   s.Count(c => c == 'a')
来源：http://bm.jctech888.com.cn

[E13] 逐字符遍历
来源：http://ls.shtwfgs.cn

Py:   for ch in s: print(ch)
来源：http://ai.haigaiapp.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sv.huanxung.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://fn.yuexingan06.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ze.huixiangedu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tz.huixinmuqiang.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hl.jctech888.com.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ov.hnjuh.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mb.colortex.cn

[E14] URL 编码与 Base64
来源：http://aj.shtwfgs.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://uo.hnjuh.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://zv.jianghongdianzi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ry.muxihuayi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ci.newstarts.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xj.haigaiapp.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bk.huixinmuqiang.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.colortex.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://us.shxzukj.cn

[E15] HTML 转义 / 反转义
来源：http://ul.521024.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://tm.gzmigu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jc.shxzskj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rf.nszjky.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://jp.shxzskj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ny.hnjuh.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://an.panjiajie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://oj.nszjky.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fn.bjjhwx.cn

[E16] 数字千分位
来源：http://gc.jianghongdianzi.cn

Py:   f"{1234567:,}"
来源：http://fg.hahajie.cn

PHP:  number_format(1234567);
来源：http://qf.newstarts.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://bz.nszjky.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://qk.huanxung.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://du.9csxet.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dk.newstarts.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ve.nszjky.cn

C#:   1234567.ToString("N0")
来源：http://dw.9csxet.cn

[E17] 首字母大写
来源：http://ps.lnxyls.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mr.jctech888.com.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://sm.521024.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pq.huixiangedu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ye.wgjwhj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ck.lnxyls.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vu.bookmarksfly.cn

Ruby: s.capitalize
来源：http://qg.huixinmuqiang.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hk.gzmigu.cn

[E18] 模板占位符替换
来源：http://br.huixiangedu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rg.hnjuh.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mc.huanxung.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://jc.jianghongdianzi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://gb.huixiangedu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rh.wgjwhj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rr.newstarts.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qz.gzmigu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ub.yuntaijiaju.cn

[E19] 多行文本按行拆分
来源：http://zf.wgjwhj.cn

Py:   s.splitlines()
来源：http://jc.yuexingan06.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pp.jctech888.com.cn

JS:   s.split(/\r?\n/)
来源：http://ve.panjiajie.cn

TS:   s.split(/\r?\n/)
来源：http://li.huixinmuqiang.cn

Java: s.lines().toList()
来源：http://ph.jctech888.com.cn

Go:   strings.Split(s, "\n")
来源：http://uk.gzmigu.cn

Ruby: s.lines
来源：http://cp.shtwfgs.cn

C#:   s.Split('\n')
来源：http://dc.bjjhwx.cn

[E20] 判断字符串是否为空
来源：http://ny.hahajie.cn

Py:   if not s:
来源：http://ta.huixiangedu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://aw.haigaiapp.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cc.shtwfgs.cn

TS:   if (s === "") {}
来源：http://wz.colortex.cn

Java: if (s.isEmpty()) {}
来源：http://fg.shtwfgs.cn

Go:   if s == "" {}
来源：http://rl.gzmigu.cn

Ruby: if s.empty?
来源：http://nm.hahajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vx.bookmarksfly.cn

[E21] 超长截断加省略号
来源：http://ew.szxytkj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ms.jianghongdianzi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ty.colortex.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wz.panjiajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ja.asd995.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dj.szxytkj.cn

Go:   // 按 rune 判断长度后截断
来源：http://cd.shtwfgs.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ff.yuntaijiaju.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hn.bjjhwx.cn

[E22] 字节长度与字符长度
来源：http://sg.jianghongdianzi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fn.lnxyls.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ta.chemitech.net.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fm.jctech888.com.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yv.szsharing.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rk.panjiajie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ax.panjiajie.cn

Ruby: s.bytesize;  s.length
来源：http://mn.shtwfgs.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ti.gzmigu.cn

================================================================================
来源：http://zq.9csxet.cn

F. 文件与目录
来源：http://kq.panjiajie.cn

================================================================================
来源：http://fd.muxihuayi.cn

[F01] 读取整个文件
来源：http://yh.yuexingan06.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ht.huanxung.cn

PHP:  file_get_contents("a.txt");
来源：http://bd.muxihuayi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jw.wgjwhj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bi.panjiajie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zr.huixiangedu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ua.szsharing.cn

Ruby: File.read("a.txt")
来源：http://bh.huixinmuqiang.cn

C#:   File.ReadAllText("a.txt");
来源：http://jp.panjiajie.cn

[F02] 逐行读取文件
来源：http://zr.nszjky.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uv.huanxung.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gv.chemitech.net.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jc.shxzukj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ng.hnjuh.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lk.hahajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vb.hnjuh.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://px.bjjhwx.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ew.lnxyls.cn

[F03] 写入文件（覆盖）
来源：http://an.shxzskj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://aq.colortex.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://gt.521024.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xf.lnxyls.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zu.bjjhwx.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://aa.asd995.cn


<!-- 参考信息 -->