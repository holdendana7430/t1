代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vj.huixiangedu.cn

PHP:  array_merge(...$nested);
来源：http://oz.hnjuh.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wc.shxzukj.cn

TS:   nested.flat();
来源：http://oh.panjiajie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ql.chemitech.net.cn

Go:   // 手写双层循环
来源：http://kn.nszjky.cn

Ruby: nested.flatten
来源：http://qe.yuexingan06.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://tg.muxihuayi.cn

[D19] 按字段分组
来源：http://no.haigaiapp.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pu.jctech888.com.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://st.shxzskj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kz.huanxung.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://nl.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ct.yuntaijiaju.cn

Go:   // 手写 map[string][]T
来源：http://sp.shxzukj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fg.shxzukj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://te.shxzukj.cn

[D20] 统计每个元素出现次数
来源：http://jz.huixinmuqiang.cn

Py:   Counter(arr)
来源：http://ke.nicolike.cn

PHP:  array_count_values($arr);
来源：http://qf.panjiajie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://es.chemitech.net.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ac.muxihuayi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://uv.shxzskj.cn

Go:   // 手写 map[T]int
来源：http://gz.jianghongdianzi.cn

Ruby: arr.tally
来源：http://mh.shxzukj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kl.huanxung.cn

[D21] 判断是否包含某元素
来源：http://nn.jianghongdianzi.cn

Py:   x in arr
来源：http://na.chemitech.net.cn

PHP:  in_array($x, $arr, true);
来源：http://vz.chemitech.net.cn

JS:   arr.includes(x)
来源：http://nh.bjjhwx.cn

TS:   arr.includes(x)
来源：http://kj.hnjuh.cn

Java: list.contains(x)
来源：http://mg.haigaiapp.cn

Go:   slices.Contains(arr, x)
来源：http://lo.huanxung.cn

Ruby: arr.include?(x)
来源：http://ud.panjiajie.cn

C#:   list.Contains(x)
来源：http://gl.yuntaijiaju.cn

[D22] 复制数组（避免共享引用）
来源：http://aj.huixiangedu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://co.newstarts.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ip.szxytkj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ux.shxzskj.cn

TS:   [...arr];
来源：http://hy.lnxyls.cn

Java: new ArrayList<>(list);
来源：http://ht.huixiangedu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://du.colortex.cn

Ruby: arr.dup;  arr.clone
来源：http://ll.szxytkj.cn

C#:   new List<int>(list);
来源：http://un.szxytkj.cn

[D23] reduce 累积计算
来源：http://ry.shxzukj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tn.asd995.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cs.yuexingan06.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zp.nszjky.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ai.jianghongdianzi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://sr.shxzskj.cn

Go:   // 手写循环
来源：http://xh.asd995.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ud.chemitech.net.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lk.huanxung.cn

[D24] 字典 / Map 基本操作
来源：http://yw.hnjuh.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bq.newstarts.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ig.szxytkj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://sb.yuntaijiaju.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jm.colortex.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mi.haigaiapp.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hr.bjjhwx.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hx.yuntaijiaju.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cz.newstarts.cn

[D25] Set 集合去重与交并差
来源：http://sq.jianghongdianzi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kg.hahajie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ml.lnxyls.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ze.nszjky.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qh.hnjuh.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wr.shxzukj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://am.yuexingan06.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ag.shtwfgs.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yi.shtwfgs.cn

[D26] 数组转字符串
来源：http://cf.jctech888.com.cn

Py:   ", ".join(map(str, arr))
来源：http://xc.shxzskj.cn

PHP:  implode(", ", $arr);
来源：http://ui.shtwfgs.cn

JS:   arr.join(", ")
来源：http://zw.nszjky.cn

TS:   arr.join(", ")
来源：http://gb.yuntaijiaju.cn

Java: String.join(", ", list)
来源：http://hv.muxihuayi.cn

Go:   strings.Join(strs, ", ")
来源：http://ip.lnxyls.cn

Ruby: arr.join(", ")
来源：http://jm.shxzskj.cn

C#:   string.Join(", ", list)
来源：http://rk.panjiajie.cn

================================================================================
来源：http://sx.chemitech.net.cn

E. 字符串处理
来源：http://yw.szsharing.cn

================================================================================
来源：http://vq.chemitech.net.cn

[E01] 拼接字符串
来源：http://ff.bjjhwx.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://db.huixinmuqiang.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ay.huanxung.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ev.shtwfgs.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tv.9csxet.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hp.jctech888.com.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gz.szsharing.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mm.shtwfgs.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bv.huixiangedu.cn

[E02] 重复字符串
来源：http://xu.hahajie.cn

Py:   "ab" * 3
来源：http://dm.szsharing.cn

PHP:  str_repeat("ab", 3);
来源：http://dl.shxzskj.cn

JS:   "ab".repeat(3)
来源：http://ge.9csxet.cn

TS:   "ab".repeat(3)
来源：http://bh.jctech888.com.cn

Java: "ab".repeat(3)
来源：http://ua.shxzskj.cn

Go:   strings.Repeat("ab", 3)
来源：http://my.wgjwhj.cn

Ruby: "ab" * 3
来源：http://th.hahajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pu.jctech888.com.cn

[E03] 截取子串
来源：http://nf.huixiangedu.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ej.jctech888.com.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wi.colortex.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jc.jctech888.com.cn

TS:   s.slice(1, 4)
来源：http://uw.nszjky.cn

Java: s.substring(1, 4)
来源：http://qc.yuntaijiaju.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pq.jianghongdianzi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://cz.hnjuh.cn

C#:   s.Substring(1, 3)
来源：http://dz.wgjwhj.cn

[E04] 查找子串位置
来源：http://sf.shxzukj.cn

Py:   s.find("x");  s.index("x")
来源：http://mi.colortex.cn

PHP:  strpos($s, "x");
来源：http://eh.yuntaijiaju.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nh.szsharing.cn

TS:   s.indexOf("x")
来源：http://hd.huixinmuqiang.cn

Java: s.indexOf("x")
来源：http://kn.chemitech.net.cn

Go:   strings.Index(s, "x")
来源：http://jc.muxihuayi.cn

Ruby: s.index("x")
来源：http://jp.nszjky.cn

C#:   s.IndexOf("x")
来源：http://mh.jctech888.com.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xm.shxzskj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ou.haigaiapp.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://eb.asd995.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qp.jctech888.com.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ev.lnxyls.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uh.shxzukj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ha.szsharing.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://og.shxzskj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://my.gzmigu.cn

[E06] 替换子串
来源：http://zx.chemitech.net.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sf.huixiangedu.cn

PHP:  str_replace("a", "b", $s);
来源：http://se.gzmigu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mr.lnxyls.cn

TS:   s.replaceAll("a", "b")
来源：http://au.chemitech.net.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qz.colortex.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ij.gzmigu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://id.lnxyls.cn

C#:   s.Replace("a", "b")
来源：http://rq.hnjuh.cn

[E07] 按分隔符拆分
来源：http://lf.colortex.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dp.huanxung.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jd.gzmigu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ax.lnxyls.cn

TS:   s.split(",")
来源：http://zs.hnjuh.cn

Java: s.split(",");  s.split("\\s+")
来源：http://sj.colortex.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kg.nicolike.cn

Ruby: s.split(",");  s.split
来源：http://cd.muxihuayi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lb.jctech888.com.cn

[E08] 数组按分隔符合并
来源：http://oa.hahajie.cn

Py:   ",".join(items)
来源：http://oz.newstarts.cn

PHP:  implode(",", $items);
来源：http://ij.huixinmuqiang.cn

JS:   items.join(",")
来源：http://li.shxzukj.cn

TS:   items.join(",")
来源：http://rd.shxzukj.cn

Java: String.join(",", items)
来源：http://jz.colortex.cn

Go:   strings.Join(items, ",")
来源：http://hu.newstarts.cn

Ruby: items.join(",")
来源：http://ii.huixiangedu.cn

C#:   string.Join(",", items)
来源：http://tn.gzmigu.cn

[E09] 去除所有空白字符
来源：http://tt.yuntaijiaju.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://uw.muxihuayi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nx.jianghongdianzi.cn

JS:   s.replace(/\s+/g, "")
来源：http://ba.huixiangedu.cn

TS:   s.replace(/\s+/g, "")
来源：http://do.chemitech.net.cn

Java: s.replaceAll("\\s+", "")
来源：http://ga.9csxet.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://xr.szxytkj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ok.chemitech.net.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ww.chemitech.net.cn

[E10] 左侧补零 / 定长填充
来源：http://vc.muxihuayi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://eq.szsharing.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hd.shxzukj.cn

JS:   "7".padStart(3, "0")
来源：http://di.9csxet.cn

TS:   "7".padStart(3, "0")
来源：http://pb.hahajie.cn

Java: String.format("%03d", 7)
来源：http://yw.jianghongdianzi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ew.haigaiapp.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rp.bjjhwx.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://em.asd995.cn

[E11] 反转字符串
来源：http://fm.huixinmuqiang.cn

Py:   s[::-1]
来源：http://jb.lnxyls.cn

PHP:  strrev($s);
来源：http://vn.nszjky.cn

JS:   [...s].reverse().join("")
来源：http://qs.colortex.cn

TS:   [...s].reverse().join("")
来源：http://zn.nicolike.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://mp.wgjwhj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ci.panjiajie.cn

Ruby: s.reverse
来源：http://lf.szsharing.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qd.chemitech.net.cn

[E12] 统计某字符出现次数
来源：http://la.jianghongdianzi.cn

Py:   s.count("a")
来源：http://fc.nszjky.cn

PHP:  substr_count($s, "a");
来源：http://fy.hnjuh.cn

JS:   s.split("a").length - 1
来源：http://dn.wgjwhj.cn

TS:   s.split("a").length - 1
来源：http://pf.nszjky.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ss.lnxyls.cn

Go:   strings.Count(s, "a")
来源：http://la.panjiajie.cn

Ruby: s.count("a")
来源：http://iz.jctech888.com.cn

C#:   s.Count(c => c == 'a')
来源：http://pu.bookmarksfly.cn

[E13] 逐字符遍历
来源：http://ye.szxytkj.cn

Py:   for ch in s: print(ch)
来源：http://nw.jctech888.com.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sx.newstarts.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://cj.wgjwhj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://yp.shxzskj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hm.huixinmuqiang.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ti.shxzskj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ev.hahajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jw.haigaiapp.cn

[E14] URL 编码与 Base64
来源：http://ys.newstarts.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vg.lnxyls.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://jx.haigaiapp.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dn.lnxyls.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wc.huixiangedu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bd.panjiajie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xf.9csxet.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mf.huanxung.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ak.9csxet.cn

[E15] HTML 转义 / 反转义
来源：http://sl.newstarts.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://pl.panjiajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://iz.gzmigu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fb.panjiajie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://gw.jctech888.com.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://nb.shtwfgs.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ig.chemitech.net.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rh.jianghongdianzi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://iw.jianghongdianzi.cn

[E16] 数字千分位
来源：http://mu.newstarts.cn

Py:   f"{1234567:,}"
来源：http://cs.panjiajie.cn

PHP:  number_format(1234567);
来源：http://sq.521024.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ga.haigaiapp.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://sm.jctech888.com.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rv.wgjwhj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ba.szxytkj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://os.yuntaijiaju.cn

C#:   1234567.ToString("N0")
来源：http://hr.szxytkj.cn

[E17] 首字母大写
来源：http://up.9csxet.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zc.colortex.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://la.shxzukj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bh.haigaiapp.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oc.521024.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lc.hnjuh.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ae.huanxung.cn

Ruby: s.capitalize
来源：http://uf.jianghongdianzi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ju.9csxet.cn

[E18] 模板占位符替换
来源：http://ms.nicolike.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wp.haigaiapp.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ms.yuntaijiaju.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://za.szsharing.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://br.jianghongdianzi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qf.nicolike.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zp.nicolike.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://yw.colortex.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ek.lnxyls.cn

[E19] 多行文本按行拆分
来源：http://zw.muxihuayi.cn

Py:   s.splitlines()
来源：http://ct.huixinmuqiang.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jh.hahajie.cn

JS:   s.split(/\r?\n/)
来源：http://pt.muxihuayi.cn

TS:   s.split(/\r?\n/)
来源：http://sl.9csxet.cn

Java: s.lines().toList()
来源：http://ia.hahajie.cn

Go:   strings.Split(s, "\n")
来源：http://li.szxytkj.cn

Ruby: s.lines
来源：http://we.szxytkj.cn

C#:   s.Split('\n')
来源：http://re.asd995.cn

[E20] 判断字符串是否为空
来源：http://cf.asd995.cn

Py:   if not s:
来源：http://gl.shtwfgs.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fo.gzmigu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zs.jianghongdianzi.cn

TS:   if (s === "") {}
来源：http://lx.lnxyls.cn

Java: if (s.isEmpty()) {}
来源：http://bb.huanxung.cn

Go:   if s == "" {}
来源：http://qc.haigaiapp.cn

Ruby: if s.empty?
来源：http://hp.hnjuh.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kv.yuexingan06.cn

[E21] 超长截断加省略号
来源：http://og.hnjuh.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://to.szsharing.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://df.yuexingan06.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ee.szsharing.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lt.hnjuh.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mk.huixiangedu.cn

Go:   // 按 rune 判断长度后截断
来源：http://qv.hnjuh.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ix.lnxyls.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fl.muxihuayi.cn

[E22] 字节长度与字符长度
来源：http://fm.hnjuh.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tj.bjjhwx.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dv.shxzskj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gx.bookmarksfly.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ar.wgjwhj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jr.hahajie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://em.bjjhwx.cn

Ruby: s.bytesize;  s.length
来源：http://db.hahajie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xf.asd995.cn

================================================================================
来源：http://nk.521024.cn

F. 文件与目录
来源：http://vu.shxzukj.cn

================================================================================
来源：http://zi.colortex.cn

[F01] 读取整个文件
来源：http://gj.521024.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ot.szxytkj.cn

PHP:  file_get_contents("a.txt");
来源：http://vr.szsharing.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wf.yuntaijiaju.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kz.nicolike.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://sr.bjjhwx.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gi.asd995.cn

Ruby: File.read("a.txt")
来源：http://dr.shxzukj.cn

C#:   File.ReadAllText("a.txt");
来源：http://lw.huixinmuqiang.cn

[F02] 逐行读取文件
来源：http://bb.nszjky.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ts.chemitech.net.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://so.huanxung.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dd.nszjky.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wk.huixiangedu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fb.521024.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zh.bjjhwx.cn


<!-- 参考信息 -->