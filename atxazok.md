代发 wailian999

TS:   [...new Set(arr)]
来源：http://wd.muxihuayi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ly.gzmigu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://iq.hnjuh.cn

Ruby: arr.uniq
来源：http://tu.panjiajie.cn

C#:   list.Distinct().ToList()
来源：http://oj.shxzskj.cn

[D16] 求和与平均值
来源：http://oy.muxihuayi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://as.lnxyls.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://um.asd995.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fo.wgjwhj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pc.shxzukj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yq.colortex.cn

Go:   // 手写循环累加
来源：http://du.newstarts.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fl.9csxet.cn

C#:   list.Sum();  list.Average()
来源：http://ey.lnxyls.cn

[D17] 最大值与最小值
来源：http://lc.hnjuh.cn

Py:   max(arr);  min(arr)
来源：http://bd.chemitech.net.cn

PHP:  max($arr);  min($arr);
来源：http://ph.panjiajie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nc.shxzukj.cn

TS:   Math.max(...arr);
来源：http://op.asd995.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://fv.huanxung.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xd.hahajie.cn

Ruby: arr.max;  arr.min
来源：http://ym.9csxet.cn

C#:   list.Max();  list.Min()
来源：http://ow.9csxet.cn

[D18] 扁平化嵌套数组
来源：http://qi.jctech888.com.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pz.nszjky.cn

PHP:  array_merge(...$nested);
来源：http://pv.521024.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gl.9csxet.cn

TS:   nested.flat();
来源：http://bw.nszjky.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fu.yuntaijiaju.cn

Go:   // 手写双层循环
来源：http://xs.panjiajie.cn

Ruby: nested.flatten
来源：http://ur.jianghongdianzi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://rn.wgjwhj.cn

[D19] 按字段分组
来源：http://kw.colortex.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nv.jianghongdianzi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://su.yuexingan06.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rf.9csxet.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qs.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wy.wgjwhj.cn

Go:   // 手写 map[string][]T
来源：http://dk.szsharing.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://gq.shtwfgs.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://de.9csxet.cn

[D20] 统计每个元素出现次数
来源：http://ru.9csxet.cn

Py:   Counter(arr)
来源：http://zd.panjiajie.cn

PHP:  array_count_values($arr);
来源：http://ra.huanxung.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://er.bjjhwx.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wc.huixiangedu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zq.haigaiapp.cn

Go:   // 手写 map[T]int
来源：http://ts.lnxyls.cn

Ruby: arr.tally
来源：http://sa.jctech888.com.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://il.chemitech.net.cn

[D21] 判断是否包含某元素
来源：http://ts.hnjuh.cn

Py:   x in arr
来源：http://hl.hahajie.cn

PHP:  in_array($x, $arr, true);
来源：http://uf.panjiajie.cn

JS:   arr.includes(x)
来源：http://dj.yuntaijiaju.cn

TS:   arr.includes(x)
来源：http://ti.haigaiapp.cn

Java: list.contains(x)
来源：http://nq.szsharing.cn

Go:   slices.Contains(arr, x)
来源：http://cu.huixinmuqiang.cn

Ruby: arr.include?(x)
来源：http://ui.nicolike.cn

C#:   list.Contains(x)
来源：http://ns.wgjwhj.cn

[D22] 复制数组（避免共享引用）
来源：http://cb.jctech888.com.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://oa.hahajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qz.bookmarksfly.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://os.bookmarksfly.cn

TS:   [...arr];
来源：http://um.huixiangedu.cn

Java: new ArrayList<>(list);
来源：http://qv.jianghongdianzi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://hz.wgjwhj.cn

Ruby: arr.dup;  arr.clone
来源：http://co.chemitech.net.cn

C#:   new List<int>(list);
来源：http://os.jianghongdianzi.cn

[D23] reduce 累积计算
来源：http://xz.lnxyls.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tm.shxzskj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cr.yuexingan06.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ri.yuexingan06.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xa.panjiajie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qm.bjjhwx.cn

Go:   // 手写循环
来源：http://gi.jianghongdianzi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fc.chemitech.net.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://iu.huixiangedu.cn

[D24] 字典 / Map 基本操作
来源：http://ps.szsharing.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ej.jianghongdianzi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rk.nicolike.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hr.haigaiapp.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://eq.newstarts.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zg.jctech888.com.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mv.shtwfgs.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xa.haigaiapp.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://da.huixiangedu.cn

[D25] Set 集合去重与交并差
来源：http://by.bookmarksfly.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://en.9csxet.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lu.colortex.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bf.yuexingan06.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jo.szxytkj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sq.muxihuayi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ze.chemitech.net.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uy.nicolike.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vs.jctech888.com.cn

[D26] 数组转字符串
来源：http://ly.shxzskj.cn

Py:   ", ".join(map(str, arr))
来源：http://xa.colortex.cn

PHP:  implode(", ", $arr);
来源：http://sw.wgjwhj.cn

JS:   arr.join(", ")
来源：http://vh.szsharing.cn

TS:   arr.join(", ")
来源：http://hj.gzmigu.cn

Java: String.join(", ", list)
来源：http://jo.9csxet.cn

Go:   strings.Join(strs, ", ")
来源：http://kt.nszjky.cn

Ruby: arr.join(", ")
来源：http://hp.shtwfgs.cn

C#:   string.Join(", ", list)
来源：http://jx.shtwfgs.cn

================================================================================
来源：http://gf.huixinmuqiang.cn

E. 字符串处理
来源：http://ml.shxzukj.cn

================================================================================
来源：http://fb.9csxet.cn

[E01] 拼接字符串
来源：http://if.hahajie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vn.521024.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ac.shxzskj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://so.gzmigu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fz.huixinmuqiang.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lj.muxihuayi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vw.yuntaijiaju.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hw.bookmarksfly.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ms.huixinmuqiang.cn

[E02] 重复字符串
来源：http://ly.huanxung.cn

Py:   "ab" * 3
来源：http://uu.muxihuayi.cn

PHP:  str_repeat("ab", 3);
来源：http://rc.yuexingan06.cn

JS:   "ab".repeat(3)
来源：http://ql.yuexingan06.cn

TS:   "ab".repeat(3)
来源：http://ee.shxzskj.cn

Java: "ab".repeat(3)
来源：http://lz.panjiajie.cn

Go:   strings.Repeat("ab", 3)
来源：http://yp.shxzskj.cn

Ruby: "ab" * 3
来源：http://xl.hahajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://io.521024.cn

[E03] 截取子串
来源：http://iu.yuexingan06.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pp.shxzskj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ug.shxzskj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bl.jctech888.com.cn

TS:   s.slice(1, 4)
来源：http://me.huixinmuqiang.cn

Java: s.substring(1, 4)
来源：http://st.bookmarksfly.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wx.nicolike.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ei.yuntaijiaju.cn

C#:   s.Substring(1, 3)
来源：http://cj.nszjky.cn

[E04] 查找子串位置
来源：http://gl.shxzukj.cn

Py:   s.find("x");  s.index("x")
来源：http://og.szxytkj.cn

PHP:  strpos($s, "x");
来源：http://ax.nicolike.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jv.colortex.cn

TS:   s.indexOf("x")
来源：http://oo.nicolike.cn

Java: s.indexOf("x")
来源：http://jh.huanxung.cn

Go:   strings.Index(s, "x")
来源：http://hd.huanxung.cn

Ruby: s.index("x")
来源：http://ba.hahajie.cn

C#:   s.IndexOf("x")
来源：http://mn.hahajie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://fn.newstarts.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bg.bjjhwx.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dt.szsharing.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bx.hnjuh.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://uw.szxytkj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kk.bookmarksfly.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://np.bjjhwx.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jp.521024.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bi.colortex.cn

[E06] 替换子串
来源：http://ac.gzmigu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nk.bookmarksfly.cn

PHP:  str_replace("a", "b", $s);
来源：http://fx.huanxung.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wp.shxzukj.cn

TS:   s.replaceAll("a", "b")
来源：http://bv.nszjky.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mz.9csxet.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ru.yuexingan06.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://np.jctech888.com.cn

C#:   s.Replace("a", "b")
来源：http://dm.yuexingan06.cn

[E07] 按分隔符拆分
来源：http://pc.huanxung.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://iv.hahajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wc.shtwfgs.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ps.colortex.cn

TS:   s.split(",")
来源：http://do.nicolike.cn

Java: s.split(",");  s.split("\\s+")
来源：http://sk.9csxet.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://di.panjiajie.cn

Ruby: s.split(",");  s.split
来源：http://xv.szxytkj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rs.muxihuayi.cn

[E08] 数组按分隔符合并
来源：http://al.panjiajie.cn

Py:   ",".join(items)
来源：http://ya.shtwfgs.cn

PHP:  implode(",", $items);
来源：http://hu.gzmigu.cn

JS:   items.join(",")
来源：http://jz.shxzskj.cn

TS:   items.join(",")
来源：http://qg.gzmigu.cn

Java: String.join(",", items)
来源：http://jg.9csxet.cn

Go:   strings.Join(items, ",")
来源：http://xi.jctech888.com.cn

Ruby: items.join(",")
来源：http://cw.jianghongdianzi.cn

C#:   string.Join(",", items)
来源：http://hx.muxihuayi.cn

[E09] 去除所有空白字符
来源：http://iz.nicolike.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://iq.panjiajie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yl.haigaiapp.cn

JS:   s.replace(/\s+/g, "")
来源：http://pl.bookmarksfly.cn

TS:   s.replace(/\s+/g, "")
来源：http://ax.lnxyls.cn

Java: s.replaceAll("\\s+", "")
来源：http://qp.haigaiapp.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ok.yuexingan06.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xx.colortex.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gv.hnjuh.cn

[E10] 左侧补零 / 定长填充
来源：http://il.huixinmuqiang.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://sz.panjiajie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nd.jctech888.com.cn

JS:   "7".padStart(3, "0")
来源：http://ub.jctech888.com.cn

TS:   "7".padStart(3, "0")
来源：http://px.shtwfgs.cn

Java: String.format("%03d", 7)
来源：http://hy.hahajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://at.chemitech.net.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gq.szsharing.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jo.9csxet.cn

[E11] 反转字符串
来源：http://ol.bookmarksfly.cn

Py:   s[::-1]
来源：http://qd.haigaiapp.cn

PHP:  strrev($s);
来源：http://gb.muxihuayi.cn

JS:   [...s].reverse().join("")
来源：http://tk.shxzukj.cn

TS:   [...s].reverse().join("")
来源：http://rm.szsharing.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://gn.szxytkj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://jd.9csxet.cn

Ruby: s.reverse
来源：http://ga.shtwfgs.cn

C#:   new string(s.Reverse().ToArray())
来源：http://fb.huixiangedu.cn

[E12] 统计某字符出现次数
来源：http://rw.shtwfgs.cn

Py:   s.count("a")
来源：http://ri.shxzskj.cn

PHP:  substr_count($s, "a");
来源：http://tf.521024.cn

JS:   s.split("a").length - 1
来源：http://yn.shtwfgs.cn

TS:   s.split("a").length - 1
来源：http://rp.hahajie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zx.jctech888.com.cn

Go:   strings.Count(s, "a")
来源：http://zs.wgjwhj.cn

Ruby: s.count("a")
来源：http://nb.jianghongdianzi.cn

C#:   s.Count(c => c == 'a')
来源：http://fu.asd995.cn

[E13] 逐字符遍历
来源：http://ry.colortex.cn

Py:   for ch in s: print(ch)
来源：http://xw.colortex.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ua.chemitech.net.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://nz.bookmarksfly.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ca.shxzukj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mv.huanxung.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ql.hahajie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ln.9csxet.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fm.huixiangedu.cn

[E14] URL 编码与 Base64
来源：http://lc.yuntaijiaju.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ne.shxzukj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://kb.newstarts.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zz.bookmarksfly.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://af.szsharing.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vr.nicolike.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gw.huanxung.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pb.nicolike.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mg.521024.cn

[E15] HTML 转义 / 反转义
来源：http://xw.asd995.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xv.bookmarksfly.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ah.jianghongdianzi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jm.shxzskj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://bz.szxytkj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fg.gzmigu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dn.chemitech.net.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lh.521024.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zh.asd995.cn

[E16] 数字千分位
来源：http://jq.nicolike.cn

Py:   f"{1234567:,}"
来源：http://iq.9csxet.cn

PHP:  number_format(1234567);
来源：http://gp.jctech888.com.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://yr.shtwfgs.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zl.yuntaijiaju.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sw.yuntaijiaju.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ck.9csxet.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fx.shtwfgs.cn

C#:   1234567.ToString("N0")
来源：http://ke.yuntaijiaju.cn

[E17] 首字母大写
来源：http://ly.asd995.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ak.shxzskj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://at.huixiangedu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vs.nszjky.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rx.newstarts.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vq.521024.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rj.yuntaijiaju.cn

Ruby: s.capitalize
来源：http://yw.9csxet.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mc.newstarts.cn

[E18] 模板占位符替换
来源：http://oz.yuntaijiaju.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xi.huixinmuqiang.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xl.jianghongdianzi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://yz.nicolike.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://jp.muxihuayi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nb.jctech888.com.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mo.shxzskj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fw.lnxyls.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mk.szxytkj.cn

[E19] 多行文本按行拆分
来源：http://kd.panjiajie.cn

Py:   s.splitlines()
来源：http://hy.huixinmuqiang.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sj.huixiangedu.cn

JS:   s.split(/\r?\n/)
来源：http://om.panjiajie.cn

TS:   s.split(/\r?\n/)
来源：http://ao.nszjky.cn

Java: s.lines().toList()
来源：http://lz.huanxung.cn

Go:   strings.Split(s, "\n")
来源：http://bz.nszjky.cn

Ruby: s.lines
来源：http://xa.gzmigu.cn

C#:   s.Split('\n')
来源：http://qf.huixinmuqiang.cn

[E20] 判断字符串是否为空
来源：http://ld.jctech888.com.cn

Py:   if not s:
来源：http://up.shtwfgs.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yg.shtwfgs.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rp.yuntaijiaju.cn

TS:   if (s === "") {}
来源：http://ut.nicolike.cn

Java: if (s.isEmpty()) {}
来源：http://ft.asd995.cn

Go:   if s == "" {}
来源：http://zn.shtwfgs.cn

Ruby: if s.empty?
来源：http://wn.panjiajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vk.nicolike.cn

[E21] 超长截断加省略号
来源：http://ts.yuntaijiaju.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zz.szxytkj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xw.colortex.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://in.newstarts.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qr.szxytkj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ka.yuexingan06.cn

Go:   // 按 rune 判断长度后截断
来源：http://bx.hahajie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hi.shtwfgs.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dk.bjjhwx.cn

[E22] 字节长度与字符长度
来源：http://dc.jianghongdianzi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kx.yuntaijiaju.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://on.muxihuayi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mn.jctech888.com.cn


<!-- 参考信息 -->