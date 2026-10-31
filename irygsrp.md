代发 wailian999

Ruby: arr.index(x)
来源：http://yc.jianghongdianzi.cn

C#:   list.IndexOf(x);
来源：http://aw.hahajie.cn

[D13] 过滤（保留满足条件的）
来源：http://jb.yuntaijiaju.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wo.haigaiapp.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qp.hnjuh.cn

JS:   arr.filter(x => x > 3)
来源：http://wl.szsharing.cn

TS:   arr.filter(x => x > 3)
来源：http://zb.shxzukj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://li.9csxet.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mc.panjiajie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://va.haigaiapp.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://wa.yuntaijiaju.cn

[D14] 映射转换（每个元素变形）
来源：http://vm.chemitech.net.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cr.huanxung.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ip.shxzukj.cn

JS:   arr.map(x => x * 2)
来源：http://hj.lnxyls.cn

TS:   arr.map(x => x * 2)
来源：http://qf.nszjky.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://js.yuntaijiaju.cn

Go:   // 手写循环
来源：http://vm.lnxyls.cn

Ruby: arr.map { |x| x * 2 }
来源：http://nm.chemitech.net.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ee.nicolike.cn

[D15] 去重
来源：http://gh.shtwfgs.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nq.yuntaijiaju.cn

PHP:  array_unique($arr);
来源：http://xm.nicolike.cn

JS:   [...new Set(arr)]
来源：http://fa.shxzukj.cn

TS:   [...new Set(arr)]
来源：http://iv.huixinmuqiang.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://en.jctech888.com.cn

Go:   // 用 map[T]struct{} 手写
来源：http://uj.szxytkj.cn

Ruby: arr.uniq
来源：http://tf.colortex.cn

C#:   list.Distinct().ToList()
来源：http://zq.9csxet.cn

[D16] 求和与平均值
来源：http://nq.521024.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dz.shxzskj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hs.shxzukj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xh.shxzukj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nh.szxytkj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://oy.shxzukj.cn

Go:   // 手写循环累加
来源：http://fg.jctech888.com.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hy.jianghongdianzi.cn

C#:   list.Sum();  list.Average()
来源：http://vo.bjjhwx.cn

[D17] 最大值与最小值
来源：http://dw.szxytkj.cn

Py:   max(arr);  min(arr)
来源：http://uq.panjiajie.cn

PHP:  max($arr);  min($arr);
来源：http://un.bjjhwx.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://so.nszjky.cn

TS:   Math.max(...arr);
来源：http://vp.haigaiapp.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://th.lnxyls.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zy.colortex.cn

Ruby: arr.max;  arr.min
来源：http://qv.shtwfgs.cn

C#:   list.Max();  list.Min()
来源：http://du.haigaiapp.cn

[D18] 扁平化嵌套数组
来源：http://if.hnjuh.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ed.szsharing.cn

PHP:  array_merge(...$nested);
来源：http://kr.huixiangedu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ev.muxihuayi.cn

TS:   nested.flat();
来源：http://pp.chemitech.net.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qo.szxytkj.cn

Go:   // 手写双层循环
来源：http://bw.shtwfgs.cn

Ruby: nested.flatten
来源：http://fk.chemitech.net.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ok.wgjwhj.cn

[D19] 按字段分组
来源：http://kx.szsharing.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cu.huixiangedu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cx.chemitech.net.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dc.nszjky.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://oj.muxihuayi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cv.521024.cn

Go:   // 手写 map[string][]T
来源：http://ev.szxytkj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ah.szsharing.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xg.gzmigu.cn

[D20] 统计每个元素出现次数
来源：http://ba.szxytkj.cn

Py:   Counter(arr)
来源：http://yd.yuntaijiaju.cn

PHP:  array_count_values($arr);
来源：http://dm.hahajie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mf.hahajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ld.huixinmuqiang.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ir.huanxung.cn

Go:   // 手写 map[T]int
来源：http://yb.huanxung.cn

Ruby: arr.tally
来源：http://vs.hnjuh.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://st.bjjhwx.cn

[D21] 判断是否包含某元素
来源：http://sk.newstarts.cn

Py:   x in arr
来源：http://ya.colortex.cn

PHP:  in_array($x, $arr, true);
来源：http://se.szsharing.cn

JS:   arr.includes(x)
来源：http://si.wgjwhj.cn

TS:   arr.includes(x)
来源：http://xf.asd995.cn

Java: list.contains(x)
来源：http://me.yuexingan06.cn

Go:   slices.Contains(arr, x)
来源：http://yv.bookmarksfly.cn

Ruby: arr.include?(x)
来源：http://rg.yuexingan06.cn

C#:   list.Contains(x)
来源：http://wj.hnjuh.cn

[D22] 复制数组（避免共享引用）
来源：http://zn.bjjhwx.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nk.9csxet.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zs.lnxyls.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://un.chemitech.net.cn

TS:   [...arr];
来源：http://wu.jctech888.com.cn

Java: new ArrayList<>(list);
来源：http://kl.huixinmuqiang.cn

Go:   copied := append([]int(nil), arr...)
来源：http://aj.lnxyls.cn

Ruby: arr.dup;  arr.clone
来源：http://aa.shxzskj.cn

C#:   new List<int>(list);
来源：http://pw.hnjuh.cn

[D23] reduce 累积计算
来源：http://wf.bookmarksfly.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ii.shtwfgs.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kx.shxzukj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ag.yuntaijiaju.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kd.asd995.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ui.asd995.cn

Go:   // 手写循环
来源：http://vn.bookmarksfly.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lf.gzmigu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yu.bookmarksfly.cn

[D24] 字典 / Map 基本操作
来源：http://pe.yuntaijiaju.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cy.nicolike.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ha.muxihuayi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xn.bjjhwx.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gr.lnxyls.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fc.nicolike.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xc.shxzskj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zv.lnxyls.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://sx.haigaiapp.cn

[D25] Set 集合去重与交并差
来源：http://lx.nszjky.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gp.shtwfgs.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wq.szxytkj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ez.hnjuh.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://he.521024.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xr.colortex.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fr.huixinmuqiang.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pb.colortex.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hj.nicolike.cn

[D26] 数组转字符串
来源：http://ot.szxytkj.cn

Py:   ", ".join(map(str, arr))
来源：http://yw.haigaiapp.cn

PHP:  implode(", ", $arr);
来源：http://sx.huixiangedu.cn

JS:   arr.join(", ")
来源：http://hy.nicolike.cn

TS:   arr.join(", ")
来源：http://sl.asd995.cn

Java: String.join(", ", list)
来源：http://cz.yuexingan06.cn

Go:   strings.Join(strs, ", ")
来源：http://hs.nicolike.cn

Ruby: arr.join(", ")
来源：http://rn.chemitech.net.cn

C#:   string.Join(", ", list)
来源：http://gb.huanxung.cn

================================================================================
来源：http://tb.shxzskj.cn

E. 字符串处理
来源：http://hw.huanxung.cn

================================================================================
来源：http://kl.shxzskj.cn

[E01] 拼接字符串
来源：http://cj.yuexingan06.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ws.szsharing.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ac.yuntaijiaju.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dq.huixinmuqiang.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tk.bookmarksfly.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fv.nicolike.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ui.nszjky.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zx.yuexingan06.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://uy.szxytkj.cn

[E02] 重复字符串
来源：http://so.muxihuayi.cn

Py:   "ab" * 3
来源：http://ra.huanxung.cn

PHP:  str_repeat("ab", 3);
来源：http://ad.9csxet.cn

JS:   "ab".repeat(3)
来源：http://wd.shxzskj.cn

TS:   "ab".repeat(3)
来源：http://sv.panjiajie.cn

Java: "ab".repeat(3)
来源：http://ru.gzmigu.cn

Go:   strings.Repeat("ab", 3)
来源：http://hm.hnjuh.cn

Ruby: "ab" * 3
来源：http://gk.huixinmuqiang.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ne.muxihuayi.cn

[E03] 截取子串
来源：http://lk.chemitech.net.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ha.yuexingan06.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ol.colortex.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ue.yuexingan06.cn

TS:   s.slice(1, 4)
来源：http://ef.bjjhwx.cn

Java: s.substring(1, 4)
来源：http://oz.huixinmuqiang.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qy.muxihuayi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://xw.colortex.cn

C#:   s.Substring(1, 3)
来源：http://km.shtwfgs.cn

[E04] 查找子串位置
来源：http://sy.521024.cn

Py:   s.find("x");  s.index("x")
来源：http://hw.gzmigu.cn

PHP:  strpos($s, "x");
来源：http://df.521024.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ec.nszjky.cn

TS:   s.indexOf("x")
来源：http://mk.huixinmuqiang.cn

Java: s.indexOf("x")
来源：http://is.hnjuh.cn

Go:   strings.Index(s, "x")
来源：http://zx.521024.cn

Ruby: s.index("x")
来源：http://dy.lnxyls.cn

C#:   s.IndexOf("x")
来源：http://so.colortex.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://tg.colortex.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vj.wgjwhj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://gx.nicolike.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vh.yuexingan06.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ci.szxytkj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ta.colortex.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ve.nszjky.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dy.nszjky.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mt.lnxyls.cn

[E06] 替换子串
来源：http://ia.bookmarksfly.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ox.bookmarksfly.cn

PHP:  str_replace("a", "b", $s);
来源：http://dg.hahajie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oo.newstarts.cn

TS:   s.replaceAll("a", "b")
来源：http://xv.panjiajie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://op.nicolike.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kf.colortex.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hu.huanxung.cn

C#:   s.Replace("a", "b")
来源：http://wi.haigaiapp.cn

[E07] 按分隔符拆分
来源：http://np.gzmigu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pj.shxzskj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://go.huixinmuqiang.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://tg.521024.cn

TS:   s.split(",")
来源：http://fo.lnxyls.cn

Java: s.split(",");  s.split("\\s+")
来源：http://fi.bookmarksfly.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kt.muxihuayi.cn

Ruby: s.split(",");  s.split
来源：http://cb.shtwfgs.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vh.muxihuayi.cn

[E08] 数组按分隔符合并
来源：http://xo.hahajie.cn

Py:   ",".join(items)
来源：http://ka.shtwfgs.cn

PHP:  implode(",", $items);
来源：http://qj.bjjhwx.cn

JS:   items.join(",")
来源：http://nu.huanxung.cn

TS:   items.join(",")
来源：http://je.521024.cn

Java: String.join(",", items)
来源：http://pp.asd995.cn

Go:   strings.Join(items, ",")
来源：http://wh.bjjhwx.cn

Ruby: items.join(",")
来源：http://pp.jianghongdianzi.cn

C#:   string.Join(",", items)
来源：http://bb.hahajie.cn

[E09] 去除所有空白字符
来源：http://zz.shxzukj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wj.colortex.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tl.haigaiapp.cn

JS:   s.replace(/\s+/g, "")
来源：http://gq.szxytkj.cn

TS:   s.replace(/\s+/g, "")
来源：http://oc.szsharing.cn

Java: s.replaceAll("\\s+", "")
来源：http://cj.521024.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://gp.shxzskj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://pl.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gb.lnxyls.cn

[E10] 左侧补零 / 定长填充
来源：http://nj.huixiangedu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fa.huixinmuqiang.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kb.yuntaijiaju.cn

JS:   "7".padStart(3, "0")
来源：http://el.shtwfgs.cn

TS:   "7".padStart(3, "0")
来源：http://kq.521024.cn

Java: String.format("%03d", 7)
来源：http://ju.huixiangedu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://se.szxytkj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yo.asd995.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hu.jctech888.com.cn

[E11] 反转字符串
来源：http://rj.shtwfgs.cn

Py:   s[::-1]
来源：http://uy.asd995.cn

PHP:  strrev($s);
来源：http://bg.shtwfgs.cn

JS:   [...s].reverse().join("")
来源：http://ve.yuexingan06.cn

TS:   [...s].reverse().join("")
来源：http://jx.muxihuayi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://qs.jctech888.com.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ef.yuntaijiaju.cn

Ruby: s.reverse
来源：http://ae.wgjwhj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://yy.muxihuayi.cn

[E12] 统计某字符出现次数
来源：http://pq.colortex.cn

Py:   s.count("a")
来源：http://np.jianghongdianzi.cn

PHP:  substr_count($s, "a");
来源：http://nl.nicolike.cn

JS:   s.split("a").length - 1
来源：http://xw.muxihuayi.cn

TS:   s.split("a").length - 1
来源：http://bz.szxytkj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ve.hahajie.cn

Go:   strings.Count(s, "a")
来源：http://mq.hahajie.cn

Ruby: s.count("a")
来源：http://zp.huixinmuqiang.cn

C#:   s.Count(c => c == 'a')
来源：http://wu.bookmarksfly.cn

[E13] 逐字符遍历
来源：http://la.newstarts.cn

Py:   for ch in s: print(ch)
来源：http://bv.gzmigu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wy.muxihuayi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://gw.panjiajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://cs.chemitech.net.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fw.9csxet.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://uh.nszjky.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://bg.muxihuayi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zz.wgjwhj.cn

[E14] URL 编码与 Base64
来源：http://wq.asd995.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ht.chemitech.net.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://yx.huixiangedu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://di.lnxyls.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ba.newstarts.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gm.szsharing.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mx.chemitech.net.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://do.asd995.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zm.hnjuh.cn

[E15] HTML 转义 / 反转义
来源：http://ro.wgjwhj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://gh.bjjhwx.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qb.szxytkj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fn.jctech888.com.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://xv.panjiajie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://er.huixiangedu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hy.huixiangedu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qo.huanxung.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zi.gzmigu.cn

[E16] 数字千分位
来源：http://do.muxihuayi.cn

Py:   f"{1234567:,}"
来源：http://rz.jctech888.com.cn

PHP:  number_format(1234567);
来源：http://qm.chemitech.net.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://pc.szsharing.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ip.szsharing.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nj.bookmarksfly.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zc.hnjuh.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kp.bjjhwx.cn

C#:   1234567.ToString("N0")
来源：http://nr.asd995.cn

[E17] 首字母大写
来源：http://rw.szxytkj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bu.bookmarksfly.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://md.bjjhwx.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://he.huixiangedu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lc.panjiajie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xr.shxzskj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yr.jctech888.com.cn

Ruby: s.capitalize
来源：http://hm.newstarts.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rk.wgjwhj.cn

[E18] 模板占位符替换
来源：http://cs.wgjwhj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xs.yuntaijiaju.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gw.asd995.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://fo.haigaiapp.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://bw.lnxyls.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bb.shtwfgs.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ey.hnjuh.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pp.nicolike.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mk.huixinmuqiang.cn

[E19] 多行文本按行拆分
来源：http://ll.jianghongdianzi.cn

Py:   s.splitlines()
来源：http://bw.asd995.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://za.nszjky.cn

JS:   s.split(/\r?\n/)
来源：http://kc.nicolike.cn

TS:   s.split(/\r?\n/)
来源：http://pp.shtwfgs.cn

Java: s.lines().toList()
来源：http://ai.wgjwhj.cn

Go:   strings.Split(s, "\n")
来源：http://of.nszjky.cn


<!-- 参考信息 -->