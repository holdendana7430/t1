代发 wailian999

Py:   len(arr)
来源：http://cq.panjiajie.cn

PHP:  count($arr);
来源：http://an.lnxyls.cn

JS:   arr.length
来源：http://tk.asd995.cn

TS:   arr.length
来源：http://cy.bookmarksfly.cn

Java: list.size();
来源：http://vy.nszjky.cn

Go:   len(arr)
来源：http://zb.panjiajie.cn

Ruby: arr.length; arr.size
来源：http://er.muxihuayi.cn

C#:   list.Count;
来源：http://ps.lnxyls.cn

[D07] 切片 / 取子数组
来源：http://ol.nicolike.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://uu.9csxet.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hm.asd995.cn

JS:   arr.slice(1, 4);
来源：http://jp.yuntaijiaju.cn

TS:   arr.slice(1, 4);
来源：http://sz.lnxyls.cn

Java: list.subList(1, 4);
来源：http://mi.huixiangedu.cn

Go:   arr[1:4]
来源：http://bw.szxytkj.cn

Ruby: arr[1, 3]
来源：http://lr.asd995.cn

C#:   list.GetRange(1, 3);
来源：http://kn.panjiajie.cn

[D08] 合并两个数组
来源：http://es.hahajie.cn

Py:   a + b;  a.extend(b)
来源：http://sk.muxihuayi.cn

PHP:  array_merge($a, $b);
来源：http://gb.newstarts.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://yj.gzmigu.cn

TS:   [...a, ...b];
来源：http://jo.gzmigu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zb.9csxet.cn

Go:   append(a, b...)
来源：http://sg.wgjwhj.cn

Ruby: a + b;  a.concat(b)
来源：http://ry.chemitech.net.cn

C#:   a.Concat(b).ToList()
来源：http://qi.huixinmuqiang.cn

[D09] 排序（升序）
来源：http://mv.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://ml.jianghongdianzi.cn

PHP:  sort($arr);
来源：http://wj.yuexingan06.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xe.9csxet.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gz.jianghongdianzi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://nm.szsharing.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://oc.bjjhwx.cn

Ruby: arr.sort
来源：http://zj.panjiajie.cn

C#:   list.Sort();
来源：http://jy.asd995.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://jk.jctech888.com.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mz.chemitech.net.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hf.szxytkj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ua.9csxet.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yo.yuexingan06.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dy.gzmigu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wa.haigaiapp.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pw.bjjhwx.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://od.hahajie.cn

[D11] 反转数组
来源：http://gt.521024.cn

Py:   arr[::-1];  arr.reverse()
来源：http://vl.newstarts.cn

PHP:  array_reverse($arr);
来源：http://pd.yuntaijiaju.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://is.chemitech.net.cn

TS:   [...arr].reverse();
来源：http://au.huixinmuqiang.cn

Java: Collections.reverse(list);
来源：http://bk.panjiajie.cn

Go:   slices.Reverse(arr)
来源：http://xh.chemitech.net.cn

Ruby: arr.reverse
来源：http://sn.bookmarksfly.cn

C#:   list.Reverse();
来源：http://yb.shxzskj.cn

[D12] 查找元素下标
来源：http://cu.shxzukj.cn

Py:   arr.index(x);  x in arr
来源：http://bf.nszjky.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ej.jianghongdianzi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uc.huixinmuqiang.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://js.asd995.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bj.chemitech.net.cn

Go:   slices.Index(arr, x)
来源：http://mb.huanxung.cn

Ruby: arr.index(x)
来源：http://lw.panjiajie.cn

C#:   list.IndexOf(x);
来源：http://nm.gzmigu.cn

[D13] 过滤（保留满足条件的）
来源：http://un.bookmarksfly.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dh.521024.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://am.nszjky.cn

JS:   arr.filter(x => x > 3)
来源：http://pt.shxzskj.cn

TS:   arr.filter(x => x > 3)
来源：http://xi.newstarts.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ls.huanxung.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://os.hnjuh.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qx.chemitech.net.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://fn.9csxet.cn

[D14] 映射转换（每个元素变形）
来源：http://bv.szsharing.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dm.huanxung.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sp.jctech888.com.cn

JS:   arr.map(x => x * 2)
来源：http://ox.szxytkj.cn

TS:   arr.map(x => x * 2)
来源：http://cz.chemitech.net.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://xf.9csxet.cn

Go:   // 手写循环
来源：http://mr.shtwfgs.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fg.shxzskj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ar.muxihuayi.cn

[D15] 去重
来源：http://lh.bjjhwx.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rh.521024.cn

PHP:  array_unique($arr);
来源：http://oi.huixinmuqiang.cn

JS:   [...new Set(arr)]
来源：http://la.huixinmuqiang.cn

TS:   [...new Set(arr)]
来源：http://nb.shxzukj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vz.panjiajie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://cr.szxytkj.cn

Ruby: arr.uniq
来源：http://kr.szxytkj.cn

C#:   list.Distinct().ToList()
来源：http://sr.colortex.cn

[D16] 求和与平均值
来源：http://fs.haigaiapp.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vj.gzmigu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zl.nszjky.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://da.szxytkj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dj.hahajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://oy.panjiajie.cn

Go:   // 手写循环累加
来源：http://fj.szxytkj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lk.bookmarksfly.cn

C#:   list.Sum();  list.Average()
来源：http://wq.panjiajie.cn

[D17] 最大值与最小值
来源：http://uf.szxytkj.cn

Py:   max(arr);  min(arr)
来源：http://dd.haigaiapp.cn

PHP:  max($arr);  min($arr);
来源：http://pt.gzmigu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qy.jctech888.com.cn

TS:   Math.max(...arr);
来源：http://dn.nicolike.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ys.jianghongdianzi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hs.haigaiapp.cn

Ruby: arr.max;  arr.min
来源：http://pz.szxytkj.cn

C#:   list.Max();  list.Min()
来源：http://ub.nicolike.cn

[D18] 扁平化嵌套数组
来源：http://ul.9csxet.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cz.bookmarksfly.cn

PHP:  array_merge(...$nested);
来源：http://uv.shxzukj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jd.wgjwhj.cn

TS:   nested.flat();
来源：http://dz.jianghongdianzi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ik.muxihuayi.cn

Go:   // 手写双层循环
来源：http://xq.haigaiapp.cn

Ruby: nested.flatten
来源：http://pe.lnxyls.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ke.huanxung.cn

[D19] 按字段分组
来源：http://tk.yuntaijiaju.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://py.newstarts.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ia.yuntaijiaju.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ri.shtwfgs.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://yy.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gh.asd995.cn

Go:   // 手写 map[string][]T
来源：http://cd.newstarts.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ls.szxytkj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ep.shtwfgs.cn

[D20] 统计每个元素出现次数
来源：http://up.panjiajie.cn

Py:   Counter(arr)
来源：http://fe.jianghongdianzi.cn

PHP:  array_count_values($arr);
来源：http://co.colortex.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wr.muxihuayi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ua.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://em.muxihuayi.cn

Go:   // 手写 map[T]int
来源：http://mw.yuntaijiaju.cn

Ruby: arr.tally
来源：http://vy.newstarts.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zf.newstarts.cn

[D21] 判断是否包含某元素
来源：http://kq.szxytkj.cn

Py:   x in arr
来源：http://gm.huanxung.cn

PHP:  in_array($x, $arr, true);
来源：http://hs.gzmigu.cn

JS:   arr.includes(x)
来源：http://cq.521024.cn

TS:   arr.includes(x)
来源：http://ni.huixiangedu.cn

Java: list.contains(x)
来源：http://rd.hahajie.cn

Go:   slices.Contains(arr, x)
来源：http://gd.bookmarksfly.cn

Ruby: arr.include?(x)
来源：http://en.colortex.cn

C#:   list.Contains(x)
来源：http://cb.huixiangedu.cn

[D22] 复制数组（避免共享引用）
来源：http://bp.yuexingan06.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cm.9csxet.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ki.muxihuayi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cf.szsharing.cn

TS:   [...arr];
来源：http://ab.yuexingan06.cn

Java: new ArrayList<>(list);
来源：http://ly.shxzskj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://uy.huixinmuqiang.cn

Ruby: arr.dup;  arr.clone
来源：http://ww.hahajie.cn

C#:   new List<int>(list);
来源：http://tq.yuntaijiaju.cn

[D23] reduce 累积计算
来源：http://sg.huanxung.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jz.huixinmuqiang.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kb.panjiajie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ar.muxihuayi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vq.hnjuh.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qe.yuntaijiaju.cn

Go:   // 手写循环
来源：http://ja.hahajie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://sv.huixinmuqiang.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://oe.colortex.cn

[D24] 字典 / Map 基本操作
来源：http://wc.yuntaijiaju.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uj.szsharing.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rm.jianghongdianzi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://la.jctech888.com.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tg.gzmigu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gm.bookmarksfly.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pq.bjjhwx.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gs.szxytkj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nk.nicolike.cn

[D25] Set 集合去重与交并差
来源：http://ql.shtwfgs.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://er.huixiangedu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hu.panjiajie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ii.shxzskj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zw.nicolike.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vz.shtwfgs.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://oo.bjjhwx.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nj.chemitech.net.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kz.hnjuh.cn

[D26] 数组转字符串
来源：http://wv.muxihuayi.cn

Py:   ", ".join(map(str, arr))
来源：http://vf.wgjwhj.cn

PHP:  implode(", ", $arr);
来源：http://ck.huixinmuqiang.cn

JS:   arr.join(", ")
来源：http://zx.yuexingan06.cn

TS:   arr.join(", ")
来源：http://bd.asd995.cn

Java: String.join(", ", list)
来源：http://yj.huixinmuqiang.cn

Go:   strings.Join(strs, ", ")
来源：http://je.huanxung.cn

Ruby: arr.join(", ")
来源：http://po.newstarts.cn

C#:   string.Join(", ", list)
来源：http://nc.shxzukj.cn

================================================================================
来源：http://oo.nicolike.cn

E. 字符串处理
来源：http://at.newstarts.cn

================================================================================
来源：http://fz.jctech888.com.cn

[E01] 拼接字符串
来源：http://dr.yuexingan06.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ww.jianghongdianzi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ri.wgjwhj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ty.huixinmuqiang.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zx.bookmarksfly.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jc.521024.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://us.shxzskj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dy.yuexingan06.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lq.colortex.cn

[E02] 重复字符串
来源：http://wy.nszjky.cn

Py:   "ab" * 3
来源：http://ez.haigaiapp.cn

PHP:  str_repeat("ab", 3);
来源：http://le.shxzukj.cn

JS:   "ab".repeat(3)
来源：http://kj.wgjwhj.cn

TS:   "ab".repeat(3)
来源：http://yn.nicolike.cn

Java: "ab".repeat(3)
来源：http://lo.hnjuh.cn

Go:   strings.Repeat("ab", 3)
来源：http://cj.gzmigu.cn

Ruby: "ab" * 3
来源：http://xr.shxzskj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zn.hnjuh.cn

[E03] 截取子串
来源：http://ou.huixinmuqiang.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gt.yuexingan06.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hw.szsharing.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zv.shtwfgs.cn

TS:   s.slice(1, 4)
来源：http://ci.muxihuayi.cn

Java: s.substring(1, 4)
来源：http://gn.huanxung.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vv.chemitech.net.cn

Ruby: s[1, 3];  s[1..3]
来源：http://nc.nicolike.cn

C#:   s.Substring(1, 3)
来源：http://hp.shxzukj.cn

[E04] 查找子串位置
来源：http://ft.521024.cn

Py:   s.find("x");  s.index("x")
来源：http://rv.shxzskj.cn

PHP:  strpos($s, "x");
来源：http://xj.hnjuh.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://as.9csxet.cn

TS:   s.indexOf("x")
来源：http://ny.shxzskj.cn

Java: s.indexOf("x")
来源：http://ye.asd995.cn

Go:   strings.Index(s, "x")
来源：http://yh.muxihuayi.cn

Ruby: s.index("x")
来源：http://gy.jctech888.com.cn

C#:   s.IndexOf("x")
来源：http://dv.bjjhwx.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xa.521024.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vq.szsharing.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ku.asd995.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pa.nicolike.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ff.asd995.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ge.hahajie.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gk.521024.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dl.gzmigu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pp.szsharing.cn

[E06] 替换子串
来源：http://dv.lnxyls.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ja.yuntaijiaju.cn

PHP:  str_replace("a", "b", $s);
来源：http://bq.wgjwhj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ms.jctech888.com.cn

TS:   s.replaceAll("a", "b")
来源：http://bc.panjiajie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tp.bookmarksfly.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bd.haigaiapp.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dg.bjjhwx.cn

C#:   s.Replace("a", "b")
来源：http://wv.bookmarksfly.cn

[E07] 按分隔符拆分
来源：http://nz.yuexingan06.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cs.yuexingan06.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hk.gzmigu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ot.lnxyls.cn

TS:   s.split(",")
来源：http://lz.nicolike.cn

Java: s.split(",");  s.split("\\s+")
来源：http://fq.szsharing.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fh.huixinmuqiang.cn

Ruby: s.split(",");  s.split
来源：http://ur.jianghongdianzi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hi.muxihuayi.cn

[E08] 数组按分隔符合并
来源：http://by.yuntaijiaju.cn

Py:   ",".join(items)
来源：http://vf.shtwfgs.cn

PHP:  implode(",", $items);
来源：http://yx.yuexingan06.cn

JS:   items.join(",")
来源：http://ts.szxytkj.cn

TS:   items.join(",")
来源：http://gm.yuntaijiaju.cn

Java: String.join(",", items)
来源：http://rd.yuntaijiaju.cn

Go:   strings.Join(items, ",")
来源：http://na.521024.cn

Ruby: items.join(",")
来源：http://hx.nicolike.cn

C#:   string.Join(",", items)
来源：http://kb.muxihuayi.cn

[E09] 去除所有空白字符
来源：http://vc.bookmarksfly.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://je.asd995.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ib.colortex.cn

JS:   s.replace(/\s+/g, "")
来源：http://kw.521024.cn

TS:   s.replace(/\s+/g, "")
来源：http://nj.huixiangedu.cn

Java: s.replaceAll("\\s+", "")
来源：http://mk.huixinmuqiang.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ua.jctech888.com.cn

Ruby: s.gsub(/\s+/, "")
来源：http://sl.haigaiapp.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bk.wgjwhj.cn

[E10] 左侧补零 / 定长填充
来源：http://rj.hnjuh.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ll.haigaiapp.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vo.huixiangedu.cn

JS:   "7".padStart(3, "0")
来源：http://it.jctech888.com.cn

TS:   "7".padStart(3, "0")
来源：http://bq.yuexingan06.cn

Java: String.format("%03d", 7)
来源：http://po.wgjwhj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://nk.yuexingan06.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ld.chemitech.net.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mg.shxzukj.cn

[E11] 反转字符串
来源：http://ye.newstarts.cn

Py:   s[::-1]
来源：http://eu.9csxet.cn

PHP:  strrev($s);
来源：http://gt.huixiangedu.cn

JS:   [...s].reverse().join("")
来源：http://gd.bookmarksfly.cn

TS:   [...s].reverse().join("")
来源：http://jw.shtwfgs.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zt.colortex.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://jy.huixiangedu.cn

Ruby: s.reverse
来源：http://jy.huanxung.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ot.shxzukj.cn

[E12] 统计某字符出现次数
来源：http://sf.haigaiapp.cn

Py:   s.count("a")
来源：http://bu.shtwfgs.cn

PHP:  substr_count($s, "a");
来源：http://kg.asd995.cn

JS:   s.split("a").length - 1
来源：http://jw.hnjuh.cn

TS:   s.split("a").length - 1
来源：http://pg.chemitech.net.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://br.colortex.cn

Go:   strings.Count(s, "a")
来源：http://te.newstarts.cn

Ruby: s.count("a")
来源：http://tz.jctech888.com.cn

C#:   s.Count(c => c == 'a')
来源：http://qh.lnxyls.cn

[E13] 逐字符遍历
来源：http://su.jctech888.com.cn


<!-- 参考信息 -->