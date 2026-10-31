代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ll.panjiajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bw.huanxung.cn

JS:   arr.map(x => x * 2)
来源：http://tq.nicolike.cn

TS:   arr.map(x => x * 2)
来源：http://ox.huanxung.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://mf.9csxet.cn

Go:   // 手写循环
来源：http://el.wgjwhj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://et.9csxet.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://sg.shxzukj.cn

[D15] 去重
来源：http://qn.jianghongdianzi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://am.521024.cn

PHP:  array_unique($arr);
来源：http://oj.huixiangedu.cn

JS:   [...new Set(arr)]
来源：http://rf.9csxet.cn

TS:   [...new Set(arr)]
来源：http://sw.szxytkj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zv.shtwfgs.cn

Go:   // 用 map[T]struct{} 手写
来源：http://av.huanxung.cn

Ruby: arr.uniq
来源：http://rr.bookmarksfly.cn

C#:   list.Distinct().ToList()
来源：http://kd.shxzskj.cn

[D16] 求和与平均值
来源：http://zy.haigaiapp.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mj.huixinmuqiang.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qa.shxzukj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nk.huixiangedu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ju.szxytkj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ge.haigaiapp.cn

Go:   // 手写循环累加
来源：http://tl.shxzukj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hj.muxihuayi.cn

C#:   list.Sum();  list.Average()
来源：http://lq.yuexingan06.cn

[D17] 最大值与最小值
来源：http://tg.bookmarksfly.cn

Py:   max(arr);  min(arr)
来源：http://yz.shxzukj.cn

PHP:  max($arr);  min($arr);
来源：http://lr.nicolike.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zr.colortex.cn

TS:   Math.max(...arr);
来源：http://bj.jctech888.com.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://eh.szxytkj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ng.yuexingan06.cn

Ruby: arr.max;  arr.min
来源：http://hh.yuntaijiaju.cn

C#:   list.Max();  list.Min()
来源：http://nb.521024.cn

[D18] 扁平化嵌套数组
来源：http://yk.nicolike.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://aj.jctech888.com.cn

PHP:  array_merge(...$nested);
来源：http://gz.nicolike.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://uk.shxzukj.cn

TS:   nested.flat();
来源：http://gt.hnjuh.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vi.jctech888.com.cn

Go:   // 手写双层循环
来源：http://eb.nszjky.cn

Ruby: nested.flatten
来源：http://tw.shxzskj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://it.jctech888.com.cn

[D19] 按字段分组
来源：http://vn.yuntaijiaju.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pl.jianghongdianzi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pe.asd995.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nx.yuexingan06.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://de.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://eg.yuntaijiaju.cn

Go:   // 手写 map[string][]T
来源：http://bs.newstarts.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rs.newstarts.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pw.gzmigu.cn

[D20] 统计每个元素出现次数
来源：http://yr.shxzukj.cn

Py:   Counter(arr)
来源：http://mc.asd995.cn

PHP:  array_count_values($arr);
来源：http://ug.yuntaijiaju.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://er.bjjhwx.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uf.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://aw.huixiangedu.cn

Go:   // 手写 map[T]int
来源：http://fu.szxytkj.cn

Ruby: arr.tally
来源：http://nu.szxytkj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://da.jctech888.com.cn

[D21] 判断是否包含某元素
来源：http://qi.nszjky.cn

Py:   x in arr
来源：http://xi.chemitech.net.cn

PHP:  in_array($x, $arr, true);
来源：http://az.szxytkj.cn

JS:   arr.includes(x)
来源：http://nf.jianghongdianzi.cn

TS:   arr.includes(x)
来源：http://rd.nszjky.cn

Java: list.contains(x)
来源：http://sh.wgjwhj.cn

Go:   slices.Contains(arr, x)
来源：http://sj.muxihuayi.cn

Ruby: arr.include?(x)
来源：http://od.jctech888.com.cn

C#:   list.Contains(x)
来源：http://fg.hahajie.cn

[D22] 复制数组（避免共享引用）
来源：http://xs.9csxet.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://sy.521024.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mb.muxihuayi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fp.wgjwhj.cn

TS:   [...arr];
来源：http://dz.nszjky.cn

Java: new ArrayList<>(list);
来源：http://zo.jctech888.com.cn

Go:   copied := append([]int(nil), arr...)
来源：http://oa.huanxung.cn

Ruby: arr.dup;  arr.clone
来源：http://yq.bjjhwx.cn

C#:   new List<int>(list);
来源：http://nl.huixinmuqiang.cn

[D23] reduce 累积计算
来源：http://cn.shxzukj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://aq.shxzukj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uj.yuntaijiaju.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ze.asd995.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gc.muxihuayi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://gf.jianghongdianzi.cn

Go:   // 手写循环
来源：http://bw.9csxet.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fz.jianghongdianzi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qa.panjiajie.cn

[D24] 字典 / Map 基本操作
来源：http://wq.muxihuayi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ya.bookmarksfly.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ay.hahajie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gh.9csxet.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jc.bjjhwx.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://en.wgjwhj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xk.szsharing.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bp.colortex.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jg.asd995.cn

[D25] Set 集合去重与交并差
来源：http://ex.hahajie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://oq.yuexingan06.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cv.shxzukj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ys.521024.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ek.yuntaijiaju.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dm.colortex.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wg.bookmarksfly.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bs.wgjwhj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://an.shtwfgs.cn

[D26] 数组转字符串
来源：http://cl.huixinmuqiang.cn

Py:   ", ".join(map(str, arr))
来源：http://vi.yuexingan06.cn

PHP:  implode(", ", $arr);
来源：http://dw.chemitech.net.cn

JS:   arr.join(", ")
来源：http://oz.chemitech.net.cn

TS:   arr.join(", ")
来源：http://db.shxzukj.cn

Java: String.join(", ", list)
来源：http://dx.huanxung.cn

Go:   strings.Join(strs, ", ")
来源：http://lo.shxzskj.cn

Ruby: arr.join(", ")
来源：http://ai.bookmarksfly.cn

C#:   string.Join(", ", list)
来源：http://fc.newstarts.cn

================================================================================
来源：http://an.huanxung.cn

E. 字符串处理
来源：http://se.yuntaijiaju.cn

================================================================================
来源：http://pg.bjjhwx.cn

[E01] 拼接字符串
来源：http://do.colortex.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://aw.asd995.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://po.chemitech.net.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://re.nicolike.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ux.521024.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rf.chemitech.net.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pi.hnjuh.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fl.asd995.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xr.huixinmuqiang.cn

[E02] 重复字符串
来源：http://xd.chemitech.net.cn

Py:   "ab" * 3
来源：http://cx.yuntaijiaju.cn

PHP:  str_repeat("ab", 3);
来源：http://pq.szsharing.cn

JS:   "ab".repeat(3)
来源：http://jl.panjiajie.cn

TS:   "ab".repeat(3)
来源：http://sc.bjjhwx.cn

Java: "ab".repeat(3)
来源：http://tq.yuexingan06.cn

Go:   strings.Repeat("ab", 3)
来源：http://mo.jctech888.com.cn

Ruby: "ab" * 3
来源：http://if.newstarts.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wy.9csxet.cn

[E03] 截取子串
来源：http://py.nszjky.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bk.asd995.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://br.panjiajie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hn.521024.cn

TS:   s.slice(1, 4)
来源：http://ei.shxzukj.cn

Java: s.substring(1, 4)
来源：http://km.bookmarksfly.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bz.gzmigu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://wp.521024.cn

C#:   s.Substring(1, 3)
来源：http://hg.shxzskj.cn

[E04] 查找子串位置
来源：http://ub.colortex.cn

Py:   s.find("x");  s.index("x")
来源：http://wn.hahajie.cn

PHP:  strpos($s, "x");
来源：http://gh.hnjuh.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qn.9csxet.cn

TS:   s.indexOf("x")
来源：http://al.szsharing.cn

Java: s.indexOf("x")
来源：http://ql.szxytkj.cn

Go:   strings.Index(s, "x")
来源：http://uh.chemitech.net.cn

Ruby: s.index("x")
来源：http://cx.gzmigu.cn

C#:   s.IndexOf("x")
来源：http://od.nicolike.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://iz.lnxyls.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://px.jctech888.com.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cn.shxzukj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ng.asd995.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://yp.jianghongdianzi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dc.yuntaijiaju.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ld.nszjky.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dr.huixiangedu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qa.huixinmuqiang.cn

[E06] 替换子串
来源：http://yf.hahajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vr.jctech888.com.cn

PHP:  str_replace("a", "b", $s);
来源：http://lp.lnxyls.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gt.521024.cn

TS:   s.replaceAll("a", "b")
来源：http://mt.huanxung.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dn.shtwfgs.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dv.yuntaijiaju.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pu.hnjuh.cn

C#:   s.Replace("a", "b")
来源：http://lz.bookmarksfly.cn

[E07] 按分隔符拆分
来源：http://xg.szxytkj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bu.lnxyls.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yz.jctech888.com.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://qb.yuexingan06.cn

TS:   s.split(",")
来源：http://eu.bookmarksfly.cn

Java: s.split(",");  s.split("\\s+")
来源：http://qa.9csxet.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yt.huanxung.cn

Ruby: s.split(",");  s.split
来源：http://kf.newstarts.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://el.yuntaijiaju.cn

[E08] 数组按分隔符合并
来源：http://qa.521024.cn

Py:   ",".join(items)
来源：http://zu.nicolike.cn

PHP:  implode(",", $items);
来源：http://ar.panjiajie.cn

JS:   items.join(",")
来源：http://nf.bjjhwx.cn

TS:   items.join(",")
来源：http://sv.shxzskj.cn

Java: String.join(",", items)
来源：http://wh.haigaiapp.cn

Go:   strings.Join(items, ",")
来源：http://jc.521024.cn

Ruby: items.join(",")
来源：http://wa.asd995.cn

C#:   string.Join(",", items)
来源：http://qz.gzmigu.cn

[E09] 去除所有空白字符
来源：http://dq.chemitech.net.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://oz.521024.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xe.yuexingan06.cn

JS:   s.replace(/\s+/g, "")
来源：http://zk.jianghongdianzi.cn

TS:   s.replace(/\s+/g, "")
来源：http://fy.shxzukj.cn

Java: s.replaceAll("\\s+", "")
来源：http://li.shxzukj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://gr.bjjhwx.cn

Ruby: s.gsub(/\s+/, "")
来源：http://bx.newstarts.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zk.szsharing.cn

[E10] 左侧补零 / 定长填充
来源：http://wi.bookmarksfly.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yl.bookmarksfly.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zv.jctech888.com.cn

JS:   "7".padStart(3, "0")
来源：http://kx.bjjhwx.cn

TS:   "7".padStart(3, "0")
来源：http://ws.shxzskj.cn

Java: String.format("%03d", 7)
来源：http://vr.jctech888.com.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://kh.bjjhwx.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bh.newstarts.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ks.9csxet.cn

[E11] 反转字符串
来源：http://gd.wgjwhj.cn

Py:   s[::-1]
来源：http://nz.nszjky.cn

PHP:  strrev($s);
来源：http://at.shxzskj.cn

JS:   [...s].reverse().join("")
来源：http://ly.muxihuayi.cn

TS:   [...s].reverse().join("")
来源：http://az.nicolike.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://tx.nszjky.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://as.shxzukj.cn

Ruby: s.reverse
来源：http://tu.shtwfgs.cn

C#:   new string(s.Reverse().ToArray())
来源：http://cr.shxzskj.cn

[E12] 统计某字符出现次数
来源：http://df.nszjky.cn

Py:   s.count("a")
来源：http://rd.9csxet.cn

PHP:  substr_count($s, "a");
来源：http://ar.bjjhwx.cn

JS:   s.split("a").length - 1
来源：http://wr.colortex.cn

TS:   s.split("a").length - 1
来源：http://bt.jctech888.com.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://em.lnxyls.cn

Go:   strings.Count(s, "a")
来源：http://tf.szsharing.cn

Ruby: s.count("a")
来源：http://hn.hnjuh.cn

C#:   s.Count(c => c == 'a')
来源：http://ei.hahajie.cn

[E13] 逐字符遍历
来源：http://xi.huixiangedu.cn

Py:   for ch in s: print(ch)
来源：http://td.shxzukj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yx.shxzukj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://vf.colortex.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://yl.9csxet.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xi.newstarts.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ra.wgjwhj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ed.bjjhwx.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://co.huixiangedu.cn

[E14] URL 编码与 Base64
来源：http://kt.nszjky.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cb.wgjwhj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://it.chemitech.net.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://sh.gzmigu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jz.chemitech.net.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dz.jianghongdianzi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bq.muxihuayi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lr.nszjky.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tp.gzmigu.cn

[E15] HTML 转义 / 反转义
来源：http://kh.shtwfgs.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://aj.bookmarksfly.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mk.huixinmuqiang.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fl.chemitech.net.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://jt.yuntaijiaju.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hc.521024.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ex.shxzukj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gi.521024.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://po.nicolike.cn

[E16] 数字千分位
来源：http://uo.wgjwhj.cn

Py:   f"{1234567:,}"
来源：http://rl.yuexingan06.cn

PHP:  number_format(1234567);
来源：http://dp.haigaiapp.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ch.panjiajie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://uj.nszjky.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://th.huixiangedu.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mf.hnjuh.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tk.hahajie.cn

C#:   1234567.ToString("N0")
来源：http://gv.yuntaijiaju.cn

[E17] 首字母大写
来源：http://zd.colortex.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cs.asd995.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ie.haigaiapp.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rj.muxihuayi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ie.szsharing.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rb.szsharing.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ym.bookmarksfly.cn

Ruby: s.capitalize
来源：http://xg.asd995.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pi.bjjhwx.cn

[E18] 模板占位符替换
来源：http://ar.nicolike.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ms.newstarts.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rd.huanxung.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xe.muxihuayi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://wk.shxzukj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zf.shtwfgs.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://el.yuntaijiaju.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bb.yuntaijiaju.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lh.haigaiapp.cn

[E19] 多行文本按行拆分
来源：http://sf.9csxet.cn

Py:   s.splitlines()
来源：http://mp.hahajie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jt.haigaiapp.cn

JS:   s.split(/\r?\n/)
来源：http://ic.panjiajie.cn

TS:   s.split(/\r?\n/)
来源：http://lt.shtwfgs.cn

Java: s.lines().toList()
来源：http://rq.yuntaijiaju.cn

Go:   strings.Split(s, "\n")
来源：http://wk.szsharing.cn

Ruby: s.lines
来源：http://bh.wgjwhj.cn

C#:   s.Split('\n')
来源：http://tw.shtwfgs.cn

[E20] 判断字符串是否为空
来源：http://nl.521024.cn

Py:   if not s:
来源：http://aa.newstarts.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xv.huixiangedu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://th.muxihuayi.cn

TS:   if (s === "") {}
来源：http://dj.nicolike.cn

Java: if (s.isEmpty()) {}
来源：http://uq.huixiangedu.cn

Go:   if s == "" {}
来源：http://lb.jctech888.com.cn

Ruby: if s.empty?
来源：http://lz.yuntaijiaju.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://za.panjiajie.cn

[E21] 超长截断加省略号
来源：http://mk.huixiangedu.cn


<!-- 参考信息 -->