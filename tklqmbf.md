代发 wailian999

C#:   list.Distinct().ToList()
来源：http://hj.521024.cn

[D16] 求和与平均值
来源：http://lx.huanxung.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://sk.yuexingan06.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kq.huixinmuqiang.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qt.huixiangedu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dt.gzmigu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ex.muxihuayi.cn

Go:   // 手写循环累加
来源：http://zr.shtwfgs.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ui.bjjhwx.cn

C#:   list.Sum();  list.Average()
来源：http://es.gzmigu.cn

[D17] 最大值与最小值
来源：http://im.huanxung.cn

Py:   max(arr);  min(arr)
来源：http://ue.521024.cn

PHP:  max($arr);  min($arr);
来源：http://ek.szxytkj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ye.shxzukj.cn

TS:   Math.max(...arr);
来源：http://jx.szxytkj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://km.jianghongdianzi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tp.gzmigu.cn

Ruby: arr.max;  arr.min
来源：http://jc.nicolike.cn

C#:   list.Max();  list.Min()
来源：http://tv.bookmarksfly.cn

[D18] 扁平化嵌套数组
来源：http://eo.shxzukj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ez.panjiajie.cn

PHP:  array_merge(...$nested);
来源：http://gf.shtwfgs.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ni.bjjhwx.cn

TS:   nested.flat();
来源：http://ss.huixinmuqiang.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yc.muxihuayi.cn

Go:   // 手写双层循环
来源：http://fq.shxzskj.cn

Ruby: nested.flatten
来源：http://wj.lnxyls.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xt.huanxung.cn

[D19] 按字段分组
来源：http://of.hnjuh.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://db.muxihuayi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ne.yuexingan06.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wt.nicolike.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qm.newstarts.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://uz.muxihuayi.cn

Go:   // 手写 map[string][]T
来源：http://nn.shtwfgs.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://sn.shxzskj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://df.hahajie.cn

[D20] 统计每个元素出现次数
来源：http://yq.521024.cn

Py:   Counter(arr)
来源：http://gh.haigaiapp.cn

PHP:  array_count_values($arr);
来源：http://iy.szxytkj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rn.nszjky.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iq.lnxyls.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gg.shxzukj.cn

Go:   // 手写 map[T]int
来源：http://gt.yuntaijiaju.cn

Ruby: arr.tally
来源：http://uc.chemitech.net.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qx.huanxung.cn

[D21] 判断是否包含某元素
来源：http://ti.huixinmuqiang.cn

Py:   x in arr
来源：http://ow.hahajie.cn

PHP:  in_array($x, $arr, true);
来源：http://yf.yuexingan06.cn

JS:   arr.includes(x)
来源：http://nn.lnxyls.cn

TS:   arr.includes(x)
来源：http://us.gzmigu.cn

Java: list.contains(x)
来源：http://hd.nicolike.cn

Go:   slices.Contains(arr, x)
来源：http://ak.hahajie.cn

Ruby: arr.include?(x)
来源：http://gv.huanxung.cn

C#:   list.Contains(x)
来源：http://uk.yuexingan06.cn

[D22] 复制数组（避免共享引用）
来源：http://se.jctech888.com.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zz.panjiajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lb.jctech888.com.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ca.gzmigu.cn

TS:   [...arr];
来源：http://ou.shxzskj.cn

Java: new ArrayList<>(list);
来源：http://fw.nicolike.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cr.lnxyls.cn

Ruby: arr.dup;  arr.clone
来源：http://lb.wgjwhj.cn

C#:   new List<int>(list);
来源：http://yk.chemitech.net.cn

[D23] reduce 累积计算
来源：http://nu.huixinmuqiang.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hq.hnjuh.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rw.jianghongdianzi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pr.bookmarksfly.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pe.panjiajie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ke.hnjuh.cn

Go:   // 手写循环
来源：http://eo.chemitech.net.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wo.wgjwhj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lg.huixiangedu.cn

[D24] 字典 / Map 基本操作
来源：http://dc.huanxung.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ky.bookmarksfly.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ec.szsharing.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dr.yuntaijiaju.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lk.gzmigu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bc.gzmigu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qb.asd995.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ad.yuntaijiaju.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rt.521024.cn

[D25] Set 集合去重与交并差
来源：http://iz.521024.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nv.shxzskj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qy.jianghongdianzi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ti.hahajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://is.chemitech.net.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hk.521024.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fc.huixiangedu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vv.asd995.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bg.nszjky.cn

[D26] 数组转字符串
来源：http://ww.hnjuh.cn

Py:   ", ".join(map(str, arr))
来源：http://td.shtwfgs.cn

PHP:  implode(", ", $arr);
来源：http://it.haigaiapp.cn

JS:   arr.join(", ")
来源：http://ws.huanxung.cn

TS:   arr.join(", ")
来源：http://gb.huanxung.cn

Java: String.join(", ", list)
来源：http://ui.nicolike.cn

Go:   strings.Join(strs, ", ")
来源：http://wf.asd995.cn

Ruby: arr.join(", ")
来源：http://oa.gzmigu.cn

C#:   string.Join(", ", list)
来源：http://ef.jctech888.com.cn

================================================================================
来源：http://dv.chemitech.net.cn

E. 字符串处理
来源：http://cg.chemitech.net.cn

================================================================================
来源：http://rx.hahajie.cn

[E01] 拼接字符串
来源：http://ii.asd995.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cy.gzmigu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zx.huixiangedu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lr.bookmarksfly.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ji.521024.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://my.shxzukj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zp.521024.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pg.shxzukj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hx.nszjky.cn

[E02] 重复字符串
来源：http://ys.haigaiapp.cn

Py:   "ab" * 3
来源：http://rc.chemitech.net.cn

PHP:  str_repeat("ab", 3);
来源：http://ck.shtwfgs.cn

JS:   "ab".repeat(3)
来源：http://wx.huixinmuqiang.cn

TS:   "ab".repeat(3)
来源：http://gd.yuexingan06.cn

Java: "ab".repeat(3)
来源：http://ri.shxzukj.cn

Go:   strings.Repeat("ab", 3)
来源：http://cp.huanxung.cn

Ruby: "ab" * 3
来源：http://hs.bookmarksfly.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://al.newstarts.cn

[E03] 截取子串
来源：http://bq.muxihuayi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ho.huanxung.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ys.panjiajie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mz.bjjhwx.cn

TS:   s.slice(1, 4)
来源：http://om.521024.cn

Java: s.substring(1, 4)
来源：http://rz.lnxyls.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://uy.huanxung.cn

Ruby: s[1, 3];  s[1..3]
来源：http://tc.haigaiapp.cn

C#:   s.Substring(1, 3)
来源：http://xj.wgjwhj.cn

[E04] 查找子串位置
来源：http://st.9csxet.cn

Py:   s.find("x");  s.index("x")
来源：http://df.521024.cn

PHP:  strpos($s, "x");
来源：http://li.9csxet.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://en.shxzukj.cn

TS:   s.indexOf("x")
来源：http://kk.bjjhwx.cn

Java: s.indexOf("x")
来源：http://pz.huanxung.cn

Go:   strings.Index(s, "x")
来源：http://gq.huixinmuqiang.cn

Ruby: s.index("x")
来源：http://vx.muxihuayi.cn

C#:   s.IndexOf("x")
来源：http://rh.nicolike.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xe.huanxung.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uz.wgjwhj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jn.haigaiapp.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wi.chemitech.net.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://fl.hnjuh.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vp.9csxet.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xh.colortex.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jb.nszjky.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qh.shxzskj.cn

[E06] 替换子串
来源：http://sj.hnjuh.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wm.lnxyls.cn

PHP:  str_replace("a", "b", $s);
来源：http://po.bjjhwx.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zn.nszjky.cn

TS:   s.replaceAll("a", "b")
来源：http://cq.gzmigu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nb.yuexingan06.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://th.chemitech.net.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://li.newstarts.cn

C#:   s.Replace("a", "b")
来源：http://zg.bjjhwx.cn

[E07] 按分隔符拆分
来源：http://lt.bjjhwx.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sd.lnxyls.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vh.yuntaijiaju.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ii.jianghongdianzi.cn

TS:   s.split(",")
来源：http://un.jianghongdianzi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://nw.hnjuh.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mv.asd995.cn

Ruby: s.split(",");  s.split
来源：http://pj.shxzskj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yw.shxzukj.cn

[E08] 数组按分隔符合并
来源：http://wh.shtwfgs.cn

Py:   ",".join(items)
来源：http://kn.nszjky.cn

PHP:  implode(",", $items);
来源：http://rw.chemitech.net.cn

JS:   items.join(",")
来源：http://rx.shtwfgs.cn

TS:   items.join(",")
来源：http://rf.haigaiapp.cn

Java: String.join(",", items)
来源：http://yz.shxzskj.cn

Go:   strings.Join(items, ",")
来源：http://ja.chemitech.net.cn

Ruby: items.join(",")
来源：http://pw.bjjhwx.cn

C#:   string.Join(",", items)
来源：http://jb.9csxet.cn

[E09] 去除所有空白字符
来源：http://ar.yuntaijiaju.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pt.muxihuayi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nt.yuexingan06.cn

JS:   s.replace(/\s+/g, "")
来源：http://bv.521024.cn

TS:   s.replace(/\s+/g, "")
来源：http://wi.chemitech.net.cn

Java: s.replaceAll("\\s+", "")
来源：http://vi.shtwfgs.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ub.szxytkj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://uz.huanxung.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ce.colortex.cn

[E10] 左侧补零 / 定长填充
来源：http://fb.gzmigu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bh.szsharing.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qp.colortex.cn

JS:   "7".padStart(3, "0")
来源：http://kr.newstarts.cn

TS:   "7".padStart(3, "0")
来源：http://fb.chemitech.net.cn

Java: String.format("%03d", 7)
来源：http://pu.chemitech.net.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://it.huixinmuqiang.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pc.521024.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://aa.colortex.cn

[E11] 反转字符串
来源：http://ac.huanxung.cn

Py:   s[::-1]
来源：http://yr.haigaiapp.cn

PHP:  strrev($s);
来源：http://fv.lnxyls.cn

JS:   [...s].reverse().join("")
来源：http://gr.yuexingan06.cn

TS:   [...s].reverse().join("")
来源：http://ld.gzmigu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://hw.newstarts.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ni.bookmarksfly.cn

Ruby: s.reverse
来源：http://xt.wgjwhj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://es.yuntaijiaju.cn

[E12] 统计某字符出现次数
来源：http://xf.newstarts.cn

Py:   s.count("a")
来源：http://rr.huanxung.cn

PHP:  substr_count($s, "a");
来源：http://lj.szsharing.cn

JS:   s.split("a").length - 1
来源：http://tt.hnjuh.cn

TS:   s.split("a").length - 1
来源：http://gs.huixiangedu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bh.gzmigu.cn

Go:   strings.Count(s, "a")
来源：http://sz.huixiangedu.cn

Ruby: s.count("a")
来源：http://wf.hahajie.cn

C#:   s.Count(c => c == 'a')
来源：http://xv.huixinmuqiang.cn

[E13] 逐字符遍历
来源：http://in.lnxyls.cn

Py:   for ch in s: print(ch)
来源：http://zj.asd995.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hs.bookmarksfly.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xi.gzmigu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://tj.9csxet.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ck.huixinmuqiang.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yr.gzmigu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://th.wgjwhj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fw.hnjuh.cn

[E14] URL 编码与 Base64
来源：http://my.bjjhwx.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qe.szxytkj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://zd.huixinmuqiang.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vp.muxihuayi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ym.huixiangedu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cl.szsharing.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ik.nicolike.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://it.wgjwhj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ir.szsharing.cn

[E15] HTML 转义 / 反转义
来源：http://as.shxzskj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://le.gzmigu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uj.haigaiapp.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kc.chemitech.net.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://zt.jianghongdianzi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dg.gzmigu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://on.asd995.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tc.521024.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ja.lnxyls.cn

[E16] 数字千分位
来源：http://vc.colortex.cn

Py:   f"{1234567:,}"
来源：http://wq.newstarts.cn

PHP:  number_format(1234567);
来源：http://dt.asd995.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://nu.bookmarksfly.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://rh.szsharing.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://iy.szsharing.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vi.huanxung.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://es.huixinmuqiang.cn

C#:   1234567.ToString("N0")
来源：http://gn.nszjky.cn

[E17] 首字母大写
来源：http://gd.huanxung.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dc.shxzukj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://cp.bjjhwx.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zs.haigaiapp.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qw.haigaiapp.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://yh.shtwfgs.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ue.521024.cn

Ruby: s.capitalize
来源：http://rs.muxihuayi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vr.panjiajie.cn

[E18] 模板占位符替换
来源：http://fu.shtwfgs.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rr.bjjhwx.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://uy.gzmigu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://eb.nszjky.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ls.521024.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zd.lnxyls.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yo.szsharing.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bm.nicolike.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xh.szsharing.cn

[E19] 多行文本按行拆分
来源：http://lg.muxihuayi.cn

Py:   s.splitlines()
来源：http://ia.panjiajie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cq.shtwfgs.cn

JS:   s.split(/\r?\n/)
来源：http://ka.haigaiapp.cn

TS:   s.split(/\r?\n/)
来源：http://gu.nszjky.cn

Java: s.lines().toList()
来源：http://xi.newstarts.cn

Go:   strings.Split(s, "\n")
来源：http://nk.asd995.cn

Ruby: s.lines
来源：http://le.szsharing.cn

C#:   s.Split('\n')
来源：http://ym.huixiangedu.cn

[E20] 判断字符串是否为空
来源：http://kk.yuexingan06.cn

Py:   if not s:
来源：http://nj.huixiangedu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pe.bjjhwx.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cd.hnjuh.cn

TS:   if (s === "") {}
来源：http://fo.hnjuh.cn

Java: if (s.isEmpty()) {}
来源：http://is.yuntaijiaju.cn

Go:   if s == "" {}
来源：http://rn.huixiangedu.cn

Ruby: if s.empty?
来源：http://kr.huixinmuqiang.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://db.hahajie.cn

[E21] 超长截断加省略号
来源：http://qp.nszjky.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wj.shtwfgs.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vw.newstarts.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ru.newstarts.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zq.521024.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hc.szxytkj.cn

Go:   // 按 rune 判断长度后截断
来源：http://pm.wgjwhj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jo.huixiangedu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ak.nicolike.cn

[E22] 字节长度与字符长度
来源：http://vc.huanxung.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://du.jctech888.com.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sf.521024.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qj.colortex.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://za.hnjuh.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://at.huixinmuqiang.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cw.nicolike.cn

Ruby: s.bytesize;  s.length
来源：http://pe.shxzskj.cn


<!-- 参考信息 -->