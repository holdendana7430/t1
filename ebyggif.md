代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://lj.nszjky.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tq.chemitech.net.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://et.jianghongdianzi.cn

[D06] 数组长度
来源：http://hh.shxzskj.cn

Py:   len(arr)
来源：http://qp.muxihuayi.cn

PHP:  count($arr);
来源：http://yu.colortex.cn

JS:   arr.length
来源：http://wq.jianghongdianzi.cn

TS:   arr.length
来源：http://bg.chemitech.net.cn

Java: list.size();
来源：http://zr.shtwfgs.cn

Go:   len(arr)
来源：http://od.colortex.cn

Ruby: arr.length; arr.size
来源：http://ct.shtwfgs.cn

C#:   list.Count;
来源：http://vq.bjjhwx.cn

[D07] 切片 / 取子数组
来源：http://fz.chemitech.net.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lc.asd995.cn

PHP:  array_slice($arr, 1, 3);
来源：http://io.muxihuayi.cn

JS:   arr.slice(1, 4);
来源：http://oq.shxzskj.cn

TS:   arr.slice(1, 4);
来源：http://ty.bookmarksfly.cn

Java: list.subList(1, 4);
来源：http://rm.chemitech.net.cn

Go:   arr[1:4]
来源：http://kv.huanxung.cn

Ruby: arr[1, 3]
来源：http://if.hahajie.cn

C#:   list.GetRange(1, 3);
来源：http://wj.shtwfgs.cn

[D08] 合并两个数组
来源：http://is.shtwfgs.cn

Py:   a + b;  a.extend(b)
来源：http://lj.shxzskj.cn

PHP:  array_merge($a, $b);
来源：http://je.jianghongdianzi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://kp.yuexingan06.cn

TS:   [...a, ...b];
来源：http://kl.shxzskj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vu.nicolike.cn

Go:   append(a, b...)
来源：http://vy.muxihuayi.cn

Ruby: a + b;  a.concat(b)
来源：http://ki.hahajie.cn

C#:   a.Concat(b).ToList()
来源：http://gl.shxzukj.cn

[D09] 排序（升序）
来源：http://jc.bjjhwx.cn

Py:   sorted(arr);  arr.sort()
来源：http://mt.hahajie.cn

PHP:  sort($arr);
来源：http://qj.panjiajie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ly.shtwfgs.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://te.gzmigu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://pq.hahajie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://oq.colortex.cn

Ruby: arr.sort
来源：http://nn.bjjhwx.cn

C#:   list.Sort();
来源：http://ym.haigaiapp.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://sm.gzmigu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ca.panjiajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oy.jctech888.com.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ub.521024.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xl.huanxung.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ga.szxytkj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lq.shxzskj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yw.hahajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qr.yuexingan06.cn

[D11] 反转数组
来源：http://ks.huanxung.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wf.szxytkj.cn

PHP:  array_reverse($arr);
来源：http://yi.bjjhwx.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.shxzskj.cn

TS:   [...arr].reverse();
来源：http://yn.nicolike.cn

Java: Collections.reverse(list);
来源：http://pf.szsharing.cn

Go:   slices.Reverse(arr)
来源：http://wr.bjjhwx.cn

Ruby: arr.reverse
来源：http://kb.bjjhwx.cn

C#:   list.Reverse();
来源：http://mg.szxytkj.cn

[D12] 查找元素下标
来源：http://oq.yuexingan06.cn

Py:   arr.index(x);  x in arr
来源：http://mk.panjiajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://iq.jianghongdianzi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rc.haigaiapp.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lw.szsharing.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://eb.panjiajie.cn

Go:   slices.Index(arr, x)
来源：http://oo.newstarts.cn

Ruby: arr.index(x)
来源：http://sf.szxytkj.cn

C#:   list.IndexOf(x);
来源：http://qy.lnxyls.cn

[D13] 过滤（保留满足条件的）
来源：http://nd.521024.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fy.szxytkj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sk.panjiajie.cn

JS:   arr.filter(x => x > 3)
来源：http://po.hahajie.cn

TS:   arr.filter(x => x > 3)
来源：http://az.9csxet.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rw.bookmarksfly.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bh.huixiangedu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://sq.bookmarksfly.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://fo.lnxyls.cn

[D14] 映射转换（每个元素变形）
来源：http://rp.muxihuayi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bx.9csxet.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ru.huixinmuqiang.cn

JS:   arr.map(x => x * 2)
来源：http://ge.huixinmuqiang.cn

TS:   arr.map(x => x * 2)
来源：http://lf.jctech888.com.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://my.lnxyls.cn

Go:   // 手写循环
来源：http://jy.huixinmuqiang.cn

Ruby: arr.map { |x| x * 2 }
来源：http://bk.gzmigu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ka.shtwfgs.cn

[D15] 去重
来源：http://yd.nszjky.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jq.yuntaijiaju.cn

PHP:  array_unique($arr);
来源：http://sm.bookmarksfly.cn

JS:   [...new Set(arr)]
来源：http://bk.chemitech.net.cn

TS:   [...new Set(arr)]
来源：http://mb.shxzukj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yg.shxzukj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://mb.jianghongdianzi.cn

Ruby: arr.uniq
来源：http://to.huanxung.cn

C#:   list.Distinct().ToList()
来源：http://yr.huixinmuqiang.cn

[D16] 求和与平均值
来源：http://co.hnjuh.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qh.yuntaijiaju.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gq.panjiajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qz.nszjky.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fo.bookmarksfly.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tq.lnxyls.cn

Go:   // 手写循环累加
来源：http://jy.muxihuayi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pd.bookmarksfly.cn

C#:   list.Sum();  list.Average()
来源：http://ft.muxihuayi.cn

[D17] 最大值与最小值
来源：http://db.yuntaijiaju.cn

Py:   max(arr);  min(arr)
来源：http://ds.muxihuayi.cn

PHP:  max($arr);  min($arr);
来源：http://pk.jianghongdianzi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ua.gzmigu.cn

TS:   Math.max(...arr);
来源：http://yo.jianghongdianzi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://tb.chemitech.net.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bv.haigaiapp.cn

Ruby: arr.max;  arr.min
来源：http://dr.huanxung.cn

C#:   list.Max();  list.Min()
来源：http://qd.chemitech.net.cn

[D18] 扁平化嵌套数组
来源：http://pb.colortex.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bo.yuntaijiaju.cn

PHP:  array_merge(...$nested);
来源：http://ap.yuexingan06.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pw.jctech888.com.cn

TS:   nested.flat();
来源：http://ze.huanxung.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jd.nicolike.cn

Go:   // 手写双层循环
来源：http://sk.newstarts.cn

Ruby: nested.flatten
来源：http://yy.hahajie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://sq.asd995.cn

[D19] 按字段分组
来源：http://km.shtwfgs.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lh.gzmigu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fo.hnjuh.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jo.hahajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xo.lnxyls.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fa.haigaiapp.cn

Go:   // 手写 map[string][]T
来源：http://oo.jianghongdianzi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ji.nszjky.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ar.9csxet.cn

[D20] 统计每个元素出现次数
来源：http://hu.newstarts.cn

Py:   Counter(arr)
来源：http://rn.yuexingan06.cn

PHP:  array_count_values($arr);
来源：http://om.panjiajie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xf.huixiangedu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oc.asd995.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dx.shtwfgs.cn

Go:   // 手写 map[T]int
来源：http://fb.nszjky.cn

Ruby: arr.tally
来源：http://cn.bookmarksfly.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rs.hahajie.cn

[D21] 判断是否包含某元素
来源：http://ma.yuexingan06.cn

Py:   x in arr
来源：http://tv.newstarts.cn

PHP:  in_array($x, $arr, true);
来源：http://vc.asd995.cn

JS:   arr.includes(x)
来源：http://vj.jianghongdianzi.cn

TS:   arr.includes(x)
来源：http://mg.shxzukj.cn

Java: list.contains(x)
来源：http://mg.colortex.cn

Go:   slices.Contains(arr, x)
来源：http://qr.shxzskj.cn

Ruby: arr.include?(x)
来源：http://la.haigaiapp.cn

C#:   list.Contains(x)
来源：http://ct.yuntaijiaju.cn

[D22] 复制数组（避免共享引用）
来源：http://dl.521024.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ge.haigaiapp.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mu.hahajie.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yq.bjjhwx.cn

TS:   [...arr];
来源：http://zb.shxzukj.cn

Java: new ArrayList<>(list);
来源：http://lk.shtwfgs.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qk.hnjuh.cn

Ruby: arr.dup;  arr.clone
来源：http://dq.nicolike.cn

C#:   new List<int>(list);
来源：http://pa.huixiangedu.cn

[D23] reduce 累积计算
来源：http://lf.muxihuayi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xd.panjiajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zs.nszjky.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rr.hnjuh.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gk.bookmarksfly.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fg.szsharing.cn

Go:   // 手写循环
来源：http://rz.wgjwhj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tc.haigaiapp.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zu.shxzukj.cn

[D24] 字典 / Map 基本操作
来源：http://ks.panjiajie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ai.yuexingan06.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sp.shxzukj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://yg.newstarts.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kg.jctech888.com.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lx.shtwfgs.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jq.szxytkj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://by.muxihuayi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://av.shxzukj.cn

[D25] Set 集合去重与交并差
来源：http://ki.9csxet.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vd.lnxyls.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jy.huanxung.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gb.szsharing.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bm.hahajie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gj.asd995.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fe.huixiangedu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wl.jctech888.com.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://eb.shxzskj.cn

[D26] 数组转字符串
来源：http://ud.huixiangedu.cn

Py:   ", ".join(map(str, arr))
来源：http://wg.huixiangedu.cn

PHP:  implode(", ", $arr);
来源：http://qj.yuexingan06.cn

JS:   arr.join(", ")
来源：http://pr.nszjky.cn

TS:   arr.join(", ")
来源：http://ay.shxzukj.cn

Java: String.join(", ", list)
来源：http://wu.haigaiapp.cn

Go:   strings.Join(strs, ", ")
来源：http://qy.colortex.cn

Ruby: arr.join(", ")
来源：http://ub.jianghongdianzi.cn

C#:   string.Join(", ", list)
来源：http://ng.huixiangedu.cn

================================================================================
来源：http://vf.nszjky.cn

E. 字符串处理
来源：http://rb.szsharing.cn

================================================================================
来源：http://xq.huanxung.cn

[E01] 拼接字符串
来源：http://ur.shtwfgs.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fw.bookmarksfly.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://so.huixinmuqiang.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qv.newstarts.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bh.huixinmuqiang.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hc.bjjhwx.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ad.jianghongdianzi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lq.lnxyls.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nh.jctech888.com.cn

[E02] 重复字符串
来源：http://sl.521024.cn

Py:   "ab" * 3
来源：http://iw.wgjwhj.cn

PHP:  str_repeat("ab", 3);
来源：http://gk.hnjuh.cn

JS:   "ab".repeat(3)
来源：http://gq.yuntaijiaju.cn

TS:   "ab".repeat(3)
来源：http://lb.huixiangedu.cn

Java: "ab".repeat(3)
来源：http://rx.shxzukj.cn

Go:   strings.Repeat("ab", 3)
来源：http://ac.szsharing.cn

Ruby: "ab" * 3
来源：http://jt.huanxung.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fi.muxihuayi.cn

[E03] 截取子串
来源：http://dl.shtwfgs.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vg.asd995.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gz.huixinmuqiang.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://aw.nszjky.cn

TS:   s.slice(1, 4)
来源：http://sk.nicolike.cn

Java: s.substring(1, 4)
来源：http://wj.hahajie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ut.szxytkj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://jx.szxytkj.cn

C#:   s.Substring(1, 3)
来源：http://zu.panjiajie.cn

[E04] 查找子串位置
来源：http://nw.yuntaijiaju.cn

Py:   s.find("x");  s.index("x")
来源：http://nw.wgjwhj.cn

PHP:  strpos($s, "x");
来源：http://va.lnxyls.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xa.bjjhwx.cn

TS:   s.indexOf("x")
来源：http://gm.huixinmuqiang.cn

Java: s.indexOf("x")
来源：http://iy.shtwfgs.cn

Go:   strings.Index(s, "x")
来源：http://lc.szxytkj.cn

Ruby: s.index("x")
来源：http://wu.shxzskj.cn

C#:   s.IndexOf("x")
来源：http://ea.jianghongdianzi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://as.wgjwhj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ts.shxzskj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ib.wgjwhj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uj.bjjhwx.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hm.haigaiapp.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rr.szsharing.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nc.shxzskj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jt.521024.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wy.huanxung.cn

[E06] 替换子串
来源：http://yy.panjiajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sb.bjjhwx.cn

PHP:  str_replace("a", "b", $s);
来源：http://ez.szsharing.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ok.yuexingan06.cn

TS:   s.replaceAll("a", "b")
来源：http://yc.shtwfgs.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rz.hnjuh.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sw.huixinmuqiang.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yh.szxytkj.cn

C#:   s.Replace("a", "b")
来源：http://yy.huixinmuqiang.cn

[E07] 按分隔符拆分
来源：http://af.huixiangedu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xe.szxytkj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://on.szxytkj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://th.newstarts.cn

TS:   s.split(",")
来源：http://zl.yuntaijiaju.cn

Java: s.split(",");  s.split("\\s+")
来源：http://cj.shxzskj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rd.shtwfgs.cn

Ruby: s.split(",");  s.split
来源：http://ed.shtwfgs.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dr.hnjuh.cn

[E08] 数组按分隔符合并
来源：http://vd.colortex.cn

Py:   ",".join(items)
来源：http://px.nicolike.cn

PHP:  implode(",", $items);
来源：http://an.huixinmuqiang.cn

JS:   items.join(",")
来源：http://pa.lnxyls.cn

TS:   items.join(",")
来源：http://co.wgjwhj.cn

Java: String.join(",", items)
来源：http://nc.hahajie.cn

Go:   strings.Join(items, ",")
来源：http://kg.szxytkj.cn

Ruby: items.join(",")
来源：http://bl.panjiajie.cn

C#:   string.Join(",", items)
来源：http://st.gzmigu.cn

[E09] 去除所有空白字符
来源：http://cn.haigaiapp.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lg.nszjky.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ct.huixinmuqiang.cn

JS:   s.replace(/\s+/g, "")
来源：http://fg.asd995.cn

TS:   s.replace(/\s+/g, "")
来源：http://tg.lnxyls.cn

Java: s.replaceAll("\\s+", "")
来源：http://ps.huixinmuqiang.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://tf.jctech888.com.cn

Ruby: s.gsub(/\s+/, "")
来源：http://sz.asd995.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gn.gzmigu.cn

[E10] 左侧补零 / 定长填充
来源：http://dr.521024.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ab.nszjky.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://iq.jianghongdianzi.cn

JS:   "7".padStart(3, "0")
来源：http://oj.hahajie.cn

TS:   "7".padStart(3, "0")
来源：http://xy.szsharing.cn

Java: String.format("%03d", 7)
来源：http://pp.szsharing.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://wn.muxihuayi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bn.shxzukj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yw.huixiangedu.cn

[E11] 反转字符串
来源：http://ju.shxzskj.cn

Py:   s[::-1]
来源：http://fs.bookmarksfly.cn

PHP:  strrev($s);
来源：http://bd.nicolike.cn

JS:   [...s].reverse().join("")
来源：http://cl.asd995.cn

TS:   [...s].reverse().join("")
来源：http://di.szsharing.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ru.chemitech.net.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://gm.nicolike.cn

Ruby: s.reverse
来源：http://az.shtwfgs.cn

C#:   new string(s.Reverse().ToArray())
来源：http://rz.bookmarksfly.cn

[E12] 统计某字符出现次数
来源：http://xt.lnxyls.cn

Py:   s.count("a")
来源：http://sr.colortex.cn

PHP:  substr_count($s, "a");
来源：http://ss.szsharing.cn

JS:   s.split("a").length - 1
来源：http://bi.hnjuh.cn

TS:   s.split("a").length - 1
来源：http://cc.huixinmuqiang.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://am.huanxung.cn


<!-- 参考信息 -->