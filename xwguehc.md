代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://ts.asd995.cn

Go:   // 手写循环
来源：http://zj.nszjky.cn

Ruby: arr.map { |x| x * 2 }
来源：http://tt.yuntaijiaju.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://bq.nszjky.cn

[D15] 去重
来源：http://qk.haigaiapp.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qr.hahajie.cn

PHP:  array_unique($arr);
来源：http://bg.hnjuh.cn

JS:   [...new Set(arr)]
来源：http://je.nicolike.cn

TS:   [...new Set(arr)]
来源：http://fg.huanxung.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pz.shtwfgs.cn

Go:   // 用 map[T]struct{} 手写
来源：http://nq.huanxung.cn

Ruby: arr.uniq
来源：http://fk.muxihuayi.cn

C#:   list.Distinct().ToList()
来源：http://dd.muxihuayi.cn

[D16] 求和与平均值
来源：http://mo.szxytkj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nb.521024.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://df.huanxung.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ff.hnjuh.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mo.shxzukj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zc.hahajie.cn

Go:   // 手写循环累加
来源：http://lp.bjjhwx.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ae.shxzskj.cn

C#:   list.Sum();  list.Average()
来源：http://rj.muxihuayi.cn

[D17] 最大值与最小值
来源：http://oz.jianghongdianzi.cn

Py:   max(arr);  min(arr)
来源：http://gc.colortex.cn

PHP:  max($arr);  min($arr);
来源：http://fk.panjiajie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ft.jctech888.com.cn

TS:   Math.max(...arr);
来源：http://cc.huixiangedu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://nh.newstarts.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kj.gzmigu.cn

Ruby: arr.max;  arr.min
来源：http://sw.521024.cn

C#:   list.Max();  list.Min()
来源：http://en.bookmarksfly.cn

[D18] 扁平化嵌套数组
来源：http://uo.shxzukj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vz.huixiangedu.cn

PHP:  array_merge(...$nested);
来源：http://gs.hnjuh.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kh.wgjwhj.cn

TS:   nested.flat();
来源：http://ah.hahajie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gl.wgjwhj.cn

Go:   // 手写双层循环
来源：http://im.shxzskj.cn

Ruby: nested.flatten
来源：http://ex.hnjuh.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ch.huixiangedu.cn

[D19] 按字段分组
来源：http://yy.gzmigu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://re.colortex.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bg.huanxung.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qs.bookmarksfly.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://et.wgjwhj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xb.newstarts.cn

Go:   // 手写 map[string][]T
来源：http://sz.gzmigu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://zs.9csxet.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ss.lnxyls.cn

[D20] 统计每个元素出现次数
来源：http://lh.huixiangedu.cn

Py:   Counter(arr)
来源：http://hn.bjjhwx.cn

PHP:  array_count_values($arr);
来源：http://uf.huanxung.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ml.chemitech.net.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kz.chemitech.net.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dl.huixiangedu.cn

Go:   // 手写 map[T]int
来源：http://pg.huixiangedu.cn

Ruby: arr.tally
来源：http://oc.jianghongdianzi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zr.nszjky.cn

[D21] 判断是否包含某元素
来源：http://od.huanxung.cn

Py:   x in arr
来源：http://jd.panjiajie.cn

PHP:  in_array($x, $arr, true);
来源：http://yo.shxzskj.cn

JS:   arr.includes(x)
来源：http://sy.jctech888.com.cn

TS:   arr.includes(x)
来源：http://am.muxihuayi.cn

Java: list.contains(x)
来源：http://pr.yuntaijiaju.cn

Go:   slices.Contains(arr, x)
来源：http://cr.shtwfgs.cn

Ruby: arr.include?(x)
来源：http://gi.521024.cn

C#:   list.Contains(x)
来源：http://gd.huanxung.cn

[D22] 复制数组（避免共享引用）
来源：http://fk.shtwfgs.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wh.bjjhwx.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ga.chemitech.net.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yr.bookmarksfly.cn

TS:   [...arr];
来源：http://rk.wgjwhj.cn

Java: new ArrayList<>(list);
来源：http://lg.haigaiapp.cn

Go:   copied := append([]int(nil), arr...)
来源：http://sr.colortex.cn

Ruby: arr.dup;  arr.clone
来源：http://ol.shxzskj.cn

C#:   new List<int>(list);
来源：http://ye.hnjuh.cn

[D23] reduce 累积计算
来源：http://qr.chemitech.net.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jb.muxihuayi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ij.shtwfgs.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xv.huixinmuqiang.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sf.hnjuh.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://jd.huixinmuqiang.cn

Go:   // 手写循环
来源：http://uj.jctech888.com.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pb.colortex.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://up.jctech888.com.cn

[D24] 字典 / Map 基本操作
来源：http://ej.chemitech.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dd.bjjhwx.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xs.lnxyls.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://du.shtwfgs.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yd.hnjuh.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://to.bookmarksfly.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wn.shxzukj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mg.shtwfgs.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://do.panjiajie.cn

[D25] Set 集合去重与交并差
来源：http://ae.hnjuh.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jn.huixiangedu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://eg.nszjky.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lg.huixiangedu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xg.colortex.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nj.szxytkj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kn.gzmigu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fb.hnjuh.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fc.9csxet.cn

[D26] 数组转字符串
来源：http://xs.huanxung.cn

Py:   ", ".join(map(str, arr))
来源：http://ro.hnjuh.cn

PHP:  implode(", ", $arr);
来源：http://cm.bookmarksfly.cn

JS:   arr.join(", ")
来源：http://lv.huixiangedu.cn

TS:   arr.join(", ")
来源：http://ht.nicolike.cn

Java: String.join(", ", list)
来源：http://mr.shxzskj.cn

Go:   strings.Join(strs, ", ")
来源：http://yt.bjjhwx.cn

Ruby: arr.join(", ")
来源：http://fy.bookmarksfly.cn

C#:   string.Join(", ", list)
来源：http://ah.9csxet.cn

================================================================================
来源：http://zs.lnxyls.cn

E. 字符串处理
来源：http://ph.hahajie.cn

================================================================================
来源：http://fu.shxzskj.cn

[E01] 拼接字符串
来源：http://ie.huanxung.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yf.yuexingan06.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mz.521024.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rq.chemitech.net.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lr.yuexingan06.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://en.yuntaijiaju.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wl.huanxung.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tr.hahajie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sn.jctech888.com.cn

[E02] 重复字符串
来源：http://fl.lnxyls.cn

Py:   "ab" * 3
来源：http://rh.panjiajie.cn

PHP:  str_repeat("ab", 3);
来源：http://hv.shtwfgs.cn

JS:   "ab".repeat(3)
来源：http://kc.asd995.cn

TS:   "ab".repeat(3)
来源：http://ig.szxytkj.cn

Java: "ab".repeat(3)
来源：http://ta.bjjhwx.cn

Go:   strings.Repeat("ab", 3)
来源：http://rn.bookmarksfly.cn

Ruby: "ab" * 3
来源：http://dj.asd995.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ch.newstarts.cn

[E03] 截取子串
来源：http://zj.shxzskj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://sw.colortex.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ao.panjiajie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nj.huixinmuqiang.cn

TS:   s.slice(1, 4)
来源：http://kl.haigaiapp.cn

Java: s.substring(1, 4)
来源：http://lx.nszjky.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dx.yuexingan06.cn

Ruby: s[1, 3];  s[1..3]
来源：http://eg.huanxung.cn

C#:   s.Substring(1, 3)
来源：http://tp.chemitech.net.cn

[E04] 查找子串位置
来源：http://sr.lnxyls.cn

Py:   s.find("x");  s.index("x")
来源：http://fd.jctech888.com.cn

PHP:  strpos($s, "x");
来源：http://sw.newstarts.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://im.shxzukj.cn

TS:   s.indexOf("x")
来源：http://hd.newstarts.cn

Java: s.indexOf("x")
来源：http://yr.newstarts.cn

Go:   strings.Index(s, "x")
来源：http://hx.bookmarksfly.cn

Ruby: s.index("x")
来源：http://tn.bjjhwx.cn

C#:   s.IndexOf("x")
来源：http://at.jianghongdianzi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ls.9csxet.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ti.gzmigu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ee.shxzskj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://un.bookmarksfly.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://bp.yuexingan06.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fz.jianghongdianzi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hb.huixinmuqiang.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gk.bookmarksfly.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qy.szxytkj.cn

[E06] 替换子串
来源：http://ab.hahajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ux.yuntaijiaju.cn

PHP:  str_replace("a", "b", $s);
来源：http://dw.huanxung.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://be.hahajie.cn

TS:   s.replaceAll("a", "b")
来源：http://lw.muxihuayi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qa.newstarts.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lk.newstarts.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pt.nszjky.cn

C#:   s.Replace("a", "b")
来源：http://sh.shxzukj.cn

[E07] 按分隔符拆分
来源：http://by.521024.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mw.shxzskj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hp.shxzukj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://vu.bookmarksfly.cn

TS:   s.split(",")
来源：http://mz.muxihuayi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ap.shtwfgs.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ld.shxzskj.cn

Ruby: s.split(",");  s.split
来源：http://rt.9csxet.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xu.jctech888.com.cn

[E08] 数组按分隔符合并
来源：http://dj.huixiangedu.cn

Py:   ",".join(items)
来源：http://ng.nicolike.cn

PHP:  implode(",", $items);
来源：http://bp.yuntaijiaju.cn

JS:   items.join(",")
来源：http://nj.shtwfgs.cn

TS:   items.join(",")
来源：http://zp.huixiangedu.cn

Java: String.join(",", items)
来源：http://nz.asd995.cn

Go:   strings.Join(items, ",")
来源：http://mv.huanxung.cn

Ruby: items.join(",")
来源：http://tt.gzmigu.cn

C#:   string.Join(",", items)
来源：http://iy.nszjky.cn

[E09] 去除所有空白字符
来源：http://pg.huanxung.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fd.shxzskj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tf.szsharing.cn

JS:   s.replace(/\s+/g, "")
来源：http://eh.colortex.cn

TS:   s.replace(/\s+/g, "")
来源：http://cd.muxihuayi.cn

Java: s.replaceAll("\\s+", "")
来源：http://ap.muxihuayi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://re.chemitech.net.cn

Ruby: s.gsub(/\s+/, "")
来源：http://bj.hnjuh.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jy.asd995.cn

[E10] 左侧补零 / 定长填充
来源：http://mr.szxytkj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xv.bjjhwx.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bf.szsharing.cn

JS:   "7".padStart(3, "0")
来源：http://ae.yuntaijiaju.cn

TS:   "7".padStart(3, "0")
来源：http://nb.yuntaijiaju.cn

Java: String.format("%03d", 7)
来源：http://mz.asd995.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ds.lnxyls.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://en.haigaiapp.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hs.newstarts.cn

[E11] 反转字符串
来源：http://nu.bookmarksfly.cn

Py:   s[::-1]
来源：http://yj.shtwfgs.cn

PHP:  strrev($s);
来源：http://ha.bookmarksfly.cn

JS:   [...s].reverse().join("")
来源：http://vh.chemitech.net.cn

TS:   [...s].reverse().join("")
来源：http://ll.wgjwhj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://mk.jianghongdianzi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://fj.huixinmuqiang.cn

Ruby: s.reverse
来源：http://as.shtwfgs.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ke.wgjwhj.cn

[E12] 统计某字符出现次数
来源：http://hh.huixiangedu.cn

Py:   s.count("a")
来源：http://he.newstarts.cn

PHP:  substr_count($s, "a");
来源：http://ql.hnjuh.cn

JS:   s.split("a").length - 1
来源：http://dm.huixiangedu.cn

TS:   s.split("a").length - 1
来源：http://zp.nicolike.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ga.szxytkj.cn

Go:   strings.Count(s, "a")
来源：http://et.jianghongdianzi.cn

Ruby: s.count("a")
来源：http://lp.nszjky.cn

C#:   s.Count(c => c == 'a')
来源：http://or.shtwfgs.cn

[E13] 逐字符遍历
来源：http://gi.huixinmuqiang.cn

Py:   for ch in s: print(ch)
来源：http://gi.9csxet.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wz.colortex.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://rv.nszjky.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://nj.hahajie.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qg.nszjky.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://na.shxzukj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://gw.nszjky.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zo.nszjky.cn

[E14] URL 编码与 Base64
来源：http://fo.hnjuh.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kn.hnjuh.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qk.gzmigu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://be.shtwfgs.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://as.gzmigu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zm.wgjwhj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kr.huanxung.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vr.yuexingan06.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://al.gzmigu.cn

[E15] HTML 转义 / 反转义
来源：http://yl.nszjky.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://mv.haigaiapp.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://za.nszjky.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bh.nszjky.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://uy.jianghongdianzi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kt.shtwfgs.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qn.jianghongdianzi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bm.shxzukj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ie.wgjwhj.cn

[E16] 数字千分位
来源：http://uz.jianghongdianzi.cn

Py:   f"{1234567:,}"
来源：http://fs.jctech888.com.cn

PHP:  number_format(1234567);
来源：http://vv.asd995.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://hp.newstarts.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://yv.nicolike.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rj.shxzukj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qe.jianghongdianzi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://iu.bookmarksfly.cn

C#:   1234567.ToString("N0")
来源：http://or.521024.cn

[E17] 首字母大写
来源：http://kr.yuexingan06.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ds.shtwfgs.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://my.lnxyls.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wy.bookmarksfly.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hu.nicolike.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://md.haigaiapp.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mj.colortex.cn

Ruby: s.capitalize
来源：http://kn.yuntaijiaju.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gj.shxzukj.cn

[E18] 模板占位符替换
来源：http://nk.nszjky.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ao.szxytkj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jz.huixinmuqiang.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://oy.hahajie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://gk.nicolike.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ab.nszjky.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ox.haigaiapp.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ua.bjjhwx.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ko.hahajie.cn

[E19] 多行文本按行拆分
来源：http://kz.panjiajie.cn

Py:   s.splitlines()
来源：http://vn.521024.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://go.huanxung.cn

JS:   s.split(/\r?\n/)
来源：http://ny.huixinmuqiang.cn

TS:   s.split(/\r?\n/)
来源：http://cg.shtwfgs.cn

Java: s.lines().toList()
来源：http://nc.shxzskj.cn

Go:   strings.Split(s, "\n")
来源：http://rw.nszjky.cn

Ruby: s.lines
来源：http://hp.hnjuh.cn

C#:   s.Split('\n')
来源：http://yy.huixiangedu.cn

[E20] 判断字符串是否为空
来源：http://bn.haigaiapp.cn

Py:   if not s:
来源：http://qc.521024.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qm.newstarts.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lh.shtwfgs.cn

TS:   if (s === "") {}
来源：http://et.gzmigu.cn

Java: if (s.isEmpty()) {}
来源：http://ev.hahajie.cn

Go:   if s == "" {}
来源：http://rl.nicolike.cn

Ruby: if s.empty?
来源：http://gz.nszjky.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://km.szsharing.cn

[E21] 超长截断加省略号
来源：http://te.bookmarksfly.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://oh.huixinmuqiang.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://td.hahajie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ey.hnjuh.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://so.9csxet.cn


<!-- 参考信息 -->