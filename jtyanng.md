代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://tr.yuntaijiaju.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://la.huixinmuqiang.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://np.gzmigu.cn

[D06] 数组长度
来源：http://fx.bjjhwx.cn

Py:   len(arr)
来源：http://po.yuntaijiaju.cn

PHP:  count($arr);
来源：http://kv.chemitech.net.cn

JS:   arr.length
来源：http://dt.9csxet.cn

TS:   arr.length
来源：http://ad.521024.cn

Java: list.size();
来源：http://ug.hnjuh.cn

Go:   len(arr)
来源：http://mn.hahajie.cn

Ruby: arr.length; arr.size
来源：http://sh.newstarts.cn

C#:   list.Count;
来源：http://gr.nszjky.cn

[D07] 切片 / 取子数组
来源：http://cm.shxzukj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kj.yuntaijiaju.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ck.colortex.cn

JS:   arr.slice(1, 4);
来源：http://mt.lnxyls.cn

TS:   arr.slice(1, 4);
来源：http://dk.jctech888.com.cn

Java: list.subList(1, 4);
来源：http://sa.huixiangedu.cn

Go:   arr[1:4]
来源：http://nq.huixinmuqiang.cn

Ruby: arr[1, 3]
来源：http://af.hnjuh.cn

C#:   list.GetRange(1, 3);
来源：http://cy.bjjhwx.cn

[D08] 合并两个数组
来源：http://ja.huixiangedu.cn

Py:   a + b;  a.extend(b)
来源：http://vq.shxzskj.cn

PHP:  array_merge($a, $b);
来源：http://jd.yuexingan06.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://iz.lnxyls.cn

TS:   [...a, ...b];
来源：http://mb.nicolike.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wz.colortex.cn

Go:   append(a, b...)
来源：http://hd.hahajie.cn

Ruby: a + b;  a.concat(b)
来源：http://si.yuntaijiaju.cn

C#:   a.Concat(b).ToList()
来源：http://tv.yuexingan06.cn

[D09] 排序（升序）
来源：http://kp.huixiangedu.cn

Py:   sorted(arr);  arr.sort()
来源：http://zn.bookmarksfly.cn

PHP:  sort($arr);
来源：http://qw.shxzskj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://eq.521024.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://uu.nicolike.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://yg.muxihuayi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lm.9csxet.cn

Ruby: arr.sort
来源：http://rb.colortex.cn

C#:   list.Sort();
来源：http://ea.colortex.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://oq.bookmarksfly.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wj.szxytkj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yc.9csxet.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lp.521024.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qz.muxihuayi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tv.huixinmuqiang.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cr.521024.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://km.muxihuayi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pz.panjiajie.cn

[D11] 反转数组
来源：http://al.yuexingan06.cn

Py:   arr[::-1];  arr.reverse()
来源：http://oz.bjjhwx.cn

PHP:  array_reverse($arr);
来源：http://sz.yuntaijiaju.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kx.huanxung.cn

TS:   [...arr].reverse();
来源：http://zp.huixinmuqiang.cn

Java: Collections.reverse(list);
来源：http://mr.asd995.cn

Go:   slices.Reverse(arr)
来源：http://ik.chemitech.net.cn

Ruby: arr.reverse
来源：http://ue.huanxung.cn

C#:   list.Reverse();
来源：http://ue.chemitech.net.cn

[D12] 查找元素下标
来源：http://ge.521024.cn

Py:   arr.index(x);  x in arr
来源：http://xr.asd995.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xa.panjiajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ps.9csxet.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oq.muxihuayi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ea.shtwfgs.cn

Go:   slices.Index(arr, x)
来源：http://zn.jianghongdianzi.cn

Ruby: arr.index(x)
来源：http://wo.yuntaijiaju.cn

C#:   list.IndexOf(x);
来源：http://jg.wgjwhj.cn

[D13] 过滤（保留满足条件的）
来源：http://pm.nicolike.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sq.newstarts.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zp.huanxung.cn

JS:   arr.filter(x => x > 3)
来源：http://kz.asd995.cn

TS:   arr.filter(x => x > 3)
来源：http://yt.asd995.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rk.panjiajie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dn.huixiangedu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ff.jctech888.com.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://kj.shxzskj.cn

[D14] 映射转换（每个元素变形）
来源：http://dq.szxytkj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://we.haigaiapp.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nx.shtwfgs.cn

JS:   arr.map(x => x * 2)
来源：http://ck.bookmarksfly.cn

TS:   arr.map(x => x * 2)
来源：http://cw.shxzukj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://dq.jctech888.com.cn

Go:   // 手写循环
来源：http://bb.huixinmuqiang.cn

Ruby: arr.map { |x| x * 2 }
来源：http://bf.colortex.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://en.bjjhwx.cn

[D15] 去重
来源：http://wm.asd995.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qe.huixinmuqiang.cn

PHP:  array_unique($arr);
来源：http://va.jctech888.com.cn

JS:   [...new Set(arr)]
来源：http://db.bjjhwx.cn

TS:   [...new Set(arr)]
来源：http://fh.chemitech.net.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gt.shxzukj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://np.panjiajie.cn

Ruby: arr.uniq
来源：http://mc.wgjwhj.cn

C#:   list.Distinct().ToList()
来源：http://ol.521024.cn

[D16] 求和与平均值
来源：http://zo.muxihuayi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zo.shtwfgs.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cj.huixinmuqiang.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xq.chemitech.net.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tb.lnxyls.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tg.gzmigu.cn

Go:   // 手写循环累加
来源：http://uk.szxytkj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hd.shtwfgs.cn

C#:   list.Sum();  list.Average()
来源：http://yp.colortex.cn

[D17] 最大值与最小值
来源：http://bz.bookmarksfly.cn

Py:   max(arr);  min(arr)
来源：http://qi.asd995.cn

PHP:  max($arr);  min($arr);
来源：http://sw.szsharing.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dg.colortex.cn

TS:   Math.max(...arr);
来源：http://bv.lnxyls.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://px.shxzukj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vg.yuexingan06.cn

Ruby: arr.max;  arr.min
来源：http://pb.hnjuh.cn

C#:   list.Max();  list.Min()
来源：http://ej.nszjky.cn

[D18] 扁平化嵌套数组
来源：http://wd.yuexingan06.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ja.yuntaijiaju.cn

PHP:  array_merge(...$nested);
来源：http://yn.bookmarksfly.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://km.lnxyls.cn

TS:   nested.flat();
来源：http://fz.yuexingan06.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fh.yuexingan06.cn

Go:   // 手写双层循环
来源：http://zn.muxihuayi.cn

Ruby: nested.flatten
来源：http://gv.9csxet.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ai.panjiajie.cn

[D19] 按字段分组
来源：http://na.shxzskj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mq.shtwfgs.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lw.bookmarksfly.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wt.huanxung.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://yh.lnxyls.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sl.huixinmuqiang.cn

Go:   // 手写 map[string][]T
来源：http://gt.huanxung.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://xb.hnjuh.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jf.colortex.cn

[D20] 统计每个元素出现次数
来源：http://xn.szsharing.cn

Py:   Counter(arr)
来源：http://jm.colortex.cn

PHP:  array_count_values($arr);
来源：http://ly.huanxung.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ya.asd995.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nd.huixinmuqiang.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vw.shxzskj.cn

Go:   // 手写 map[T]int
来源：http://vz.shtwfgs.cn

Ruby: arr.tally
来源：http://ug.521024.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jt.wgjwhj.cn

[D21] 判断是否包含某元素
来源：http://yb.jianghongdianzi.cn

Py:   x in arr
来源：http://jg.huixiangedu.cn

PHP:  in_array($x, $arr, true);
来源：http://ub.shtwfgs.cn

JS:   arr.includes(x)
来源：http://fh.szxytkj.cn

TS:   arr.includes(x)
来源：http://jp.huanxung.cn

Java: list.contains(x)
来源：http://ym.jianghongdianzi.cn

Go:   slices.Contains(arr, x)
来源：http://hl.hnjuh.cn

Ruby: arr.include?(x)
来源：http://rr.yuexingan06.cn

C#:   list.Contains(x)
来源：http://ux.jctech888.com.cn

[D22] 复制数组（避免共享引用）
来源：http://gv.colortex.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pc.hahajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kz.jctech888.com.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lr.muxihuayi.cn

TS:   [...arr];
来源：http://xv.bjjhwx.cn

Java: new ArrayList<>(list);
来源：http://lf.newstarts.cn

Go:   copied := append([]int(nil), arr...)
来源：http://pl.shxzskj.cn

Ruby: arr.dup;  arr.clone
来源：http://tc.huixiangedu.cn

C#:   new List<int>(list);
来源：http://sc.shtwfgs.cn

[D23] reduce 累积计算
来源：http://px.hahajie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hu.gzmigu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tq.newstarts.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pl.nszjky.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iy.colortex.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://cr.lnxyls.cn

Go:   // 手写循环
来源：http://uc.yuntaijiaju.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pz.haigaiapp.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cm.yuntaijiaju.cn

[D24] 字典 / Map 基本操作
来源：http://yj.yuntaijiaju.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rj.bjjhwx.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hi.hahajie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pp.chemitech.net.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wn.newstarts.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ke.huixinmuqiang.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ut.521024.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rp.wgjwhj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ef.newstarts.cn

[D25] Set 集合去重与交并差
来源：http://it.huixiangedu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ki.9csxet.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lk.newstarts.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mp.huixinmuqiang.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fr.9csxet.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bg.chemitech.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mz.huixinmuqiang.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fm.hnjuh.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qq.huixinmuqiang.cn

[D26] 数组转字符串
来源：http://jj.jctech888.com.cn

Py:   ", ".join(map(str, arr))
来源：http://xl.newstarts.cn

PHP:  implode(", ", $arr);
来源：http://oz.bookmarksfly.cn

JS:   arr.join(", ")
来源：http://nc.jianghongdianzi.cn

TS:   arr.join(", ")
来源：http://wi.colortex.cn

Java: String.join(", ", list)
来源：http://ck.lnxyls.cn

Go:   strings.Join(strs, ", ")
来源：http://be.bookmarksfly.cn

Ruby: arr.join(", ")
来源：http://uh.szxytkj.cn

C#:   string.Join(", ", list)
来源：http://tn.bookmarksfly.cn

================================================================================
来源：http://rr.jctech888.com.cn

E. 字符串处理
来源：http://ox.panjiajie.cn

================================================================================
来源：http://od.asd995.cn

[E01] 拼接字符串
来源：http://br.asd995.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yt.haigaiapp.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xt.chemitech.net.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xf.nicolike.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ke.yuntaijiaju.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ve.colortex.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sl.bookmarksfly.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wa.huixiangedu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ie.wgjwhj.cn

[E02] 重复字符串
来源：http://iu.haigaiapp.cn

Py:   "ab" * 3
来源：http://dt.yuexingan06.cn

PHP:  str_repeat("ab", 3);
来源：http://hu.jianghongdianzi.cn

JS:   "ab".repeat(3)
来源：http://il.huanxung.cn

TS:   "ab".repeat(3)
来源：http://wu.lnxyls.cn

Java: "ab".repeat(3)
来源：http://dd.szxytkj.cn

Go:   strings.Repeat("ab", 3)
来源：http://ps.nicolike.cn

Ruby: "ab" * 3
来源：http://qh.huanxung.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bj.wgjwhj.cn

[E03] 截取子串
来源：http://sv.wgjwhj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dr.nicolike.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lp.huixinmuqiang.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yy.muxihuayi.cn

TS:   s.slice(1, 4)
来源：http://wj.gzmigu.cn

Java: s.substring(1, 4)
来源：http://zm.szxytkj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vf.yuexingan06.cn

Ruby: s[1, 3];  s[1..3]
来源：http://lb.haigaiapp.cn

C#:   s.Substring(1, 3)
来源：http://kp.panjiajie.cn

[E04] 查找子串位置
来源：http://pc.colortex.cn

Py:   s.find("x");  s.index("x")
来源：http://bm.bookmarksfly.cn

PHP:  strpos($s, "x");
来源：http://qy.huanxung.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tb.gzmigu.cn

TS:   s.indexOf("x")
来源：http://dj.newstarts.cn

Java: s.indexOf("x")
来源：http://ph.9csxet.cn

Go:   strings.Index(s, "x")
来源：http://rx.huixinmuqiang.cn

Ruby: s.index("x")
来源：http://tb.chemitech.net.cn

C#:   s.IndexOf("x")
来源：http://ab.hnjuh.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://on.colortex.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://od.muxihuayi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yd.panjiajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uf.newstarts.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://eb.chemitech.net.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wc.521024.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://io.jianghongdianzi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hm.haigaiapp.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kz.hnjuh.cn

[E06] 替换子串
来源：http://pg.huixinmuqiang.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wm.huixiangedu.cn

PHP:  str_replace("a", "b", $s);
来源：http://xa.newstarts.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jn.jctech888.com.cn

TS:   s.replaceAll("a", "b")
来源：http://oo.huanxung.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zc.asd995.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://em.wgjwhj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://py.shxzukj.cn

C#:   s.Replace("a", "b")
来源：http://ya.szsharing.cn

[E07] 按分隔符拆分
来源：http://xn.szsharing.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lf.bjjhwx.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nl.hahajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://dz.szsharing.cn

TS:   s.split(",")
来源：http://it.wgjwhj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://mu.nicolike.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mt.nicolike.cn

Ruby: s.split(",");  s.split
来源：http://rt.gzmigu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kl.lnxyls.cn

[E08] 数组按分隔符合并
来源：http://lz.newstarts.cn

Py:   ",".join(items)
来源：http://ko.shtwfgs.cn

PHP:  implode(",", $items);
来源：http://zi.9csxet.cn

JS:   items.join(",")
来源：http://zu.haigaiapp.cn

TS:   items.join(",")
来源：http://ci.521024.cn

Java: String.join(",", items)
来源：http://ax.huixiangedu.cn

Go:   strings.Join(items, ",")
来源：http://qi.huixinmuqiang.cn

Ruby: items.join(",")
来源：http://dw.shtwfgs.cn

C#:   string.Join(",", items)
来源：http://ve.lnxyls.cn

[E09] 去除所有空白字符
来源：http://qt.bjjhwx.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hx.521024.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://et.asd995.cn

JS:   s.replace(/\s+/g, "")
来源：http://ck.nszjky.cn

TS:   s.replace(/\s+/g, "")
来源：http://yl.9csxet.cn

Java: s.replaceAll("\\s+", "")
来源：http://xa.9csxet.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://sg.jctech888.com.cn

Ruby: s.gsub(/\s+/, "")
来源：http://zp.wgjwhj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zq.yuexingan06.cn

[E10] 左侧补零 / 定长填充
来源：http://yv.hahajie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mi.wgjwhj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ky.nszjky.cn

JS:   "7".padStart(3, "0")
来源：http://il.shxzukj.cn

TS:   "7".padStart(3, "0")
来源：http://jd.hnjuh.cn

Java: String.format("%03d", 7)
来源：http://ca.bjjhwx.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://yh.jctech888.com.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hn.yuexingan06.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://en.jctech888.com.cn

[E11] 反转字符串
来源：http://qq.chemitech.net.cn

Py:   s[::-1]
来源：http://hj.yuntaijiaju.cn

PHP:  strrev($s);
来源：http://fj.nszjky.cn

JS:   [...s].reverse().join("")
来源：http://td.haigaiapp.cn

TS:   [...s].reverse().join("")
来源：http://mr.panjiajie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://kn.muxihuayi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://xi.szsharing.cn

Ruby: s.reverse
来源：http://ix.huixiangedu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://le.muxihuayi.cn

[E12] 统计某字符出现次数
来源：http://ju.szsharing.cn

Py:   s.count("a")
来源：http://nj.asd995.cn

PHP:  substr_count($s, "a");
来源：http://oh.haigaiapp.cn

JS:   s.split("a").length - 1
来源：http://xw.szsharing.cn

TS:   s.split("a").length - 1
来源：http://xa.huixinmuqiang.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vt.colortex.cn


<!-- 参考信息 -->