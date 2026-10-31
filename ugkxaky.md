代发 wailian999

[D15] 去重
来源：http://ir.colortex.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ju.yuntaijiaju.cn

PHP:  array_unique($arr);
来源：http://hc.newstarts.cn

JS:   [...new Set(arr)]
来源：http://lf.yuexingan06.cn

TS:   [...new Set(arr)]
来源：http://qq.muxihuayi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ap.bjjhwx.cn

Go:   // 用 map[T]struct{} 手写
来源：http://jk.shxzukj.cn

Ruby: arr.uniq
来源：http://yy.huixiangedu.cn

C#:   list.Distinct().ToList()
来源：http://of.szsharing.cn

[D16] 求和与平均值
来源：http://od.haigaiapp.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ic.colortex.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mu.colortex.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rs.chemitech.net.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://uc.muxihuayi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kw.shtwfgs.cn

Go:   // 手写循环累加
来源：http://ht.bjjhwx.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ep.shxzskj.cn

C#:   list.Sum();  list.Average()
来源：http://jk.nicolike.cn

[D17] 最大值与最小值
来源：http://fk.bjjhwx.cn

Py:   max(arr);  min(arr)
来源：http://qe.521024.cn

PHP:  max($arr);  min($arr);
来源：http://au.chemitech.net.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fb.chemitech.net.cn

TS:   Math.max(...arr);
来源：http://eg.jctech888.com.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ob.shxzskj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yb.jctech888.com.cn

Ruby: arr.max;  arr.min
来源：http://lr.shtwfgs.cn

C#:   list.Max();  list.Min()
来源：http://mi.nicolike.cn

[D18] 扁平化嵌套数组
来源：http://ds.asd995.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dh.gzmigu.cn

PHP:  array_merge(...$nested);
来源：http://hu.newstarts.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hb.szxytkj.cn

TS:   nested.flat();
来源：http://zs.szsharing.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vb.newstarts.cn

Go:   // 手写双层循环
来源：http://oc.bjjhwx.cn

Ruby: nested.flatten
来源：http://sn.yuexingan06.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://gy.nicolike.cn

[D19] 按字段分组
来源：http://to.shxzukj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xj.yuexingan06.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wv.bjjhwx.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gk.jctech888.com.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://um.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qc.jctech888.com.cn

Go:   // 手写 map[string][]T
来源：http://re.jctech888.com.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ib.nicolike.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ez.huixinmuqiang.cn

[D20] 统计每个元素出现次数
来源：http://ir.huixiangedu.cn

Py:   Counter(arr)
来源：http://io.nicolike.cn

PHP:  array_count_values($arr);
来源：http://th.jianghongdianzi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gi.panjiajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ho.szsharing.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://sa.nicolike.cn

Go:   // 手写 map[T]int
来源：http://nu.szxytkj.cn

Ruby: arr.tally
来源：http://hb.newstarts.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bj.haigaiapp.cn

[D21] 判断是否包含某元素
来源：http://uj.yuexingan06.cn

Py:   x in arr
来源：http://qk.panjiajie.cn

PHP:  in_array($x, $arr, true);
来源：http://wr.colortex.cn

JS:   arr.includes(x)
来源：http://wc.shxzukj.cn

TS:   arr.includes(x)
来源：http://ui.gzmigu.cn

Java: list.contains(x)
来源：http://fa.newstarts.cn

Go:   slices.Contains(arr, x)
来源：http://bx.jianghongdianzi.cn

Ruby: arr.include?(x)
来源：http://fg.yuntaijiaju.cn

C#:   list.Contains(x)
来源：http://hd.bjjhwx.cn

[D22] 复制数组（避免共享引用）
来源：http://lf.521024.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qi.muxihuayi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cl.huanxung.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rb.9csxet.cn

TS:   [...arr];
来源：http://un.jianghongdianzi.cn

Java: new ArrayList<>(list);
来源：http://wt.nicolike.cn

Go:   copied := append([]int(nil), arr...)
来源：http://mw.huixinmuqiang.cn

Ruby: arr.dup;  arr.clone
来源：http://ck.szxytkj.cn

C#:   new List<int>(list);
来源：http://fv.nicolike.cn

[D23] reduce 累积计算
来源：http://te.chemitech.net.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ae.hahajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hq.asd995.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://id.gzmigu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://er.asd995.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qb.yuexingan06.cn

Go:   // 手写循环
来源：http://bq.shtwfgs.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wl.9csxet.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ok.shxzukj.cn

[D24] 字典 / Map 基本操作
来源：http://yf.hnjuh.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ln.9csxet.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gd.yuexingan06.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fy.huixinmuqiang.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://va.nszjky.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zu.huixinmuqiang.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yc.chemitech.net.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://sd.asd995.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pw.huanxung.cn

[D25] Set 集合去重与交并差
来源：http://tw.gzmigu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://eh.bookmarksfly.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pc.asd995.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xd.asd995.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vw.bookmarksfly.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://es.szsharing.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mu.haigaiapp.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gp.jianghongdianzi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hl.huixiangedu.cn

[D26] 数组转字符串
来源：http://rl.bjjhwx.cn

Py:   ", ".join(map(str, arr))
来源：http://at.colortex.cn

PHP:  implode(", ", $arr);
来源：http://gm.muxihuayi.cn

JS:   arr.join(", ")
来源：http://vl.huixiangedu.cn

TS:   arr.join(", ")
来源：http://dv.shxzukj.cn

Java: String.join(", ", list)
来源：http://mw.colortex.cn

Go:   strings.Join(strs, ", ")
来源：http://tz.bookmarksfly.cn

Ruby: arr.join(", ")
来源：http://zz.hnjuh.cn

C#:   string.Join(", ", list)
来源：http://ld.yuexingan06.cn

================================================================================
来源：http://to.shtwfgs.cn

E. 字符串处理
来源：http://hx.hnjuh.cn

================================================================================
来源：http://ts.521024.cn

[E01] 拼接字符串
来源：http://bx.shxzukj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ng.chemitech.net.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wi.huixinmuqiang.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://si.jianghongdianzi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ww.nicolike.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xk.muxihuayi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dy.jctech888.com.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sx.huanxung.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vq.newstarts.cn

[E02] 重复字符串
来源：http://jz.colortex.cn

Py:   "ab" * 3
来源：http://gr.asd995.cn

PHP:  str_repeat("ab", 3);
来源：http://vd.asd995.cn

JS:   "ab".repeat(3)
来源：http://cf.9csxet.cn

TS:   "ab".repeat(3)
来源：http://mv.jianghongdianzi.cn

Java: "ab".repeat(3)
来源：http://dx.nszjky.cn

Go:   strings.Repeat("ab", 3)
来源：http://ku.haigaiapp.cn

Ruby: "ab" * 3
来源：http://ec.szsharing.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yd.gzmigu.cn

[E03] 截取子串
来源：http://fz.wgjwhj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://oh.szxytkj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nh.chemitech.net.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bo.lnxyls.cn

TS:   s.slice(1, 4)
来源：http://gg.521024.cn

Java: s.substring(1, 4)
来源：http://sk.hnjuh.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kz.huixiangedu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://tm.huixinmuqiang.cn

C#:   s.Substring(1, 3)
来源：http://tv.yuexingan06.cn

[E04] 查找子串位置
来源：http://kl.nszjky.cn

Py:   s.find("x");  s.index("x")
来源：http://xm.haigaiapp.cn

PHP:  strpos($s, "x");
来源：http://zp.szxytkj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gp.szsharing.cn

TS:   s.indexOf("x")
来源：http://wx.bjjhwx.cn

Java: s.indexOf("x")
来源：http://ub.colortex.cn

Go:   strings.Index(s, "x")
来源：http://ea.colortex.cn

Ruby: s.index("x")
来源：http://os.lnxyls.cn

C#:   s.IndexOf("x")
来源：http://ht.lnxyls.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://hf.521024.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://to.shxzukj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nz.szxytkj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dh.shtwfgs.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://tp.colortex.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ub.yuntaijiaju.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cu.huixinmuqiang.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hq.yuntaijiaju.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://oi.huixiangedu.cn

[E06] 替换子串
来源：http://mw.hahajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://oz.hnjuh.cn

PHP:  str_replace("a", "b", $s);
来源：http://el.521024.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qu.huixiangedu.cn

TS:   s.replaceAll("a", "b")
来源：http://ko.gzmigu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kk.colortex.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://go.521024.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nq.colortex.cn

C#:   s.Replace("a", "b")
来源：http://rk.chemitech.net.cn

[E07] 按分隔符拆分
来源：http://vy.hnjuh.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jw.jctech888.com.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ef.gzmigu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://sg.hahajie.cn

TS:   s.split(",")
来源：http://le.nszjky.cn

Java: s.split(",");  s.split("\\s+")
来源：http://kb.yuexingan06.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qm.nicolike.cn

Ruby: s.split(",");  s.split
来源：http://ik.hnjuh.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zo.newstarts.cn

[E08] 数组按分隔符合并
来源：http://nq.huixiangedu.cn

Py:   ",".join(items)
来源：http://wy.wgjwhj.cn

PHP:  implode(",", $items);
来源：http://zg.521024.cn

JS:   items.join(",")
来源：http://tv.szsharing.cn

TS:   items.join(",")
来源：http://pz.nszjky.cn

Java: String.join(",", items)
来源：http://lj.521024.cn

Go:   strings.Join(items, ",")
来源：http://yf.shxzukj.cn

Ruby: items.join(",")
来源：http://rp.huanxung.cn

C#:   string.Join(",", items)
来源：http://be.wgjwhj.cn

[E09] 去除所有空白字符
来源：http://ya.szsharing.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mo.521024.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fa.gzmigu.cn

JS:   s.replace(/\s+/g, "")
来源：http://vb.newstarts.cn

TS:   s.replace(/\s+/g, "")
来源：http://ke.huanxung.cn

Java: s.replaceAll("\\s+", "")
来源：http://pc.nszjky.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://of.yuexingan06.cn

Ruby: s.gsub(/\s+/, "")
来源：http://nk.bookmarksfly.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gv.nicolike.cn

[E10] 左侧补零 / 定长填充
来源：http://lq.shtwfgs.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jc.chemitech.net.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wu.shtwfgs.cn

JS:   "7".padStart(3, "0")
来源：http://gs.hahajie.cn

TS:   "7".padStart(3, "0")
来源：http://nv.9csxet.cn

Java: String.format("%03d", 7)
来源：http://ae.nszjky.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://wy.521024.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hb.bookmarksfly.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://da.haigaiapp.cn

[E11] 反转字符串
来源：http://gq.huixiangedu.cn

Py:   s[::-1]
来源：http://le.shtwfgs.cn

PHP:  strrev($s);
来源：http://in.huixiangedu.cn

JS:   [...s].reverse().join("")
来源：http://ie.nszjky.cn

TS:   [...s].reverse().join("")
来源：http://bz.nszjky.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ft.jctech888.com.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://wi.wgjwhj.cn

Ruby: s.reverse
来源：http://yi.panjiajie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://gu.shtwfgs.cn

[E12] 统计某字符出现次数
来源：http://gy.nszjky.cn

Py:   s.count("a")
来源：http://zs.yuexingan06.cn

PHP:  substr_count($s, "a");
来源：http://ed.jctech888.com.cn

JS:   s.split("a").length - 1
来源：http://dq.chemitech.net.cn

TS:   s.split("a").length - 1
来源：http://it.jianghongdianzi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://su.asd995.cn

Go:   strings.Count(s, "a")
来源：http://rv.huixiangedu.cn

Ruby: s.count("a")
来源：http://cm.jctech888.com.cn

C#:   s.Count(c => c == 'a')
来源：http://ki.521024.cn

[E13] 逐字符遍历
来源：http://hw.gzmigu.cn

Py:   for ch in s: print(ch)
来源：http://oq.szxytkj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sw.521024.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://us.huanxung.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://pi.lnxyls.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hi.newstarts.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yo.szxytkj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ft.yuexingan06.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ld.hnjuh.cn

[E14] URL 编码与 Base64
来源：http://hd.colortex.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mv.521024.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://sb.nicolike.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ys.szxytkj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://km.haigaiapp.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ge.szxytkj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://id.jianghongdianzi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ey.bookmarksfly.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gb.newstarts.cn

[E15] HTML 转义 / 反转义
来源：http://lr.nicolike.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://fa.yuntaijiaju.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zw.muxihuayi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ah.huanxung.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://md.yuexingan06.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://am.colortex.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sr.chemitech.net.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qt.nicolike.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mk.nicolike.cn

[E16] 数字千分位
来源：http://ix.yuntaijiaju.cn

Py:   f"{1234567:,}"
来源：http://jg.colortex.cn

PHP:  number_format(1234567);
来源：http://rs.haigaiapp.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://td.gzmigu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://sm.panjiajie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fu.jctech888.com.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qv.colortex.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lf.shxzskj.cn

C#:   1234567.ToString("N0")
来源：http://vq.huixinmuqiang.cn

[E17] 首字母大写
来源：http://ab.521024.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hp.shxzukj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://vh.521024.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hk.shxzukj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pr.yuntaijiaju.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dc.colortex.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xo.521024.cn

Ruby: s.capitalize
来源：http://cy.9csxet.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://et.chemitech.net.cn

[E18] 模板占位符替换
来源：http://mx.hahajie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kt.newstarts.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lq.chemitech.net.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://cp.colortex.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://tl.lnxyls.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pi.szsharing.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ne.9csxet.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ai.shxzukj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gc.chemitech.net.cn

[E19] 多行文本按行拆分
来源：http://di.panjiajie.cn

Py:   s.splitlines()
来源：http://pr.yuntaijiaju.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vx.newstarts.cn

JS:   s.split(/\r?\n/)
来源：http://vw.jctech888.com.cn

TS:   s.split(/\r?\n/)
来源：http://bc.shtwfgs.cn

Java: s.lines().toList()
来源：http://wy.huanxung.cn

Go:   strings.Split(s, "\n")
来源：http://xr.shtwfgs.cn

Ruby: s.lines
来源：http://js.colortex.cn

C#:   s.Split('\n')
来源：http://le.shxzukj.cn

[E20] 判断字符串是否为空
来源：http://rm.hnjuh.cn

Py:   if not s:
来源：http://cj.yuexingan06.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ib.panjiajie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://am.nszjky.cn

TS:   if (s === "") {}
来源：http://ou.shxzskj.cn

Java: if (s.isEmpty()) {}
来源：http://kb.gzmigu.cn

Go:   if s == "" {}
来源：http://ca.nicolike.cn

Ruby: if s.empty?
来源：http://ow.521024.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zq.muxihuayi.cn

[E21] 超长截断加省略号
来源：http://uj.huixiangedu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hp.bookmarksfly.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tw.bjjhwx.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wm.szxytkj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mx.shxzukj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://no.shxzukj.cn

Go:   // 按 rune 判断长度后截断
来源：http://sr.9csxet.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wc.chemitech.net.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mw.newstarts.cn


<!-- 参考信息 -->