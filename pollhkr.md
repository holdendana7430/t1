代发 wailian999

TS:   [...new Set(arr)]
来源：http://vq.9csxet.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ob.lnxyls.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wi.521024.cn

Ruby: arr.uniq
来源：http://ko.muxihuayi.cn

C#:   list.Distinct().ToList()
来源：http://ka.szxytkj.cn

[D16] 求和与平均值
来源：http://rw.lnxyls.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ss.huixinmuqiang.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jz.szxytkj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rz.haigaiapp.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gf.szsharing.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ef.shxzukj.cn

Go:   // 手写循环累加
来源：http://el.bookmarksfly.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rg.521024.cn

C#:   list.Sum();  list.Average()
来源：http://wb.yuexingan06.cn

[D17] 最大值与最小值
来源：http://py.shxzskj.cn

Py:   max(arr);  min(arr)
来源：http://qx.jctech888.com.cn

PHP:  max($arr);  min($arr);
来源：http://yp.521024.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ol.shxzukj.cn

TS:   Math.max(...arr);
来源：http://uj.shxzskj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://wq.asd995.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://af.yuexingan06.cn

Ruby: arr.max;  arr.min
来源：http://qm.szxytkj.cn

C#:   list.Max();  list.Min()
来源：http://de.yuexingan06.cn

[D18] 扁平化嵌套数组
来源：http://bp.muxihuayi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dm.muxihuayi.cn

PHP:  array_merge(...$nested);
来源：http://xj.wgjwhj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kh.bookmarksfly.cn

TS:   nested.flat();
来源：http://vb.9csxet.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pl.panjiajie.cn

Go:   // 手写双层循环
来源：http://ud.521024.cn

Ruby: nested.flatten
来源：http://di.wgjwhj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hr.shxzukj.cn

[D19] 按字段分组
来源：http://lf.nszjky.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ba.nszjky.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://as.asd995.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yi.huixinmuqiang.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ap.521024.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zk.521024.cn

Go:   // 手写 map[string][]T
来源：http://jh.chemitech.net.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ed.szsharing.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pm.bookmarksfly.cn

[D20] 统计每个元素出现次数
来源：http://mh.chemitech.net.cn

Py:   Counter(arr)
来源：http://ox.hahajie.cn

PHP:  array_count_values($arr);
来源：http://vu.jctech888.com.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ar.panjiajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sl.huixiangedu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://uc.haigaiapp.cn

Go:   // 手写 map[T]int
来源：http://mz.lnxyls.cn

Ruby: arr.tally
来源：http://bi.lnxyls.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://is.yuntaijiaju.cn

[D21] 判断是否包含某元素
来源：http://xv.nszjky.cn

Py:   x in arr
来源：http://ik.huanxung.cn

PHP:  in_array($x, $arr, true);
来源：http://ov.huixinmuqiang.cn

JS:   arr.includes(x)
来源：http://uo.chemitech.net.cn

TS:   arr.includes(x)
来源：http://vm.muxihuayi.cn

Java: list.contains(x)
来源：http://ds.panjiajie.cn

Go:   slices.Contains(arr, x)
来源：http://xq.shxzukj.cn

Ruby: arr.include?(x)
来源：http://kg.bookmarksfly.cn

C#:   list.Contains(x)
来源：http://uy.521024.cn

[D22] 复制数组（避免共享引用）
来源：http://td.haigaiapp.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jh.haigaiapp.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://uh.nicolike.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vm.shxzukj.cn

TS:   [...arr];
来源：http://ql.nicolike.cn

Java: new ArrayList<>(list);
来源：http://bk.yuexingan06.cn

Go:   copied := append([]int(nil), arr...)
来源：http://mk.bookmarksfly.cn

Ruby: arr.dup;  arr.clone
来源：http://yf.colortex.cn

C#:   new List<int>(list);
来源：http://nh.chemitech.net.cn

[D23] reduce 累积计算
来源：http://rz.panjiajie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rl.shtwfgs.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mr.bookmarksfly.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vp.jianghongdianzi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iu.nicolike.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://hg.colortex.cn

Go:   // 手写循环
来源：http://yi.hahajie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fo.hahajie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://or.szxytkj.cn

[D24] 字典 / Map 基本操作
来源：http://sd.lnxyls.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bp.panjiajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pa.shxzukj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xb.521024.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://il.szsharing.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lz.panjiajie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cc.colortex.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gj.asd995.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vi.asd995.cn

[D25] Set 集合去重与交并差
来源：http://ds.panjiajie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qu.newstarts.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sd.huanxung.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gl.gzmigu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://we.panjiajie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://co.9csxet.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hy.hahajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://oc.lnxyls.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xg.bjjhwx.cn

[D26] 数组转字符串
来源：http://db.shxzskj.cn

Py:   ", ".join(map(str, arr))
来源：http://zt.jianghongdianzi.cn

PHP:  implode(", ", $arr);
来源：http://ze.9csxet.cn

JS:   arr.join(", ")
来源：http://bc.521024.cn

TS:   arr.join(", ")
来源：http://ww.newstarts.cn

Java: String.join(", ", list)
来源：http://re.wgjwhj.cn

Go:   strings.Join(strs, ", ")
来源：http://ex.jianghongdianzi.cn

Ruby: arr.join(", ")
来源：http://ru.gzmigu.cn

C#:   string.Join(", ", list)
来源：http://fu.shxzukj.cn

================================================================================
来源：http://pd.huanxung.cn

E. 字符串处理
来源：http://xf.bjjhwx.cn

================================================================================
来源：http://ht.yuntaijiaju.cn

[E01] 拼接字符串
来源：http://gm.wgjwhj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://go.shxzskj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xm.jctech888.com.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cr.huanxung.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rv.muxihuayi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://eu.nszjky.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gc.hahajie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jg.shxzukj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://va.nszjky.cn

[E02] 重复字符串
来源：http://ic.jianghongdianzi.cn

Py:   "ab" * 3
来源：http://lj.9csxet.cn

PHP:  str_repeat("ab", 3);
来源：http://qn.yuexingan06.cn

JS:   "ab".repeat(3)
来源：http://vp.yuntaijiaju.cn

TS:   "ab".repeat(3)
来源：http://ls.hahajie.cn

Java: "ab".repeat(3)
来源：http://wq.asd995.cn

Go:   strings.Repeat("ab", 3)
来源：http://nq.9csxet.cn

Ruby: "ab" * 3
来源：http://kq.wgjwhj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ol.asd995.cn

[E03] 截取子串
来源：http://ia.asd995.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ry.bookmarksfly.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jl.jctech888.com.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qi.yuntaijiaju.cn

TS:   s.slice(1, 4)
来源：http://qd.yuexingan06.cn

Java: s.substring(1, 4)
来源：http://ia.shxzukj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wc.jianghongdianzi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ot.lnxyls.cn

C#:   s.Substring(1, 3)
来源：http://xs.521024.cn

[E04] 查找子串位置
来源：http://iy.asd995.cn

Py:   s.find("x");  s.index("x")
来源：http://pt.yuntaijiaju.cn

PHP:  strpos($s, "x");
来源：http://pl.hahajie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sf.haigaiapp.cn

TS:   s.indexOf("x")
来源：http://as.gzmigu.cn

Java: s.indexOf("x")
来源：http://yq.hnjuh.cn

Go:   strings.Index(s, "x")
来源：http://ye.jctech888.com.cn

Ruby: s.index("x")
来源：http://yh.huanxung.cn

C#:   s.IndexOf("x")
来源：http://fa.panjiajie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://wx.huixinmuqiang.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bk.9csxet.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fq.huixinmuqiang.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://im.shxzskj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://au.lnxyls.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://or.wgjwhj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ks.huixinmuqiang.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xb.huixiangedu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nz.muxihuayi.cn

[E06] 替换子串
来源：http://yu.521024.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rb.chemitech.net.cn

PHP:  str_replace("a", "b", $s);
来源：http://hl.bookmarksfly.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hh.chemitech.net.cn

TS:   s.replaceAll("a", "b")
来源：http://pj.colortex.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ko.shtwfgs.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ib.yuexingan06.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zr.lnxyls.cn

C#:   s.Replace("a", "b")
来源：http://tp.yuexingan06.cn

[E07] 按分隔符拆分
来源：http://ar.shxzukj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cz.lnxyls.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jy.panjiajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://xy.9csxet.cn

TS:   s.split(",")
来源：http://tf.jianghongdianzi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://qp.bjjhwx.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vh.szxytkj.cn

Ruby: s.split(",");  s.split
来源：http://fy.asd995.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bg.hahajie.cn

[E08] 数组按分隔符合并
来源：http://ye.9csxet.cn

Py:   ",".join(items)
来源：http://hm.lnxyls.cn

PHP:  implode(",", $items);
来源：http://bt.asd995.cn

JS:   items.join(",")
来源：http://cn.yuexingan06.cn

TS:   items.join(",")
来源：http://vr.wgjwhj.cn

Java: String.join(",", items)
来源：http://ir.bjjhwx.cn

Go:   strings.Join(items, ",")
来源：http://go.panjiajie.cn

Ruby: items.join(",")
来源：http://mi.huixinmuqiang.cn

C#:   string.Join(",", items)
来源：http://iy.shxzukj.cn

[E09] 去除所有空白字符
来源：http://lb.muxihuayi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://af.gzmigu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://no.yuexingan06.cn

JS:   s.replace(/\s+/g, "")
来源：http://sr.szxytkj.cn

TS:   s.replace(/\s+/g, "")
来源：http://tl.lnxyls.cn

Java: s.replaceAll("\\s+", "")
来源：http://ob.shtwfgs.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://mm.hahajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://lb.lnxyls.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jn.huixiangedu.cn

[E10] 左侧补零 / 定长填充
来源：http://jc.hnjuh.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://eh.szxytkj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://yo.panjiajie.cn

JS:   "7".padStart(3, "0")
来源：http://vs.hahajie.cn

TS:   "7".padStart(3, "0")
来源：http://kd.shxzukj.cn

Java: String.format("%03d", 7)
来源：http://bg.hnjuh.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://um.huanxung.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gm.panjiajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://uu.521024.cn

[E11] 反转字符串
来源：http://fe.nszjky.cn

Py:   s[::-1]
来源：http://wn.9csxet.cn

PHP:  strrev($s);
来源：http://aw.wgjwhj.cn

JS:   [...s].reverse().join("")
来源：http://nr.hahajie.cn

TS:   [...s].reverse().join("")
来源：http://sv.gzmigu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wt.bjjhwx.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://hf.jctech888.com.cn

Ruby: s.reverse
来源：http://ks.hahajie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vk.521024.cn

[E12] 统计某字符出现次数
来源：http://su.colortex.cn

Py:   s.count("a")
来源：http://yw.jctech888.com.cn

PHP:  substr_count($s, "a");
来源：http://rh.yuntaijiaju.cn

JS:   s.split("a").length - 1
来源：http://zk.haigaiapp.cn

TS:   s.split("a").length - 1
来源：http://qw.huixiangedu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vx.nicolike.cn

Go:   strings.Count(s, "a")
来源：http://ob.colortex.cn

Ruby: s.count("a")
来源：http://km.9csxet.cn

C#:   s.Count(c => c == 'a')
来源：http://fr.muxihuayi.cn

[E13] 逐字符遍历
来源：http://tq.panjiajie.cn

Py:   for ch in s: print(ch)
来源：http://hu.huanxung.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vl.jianghongdianzi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://rx.hahajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wf.nicolike.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rq.jctech888.com.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tf.521024.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://lm.huanxung.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hb.nszjky.cn

[E14] URL 编码与 Base64
来源：http://uw.bookmarksfly.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ev.colortex.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://iq.9csxet.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://aw.yuexingan06.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vl.hahajie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://br.521024.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://oa.9csxet.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://iz.521024.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yq.shxzskj.cn

[E15] HTML 转义 / 反转义
来源：http://ky.shxzskj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://to.szsharing.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sr.chemitech.net.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dn.shtwfgs.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ue.521024.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pd.hahajie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pz.shxzskj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qs.bookmarksfly.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hk.521024.cn

[E16] 数字千分位
来源：http://jg.huixiangedu.cn

Py:   f"{1234567:,}"
来源：http://cu.huixinmuqiang.cn

PHP:  number_format(1234567);
来源：http://ds.nicolike.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ai.newstarts.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://cr.lnxyls.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://eb.muxihuayi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hv.bookmarksfly.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dt.521024.cn

C#:   1234567.ToString("N0")
来源：http://qv.yuexingan06.cn

[E17] 首字母大写
来源：http://fg.szsharing.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vb.shxzukj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://kk.chemitech.net.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tp.huixiangedu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zi.muxihuayi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://uk.hahajie.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tm.shxzskj.cn

Ruby: s.capitalize
来源：http://fh.haigaiapp.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dm.panjiajie.cn

[E18] 模板占位符替换
来源：http://bc.asd995.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://un.nicolike.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ch.bjjhwx.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://on.huanxung.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://xt.huanxung.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gw.9csxet.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ue.shxzukj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xv.shtwfgs.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://br.asd995.cn

[E19] 多行文本按行拆分
来源：http://qk.huixinmuqiang.cn

Py:   s.splitlines()
来源：http://yx.chemitech.net.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kh.panjiajie.cn

JS:   s.split(/\r?\n/)
来源：http://oj.muxihuayi.cn

TS:   s.split(/\r?\n/)
来源：http://ru.asd995.cn

Java: s.lines().toList()
来源：http://ih.521024.cn

Go:   strings.Split(s, "\n")
来源：http://tm.shtwfgs.cn

Ruby: s.lines
来源：http://so.gzmigu.cn

C#:   s.Split('\n')
来源：http://df.wgjwhj.cn

[E20] 判断字符串是否为空
来源：http://jb.huixinmuqiang.cn

Py:   if not s:
来源：http://nr.wgjwhj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ky.szsharing.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rp.gzmigu.cn

TS:   if (s === "") {}
来源：http://nt.bookmarksfly.cn

Java: if (s.isEmpty()) {}
来源：http://zx.hnjuh.cn

Go:   if s == "" {}
来源：http://kw.muxihuayi.cn

Ruby: if s.empty?
来源：http://vn.colortex.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nq.asd995.cn

[E21] 超长截断加省略号
来源：http://ko.bjjhwx.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ng.shxzskj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xa.nszjky.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://px.yuexingan06.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nb.9csxet.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lx.asd995.cn

Go:   // 按 rune 判断长度后截断
来源：http://ui.9csxet.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cb.nszjky.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://on.shxzukj.cn

[E22] 字节长度与字符长度
来源：http://kw.colortex.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://uv.nicolike.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vk.shxzskj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tc.szsharing.cn


<!-- 参考信息 -->