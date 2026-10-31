代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://pa.huanxung.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ro.muxihuayi.cn

TS:   Math.max(...arr);
来源：http://ow.shxzukj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://em.yuexingan06.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vj.lnxyls.cn

Ruby: arr.max;  arr.min
来源：http://qc.newstarts.cn

C#:   list.Max();  list.Min()
来源：http://cp.shtwfgs.cn

[D18] 扁平化嵌套数组
来源：http://fm.huixiangedu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://su.huixiangedu.cn

PHP:  array_merge(...$nested);
来源：http://fz.hahajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mr.panjiajie.cn

TS:   nested.flat();
来源：http://ze.bjjhwx.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rs.bookmarksfly.cn

Go:   // 手写双层循环
来源：http://rj.521024.cn

Ruby: nested.flatten
来源：http://rv.nszjky.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://vn.szsharing.cn

[D19] 按字段分组
来源：http://ra.panjiajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ek.yuntaijiaju.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ip.panjiajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qj.chemitech.net.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ci.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ay.nicolike.cn

Go:   // 手写 map[string][]T
来源：http://zu.asd995.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ig.newstarts.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mm.szxytkj.cn

[D20] 统计每个元素出现次数
来源：http://bv.huixiangedu.cn

Py:   Counter(arr)
来源：http://lk.szxytkj.cn

PHP:  array_count_values($arr);
来源：http://ay.asd995.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yz.bjjhwx.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://co.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://us.jianghongdianzi.cn

Go:   // 手写 map[T]int
来源：http://oz.gzmigu.cn

Ruby: arr.tally
来源：http://db.hnjuh.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fx.szxytkj.cn

[D21] 判断是否包含某元素
来源：http://dt.wgjwhj.cn

Py:   x in arr
来源：http://li.nszjky.cn

PHP:  in_array($x, $arr, true);
来源：http://ya.9csxet.cn

JS:   arr.includes(x)
来源：http://xh.newstarts.cn

TS:   arr.includes(x)
来源：http://na.nicolike.cn

Java: list.contains(x)
来源：http://cl.521024.cn

Go:   slices.Contains(arr, x)
来源：http://qw.hahajie.cn

Ruby: arr.include?(x)
来源：http://as.shxzukj.cn

C#:   list.Contains(x)
来源：http://fz.jctech888.com.cn

[D22] 复制数组（避免共享引用）
来源：http://ol.panjiajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wr.9csxet.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vi.asd995.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://sz.nicolike.cn

TS:   [...arr];
来源：http://rk.shxzskj.cn

Java: new ArrayList<>(list);
来源：http://ft.szxytkj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://gk.szxytkj.cn

Ruby: arr.dup;  arr.clone
来源：http://ia.shxzskj.cn

C#:   new List<int>(list);
来源：http://to.bjjhwx.cn

[D23] reduce 累积计算
来源：http://mw.asd995.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cn.hahajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ob.szxytkj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cm.nicolike.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vr.jianghongdianzi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://cl.huixiangedu.cn

Go:   // 手写循环
来源：http://ik.hahajie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gm.bookmarksfly.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://uu.szxytkj.cn

[D24] 字典 / Map 基本操作
来源：http://ja.huanxung.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tf.gzmigu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jj.asd995.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hd.panjiajie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qe.hahajie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://df.nicolike.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dm.yuntaijiaju.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ao.huixinmuqiang.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://aq.colortex.cn

[D25] Set 集合去重与交并差
来源：http://xe.lnxyls.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ac.yuntaijiaju.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xg.nicolike.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://as.nicolike.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://iw.yuexingan06.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://in.huixinmuqiang.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xd.521024.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kv.9csxet.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://za.newstarts.cn

[D26] 数组转字符串
来源：http://rt.gzmigu.cn

Py:   ", ".join(map(str, arr))
来源：http://ma.bookmarksfly.cn

PHP:  implode(", ", $arr);
来源：http://ro.szsharing.cn

JS:   arr.join(", ")
来源：http://vk.chemitech.net.cn

TS:   arr.join(", ")
来源：http://fs.colortex.cn

Java: String.join(", ", list)
来源：http://el.shtwfgs.cn

Go:   strings.Join(strs, ", ")
来源：http://td.huixinmuqiang.cn

Ruby: arr.join(", ")
来源：http://wi.jctech888.com.cn

C#:   string.Join(", ", list)
来源：http://bh.521024.cn

================================================================================
来源：http://yc.muxihuayi.cn

E. 字符串处理
来源：http://ue.yuntaijiaju.cn

================================================================================
来源：http://rd.521024.cn

[E01] 拼接字符串
来源：http://db.newstarts.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://eu.bjjhwx.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mb.szxytkj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lw.muxihuayi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cv.nszjky.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ms.huixiangedu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bq.huixinmuqiang.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://uh.hnjuh.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://em.hahajie.cn

[E02] 重复字符串
来源：http://ym.asd995.cn

Py:   "ab" * 3
来源：http://xz.jianghongdianzi.cn

PHP:  str_repeat("ab", 3);
来源：http://wr.shxzukj.cn

JS:   "ab".repeat(3)
来源：http://px.panjiajie.cn

TS:   "ab".repeat(3)
来源：http://jl.bjjhwx.cn

Java: "ab".repeat(3)
来源：http://lm.shxzskj.cn

Go:   strings.Repeat("ab", 3)
来源：http://dp.huixinmuqiang.cn

Ruby: "ab" * 3
来源：http://dg.jianghongdianzi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bc.huanxung.cn

[E03] 截取子串
来源：http://jl.nszjky.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xo.muxihuayi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://se.bookmarksfly.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cy.jctech888.com.cn

TS:   s.slice(1, 4)
来源：http://ka.szsharing.cn

Java: s.substring(1, 4)
来源：http://ju.shxzukj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tv.shxzukj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ja.bookmarksfly.cn

C#:   s.Substring(1, 3)
来源：http://zl.chemitech.net.cn

[E04] 查找子串位置
来源：http://re.huanxung.cn

Py:   s.find("x");  s.index("x")
来源：http://ni.gzmigu.cn

PHP:  strpos($s, "x");
来源：http://qb.shxzukj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jy.lnxyls.cn

TS:   s.indexOf("x")
来源：http://mg.lnxyls.cn

Java: s.indexOf("x")
来源：http://kx.szxytkj.cn

Go:   strings.Index(s, "x")
来源：http://uw.panjiajie.cn

Ruby: s.index("x")
来源：http://xq.asd995.cn

C#:   s.IndexOf("x")
来源：http://ho.yuntaijiaju.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xa.szxytkj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fb.bookmarksfly.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lb.huanxung.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nn.colortex.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://tm.gzmigu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tt.colortex.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://in.9csxet.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ae.gzmigu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://aa.gzmigu.cn

[E06] 替换子串
来源：http://lm.521024.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lf.jianghongdianzi.cn

PHP:  str_replace("a", "b", $s);
来源：http://gw.lnxyls.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://za.newstarts.cn

TS:   s.replaceAll("a", "b")
来源：http://zd.jianghongdianzi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ia.newstarts.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://it.bookmarksfly.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xi.nicolike.cn

C#:   s.Replace("a", "b")
来源：http://qp.huanxung.cn

[E07] 按分隔符拆分
来源：http://ds.asd995.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cg.hnjuh.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jd.nszjky.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://fr.haigaiapp.cn

TS:   s.split(",")
来源：http://es.nicolike.cn

Java: s.split(",");  s.split("\\s+")
来源：http://dy.bjjhwx.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yt.szsharing.cn

Ruby: s.split(",");  s.split
来源：http://rb.szsharing.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vr.lnxyls.cn

[E08] 数组按分隔符合并
来源：http://au.jianghongdianzi.cn

Py:   ",".join(items)
来源：http://pz.shtwfgs.cn

PHP:  implode(",", $items);
来源：http://mn.haigaiapp.cn

JS:   items.join(",")
来源：http://ph.nicolike.cn

TS:   items.join(",")
来源：http://ka.huixinmuqiang.cn

Java: String.join(",", items)
来源：http://yr.hnjuh.cn

Go:   strings.Join(items, ",")
来源：http://lz.hnjuh.cn

Ruby: items.join(",")
来源：http://rs.gzmigu.cn

C#:   string.Join(",", items)
来源：http://zl.asd995.cn

[E09] 去除所有空白字符
来源：http://bf.haigaiapp.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bt.gzmigu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://eb.shtwfgs.cn

JS:   s.replace(/\s+/g, "")
来源：http://as.bjjhwx.cn

TS:   s.replace(/\s+/g, "")
来源：http://qb.muxihuayi.cn

Java: s.replaceAll("\\s+", "")
来源：http://io.shxzukj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://xg.huanxung.cn

Ruby: s.gsub(/\s+/, "")
来源：http://le.huixiangedu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pb.colortex.cn

[E10] 左侧补零 / 定长填充
来源：http://lo.panjiajie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dj.shxzukj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ah.hnjuh.cn

JS:   "7".padStart(3, "0")
来源：http://tu.szsharing.cn

TS:   "7".padStart(3, "0")
来源：http://me.jianghongdianzi.cn

Java: String.format("%03d", 7)
来源：http://rz.521024.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://kd.asd995.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tx.szsharing.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rq.hahajie.cn

[E11] 反转字符串
来源：http://rj.521024.cn

Py:   s[::-1]
来源：http://bz.huanxung.cn

PHP:  strrev($s);
来源：http://ix.szxytkj.cn

JS:   [...s].reverse().join("")
来源：http://rl.gzmigu.cn

TS:   [...s].reverse().join("")
来源：http://te.hahajie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://uy.huixinmuqiang.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://hh.jianghongdianzi.cn

Ruby: s.reverse
来源：http://fe.bookmarksfly.cn

C#:   new string(s.Reverse().ToArray())
来源：http://so.haigaiapp.cn

[E12] 统计某字符出现次数
来源：http://qp.panjiajie.cn

Py:   s.count("a")
来源：http://vx.521024.cn

PHP:  substr_count($s, "a");
来源：http://qm.521024.cn

JS:   s.split("a").length - 1
来源：http://dx.colortex.cn

TS:   s.split("a").length - 1
来源：http://rr.shtwfgs.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rn.shtwfgs.cn

Go:   strings.Count(s, "a")
来源：http://kb.bjjhwx.cn

Ruby: s.count("a")
来源：http://zp.huixinmuqiang.cn

C#:   s.Count(c => c == 'a')
来源：http://lj.bookmarksfly.cn

[E13] 逐字符遍历
来源：http://pg.szxytkj.cn

Py:   for ch in s: print(ch)
来源：http://hz.colortex.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ch.gzmigu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://rf.chemitech.net.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://tl.nszjky.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wc.panjiajie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ra.haigaiapp.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://tf.newstarts.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fz.bookmarksfly.cn

[E14] URL 编码与 Base64
来源：http://on.shxzukj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ur.jianghongdianzi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://pg.huanxung.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fq.521024.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wj.lnxyls.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ud.shtwfgs.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tm.huanxung.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ur.shxzukj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yi.newstarts.cn

[E15] HTML 转义 / 反转义
来源：http://xd.nicolike.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://jc.huanxung.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zi.wgjwhj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wl.shxzskj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://fy.huixiangedu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xh.yuntaijiaju.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://lf.huixiangedu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rk.muxihuayi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vl.wgjwhj.cn

[E16] 数字千分位
来源：http://ur.shxzukj.cn

Py:   f"{1234567:,}"
来源：http://fg.yuexingan06.cn

PHP:  number_format(1234567);
来源：http://xv.huixiangedu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://nx.jianghongdianzi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://kq.shtwfgs.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://de.521024.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ck.huixiangedu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cu.shtwfgs.cn

C#:   1234567.ToString("N0")
来源：http://ih.9csxet.cn

[E17] 首字母大写
来源：http://mc.yuexingan06.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sq.huixiangedu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://dd.9csxet.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sl.jianghongdianzi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://of.colortex.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://al.521024.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pg.hnjuh.cn

Ruby: s.capitalize
来源：http://lk.shxzukj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hr.haigaiapp.cn

[E18] 模板占位符替换
来源：http://op.szxytkj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fj.nszjky.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vv.bookmarksfly.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://wm.shxzskj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://cz.colortex.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://se.haigaiapp.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wi.colortex.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vd.muxihuayi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xh.nszjky.cn

[E19] 多行文本按行拆分
来源：http://qz.nszjky.cn

Py:   s.splitlines()
来源：http://ps.9csxet.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ik.huanxung.cn

JS:   s.split(/\r?\n/)
来源：http://hn.9csxet.cn

TS:   s.split(/\r?\n/)
来源：http://mn.asd995.cn

Java: s.lines().toList()
来源：http://pk.yuntaijiaju.cn

Go:   strings.Split(s, "\n")
来源：http://im.521024.cn

Ruby: s.lines
来源：http://tz.wgjwhj.cn

C#:   s.Split('\n')
来源：http://wp.shxzukj.cn

[E20] 判断字符串是否为空
来源：http://ca.jctech888.com.cn

Py:   if not s:
来源：http://rn.shtwfgs.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://om.shxzukj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ol.huanxung.cn

TS:   if (s === "") {}
来源：http://un.muxihuayi.cn

Java: if (s.isEmpty()) {}
来源：http://tk.colortex.cn

Go:   if s == "" {}
来源：http://ip.newstarts.cn

Ruby: if s.empty?
来源：http://wy.colortex.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dl.nicolike.cn

[E21] 超长截断加省略号
来源：http://ik.bookmarksfly.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pq.colortex.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fm.haigaiapp.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://br.bookmarksfly.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gd.bookmarksfly.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bt.huixinmuqiang.cn

Go:   // 按 rune 判断长度后截断
来源：http://vj.huanxung.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nn.bookmarksfly.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xu.shtwfgs.cn

[E22] 字节长度与字符长度
来源：http://qo.huixiangedu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zv.bjjhwx.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jj.haigaiapp.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://te.chemitech.net.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pb.yuexingan06.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ig.huixiangedu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ku.haigaiapp.cn

Ruby: s.bytesize;  s.length
来源：http://jg.bookmarksfly.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hf.asd995.cn

================================================================================
来源：http://ot.chemitech.net.cn

F. 文件与目录
来源：http://ov.wgjwhj.cn

================================================================================
来源：http://gy.gzmigu.cn

[F01] 读取整个文件
来源：http://jm.bookmarksfly.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mc.lnxyls.cn

PHP:  file_get_contents("a.txt");
来源：http://zf.shxzukj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ri.jctech888.com.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ik.asd995.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://mb.colortex.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wb.nicolike.cn

Ruby: File.read("a.txt")
来源：http://ox.yuexingan06.cn


<!-- 参考信息 -->