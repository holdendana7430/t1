代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yf.521024.cn

PHP:  array_merge(...$nested);
来源：http://mu.haigaiapp.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hu.lnxyls.cn

TS:   nested.flat();
来源：http://gy.bjjhwx.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lw.nicolike.cn

Go:   // 手写双层循环
来源：http://gj.haigaiapp.cn

Ruby: nested.flatten
来源：http://kp.shtwfgs.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ta.shtwfgs.cn

[D19] 按字段分组
来源：http://jy.gzmigu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.szxytkj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cc.szxytkj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tr.shtwfgs.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xt.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://la.bjjhwx.cn

Go:   // 手写 map[string][]T
来源：http://iy.jctech888.com.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ss.nicolike.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://sp.hnjuh.cn

[D20] 统计每个元素出现次数
来源：http://yb.huixiangedu.cn

Py:   Counter(arr)
来源：http://qc.szxytkj.cn

PHP:  array_count_values($arr);
来源：http://ie.huixiangedu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kq.9csxet.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bz.shxzukj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qu.wgjwhj.cn

Go:   // 手写 map[T]int
来源：http://er.wgjwhj.cn

Ruby: arr.tally
来源：http://tg.muxihuayi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qq.9csxet.cn

[D21] 判断是否包含某元素
来源：http://vh.muxihuayi.cn

Py:   x in arr
来源：http://jq.nszjky.cn

PHP:  in_array($x, $arr, true);
来源：http://es.chemitech.net.cn

JS:   arr.includes(x)
来源：http://ek.shxzukj.cn

TS:   arr.includes(x)
来源：http://xu.bookmarksfly.cn

Java: list.contains(x)
来源：http://ru.hahajie.cn

Go:   slices.Contains(arr, x)
来源：http://ef.newstarts.cn

Ruby: arr.include?(x)
来源：http://ba.newstarts.cn

C#:   list.Contains(x)
来源：http://tn.jctech888.com.cn

[D22] 复制数组（避免共享引用）
来源：http://tr.yuexingan06.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tv.huixiangedu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vi.haigaiapp.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tk.newstarts.cn

TS:   [...arr];
来源：http://df.jianghongdianzi.cn

Java: new ArrayList<>(list);
来源：http://xx.nicolike.cn

Go:   copied := append([]int(nil), arr...)
来源：http://yj.yuexingan06.cn

Ruby: arr.dup;  arr.clone
来源：http://pm.lnxyls.cn

C#:   new List<int>(list);
来源：http://vi.panjiajie.cn

[D23] reduce 累积计算
来源：http://sb.nicolike.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tt.asd995.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://sa.hnjuh.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://us.jctech888.com.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vh.nszjky.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://gh.szxytkj.cn

Go:   // 手写循环
来源：http://hi.shxzskj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ca.hnjuh.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sm.gzmigu.cn

[D24] 字典 / Map 基本操作
来源：http://wo.hnjuh.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ak.chemitech.net.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nd.shxzukj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://su.yuntaijiaju.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sj.bjjhwx.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nu.nicolike.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qs.gzmigu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rs.huixiangedu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ne.huixinmuqiang.cn

[D25] Set 集合去重与交并差
来源：http://ju.szxytkj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bw.colortex.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rl.muxihuayi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vw.gzmigu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wj.nicolike.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://yc.muxihuayi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wj.yuntaijiaju.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nv.yuexingan06.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nz.jianghongdianzi.cn

[D26] 数组转字符串
来源：http://wr.yuntaijiaju.cn

Py:   ", ".join(map(str, arr))
来源：http://cm.hnjuh.cn

PHP:  implode(", ", $arr);
来源：http://or.hahajie.cn

JS:   arr.join(", ")
来源：http://ts.shtwfgs.cn

TS:   arr.join(", ")
来源：http://cp.szxytkj.cn

Java: String.join(", ", list)
来源：http://hr.hnjuh.cn

Go:   strings.Join(strs, ", ")
来源：http://yo.nicolike.cn

Ruby: arr.join(", ")
来源：http://mp.gzmigu.cn

C#:   string.Join(", ", list)
来源：http://sb.bookmarksfly.cn

================================================================================
来源：http://fk.bjjhwx.cn

E. 字符串处理
来源：http://pq.bookmarksfly.cn

================================================================================
来源：http://bq.yuntaijiaju.cn

[E01] 拼接字符串
来源：http://iz.nicolike.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://il.shxzukj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dd.newstarts.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uo.nicolike.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ku.bookmarksfly.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zo.521024.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nx.jctech888.com.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ec.chemitech.net.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ce.wgjwhj.cn

[E02] 重复字符串
来源：http://sz.jianghongdianzi.cn

Py:   "ab" * 3
来源：http://uq.huanxung.cn

PHP:  str_repeat("ab", 3);
来源：http://dt.lnxyls.cn

JS:   "ab".repeat(3)
来源：http://zf.nicolike.cn

TS:   "ab".repeat(3)
来源：http://mz.huixiangedu.cn

Java: "ab".repeat(3)
来源：http://ea.bjjhwx.cn

Go:   strings.Repeat("ab", 3)
来源：http://ob.gzmigu.cn

Ruby: "ab" * 3
来源：http://oe.hnjuh.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zl.bjjhwx.cn

[E03] 截取子串
来源：http://rp.shxzskj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ay.jctech888.com.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xc.hnjuh.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tg.colortex.cn

TS:   s.slice(1, 4)
来源：http://my.bookmarksfly.cn

Java: s.substring(1, 4)
来源：http://ts.hahajie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ln.bjjhwx.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ej.shtwfgs.cn

C#:   s.Substring(1, 3)
来源：http://tb.hahajie.cn

[E04] 查找子串位置
来源：http://pv.lnxyls.cn

Py:   s.find("x");  s.index("x")
来源：http://bj.shxzukj.cn

PHP:  strpos($s, "x");
来源：http://pw.nszjky.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dt.huixiangedu.cn

TS:   s.indexOf("x")
来源：http://ot.jctech888.com.cn

Java: s.indexOf("x")
来源：http://tb.shxzskj.cn

Go:   strings.Index(s, "x")
来源：http://wl.huixinmuqiang.cn

Ruby: s.index("x")
来源：http://xz.muxihuayi.cn

C#:   s.IndexOf("x")
来源：http://qv.haigaiapp.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://fi.szsharing.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fm.chemitech.net.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tc.521024.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ez.asd995.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://uq.newstarts.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tr.jctech888.com.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://oh.hahajie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xl.yuntaijiaju.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ju.huixiangedu.cn

[E06] 替换子串
来源：http://st.gzmigu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://we.hahajie.cn

PHP:  str_replace("a", "b", $s);
来源：http://ub.szxytkj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tu.szxytkj.cn

TS:   s.replaceAll("a", "b")
来源：http://sw.colortex.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fl.9csxet.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://br.colortex.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xk.huixinmuqiang.cn

C#:   s.Replace("a", "b")
来源：http://tc.521024.cn

[E07] 按分隔符拆分
来源：http://by.huanxung.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tk.huanxung.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://io.newstarts.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://hm.9csxet.cn

TS:   s.split(",")
来源：http://rh.huanxung.cn

Java: s.split(",");  s.split("\\s+")
来源：http://we.yuexingan06.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ou.bjjhwx.cn

Ruby: s.split(",");  s.split
来源：http://he.huanxung.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wp.gzmigu.cn

[E08] 数组按分隔符合并
来源：http://jm.colortex.cn

Py:   ",".join(items)
来源：http://ol.shtwfgs.cn

PHP:  implode(",", $items);
来源：http://li.huixinmuqiang.cn

JS:   items.join(",")
来源：http://fz.lnxyls.cn

TS:   items.join(",")
来源：http://dg.wgjwhj.cn

Java: String.join(",", items)
来源：http://jj.bjjhwx.cn

Go:   strings.Join(items, ",")
来源：http://jf.shxzskj.cn

Ruby: items.join(",")
来源：http://el.huixinmuqiang.cn

C#:   string.Join(",", items)
来源：http://po.nszjky.cn

[E09] 去除所有空白字符
来源：http://pa.chemitech.net.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cl.panjiajie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://sr.chemitech.net.cn

JS:   s.replace(/\s+/g, "")
来源：http://bv.newstarts.cn

TS:   s.replace(/\s+/g, "")
来源：http://bq.huixinmuqiang.cn

Java: s.replaceAll("\\s+", "")
来源：http://ll.panjiajie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ez.hahajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://zh.9csxet.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ex.colortex.cn

[E10] 左侧补零 / 定长填充
来源：http://ak.shxzskj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vb.hnjuh.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ap.gzmigu.cn

JS:   "7".padStart(3, "0")
来源：http://fk.nicolike.cn

TS:   "7".padStart(3, "0")
来源：http://cl.wgjwhj.cn

Java: String.format("%03d", 7)
来源：http://yr.nicolike.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ev.huixinmuqiang.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fz.9csxet.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tv.9csxet.cn

[E11] 反转字符串
来源：http://vc.huanxung.cn

Py:   s[::-1]
来源：http://jh.nicolike.cn

PHP:  strrev($s);
来源：http://ys.muxihuayi.cn

JS:   [...s].reverse().join("")
来源：http://fz.huixiangedu.cn

TS:   [...s].reverse().join("")
来源：http://ar.gzmigu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wv.haigaiapp.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://yr.panjiajie.cn

Ruby: s.reverse
来源：http://ai.huanxung.cn

C#:   new string(s.Reverse().ToArray())
来源：http://zj.asd995.cn

[E12] 统计某字符出现次数
来源：http://xp.hnjuh.cn

Py:   s.count("a")
来源：http://cl.521024.cn

PHP:  substr_count($s, "a");
来源：http://xc.yuntaijiaju.cn

JS:   s.split("a").length - 1
来源：http://kl.newstarts.cn

TS:   s.split("a").length - 1
来源：http://ml.szxytkj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cs.asd995.cn

Go:   strings.Count(s, "a")
来源：http://ys.chemitech.net.cn

Ruby: s.count("a")
来源：http://as.panjiajie.cn

C#:   s.Count(c => c == 'a')
来源：http://vy.wgjwhj.cn

[E13] 逐字符遍历
来源：http://zm.bookmarksfly.cn

Py:   for ch in s: print(ch)
来源：http://ys.chemitech.net.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rs.shxzskj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://zp.newstarts.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://el.colortex.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cj.huanxung.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hg.521024.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://nc.huixiangedu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ik.lnxyls.cn

[E14] URL 编码与 Base64
来源：http://hs.huixinmuqiang.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sn.jctech888.com.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ia.521024.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wm.chemitech.net.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nn.gzmigu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zn.haigaiapp.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ll.huixiangedu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fq.szsharing.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ho.yuexingan06.cn

[E15] HTML 转义 / 反转义
来源：http://ac.newstarts.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://zg.bjjhwx.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bn.shxzukj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gh.nszjky.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://bn.asd995.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://iv.colortex.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://go.shxzukj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ah.shxzukj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jw.521024.cn

[E16] 数字千分位
来源：http://nv.jianghongdianzi.cn

Py:   f"{1234567:,}"
来源：http://dr.chemitech.net.cn

PHP:  number_format(1234567);
来源：http://vl.shxzskj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://qk.jianghongdianzi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://jj.9csxet.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ka.lnxyls.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lt.shxzskj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gu.huixinmuqiang.cn

C#:   1234567.ToString("N0")
来源：http://sb.newstarts.cn

[E17] 首字母大写
来源：http://er.9csxet.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qu.hnjuh.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://as.nszjky.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qe.shxzskj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ox.huixiangedu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wf.nicolike.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wl.huixiangedu.cn

Ruby: s.capitalize
来源：http://re.yuntaijiaju.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vr.shxzskj.cn

[E18] 模板占位符替换
来源：http://es.shtwfgs.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ew.nicolike.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hs.huixiangedu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://oz.haigaiapp.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://mk.nicolike.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hj.panjiajie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sw.hahajie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cw.jianghongdianzi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ap.nicolike.cn

[E19] 多行文本按行拆分
来源：http://er.yuexingan06.cn

Py:   s.splitlines()
来源：http://xh.jianghongdianzi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rp.bookmarksfly.cn

JS:   s.split(/\r?\n/)
来源：http://yu.yuexingan06.cn

TS:   s.split(/\r?\n/)
来源：http://xk.jianghongdianzi.cn

Java: s.lines().toList()
来源：http://ol.shtwfgs.cn

Go:   strings.Split(s, "\n")
来源：http://ju.szsharing.cn

Ruby: s.lines
来源：http://ur.yuntaijiaju.cn

C#:   s.Split('\n')
来源：http://nv.gzmigu.cn

[E20] 判断字符串是否为空
来源：http://jl.muxihuayi.cn

Py:   if not s:
来源：http://to.hnjuh.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pf.bookmarksfly.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bh.shtwfgs.cn

TS:   if (s === "") {}
来源：http://hr.nszjky.cn

Java: if (s.isEmpty()) {}
来源：http://oz.yuntaijiaju.cn

Go:   if s == "" {}
来源：http://tv.szsharing.cn

Ruby: if s.empty?
来源：http://ey.colortex.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sy.szsharing.cn

[E21] 超长截断加省略号
来源：http://ki.jctech888.com.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://si.lnxyls.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rx.bjjhwx.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wp.lnxyls.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lx.colortex.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rt.hahajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://uo.9csxet.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gj.wgjwhj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fn.huixinmuqiang.cn

[E22] 字节长度与字符长度
来源：http://ee.panjiajie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ne.huanxung.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nm.huixinmuqiang.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wn.newstarts.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ju.hahajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sm.bjjhwx.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ee.szsharing.cn

Ruby: s.bytesize;  s.length
来源：http://xo.chemitech.net.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jb.jianghongdianzi.cn

================================================================================
来源：http://fi.gzmigu.cn

F. 文件与目录
来源：http://wz.colortex.cn

================================================================================
来源：http://cb.lnxyls.cn

[F01] 读取整个文件
来源：http://oj.bookmarksfly.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bi.yuntaijiaju.cn

PHP:  file_get_contents("a.txt");
来源：http://gd.bjjhwx.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lq.asd995.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lx.bjjhwx.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jw.haigaiapp.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xm.gzmigu.cn

Ruby: File.read("a.txt")
来源：http://kw.chemitech.net.cn

C#:   File.ReadAllText("a.txt");
来源：http://qk.wgjwhj.cn

[F02] 逐行读取文件
来源：http://rf.nicolike.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ri.yuexingan06.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://oq.muxihuayi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nd.9csxet.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kl.nszjky.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ui.jianghongdianzi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xj.shxzskj.cn


<!-- 参考信息 -->