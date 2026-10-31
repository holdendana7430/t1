代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://cf.yuexingan06.cn

[D08] 合并两个数组
来源：http://ab.huanxung.cn

Py:   a + b;  a.extend(b)
来源：http://ht.521024.cn

PHP:  array_merge($a, $b);
来源：http://da.yuexingan06.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://sl.bookmarksfly.cn

TS:   [...a, ...b];
来源：http://qw.yuexingan06.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zv.nicolike.cn

Go:   append(a, b...)
来源：http://pl.shxzskj.cn

Ruby: a + b;  a.concat(b)
来源：http://px.521024.cn

C#:   a.Concat(b).ToList()
来源：http://ye.huixiangedu.cn

[D09] 排序（升序）
来源：http://rk.huanxung.cn

Py:   sorted(arr);  arr.sort()
来源：http://zh.shxzukj.cn

PHP:  sort($arr);
来源：http://gd.haigaiapp.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xo.haigaiapp.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.haigaiapp.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://fl.newstarts.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://um.nicolike.cn

Ruby: arr.sort
来源：http://yk.shxzukj.cn

C#:   list.Sort();
来源：http://nb.hahajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://hs.huanxung.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tn.huanxung.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bo.wgjwhj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fp.521024.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hg.colortex.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://as.jctech888.com.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rn.shxzukj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ev.hahajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://go.newstarts.cn

[D11] 反转数组
来源：http://zt.yuexingan06.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ku.hahajie.cn

PHP:  array_reverse($arr);
来源：http://zj.haigaiapp.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fm.shxzskj.cn

TS:   [...arr].reverse();
来源：http://qn.9csxet.cn

Java: Collections.reverse(list);
来源：http://ut.gzmigu.cn

Go:   slices.Reverse(arr)
来源：http://iz.9csxet.cn

Ruby: arr.reverse
来源：http://iu.huanxung.cn

C#:   list.Reverse();
来源：http://wp.colortex.cn

[D12] 查找元素下标
来源：http://qu.jctech888.com.cn

Py:   arr.index(x);  x in arr
来源：http://rq.hnjuh.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hv.jianghongdianzi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://az.jctech888.com.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qj.huanxung.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://em.nszjky.cn

Go:   slices.Index(arr, x)
来源：http://kq.shxzskj.cn

Ruby: arr.index(x)
来源：http://lm.shtwfgs.cn

C#:   list.IndexOf(x);
来源：http://lk.hahajie.cn

[D13] 过滤（保留满足条件的）
来源：http://te.szsharing.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bh.hnjuh.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lb.shtwfgs.cn

JS:   arr.filter(x => x > 3)
来源：http://dd.bookmarksfly.cn

TS:   arr.filter(x => x > 3)
来源：http://st.asd995.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mk.nicolike.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ht.huixiangedu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wl.wgjwhj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://bd.nszjky.cn

[D14] 映射转换（每个元素变形）
来源：http://rx.521024.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bs.lnxyls.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cx.newstarts.cn

JS:   arr.map(x => x * 2)
来源：http://wy.bjjhwx.cn

TS:   arr.map(x => x * 2)
来源：http://pb.521024.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://io.nszjky.cn

Go:   // 手写循环
来源：http://mm.szsharing.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ux.nicolike.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://yo.yuntaijiaju.cn

[D15] 去重
来源：http://un.jctech888.com.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lt.huixiangedu.cn

PHP:  array_unique($arr);
来源：http://cb.panjiajie.cn

JS:   [...new Set(arr)]
来源：http://hf.chemitech.net.cn

TS:   [...new Set(arr)]
来源：http://vs.muxihuayi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lk.9csxet.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ag.nicolike.cn

Ruby: arr.uniq
来源：http://gu.colortex.cn

C#:   list.Distinct().ToList()
来源：http://so.gzmigu.cn

[D16] 求和与平均值
来源：http://ik.hnjuh.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qc.bjjhwx.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ow.colortex.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nl.jianghongdianzi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ja.newstarts.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ap.yuexingan06.cn

Go:   // 手写循环累加
来源：http://gr.asd995.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://sv.lnxyls.cn

C#:   list.Sum();  list.Average()
来源：http://ns.chemitech.net.cn

[D17] 最大值与最小值
来源：http://bd.hahajie.cn

Py:   max(arr);  min(arr)
来源：http://op.hahajie.cn

PHP:  max($arr);  min($arr);
来源：http://fb.bookmarksfly.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xc.chemitech.net.cn

TS:   Math.max(...arr);
来源：http://bx.yuntaijiaju.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ig.szsharing.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mt.asd995.cn

Ruby: arr.max;  arr.min
来源：http://ig.jctech888.com.cn

C#:   list.Max();  list.Min()
来源：http://qs.szxytkj.cn

[D18] 扁平化嵌套数组
来源：http://co.hahajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://db.yuntaijiaju.cn

PHP:  array_merge(...$nested);
来源：http://ws.bookmarksfly.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bf.nicolike.cn

TS:   nested.flat();
来源：http://ef.huixiangedu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mz.wgjwhj.cn

Go:   // 手写双层循环
来源：http://ob.hnjuh.cn

Ruby: nested.flatten
来源：http://he.bjjhwx.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://kf.huixinmuqiang.cn

[D19] 按字段分组
来源：http://nw.shxzukj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pi.chemitech.net.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tv.bookmarksfly.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rm.hnjuh.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xd.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://be.lnxyls.cn

Go:   // 手写 map[string][]T
来源：http://lv.yuntaijiaju.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://nr.asd995.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tv.nszjky.cn

[D20] 统计每个元素出现次数
来源：http://ns.huixiangedu.cn

Py:   Counter(arr)
来源：http://uw.szsharing.cn

PHP:  array_count_values($arr);
来源：http://dj.shxzskj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ts.jianghongdianzi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gh.shxzskj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kr.newstarts.cn

Go:   // 手写 map[T]int
来源：http://pq.jctech888.com.cn

Ruby: arr.tally
来源：http://mi.huanxung.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://uz.9csxet.cn

[D21] 判断是否包含某元素
来源：http://eh.muxihuayi.cn

Py:   x in arr
来源：http://yw.shxzskj.cn

PHP:  in_array($x, $arr, true);
来源：http://jp.521024.cn

JS:   arr.includes(x)
来源：http://ta.521024.cn

TS:   arr.includes(x)
来源：http://gz.9csxet.cn

Java: list.contains(x)
来源：http://el.shtwfgs.cn

Go:   slices.Contains(arr, x)
来源：http://su.shxzskj.cn

Ruby: arr.include?(x)
来源：http://gn.muxihuayi.cn

C#:   list.Contains(x)
来源：http://ll.yuntaijiaju.cn

[D22] 复制数组（避免共享引用）
来源：http://ed.haigaiapp.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tg.chemitech.net.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dn.lnxyls.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jc.szxytkj.cn

TS:   [...arr];
来源：http://xq.huixiangedu.cn

Java: new ArrayList<>(list);
来源：http://uc.shtwfgs.cn

Go:   copied := append([]int(nil), arr...)
来源：http://kf.yuntaijiaju.cn

Ruby: arr.dup;  arr.clone
来源：http://dw.jctech888.com.cn

C#:   new List<int>(list);
来源：http://dl.colortex.cn

[D23] reduce 累积计算
来源：http://ac.panjiajie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mj.shtwfgs.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ve.asd995.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qj.huixinmuqiang.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ph.nicolike.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://de.wgjwhj.cn

Go:   // 手写循环
来源：http://jb.gzmigu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dw.yuexingan06.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ov.wgjwhj.cn

[D24] 字典 / Map 基本操作
来源：http://td.yuexingan06.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rj.huanxung.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ch.9csxet.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tf.yuexingan06.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xt.newstarts.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cm.huixiangedu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tb.huixinmuqiang.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://yo.yuexingan06.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xs.huixinmuqiang.cn

[D25] Set 集合去重与交并差
来源：http://hp.9csxet.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kn.yuntaijiaju.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://es.colortex.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://le.huixinmuqiang.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cs.lnxyls.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://iv.shtwfgs.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ni.9csxet.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rc.gzmigu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gh.wgjwhj.cn

[D26] 数组转字符串
来源：http://xo.szsharing.cn

Py:   ", ".join(map(str, arr))
来源：http://sv.bookmarksfly.cn

PHP:  implode(", ", $arr);
来源：http://xk.szsharing.cn

JS:   arr.join(", ")
来源：http://xr.hnjuh.cn

TS:   arr.join(", ")
来源：http://ye.hnjuh.cn

Java: String.join(", ", list)
来源：http://fy.gzmigu.cn

Go:   strings.Join(strs, ", ")
来源：http://ad.muxihuayi.cn

Ruby: arr.join(", ")
来源：http://ri.bookmarksfly.cn

C#:   string.Join(", ", list)
来源：http://ey.wgjwhj.cn

================================================================================
来源：http://ke.gzmigu.cn

E. 字符串处理
来源：http://fp.muxihuayi.cn

================================================================================
来源：http://uv.shxzukj.cn

[E01] 拼接字符串
来源：http://jc.muxihuayi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xr.nicolike.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gr.huixinmuqiang.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ir.gzmigu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xd.9csxet.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ks.hnjuh.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ej.jianghongdianzi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://uu.hnjuh.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kw.panjiajie.cn

[E02] 重复字符串
来源：http://bo.chemitech.net.cn

Py:   "ab" * 3
来源：http://xz.9csxet.cn

PHP:  str_repeat("ab", 3);
来源：http://aw.newstarts.cn

JS:   "ab".repeat(3)
来源：http://wp.huanxung.cn

TS:   "ab".repeat(3)
来源：http://ee.huanxung.cn

Java: "ab".repeat(3)
来源：http://mf.newstarts.cn

Go:   strings.Repeat("ab", 3)
来源：http://rv.panjiajie.cn

Ruby: "ab" * 3
来源：http://kc.wgjwhj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rg.newstarts.cn

[E03] 截取子串
来源：http://uo.haigaiapp.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qz.nicolike.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gv.panjiajie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yz.hnjuh.cn

TS:   s.slice(1, 4)
来源：http://kh.jianghongdianzi.cn

Java: s.substring(1, 4)
来源：http://dg.huixinmuqiang.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pp.haigaiapp.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ec.yuexingan06.cn

C#:   s.Substring(1, 3)
来源：http://be.gzmigu.cn

[E04] 查找子串位置
来源：http://ou.jianghongdianzi.cn

Py:   s.find("x");  s.index("x")
来源：http://be.jianghongdianzi.cn

PHP:  strpos($s, "x");
来源：http://db.jctech888.com.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mz.panjiajie.cn

TS:   s.indexOf("x")
来源：http://kk.wgjwhj.cn

Java: s.indexOf("x")
来源：http://jf.shtwfgs.cn

Go:   strings.Index(s, "x")
来源：http://ab.asd995.cn

Ruby: s.index("x")
来源：http://wz.nicolike.cn

C#:   s.IndexOf("x")
来源：http://yy.panjiajie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://uz.bjjhwx.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://et.nszjky.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wg.huixinmuqiang.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fo.shxzskj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://aj.szsharing.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nd.yuntaijiaju.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yk.muxihuayi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jl.chemitech.net.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pb.gzmigu.cn

[E06] 替换子串
来源：http://me.nszjky.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://el.hnjuh.cn

PHP:  str_replace("a", "b", $s);
来源：http://ol.yuntaijiaju.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ry.chemitech.net.cn

TS:   s.replaceAll("a", "b")
来源：http://ix.lnxyls.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bg.newstarts.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://th.huixinmuqiang.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gr.shxzukj.cn

C#:   s.Replace("a", "b")
来源：http://cs.hnjuh.cn

[E07] 按分隔符拆分
来源：http://yz.colortex.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pc.hahajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ov.gzmigu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://us.bookmarksfly.cn

TS:   s.split(",")
来源：http://sh.haigaiapp.cn

Java: s.split(",");  s.split("\\s+")
来源：http://wv.bjjhwx.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kg.asd995.cn

Ruby: s.split(",");  s.split
来源：http://pm.9csxet.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xg.lnxyls.cn

[E08] 数组按分隔符合并
来源：http://ng.shxzskj.cn

Py:   ",".join(items)
来源：http://am.hahajie.cn

PHP:  implode(",", $items);
来源：http://tt.huanxung.cn

JS:   items.join(",")
来源：http://qx.yuntaijiaju.cn

TS:   items.join(",")
来源：http://xx.szxytkj.cn

Java: String.join(",", items)
来源：http://cm.hnjuh.cn

Go:   strings.Join(items, ",")
来源：http://ux.colortex.cn

Ruby: items.join(",")
来源：http://qm.nszjky.cn

C#:   string.Join(",", items)
来源：http://ai.shxzukj.cn

[E09] 去除所有空白字符
来源：http://gj.lnxyls.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lg.asd995.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pc.shtwfgs.cn

JS:   s.replace(/\s+/g, "")
来源：http://eh.9csxet.cn

TS:   s.replace(/\s+/g, "")
来源：http://sg.hnjuh.cn

Java: s.replaceAll("\\s+", "")
来源：http://ql.shtwfgs.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://dq.hahajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://pg.shxzskj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rx.521024.cn

[E10] 左侧补零 / 定长填充
来源：http://kq.nszjky.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://np.gzmigu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://iu.hnjuh.cn

JS:   "7".padStart(3, "0")
来源：http://et.yuntaijiaju.cn

TS:   "7".padStart(3, "0")
来源：http://jo.haigaiapp.cn

Java: String.format("%03d", 7)
来源：http://ts.yuntaijiaju.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://dy.colortex.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ov.szxytkj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lk.jctech888.com.cn

[E11] 反转字符串
来源：http://lm.haigaiapp.cn

Py:   s[::-1]
来源：http://yk.szsharing.cn

PHP:  strrev($s);
来源：http://fw.lnxyls.cn

JS:   [...s].reverse().join("")
来源：http://ps.lnxyls.cn

TS:   [...s].reverse().join("")
来源：http://ob.shxzukj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://nr.colortex.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://hl.colortex.cn

Ruby: s.reverse
来源：http://tg.haigaiapp.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ik.huixinmuqiang.cn

[E12] 统计某字符出现次数
来源：http://zj.gzmigu.cn

Py:   s.count("a")
来源：http://xk.huixiangedu.cn

PHP:  substr_count($s, "a");
来源：http://hd.shtwfgs.cn

JS:   s.split("a").length - 1
来源：http://za.nicolike.cn

TS:   s.split("a").length - 1
来源：http://nt.haigaiapp.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qg.muxihuayi.cn

Go:   strings.Count(s, "a")
来源：http://em.panjiajie.cn

Ruby: s.count("a")
来源：http://jz.huixinmuqiang.cn

C#:   s.Count(c => c == 'a')
来源：http://qk.huanxung.cn

[E13] 逐字符遍历
来源：http://tc.panjiajie.cn

Py:   for ch in s: print(ch)
来源：http://cq.shxzukj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zd.huixinmuqiang.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://yt.haigaiapp.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://li.hahajie.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xy.panjiajie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://oa.gzmigu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://co.9csxet.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wx.521024.cn

[E14] URL 编码与 Base64
来源：http://pv.haigaiapp.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ic.chemitech.net.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://fe.panjiajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://md.bookmarksfly.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ck.colortex.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jq.huanxung.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mx.521024.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cu.bookmarksfly.cn


<!-- 参考信息 -->