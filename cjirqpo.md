代发 wailian999

TS:   [...new Set(arr)]
来源：http://do.bjjhwx.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cl.szxytkj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://mh.nszjky.cn

Ruby: arr.uniq
来源：http://ss.hnjuh.cn

C#:   list.Distinct().ToList()
来源：http://wa.yuexingan06.cn

[D16] 求和与平均值
来源：http://pe.chemitech.net.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://km.szxytkj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://po.521024.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sy.hahajie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xp.asd995.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bj.hnjuh.cn

Go:   // 手写循环累加
来源：http://ck.chemitech.net.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fu.haigaiapp.cn

C#:   list.Sum();  list.Average()
来源：http://br.nicolike.cn

[D17] 最大值与最小值
来源：http://gk.9csxet.cn

Py:   max(arr);  min(arr)
来源：http://zh.szxytkj.cn

PHP:  max($arr);  min($arr);
来源：http://yc.bjjhwx.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://od.colortex.cn

TS:   Math.max(...arr);
来源：http://ni.huixinmuqiang.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://pe.nszjky.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lp.shtwfgs.cn

Ruby: arr.max;  arr.min
来源：http://er.nszjky.cn

C#:   list.Max();  list.Min()
来源：http://vu.muxihuayi.cn

[D18] 扁平化嵌套数组
来源：http://gu.gzmigu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://io.wgjwhj.cn

PHP:  array_merge(...$nested);
来源：http://dt.szsharing.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hw.hahajie.cn

TS:   nested.flat();
来源：http://ws.haigaiapp.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dc.521024.cn

Go:   // 手写双层循环
来源：http://qs.yuntaijiaju.cn

Ruby: nested.flatten
来源：http://uy.chemitech.net.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://se.asd995.cn

[D19] 按字段分组
来源：http://ux.colortex.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zm.huanxung.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ho.hnjuh.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://om.asd995.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://rr.gzmigu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hb.wgjwhj.cn

Go:   // 手写 map[string][]T
来源：http://tp.hnjuh.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://pp.wgjwhj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://be.newstarts.cn

[D20] 统计每个元素出现次数
来源：http://ks.gzmigu.cn

Py:   Counter(arr)
来源：http://jt.huixiangedu.cn

PHP:  array_count_values($arr);
来源：http://fy.shxzskj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xa.panjiajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sp.huixinmuqiang.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://at.nszjky.cn

Go:   // 手写 map[T]int
来源：http://ee.jianghongdianzi.cn

Ruby: arr.tally
来源：http://lt.wgjwhj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mi.muxihuayi.cn

[D21] 判断是否包含某元素
来源：http://hv.hahajie.cn

Py:   x in arr
来源：http://wa.panjiajie.cn

PHP:  in_array($x, $arr, true);
来源：http://or.hnjuh.cn

JS:   arr.includes(x)
来源：http://ol.shtwfgs.cn

TS:   arr.includes(x)
来源：http://pi.lnxyls.cn

Java: list.contains(x)
来源：http://mg.jianghongdianzi.cn

Go:   slices.Contains(arr, x)
来源：http://co.newstarts.cn

Ruby: arr.include?(x)
来源：http://bq.jianghongdianzi.cn

C#:   list.Contains(x)
来源：http://ra.haigaiapp.cn

[D22] 复制数组（避免共享引用）
来源：http://ek.szxytkj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pr.bjjhwx.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yx.hnjuh.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mc.chemitech.net.cn

TS:   [...arr];
来源：http://tx.lnxyls.cn

Java: new ArrayList<>(list);
来源：http://zt.szsharing.cn

Go:   copied := append([]int(nil), arr...)
来源：http://nn.wgjwhj.cn

Ruby: arr.dup;  arr.clone
来源：http://dh.bookmarksfly.cn

C#:   new List<int>(list);
来源：http://ym.bjjhwx.cn

[D23] reduce 累积计算
来源：http://fq.nszjky.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sw.haigaiapp.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wx.bookmarksfly.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vp.bookmarksfly.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sl.hnjuh.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://jf.jianghongdianzi.cn

Go:   // 手写循环
来源：http://vx.gzmigu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dd.shxzukj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://al.colortex.cn

[D24] 字典 / Map 基本操作
来源：http://fu.hahajie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://id.colortex.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zj.jctech888.com.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wr.asd995.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kb.haigaiapp.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jh.lnxyls.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zr.hahajie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://it.jianghongdianzi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kf.huixiangedu.cn

[D25] Set 集合去重与交并差
来源：http://er.panjiajie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://si.nicolike.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://of.jctech888.com.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vr.huanxung.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://aj.hnjuh.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://le.haigaiapp.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://po.jctech888.com.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uc.nszjky.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gz.shxzskj.cn

[D26] 数组转字符串
来源：http://yt.chemitech.net.cn

Py:   ", ".join(map(str, arr))
来源：http://qf.bookmarksfly.cn

PHP:  implode(", ", $arr);
来源：http://qu.huanxung.cn

JS:   arr.join(", ")
来源：http://ox.nszjky.cn

TS:   arr.join(", ")
来源：http://dz.wgjwhj.cn

Java: String.join(", ", list)
来源：http://br.shxzskj.cn

Go:   strings.Join(strs, ", ")
来源：http://hg.jianghongdianzi.cn

Ruby: arr.join(", ")
来源：http://bi.huixiangedu.cn

C#:   string.Join(", ", list)
来源：http://iz.szxytkj.cn

================================================================================
来源：http://xp.shtwfgs.cn

E. 字符串处理
来源：http://wf.huixiangedu.cn

================================================================================
来源：http://kw.szsharing.cn

[E01] 拼接字符串
来源：http://fv.chemitech.net.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pl.huixiangedu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://os.muxihuayi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cu.chemitech.net.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qc.lnxyls.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fe.hnjuh.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ri.bjjhwx.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dv.nszjky.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qk.colortex.cn

[E02] 重复字符串
来源：http://nx.521024.cn

Py:   "ab" * 3
来源：http://go.nszjky.cn

PHP:  str_repeat("ab", 3);
来源：http://ju.shxzskj.cn

JS:   "ab".repeat(3)
来源：http://tn.hahajie.cn

TS:   "ab".repeat(3)
来源：http://rf.nszjky.cn

Java: "ab".repeat(3)
来源：http://wq.newstarts.cn

Go:   strings.Repeat("ab", 3)
来源：http://yd.colortex.cn

Ruby: "ab" * 3
来源：http://cv.hahajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tt.muxihuayi.cn

[E03] 截取子串
来源：http://qx.muxihuayi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ig.shxzukj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xw.colortex.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://st.521024.cn

TS:   s.slice(1, 4)
来源：http://cz.wgjwhj.cn

Java: s.substring(1, 4)
来源：http://ic.shtwfgs.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mz.huixiangedu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://hl.szxytkj.cn

C#:   s.Substring(1, 3)
来源：http://mq.nicolike.cn

[E04] 查找子串位置
来源：http://uk.panjiajie.cn

Py:   s.find("x");  s.index("x")
来源：http://rk.panjiajie.cn

PHP:  strpos($s, "x");
来源：http://wj.szxytkj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://up.chemitech.net.cn

TS:   s.indexOf("x")
来源：http://jc.bookmarksfly.cn

Java: s.indexOf("x")
来源：http://pl.yuntaijiaju.cn

Go:   strings.Index(s, "x")
来源：http://im.shxzskj.cn

Ruby: s.index("x")
来源：http://th.huixiangedu.cn

C#:   s.IndexOf("x")
来源：http://zb.huanxung.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://cp.jianghongdianzi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uo.jctech888.com.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ig.gzmigu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yk.shxzskj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://kt.9csxet.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uv.yuexingan06.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kl.huixinmuqiang.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pt.muxihuayi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cy.wgjwhj.cn

[E06] 替换子串
来源：http://qm.yuntaijiaju.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ic.hnjuh.cn

PHP:  str_replace("a", "b", $s);
来源：http://ir.szxytkj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ze.haigaiapp.cn

TS:   s.replaceAll("a", "b")
来源：http://po.nicolike.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mz.newstarts.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bh.shxzukj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hw.jianghongdianzi.cn

C#:   s.Replace("a", "b")
来源：http://da.shtwfgs.cn

[E07] 按分隔符拆分
来源：http://yf.szsharing.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qe.hnjuh.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xz.hahajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://lg.bjjhwx.cn

TS:   s.split(",")
来源：http://gu.bjjhwx.cn

Java: s.split(",");  s.split("\\s+")
来源：http://jd.szsharing.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ur.hnjuh.cn

Ruby: s.split(",");  s.split
来源：http://ml.nicolike.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vu.haigaiapp.cn

[E08] 数组按分隔符合并
来源：http://bp.hahajie.cn

Py:   ",".join(items)
来源：http://nb.jctech888.com.cn

PHP:  implode(",", $items);
来源：http://kj.nszjky.cn

JS:   items.join(",")
来源：http://aa.huixinmuqiang.cn

TS:   items.join(",")
来源：http://hi.huanxung.cn

Java: String.join(",", items)
来源：http://rx.szsharing.cn

Go:   strings.Join(items, ",")
来源：http://et.jianghongdianzi.cn

Ruby: items.join(",")
来源：http://dh.bookmarksfly.cn

C#:   string.Join(",", items)
来源：http://yx.haigaiapp.cn

[E09] 去除所有空白字符
来源：http://bp.yuntaijiaju.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ig.yuntaijiaju.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://uy.muxihuayi.cn

JS:   s.replace(/\s+/g, "")
来源：http://in.szxytkj.cn

TS:   s.replace(/\s+/g, "")
来源：http://vg.newstarts.cn

Java: s.replaceAll("\\s+", "")
来源：http://ag.chemitech.net.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://jm.muxihuayi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://et.bookmarksfly.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zh.nicolike.cn

[E10] 左侧补零 / 定长填充
来源：http://fe.shxzskj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jb.asd995.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fd.jctech888.com.cn

JS:   "7".padStart(3, "0")
来源：http://qw.jianghongdianzi.cn

TS:   "7".padStart(3, "0")
来源：http://bc.nicolike.cn

Java: String.format("%03d", 7)
来源：http://tb.huixinmuqiang.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ib.colortex.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ge.9csxet.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bp.asd995.cn

[E11] 反转字符串
来源：http://jm.gzmigu.cn

Py:   s[::-1]
来源：http://hq.shxzukj.cn

PHP:  strrev($s);
来源：http://lw.bookmarksfly.cn

JS:   [...s].reverse().join("")
来源：http://ue.bjjhwx.cn

TS:   [...s].reverse().join("")
来源：http://sa.hnjuh.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://vk.gzmigu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ah.szxytkj.cn

Ruby: s.reverse
来源：http://lu.asd995.cn

C#:   new string(s.Reverse().ToArray())
来源：http://es.asd995.cn

[E12] 统计某字符出现次数
来源：http://ct.yuntaijiaju.cn

Py:   s.count("a")
来源：http://ae.gzmigu.cn

PHP:  substr_count($s, "a");
来源：http://ah.jctech888.com.cn

JS:   s.split("a").length - 1
来源：http://xq.shtwfgs.cn

TS:   s.split("a").length - 1
来源：http://zz.nicolike.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ts.nicolike.cn

Go:   strings.Count(s, "a")
来源：http://ht.huixiangedu.cn

Ruby: s.count("a")
来源：http://qz.wgjwhj.cn

C#:   s.Count(c => c == 'a')
来源：http://wd.hahajie.cn

[E13] 逐字符遍历
来源：http://fp.yuexingan06.cn

Py:   for ch in s: print(ch)
来源：http://dz.huixinmuqiang.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pu.jctech888.com.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://eb.huixiangedu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ua.lnxyls.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vo.panjiajie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gp.wgjwhj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://pe.gzmigu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://am.haigaiapp.cn

[E14] URL 编码与 Base64
来源：http://ut.521024.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hu.newstarts.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://jl.panjiajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ht.haigaiapp.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zs.chemitech.net.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ce.hahajie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ez.huanxung.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ty.shtwfgs.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hm.shxzukj.cn

[E15] HTML 转义 / 反转义
来源：http://tr.muxihuayi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://eo.9csxet.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qr.muxihuayi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zt.haigaiapp.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://kv.yuexingan06.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ff.yuntaijiaju.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mt.huanxung.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pd.muxihuayi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dc.bjjhwx.cn

[E16] 数字千分位
来源：http://pu.panjiajie.cn

Py:   f"{1234567:,}"
来源：http://hb.lnxyls.cn

PHP:  number_format(1234567);
来源：http://mk.nicolike.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://cj.asd995.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://uo.jctech888.com.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vh.shxzukj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dh.shxzskj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wl.nszjky.cn

C#:   1234567.ToString("N0")
来源：http://hu.colortex.cn

[E17] 首字母大写
来源：http://ma.szsharing.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wz.haigaiapp.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://qu.huixiangedu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hr.yuexingan06.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://io.9csxet.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sl.9csxet.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gg.chemitech.net.cn

Ruby: s.capitalize
来源：http://ur.yuntaijiaju.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ko.shxzskj.cn

[E18] 模板占位符替换
来源：http://fl.nszjky.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tm.szxytkj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bu.nicolike.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://gf.newstarts.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://yf.lnxyls.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lf.yuntaijiaju.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lp.9csxet.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vs.szxytkj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://of.newstarts.cn

[E19] 多行文本按行拆分
来源：http://qr.lnxyls.cn

Py:   s.splitlines()
来源：http://gw.521024.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ly.huixinmuqiang.cn

JS:   s.split(/\r?\n/)
来源：http://zq.jctech888.com.cn

TS:   s.split(/\r?\n/)
来源：http://iv.huixiangedu.cn

Java: s.lines().toList()
来源：http://rk.bookmarksfly.cn

Go:   strings.Split(s, "\n")
来源：http://bu.9csxet.cn

Ruby: s.lines
来源：http://jp.9csxet.cn

C#:   s.Split('\n')
来源：http://bt.gzmigu.cn

[E20] 判断字符串是否为空
来源：http://wy.huixinmuqiang.cn

Py:   if not s:
来源：http://cw.newstarts.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yr.bookmarksfly.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://un.muxihuayi.cn

TS:   if (s === "") {}
来源：http://iw.muxihuayi.cn

Java: if (s.isEmpty()) {}
来源：http://lc.9csxet.cn

Go:   if s == "" {}
来源：http://ni.szxytkj.cn

Ruby: if s.empty?
来源：http://dv.huanxung.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gh.nszjky.cn

[E21] 超长截断加省略号
来源：http://yv.9csxet.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://oy.shxzskj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hd.asd995.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fy.panjiajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yb.jianghongdianzi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tr.wgjwhj.cn

Go:   // 按 rune 判断长度后截断
来源：http://vq.hnjuh.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lr.hahajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zw.haigaiapp.cn

[E22] 字节长度与字符长度
来源：http://gr.szxytkj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fw.wgjwhj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jc.haigaiapp.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pl.nicolike.cn


<!-- 参考信息 -->