代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yq.lnxyls.cn

JS:   arr.filter(x => x > 3)
来源：http://xf.shxzukj.cn

TS:   arr.filter(x => x > 3)
来源：http://qd.shxzskj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://az.gzmigu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dx.chemitech.net.cn

Ruby: arr.select { |x| x > 3 }
来源：http://gs.521024.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://hj.panjiajie.cn

[D14] 映射转换（每个元素变形）
来源：http://jw.bjjhwx.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zp.gzmigu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yw.yuntaijiaju.cn

JS:   arr.map(x => x * 2)
来源：http://xj.bookmarksfly.cn

TS:   arr.map(x => x * 2)
来源：http://fo.jctech888.com.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://an.9csxet.cn

Go:   // 手写循环
来源：http://bs.huanxung.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fz.hnjuh.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://cn.huixiangedu.cn

[D15] 去重
来源：http://cs.shxzukj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ks.chemitech.net.cn

PHP:  array_unique($arr);
来源：http://pl.panjiajie.cn

JS:   [...new Set(arr)]
来源：http://mt.nicolike.cn

TS:   [...new Set(arr)]
来源：http://vf.newstarts.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ga.shxzskj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://se.panjiajie.cn

Ruby: arr.uniq
来源：http://fn.jianghongdianzi.cn

C#:   list.Distinct().ToList()
来源：http://oj.bookmarksfly.cn

[D16] 求和与平均值
来源：http://ab.huanxung.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gk.panjiajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xj.newstarts.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zc.shxzskj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sl.panjiajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kh.shtwfgs.cn

Go:   // 手写循环累加
来源：http://pl.asd995.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://sk.chemitech.net.cn

C#:   list.Sum();  list.Average()
来源：http://ud.nszjky.cn

[D17] 最大值与最小值
来源：http://si.gzmigu.cn

Py:   max(arr);  min(arr)
来源：http://ap.nicolike.cn

PHP:  max($arr);  min($arr);
来源：http://so.szsharing.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zc.shxzskj.cn

TS:   Math.max(...arr);
来源：http://yg.hnjuh.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://xw.bjjhwx.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://he.asd995.cn

Ruby: arr.max;  arr.min
来源：http://bz.yuexingan06.cn

C#:   list.Max();  list.Min()
来源：http://uj.hnjuh.cn

[D18] 扁平化嵌套数组
来源：http://sc.muxihuayi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dm.nszjky.cn

PHP:  array_merge(...$nested);
来源：http://yy.szsharing.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mw.yuexingan06.cn

TS:   nested.flat();
来源：http://bw.shxzukj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qw.521024.cn

Go:   // 手写双层循环
来源：http://uk.nszjky.cn

Ruby: nested.flatten
来源：http://mp.haigaiapp.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://lk.hnjuh.cn

[D19] 按字段分组
来源：http://yg.nicolike.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pt.hnjuh.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lj.jctech888.com.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ld.nszjky.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://hc.lnxyls.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vp.panjiajie.cn

Go:   // 手写 map[string][]T
来源：http://fp.521024.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://bp.szxytkj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ax.yuntaijiaju.cn

[D20] 统计每个元素出现次数
来源：http://id.nszjky.cn

Py:   Counter(arr)
来源：http://hu.nicolike.cn

PHP:  array_count_values($arr);
来源：http://os.yuexingan06.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ya.shxzukj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yz.yuntaijiaju.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ra.bookmarksfly.cn

Go:   // 手写 map[T]int
来源：http://nw.szxytkj.cn

Ruby: arr.tally
来源：http://ta.jctech888.com.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gj.jianghongdianzi.cn

[D21] 判断是否包含某元素
来源：http://nd.lnxyls.cn

Py:   x in arr
来源：http://sy.panjiajie.cn

PHP:  in_array($x, $arr, true);
来源：http://ab.muxihuayi.cn

JS:   arr.includes(x)
来源：http://dh.colortex.cn

TS:   arr.includes(x)
来源：http://nh.hnjuh.cn

Java: list.contains(x)
来源：http://hu.nszjky.cn

Go:   slices.Contains(arr, x)
来源：http://no.521024.cn

Ruby: arr.include?(x)
来源：http://re.muxihuayi.cn

C#:   list.Contains(x)
来源：http://xz.panjiajie.cn

[D22] 复制数组（避免共享引用）
来源：http://mk.lnxyls.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ak.jctech888.com.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xb.shtwfgs.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ka.asd995.cn

TS:   [...arr];
来源：http://to.huixiangedu.cn

Java: new ArrayList<>(list);
来源：http://lz.yuexingan06.cn

Go:   copied := append([]int(nil), arr...)
来源：http://sp.szxytkj.cn

Ruby: arr.dup;  arr.clone
来源：http://dd.9csxet.cn

C#:   new List<int>(list);
来源：http://wq.shxzskj.cn

[D23] reduce 累积计算
来源：http://qv.gzmigu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gr.huanxung.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ap.nszjky.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ed.shxzukj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rq.colortex.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://lj.yuntaijiaju.cn

Go:   // 手写循环
来源：http://tl.shxzukj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ir.shxzukj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://be.asd995.cn

[D24] 字典 / Map 基本操作
来源：http://ul.bookmarksfly.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vl.jianghongdianzi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dz.gzmigu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hk.huanxung.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rw.colortex.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tz.jctech888.com.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xm.gzmigu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://in.bookmarksfly.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hf.nicolike.cn

[D25] Set 集合去重与交并差
来源：http://ej.panjiajie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rh.muxihuayi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fj.huixinmuqiang.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zz.9csxet.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://il.huixiangedu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cs.jctech888.com.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://my.9csxet.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ag.asd995.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ou.hnjuh.cn

[D26] 数组转字符串
来源：http://lz.colortex.cn

Py:   ", ".join(map(str, arr))
来源：http://fh.nszjky.cn

PHP:  implode(", ", $arr);
来源：http://vh.huanxung.cn

JS:   arr.join(", ")
来源：http://ac.asd995.cn

TS:   arr.join(", ")
来源：http://wc.asd995.cn

Java: String.join(", ", list)
来源：http://wc.haigaiapp.cn

Go:   strings.Join(strs, ", ")
来源：http://mg.haigaiapp.cn

Ruby: arr.join(", ")
来源：http://zp.jctech888.com.cn

C#:   string.Join(", ", list)
来源：http://bn.muxihuayi.cn

================================================================================
来源：http://pf.szxytkj.cn

E. 字符串处理
来源：http://jw.jianghongdianzi.cn

================================================================================
来源：http://ay.szsharing.cn

[E01] 拼接字符串
来源：http://pc.yuntaijiaju.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rj.jianghongdianzi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://df.yuntaijiaju.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vj.9csxet.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jb.gzmigu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yp.jianghongdianzi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xd.hnjuh.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vh.yuntaijiaju.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qb.shtwfgs.cn

[E02] 重复字符串
来源：http://uw.nicolike.cn

Py:   "ab" * 3
来源：http://cl.521024.cn

PHP:  str_repeat("ab", 3);
来源：http://kt.bookmarksfly.cn

JS:   "ab".repeat(3)
来源：http://tq.newstarts.cn

TS:   "ab".repeat(3)
来源：http://oq.jctech888.com.cn

Java: "ab".repeat(3)
来源：http://ma.muxihuayi.cn

Go:   strings.Repeat("ab", 3)
来源：http://eu.wgjwhj.cn

Ruby: "ab" * 3
来源：http://nl.panjiajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ma.haigaiapp.cn

[E03] 截取子串
来源：http://sw.jianghongdianzi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://oc.9csxet.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://om.jianghongdianzi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mg.521024.cn

TS:   s.slice(1, 4)
来源：http://hp.szxytkj.cn

Java: s.substring(1, 4)
来源：http://gb.bookmarksfly.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://oj.hahajie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ch.jianghongdianzi.cn

C#:   s.Substring(1, 3)
来源：http://ax.asd995.cn

[E04] 查找子串位置
来源：http://ly.bookmarksfly.cn

Py:   s.find("x");  s.index("x")
来源：http://mi.jianghongdianzi.cn

PHP:  strpos($s, "x");
来源：http://ty.bookmarksfly.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pc.nicolike.cn

TS:   s.indexOf("x")
来源：http://sk.panjiajie.cn

Java: s.indexOf("x")
来源：http://qx.newstarts.cn

Go:   strings.Index(s, "x")
来源：http://bb.wgjwhj.cn

Ruby: s.index("x")
来源：http://wq.bookmarksfly.cn

C#:   s.IndexOf("x")
来源：http://ys.hnjuh.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://qr.521024.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rb.chemitech.net.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wo.hnjuh.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tv.muxihuayi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ei.nszjky.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fw.nicolike.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hn.hahajie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lu.gzmigu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rk.asd995.cn

[E06] 替换子串
来源：http://lc.newstarts.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ez.yuexingan06.cn

PHP:  str_replace("a", "b", $s);
来源：http://pq.jctech888.com.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wg.shxzskj.cn

TS:   s.replaceAll("a", "b")
来源：http://aj.hahajie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sv.szxytkj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wp.shxzukj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ym.haigaiapp.cn

C#:   s.Replace("a", "b")
来源：http://ux.bookmarksfly.cn

[E07] 按分隔符拆分
来源：http://di.szxytkj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://eh.newstarts.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vd.huanxung.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://qk.haigaiapp.cn

TS:   s.split(",")
来源：http://ty.yuexingan06.cn

Java: s.split(",");  s.split("\\s+")
来源：http://te.bjjhwx.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://so.nszjky.cn

Ruby: s.split(",");  s.split
来源：http://gg.wgjwhj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://if.shxzskj.cn

[E08] 数组按分隔符合并
来源：http://qr.shxzukj.cn

Py:   ",".join(items)
来源：http://nn.521024.cn

PHP:  implode(",", $items);
来源：http://bh.lnxyls.cn

JS:   items.join(",")
来源：http://xi.muxihuayi.cn

TS:   items.join(",")
来源：http://zq.nicolike.cn

Java: String.join(",", items)
来源：http://lt.bookmarksfly.cn

Go:   strings.Join(items, ",")
来源：http://ye.9csxet.cn

Ruby: items.join(",")
来源：http://gj.lnxyls.cn

C#:   string.Join(",", items)
来源：http://fm.shxzukj.cn

[E09] 去除所有空白字符
来源：http://do.shxzukj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nd.shxzskj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://od.newstarts.cn

JS:   s.replace(/\s+/g, "")
来源：http://xg.asd995.cn

TS:   s.replace(/\s+/g, "")
来源：http://ai.newstarts.cn

Java: s.replaceAll("\\s+", "")
来源：http://xc.jctech888.com.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://tn.shxzukj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://em.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://oz.shxzskj.cn

[E10] 左侧补零 / 定长填充
来源：http://ew.gzmigu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ae.yuexingan06.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tt.panjiajie.cn

JS:   "7".padStart(3, "0")
来源：http://at.jctech888.com.cn

TS:   "7".padStart(3, "0")
来源：http://oc.newstarts.cn

Java: String.format("%03d", 7)
来源：http://op.chemitech.net.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://fz.huixinmuqiang.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tp.asd995.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ok.shtwfgs.cn

[E11] 反转字符串
来源：http://uz.szsharing.cn

Py:   s[::-1]
来源：http://kq.muxihuayi.cn

PHP:  strrev($s);
来源：http://yg.bookmarksfly.cn

JS:   [...s].reverse().join("")
来源：http://as.bjjhwx.cn

TS:   [...s].reverse().join("")
来源：http://jl.bookmarksfly.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://dw.nicolike.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://bs.bookmarksfly.cn

Ruby: s.reverse
来源：http://cp.hahajie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://uu.jctech888.com.cn

[E12] 统计某字符出现次数
来源：http://ml.asd995.cn

Py:   s.count("a")
来源：http://kv.huixinmuqiang.cn

PHP:  substr_count($s, "a");
来源：http://wg.shxzskj.cn

JS:   s.split("a").length - 1
来源：http://bp.shtwfgs.cn

TS:   s.split("a").length - 1
来源：http://hq.nszjky.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gm.jianghongdianzi.cn

Go:   strings.Count(s, "a")
来源：http://bw.shxzukj.cn

Ruby: s.count("a")
来源：http://zf.haigaiapp.cn

C#:   s.Count(c => c == 'a')
来源：http://ch.yuexingan06.cn

[E13] 逐字符遍历
来源：http://lt.hahajie.cn

Py:   for ch in s: print(ch)
来源：http://xg.huixinmuqiang.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zp.gzmigu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://hs.bookmarksfly.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bx.huanxung.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cv.shxzukj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lv.muxihuayi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://eg.hnjuh.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://py.huixinmuqiang.cn

[E14] URL 编码与 Base64
来源：http://bw.521024.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kq.bjjhwx.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ok.lnxyls.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://im.huanxung.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sx.newstarts.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://io.nszjky.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jm.szxytkj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xq.hnjuh.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cd.bjjhwx.cn

[E15] HTML 转义 / 反转义
来源：http://bw.hnjuh.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://oz.huanxung.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ke.521024.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yk.lnxyls.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://be.newstarts.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zo.asd995.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dx.jctech888.com.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://we.shxzukj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ao.jctech888.com.cn

[E16] 数字千分位
来源：http://cb.nszjky.cn

Py:   f"{1234567:,}"
来源：http://wo.bookmarksfly.cn

PHP:  number_format(1234567);
来源：http://le.nszjky.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mj.colortex.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://tf.muxihuayi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qx.lnxyls.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cx.shxzskj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://az.huixiangedu.cn

C#:   1234567.ToString("N0")
来源：http://wq.huanxung.cn

[E17] 首字母大写
来源：http://ob.bjjhwx.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rv.huixiangedu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xo.gzmigu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ku.bookmarksfly.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rg.gzmigu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gt.bookmarksfly.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fz.shtwfgs.cn

Ruby: s.capitalize
来源：http://gk.shxzukj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dx.panjiajie.cn

[E18] 模板占位符替换
来源：http://pt.bookmarksfly.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://di.huanxung.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rf.huixinmuqiang.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://nr.colortex.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ck.asd995.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kh.bookmarksfly.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fh.muxihuayi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wf.bookmarksfly.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xx.huanxung.cn

[E19] 多行文本按行拆分
来源：http://ra.huixiangedu.cn

Py:   s.splitlines()
来源：http://mc.lnxyls.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xg.lnxyls.cn

JS:   s.split(/\r?\n/)
来源：http://jg.jctech888.com.cn

TS:   s.split(/\r?\n/)
来源：http://hj.szxytkj.cn

Java: s.lines().toList()
来源：http://xe.haigaiapp.cn

Go:   strings.Split(s, "\n")
来源：http://xh.bjjhwx.cn

Ruby: s.lines
来源：http://tu.asd995.cn

C#:   s.Split('\n')
来源：http://pg.shxzukj.cn

[E20] 判断字符串是否为空
来源：http://xi.haigaiapp.cn

Py:   if not s:
来源：http://ue.muxihuayi.cn


<!-- 参考信息 -->