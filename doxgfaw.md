代发 wailian999

C#:   list.Reverse();
来源：http://vn.bjjhwx.cn

[D12] 查找元素下标
来源：http://rl.muxihuayi.cn

Py:   arr.index(x);  x in arr
来源：http://re.jctech888.com.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hv.yuntaijiaju.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fy.panjiajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pi.panjiajie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ey.muxihuayi.cn

Go:   slices.Index(arr, x)
来源：http://zo.nszjky.cn

Ruby: arr.index(x)
来源：http://rl.shxzukj.cn

C#:   list.IndexOf(x);
来源：http://ty.gzmigu.cn

[D13] 过滤（保留满足条件的）
来源：http://kt.shxzskj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dt.jctech888.com.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dz.nszjky.cn

JS:   arr.filter(x => x > 3)
来源：http://yr.jianghongdianzi.cn

TS:   arr.filter(x => x > 3)
来源：http://xn.bjjhwx.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zg.jctech888.com.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jo.shxzukj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://rh.szsharing.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vy.gzmigu.cn

[D14] 映射转换（每个元素变形）
来源：http://rz.huixiangedu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lx.bjjhwx.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lv.wgjwhj.cn

JS:   arr.map(x => x * 2)
来源：http://un.panjiajie.cn

TS:   arr.map(x => x * 2)
来源：http://zb.haigaiapp.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ba.chemitech.net.cn

Go:   // 手写循环
来源：http://hs.lnxyls.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qm.panjiajie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://fw.jctech888.com.cn

[D15] 去重
来源：http://xg.panjiajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nv.muxihuayi.cn

PHP:  array_unique($arr);
来源：http://ex.9csxet.cn

JS:   [...new Set(arr)]
来源：http://gh.haigaiapp.cn

TS:   [...new Set(arr)]
来源：http://gg.9csxet.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wz.szxytkj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://bk.yuntaijiaju.cn

Ruby: arr.uniq
来源：http://hv.521024.cn

C#:   list.Distinct().ToList()
来源：http://gb.wgjwhj.cn

[D16] 求和与平均值
来源：http://xo.shxzskj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gs.521024.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://uk.asd995.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nj.shxzukj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fn.wgjwhj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mo.hnjuh.cn

Go:   // 手写循环累加
来源：http://rv.shxzukj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bs.wgjwhj.cn

C#:   list.Sum();  list.Average()
来源：http://hb.nicolike.cn

[D17] 最大值与最小值
来源：http://kn.huixiangedu.cn

Py:   max(arr);  min(arr)
来源：http://gj.szxytkj.cn

PHP:  max($arr);  min($arr);
来源：http://aw.hnjuh.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mg.huanxung.cn

TS:   Math.max(...arr);
来源：http://cg.hahajie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://iz.yuntaijiaju.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mh.shxzskj.cn

Ruby: arr.max;  arr.min
来源：http://gn.lnxyls.cn

C#:   list.Max();  list.Min()
来源：http://ev.huixinmuqiang.cn

[D18] 扁平化嵌套数组
来源：http://qw.newstarts.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wy.jianghongdianzi.cn

PHP:  array_merge(...$nested);
来源：http://ri.yuexingan06.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://od.asd995.cn

TS:   nested.flat();
来源：http://lb.colortex.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lt.521024.cn

Go:   // 手写双层循环
来源：http://wb.lnxyls.cn

Ruby: nested.flatten
来源：http://hw.hahajie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://dz.shxzskj.cn

[D19] 按字段分组
来源：http://ik.jctech888.com.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vw.lnxyls.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://du.bjjhwx.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xk.huixiangedu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://wa.asd995.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://uy.muxihuayi.cn

Go:   // 手写 map[string][]T
来源：http://ca.bjjhwx.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://kc.haigaiapp.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gs.wgjwhj.cn

[D20] 统计每个元素出现次数
来源：http://wo.jianghongdianzi.cn

Py:   Counter(arr)
来源：http://ke.huixinmuqiang.cn

PHP:  array_count_values($arr);
来源：http://qu.huixinmuqiang.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gg.huixiangedu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://za.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://uu.chemitech.net.cn

Go:   // 手写 map[T]int
来源：http://uw.huanxung.cn

Ruby: arr.tally
来源：http://gr.yuntaijiaju.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jo.gzmigu.cn

[D21] 判断是否包含某元素
来源：http://hh.hnjuh.cn

Py:   x in arr
来源：http://bb.shtwfgs.cn

PHP:  in_array($x, $arr, true);
来源：http://pg.huixinmuqiang.cn

JS:   arr.includes(x)
来源：http://su.muxihuayi.cn

TS:   arr.includes(x)
来源：http://bq.hahajie.cn

Java: list.contains(x)
来源：http://xk.chemitech.net.cn

Go:   slices.Contains(arr, x)
来源：http://fa.jianghongdianzi.cn

Ruby: arr.include?(x)
来源：http://dj.521024.cn

C#:   list.Contains(x)
来源：http://qz.yuexingan06.cn

[D22] 复制数组（避免共享引用）
来源：http://uv.nszjky.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gd.huixinmuqiang.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hx.asd995.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://if.chemitech.net.cn

TS:   [...arr];
来源：http://gm.521024.cn

Java: new ArrayList<>(list);
来源：http://yj.huixiangedu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://gk.hahajie.cn

Ruby: arr.dup;  arr.clone
来源：http://fg.gzmigu.cn

C#:   new List<int>(list);
来源：http://dc.shxzukj.cn

[D23] reduce 累积计算
来源：http://zv.9csxet.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rw.9csxet.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rr.huanxung.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lu.colortex.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xj.9csxet.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rn.shxzukj.cn

Go:   // 手写循环
来源：http://ea.lnxyls.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cf.shtwfgs.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bd.yuntaijiaju.cn

[D24] 字典 / Map 基本操作
来源：http://vv.colortex.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qd.lnxyls.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mw.bjjhwx.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jw.chemitech.net.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zf.haigaiapp.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tu.huixinmuqiang.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nd.lnxyls.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://sd.nicolike.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rz.hnjuh.cn

[D25] Set 集合去重与交并差
来源：http://ia.huixiangedu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fl.wgjwhj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nf.szsharing.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ro.hahajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cr.jianghongdianzi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ie.szxytkj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ux.wgjwhj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hf.chemitech.net.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ym.bookmarksfly.cn

[D26] 数组转字符串
来源：http://jg.nicolike.cn

Py:   ", ".join(map(str, arr))
来源：http://lb.asd995.cn

PHP:  implode(", ", $arr);
来源：http://ag.colortex.cn

JS:   arr.join(", ")
来源：http://bp.lnxyls.cn

TS:   arr.join(", ")
来源：http://nz.asd995.cn

Java: String.join(", ", list)
来源：http://kx.bookmarksfly.cn

Go:   strings.Join(strs, ", ")
来源：http://rj.jctech888.com.cn

Ruby: arr.join(", ")
来源：http://jf.9csxet.cn

C#:   string.Join(", ", list)
来源：http://wu.wgjwhj.cn

================================================================================
来源：http://nw.huixinmuqiang.cn

E. 字符串处理
来源：http://py.huixiangedu.cn

================================================================================
来源：http://mr.huanxung.cn

[E01] 拼接字符串
来源：http://gr.newstarts.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kn.asd995.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vk.nszjky.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uy.asd995.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gx.colortex.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://np.asd995.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ul.wgjwhj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jl.jianghongdianzi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wg.521024.cn

[E02] 重复字符串
来源：http://sq.nszjky.cn

Py:   "ab" * 3
来源：http://pp.521024.cn

PHP:  str_repeat("ab", 3);
来源：http://yw.haigaiapp.cn

JS:   "ab".repeat(3)
来源：http://mu.gzmigu.cn

TS:   "ab".repeat(3)
来源：http://xw.huixinmuqiang.cn

Java: "ab".repeat(3)
来源：http://dj.hnjuh.cn

Go:   strings.Repeat("ab", 3)
来源：http://tp.muxihuayi.cn

Ruby: "ab" * 3
来源：http://nj.haigaiapp.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qf.muxihuayi.cn

[E03] 截取子串
来源：http://jk.asd995.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ny.asd995.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://sk.shxzskj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wu.szsharing.cn

TS:   s.slice(1, 4)
来源：http://ye.lnxyls.cn

Java: s.substring(1, 4)
来源：http://vj.newstarts.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tx.muxihuayi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://tl.shxzskj.cn

C#:   s.Substring(1, 3)
来源：http://lz.muxihuayi.cn

[E04] 查找子串位置
来源：http://ty.chemitech.net.cn

Py:   s.find("x");  s.index("x")
来源：http://et.newstarts.cn

PHP:  strpos($s, "x");
来源：http://hf.nicolike.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bb.asd995.cn

TS:   s.indexOf("x")
来源：http://gv.lnxyls.cn

Java: s.indexOf("x")
来源：http://qd.wgjwhj.cn

Go:   strings.Index(s, "x")
来源：http://be.yuntaijiaju.cn

Ruby: s.index("x")
来源：http://sa.haigaiapp.cn

C#:   s.IndexOf("x")
来源：http://gk.jctech888.com.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://dt.panjiajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uu.wgjwhj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://aw.lnxyls.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bf.bookmarksfly.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://vr.huixiangedu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://px.szsharing.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bv.bjjhwx.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ig.newstarts.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jr.asd995.cn

[E06] 替换子串
来源：http://ef.huanxung.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ke.panjiajie.cn

PHP:  str_replace("a", "b", $s);
来源：http://ko.szxytkj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oe.nszjky.cn

TS:   s.replaceAll("a", "b")
来源：http://yr.hahajie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vd.yuexingan06.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fg.bjjhwx.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ow.szsharing.cn

C#:   s.Replace("a", "b")
来源：http://ts.shtwfgs.cn

[E07] 按分隔符拆分
来源：http://jf.yuntaijiaju.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lg.yuntaijiaju.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dz.jianghongdianzi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ve.hahajie.cn

TS:   s.split(",")
来源：http://hd.gzmigu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://wb.yuntaijiaju.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ld.bookmarksfly.cn

Ruby: s.split(",");  s.split
来源：http://uh.szxytkj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hj.newstarts.cn

[E08] 数组按分隔符合并
来源：http://um.shxzskj.cn

Py:   ",".join(items)
来源：http://wp.jianghongdianzi.cn

PHP:  implode(",", $items);
来源：http://ux.hahajie.cn

JS:   items.join(",")
来源：http://oa.lnxyls.cn

TS:   items.join(",")
来源：http://xh.muxihuayi.cn

Java: String.join(",", items)
来源：http://nm.hahajie.cn

Go:   strings.Join(items, ",")
来源：http://es.jianghongdianzi.cn

Ruby: items.join(",")
来源：http://tt.shtwfgs.cn

C#:   string.Join(",", items)
来源：http://bh.bjjhwx.cn

[E09] 去除所有空白字符
来源：http://fn.shxzskj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rl.huanxung.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ir.huanxung.cn

JS:   s.replace(/\s+/g, "")
来源：http://pg.huixinmuqiang.cn

TS:   s.replace(/\s+/g, "")
来源：http://bp.haigaiapp.cn

Java: s.replaceAll("\\s+", "")
来源：http://iy.9csxet.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ek.9csxet.cn

Ruby: s.gsub(/\s+/, "")
来源：http://pf.bookmarksfly.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rt.shxzukj.cn

[E10] 左侧补零 / 定长填充
来源：http://vu.szxytkj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tv.lnxyls.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lk.huixiangedu.cn

JS:   "7".padStart(3, "0")
来源：http://ho.huixiangedu.cn

TS:   "7".padStart(3, "0")
来源：http://dz.shxzskj.cn

Java: String.format("%03d", 7)
来源：http://pd.szxytkj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://hn.szsharing.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ca.asd995.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bb.shtwfgs.cn

[E11] 反转字符串
来源：http://nw.huanxung.cn

Py:   s[::-1]
来源：http://vu.shxzskj.cn

PHP:  strrev($s);
来源：http://ej.jctech888.com.cn

JS:   [...s].reverse().join("")
来源：http://lc.9csxet.cn

TS:   [...s].reverse().join("")
来源：http://ii.nicolike.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://mq.9csxet.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://sw.huixinmuqiang.cn

Ruby: s.reverse
来源：http://du.szxytkj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://gr.gzmigu.cn

[E12] 统计某字符出现次数
来源：http://bk.hnjuh.cn

Py:   s.count("a")
来源：http://zz.huanxung.cn

PHP:  substr_count($s, "a");
来源：http://ca.nszjky.cn

JS:   s.split("a").length - 1
来源：http://fz.yuntaijiaju.cn

TS:   s.split("a").length - 1
来源：http://gb.colortex.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kd.shtwfgs.cn

Go:   strings.Count(s, "a")
来源：http://sc.521024.cn

Ruby: s.count("a")
来源：http://un.hnjuh.cn

C#:   s.Count(c => c == 'a')
来源：http://cg.bjjhwx.cn

[E13] 逐字符遍历
来源：http://jd.huanxung.cn

Py:   for ch in s: print(ch)
来源：http://ag.nszjky.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ix.hahajie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://rl.szsharing.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://vk.shxzukj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://aw.bjjhwx.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tl.szsharing.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://kb.jctech888.com.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gq.jianghongdianzi.cn

[E14] URL 编码与 Base64
来源：http://zk.bookmarksfly.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sd.yuntaijiaju.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://nt.chemitech.net.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mf.yuntaijiaju.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wf.shxzukj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://te.shxzskj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qf.szxytkj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gq.lnxyls.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kw.haigaiapp.cn

[E15] HTML 转义 / 反转义
来源：http://lm.jianghongdianzi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://yl.chemitech.net.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zq.shxzukj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://co.szsharing.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://xl.bookmarksfly.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ww.521024.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ce.asd995.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wm.nszjky.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pl.asd995.cn

[E16] 数字千分位
来源：http://tr.huixiangedu.cn

Py:   f"{1234567:,}"
来源：http://dz.bookmarksfly.cn

PHP:  number_format(1234567);
来源：http://sc.huixiangedu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://bh.lnxyls.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wd.szxytkj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nv.huixinmuqiang.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yd.shxzskj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vu.bookmarksfly.cn

C#:   1234567.ToString("N0")
来源：http://ks.szsharing.cn

[E17] 首字母大写
来源：http://kf.gzmigu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wz.asd995.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://wo.jianghongdianzi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hl.szsharing.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xv.nszjky.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mn.szxytkj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fu.huixinmuqiang.cn

Ruby: s.capitalize
来源：http://nm.haigaiapp.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://so.panjiajie.cn

[E18] 模板占位符替换
来源：http://as.gzmigu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pj.bjjhwx.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ae.hnjuh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://oz.shxzukj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://kk.szsharing.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ov.hnjuh.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ei.shtwfgs.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vz.huanxung.cn


<!-- 参考信息 -->