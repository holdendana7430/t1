代发 wailian999

C#:   list.Distinct().ToList()
来源：http://lk.jianghongdianzi.cn

[D16] 求和与平均值
来源：http://pf.hnjuh.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://cq.chemitech.net.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rc.panjiajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ce.szxytkj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ve.muxihuayi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qt.521024.cn

Go:   // 手写循环累加
来源：http://yv.panjiajie.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hq.hnjuh.cn

C#:   list.Sum();  list.Average()
来源：http://cx.panjiajie.cn

[D17] 最大值与最小值
来源：http://zk.newstarts.cn

Py:   max(arr);  min(arr)
来源：http://kj.yuexingan06.cn

PHP:  max($arr);  min($arr);
来源：http://mw.gzmigu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ln.colortex.cn

TS:   Math.max(...arr);
来源：http://zj.chemitech.net.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://nj.hnjuh.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cd.lnxyls.cn

Ruby: arr.max;  arr.min
来源：http://pd.wgjwhj.cn

C#:   list.Max();  list.Min()
来源：http://zl.huixinmuqiang.cn

[D18] 扁平化嵌套数组
来源：http://ai.yuntaijiaju.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://do.panjiajie.cn

PHP:  array_merge(...$nested);
来源：http://kf.nszjky.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ut.huanxung.cn

TS:   nested.flat();
来源：http://te.9csxet.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qh.9csxet.cn

Go:   // 手写双层循环
来源：http://st.nicolike.cn

Ruby: nested.flatten
来源：http://eo.bookmarksfly.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ah.gzmigu.cn

[D19] 按字段分组
来源：http://ha.gzmigu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ho.huixiangedu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mo.9csxet.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zx.panjiajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://sn.wgjwhj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dq.nicolike.cn

Go:   // 手写 map[string][]T
来源：http://ge.colortex.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://gr.szxytkj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pu.521024.cn

[D20] 统计每个元素出现次数
来源：http://lg.szxytkj.cn

Py:   Counter(arr)
来源：http://ub.9csxet.cn

PHP:  array_count_values($arr);
来源：http://ha.newstarts.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ns.bjjhwx.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gs.huixinmuqiang.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://op.asd995.cn

Go:   // 手写 map[T]int
来源：http://nf.newstarts.cn

Ruby: arr.tally
来源：http://gg.yuexingan06.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sl.haigaiapp.cn

[D21] 判断是否包含某元素
来源：http://fp.szxytkj.cn

Py:   x in arr
来源：http://su.nicolike.cn

PHP:  in_array($x, $arr, true);
来源：http://zj.panjiajie.cn

JS:   arr.includes(x)
来源：http://cg.shtwfgs.cn

TS:   arr.includes(x)
来源：http://fz.szxytkj.cn

Java: list.contains(x)
来源：http://gz.panjiajie.cn

Go:   slices.Contains(arr, x)
来源：http://vm.shtwfgs.cn

Ruby: arr.include?(x)
来源：http://ge.hahajie.cn

C#:   list.Contains(x)
来源：http://xg.panjiajie.cn

[D22] 复制数组（避免共享引用）
来源：http://rf.yuexingan06.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yb.shtwfgs.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hu.bjjhwx.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nq.newstarts.cn

TS:   [...arr];
来源：http://ay.shxzukj.cn

Java: new ArrayList<>(list);
来源：http://ad.yuexingan06.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ld.wgjwhj.cn

Ruby: arr.dup;  arr.clone
来源：http://hw.yuexingan06.cn

C#:   new List<int>(list);
来源：http://mt.nszjky.cn

[D23] reduce 累积计算
来源：http://oh.muxihuayi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ln.muxihuayi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tg.yuexingan06.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ox.bookmarksfly.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://si.bookmarksfly.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://yb.panjiajie.cn

Go:   // 手写循环
来源：http://th.wgjwhj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hl.szxytkj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lz.nszjky.cn

[D24] 字典 / Map 基本操作
来源：http://nc.wgjwhj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xj.huixiangedu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ir.muxihuayi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jb.yuexingan06.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pd.jctech888.com.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bj.newstarts.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wd.szxytkj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tg.9csxet.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://to.bjjhwx.cn

[D25] Set 集合去重与交并差
来源：http://mj.521024.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ar.hahajie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ld.bookmarksfly.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pm.huixiangedu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rl.521024.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zh.newstarts.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dj.shxzskj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hy.huanxung.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ki.panjiajie.cn

[D26] 数组转字符串
来源：http://dt.nicolike.cn

Py:   ", ".join(map(str, arr))
来源：http://df.panjiajie.cn

PHP:  implode(", ", $arr);
来源：http://yr.wgjwhj.cn

JS:   arr.join(", ")
来源：http://sn.nicolike.cn

TS:   arr.join(", ")
来源：http://mc.yuexingan06.cn

Java: String.join(", ", list)
来源：http://vt.shxzukj.cn

Go:   strings.Join(strs, ", ")
来源：http://tu.521024.cn

Ruby: arr.join(", ")
来源：http://hd.haigaiapp.cn

C#:   string.Join(", ", list)
来源：http://iy.jctech888.com.cn

================================================================================
来源：http://ew.shxzskj.cn

E. 字符串处理
来源：http://oz.yuexingan06.cn

================================================================================
来源：http://cc.bookmarksfly.cn

[E01] 拼接字符串
来源：http://wl.nicolike.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dg.huixiangedu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sp.szxytkj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qm.yuntaijiaju.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xj.colortex.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zk.jctech888.com.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dw.hahajie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lo.muxihuayi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sk.szxytkj.cn

[E02] 重复字符串
来源：http://gi.chemitech.net.cn

Py:   "ab" * 3
来源：http://rh.nicolike.cn

PHP:  str_repeat("ab", 3);
来源：http://lu.nicolike.cn

JS:   "ab".repeat(3)
来源：http://cx.szxytkj.cn

TS:   "ab".repeat(3)
来源：http://wu.lnxyls.cn

Java: "ab".repeat(3)
来源：http://do.lnxyls.cn

Go:   strings.Repeat("ab", 3)
来源：http://rf.lnxyls.cn

Ruby: "ab" * 3
来源：http://ou.huixiangedu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qk.9csxet.cn

[E03] 截取子串
来源：http://bl.shtwfgs.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fq.lnxyls.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nz.huixiangedu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ec.wgjwhj.cn

TS:   s.slice(1, 4)
来源：http://xp.nicolike.cn

Java: s.substring(1, 4)
来源：http://mo.shxzskj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yk.chemitech.net.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mp.asd995.cn

C#:   s.Substring(1, 3)
来源：http://uf.wgjwhj.cn

[E04] 查找子串位置
来源：http://wt.colortex.cn

Py:   s.find("x");  s.index("x")
来源：http://fk.muxihuayi.cn

PHP:  strpos($s, "x");
来源：http://dt.chemitech.net.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://le.muxihuayi.cn

TS:   s.indexOf("x")
来源：http://rb.newstarts.cn

Java: s.indexOf("x")
来源：http://es.huanxung.cn

Go:   strings.Index(s, "x")
来源：http://oo.jctech888.com.cn

Ruby: s.index("x")
来源：http://dh.yuntaijiaju.cn

C#:   s.IndexOf("x")
来源：http://am.nicolike.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://yg.521024.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hm.gzmigu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xj.shxzskj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qr.shxzskj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://pc.shxzskj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hi.yuntaijiaju.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://le.huixinmuqiang.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://la.muxihuayi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qy.panjiajie.cn

[E06] 替换子串
来源：http://ig.panjiajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mv.nicolike.cn

PHP:  str_replace("a", "b", $s);
来源：http://kf.panjiajie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://md.yuntaijiaju.cn

TS:   s.replaceAll("a", "b")
来源：http://my.bookmarksfly.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://or.huixiangedu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cd.jctech888.com.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ao.szsharing.cn

C#:   s.Replace("a", "b")
来源：http://iv.bjjhwx.cn

[E07] 按分隔符拆分
来源：http://py.chemitech.net.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wn.hnjuh.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ji.asd995.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://cn.haigaiapp.cn

TS:   s.split(",")
来源：http://yg.yuexingan06.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ko.jianghongdianzi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ch.bjjhwx.cn

Ruby: s.split(",");  s.split
来源：http://wz.huixiangedu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jo.lnxyls.cn

[E08] 数组按分隔符合并
来源：http://qz.bookmarksfly.cn

Py:   ",".join(items)
来源：http://xh.asd995.cn

PHP:  implode(",", $items);
来源：http://xc.hnjuh.cn

JS:   items.join(",")
来源：http://xd.yuntaijiaju.cn

TS:   items.join(",")
来源：http://kf.haigaiapp.cn

Java: String.join(",", items)
来源：http://yz.bjjhwx.cn

Go:   strings.Join(items, ",")
来源：http://sj.bjjhwx.cn

Ruby: items.join(",")
来源：http://ux.lnxyls.cn

C#:   string.Join(",", items)
来源：http://kj.lnxyls.cn

[E09] 去除所有空白字符
来源：http://lk.asd995.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bo.muxihuayi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kj.huixiangedu.cn

JS:   s.replace(/\s+/g, "")
来源：http://th.huixiangedu.cn

TS:   s.replace(/\s+/g, "")
来源：http://gh.9csxet.cn

Java: s.replaceAll("\\s+", "")
来源：http://zl.shxzukj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://zi.huixiangedu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://de.panjiajie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tc.wgjwhj.cn

[E10] 左侧补零 / 定长填充
来源：http://an.lnxyls.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ke.newstarts.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://th.nszjky.cn

JS:   "7".padStart(3, "0")
来源：http://hc.colortex.cn

TS:   "7".padStart(3, "0")
来源：http://cw.szxytkj.cn

Java: String.format("%03d", 7)
来源：http://xw.szsharing.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://oy.szsharing.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jp.hahajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ei.shtwfgs.cn

[E11] 反转字符串
来源：http://ql.jctech888.com.cn

Py:   s[::-1]
来源：http://xo.bjjhwx.cn

PHP:  strrev($s);
来源：http://od.nicolike.cn

JS:   [...s].reverse().join("")
来源：http://yj.muxihuayi.cn

TS:   [...s].reverse().join("")
来源：http://dy.huixinmuqiang.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://td.asd995.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://sg.colortex.cn

Ruby: s.reverse
来源：http://sh.asd995.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ux.521024.cn

[E12] 统计某字符出现次数
来源：http://xf.huanxung.cn

Py:   s.count("a")
来源：http://ww.yuexingan06.cn

PHP:  substr_count($s, "a");
来源：http://hm.nicolike.cn

JS:   s.split("a").length - 1
来源：http://rl.shxzskj.cn

TS:   s.split("a").length - 1
来源：http://yl.chemitech.net.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://za.hnjuh.cn

Go:   strings.Count(s, "a")
来源：http://ne.haigaiapp.cn

Ruby: s.count("a")
来源：http://dh.hahajie.cn

C#:   s.Count(c => c == 'a')
来源：http://et.szsharing.cn

[E13] 逐字符遍历
来源：http://sd.newstarts.cn

Py:   for ch in s: print(ch)
来源：http://me.hahajie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vk.shxzukj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://bo.jianghongdianzi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wa.huanxung.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rt.huixiangedu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gc.newstarts.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://de.hahajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rx.wgjwhj.cn

[E14] URL 编码与 Base64
来源：http://vp.szsharing.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hr.521024.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://dn.huanxung.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vy.szxytkj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sg.gzmigu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ie.shxzukj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://of.szsharing.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://js.szxytkj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tp.lnxyls.cn

[E15] HTML 转义 / 反转义
来源：http://pf.newstarts.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ce.hnjuh.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tl.bookmarksfly.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bd.haigaiapp.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://rr.shxzukj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fp.jianghongdianzi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jy.asd995.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jd.huixinmuqiang.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ae.huanxung.cn

[E16] 数字千分位
来源：http://fx.huanxung.cn

Py:   f"{1234567:,}"
来源：http://kl.hnjuh.cn

PHP:  number_format(1234567);
来源：http://bd.bookmarksfly.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://zz.chemitech.net.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ly.szxytkj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dw.huixinmuqiang.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bs.colortex.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dy.haigaiapp.cn

C#:   1234567.ToString("N0")
来源：http://aw.gzmigu.cn

[E17] 首字母大写
来源：http://mo.jianghongdianzi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ao.shtwfgs.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://tw.bjjhwx.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://de.yuexingan06.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dz.szsharing.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xm.muxihuayi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kq.nszjky.cn

Ruby: s.capitalize
来源：http://ty.bookmarksfly.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://sq.huixiangedu.cn

[E18] 模板占位符替换
来源：http://rx.szsharing.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gd.shxzskj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nw.nszjky.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zo.hnjuh.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://bg.lnxyls.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zo.wgjwhj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wl.haigaiapp.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://oo.asd995.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kr.huixiangedu.cn

[E19] 多行文本按行拆分
来源：http://cl.jctech888.com.cn

Py:   s.splitlines()
来源：http://zm.yuexingan06.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hx.hahajie.cn

JS:   s.split(/\r?\n/)
来源：http://ox.shxzukj.cn

TS:   s.split(/\r?\n/)
来源：http://cy.shxzukj.cn

Java: s.lines().toList()
来源：http://oj.hnjuh.cn

Go:   strings.Split(s, "\n")
来源：http://dw.huixiangedu.cn

Ruby: s.lines
来源：http://im.asd995.cn

C#:   s.Split('\n')
来源：http://bm.szxytkj.cn

[E20] 判断字符串是否为空
来源：http://te.nicolike.cn

Py:   if not s:
来源：http://ef.lnxyls.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mj.shtwfgs.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yn.colortex.cn

TS:   if (s === "") {}
来源：http://oz.521024.cn

Java: if (s.isEmpty()) {}
来源：http://iz.nszjky.cn

Go:   if s == "" {}
来源：http://vt.colortex.cn

Ruby: if s.empty?
来源：http://jz.szsharing.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://no.huanxung.cn

[E21] 超长截断加省略号
来源：http://ny.lnxyls.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ut.jianghongdianzi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ff.lnxyls.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ga.lnxyls.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xd.jctech888.com.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wu.jianghongdianzi.cn

Go:   // 按 rune 判断长度后截断
来源：http://bq.asd995.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sm.bjjhwx.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tp.nicolike.cn

[E22] 字节长度与字符长度
来源：http://vl.yuexingan06.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tr.jianghongdianzi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pp.wgjwhj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://la.yuexingan06.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cf.bookmarksfly.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jk.panjiajie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ex.muxihuayi.cn

Ruby: s.bytesize;  s.length
来源：http://ao.gzmigu.cn


<!-- 参考信息 -->