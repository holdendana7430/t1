代发 wailian999

Py:   len(arr)
来源：http://ix.huixinmuqiang.cn

PHP:  count($arr);
来源：http://vg.panjiajie.cn

JS:   arr.length
来源：http://oe.yuntaijiaju.cn

TS:   arr.length
来源：http://ke.yuexingan06.cn

Java: list.size();
来源：http://xs.haigaiapp.cn

Go:   len(arr)
来源：http://ic.jctech888.com.cn

Ruby: arr.length; arr.size
来源：http://fh.asd995.cn

C#:   list.Count;
来源：http://ad.newstarts.cn

[D07] 切片 / 取子数组
来源：http://yi.huixiangedu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vm.huanxung.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gp.jctech888.com.cn

JS:   arr.slice(1, 4);
来源：http://zq.muxihuayi.cn

TS:   arr.slice(1, 4);
来源：http://hl.yuntaijiaju.cn

Java: list.subList(1, 4);
来源：http://wq.asd995.cn

Go:   arr[1:4]
来源：http://hy.szsharing.cn

Ruby: arr[1, 3]
来源：http://fb.huixinmuqiang.cn

C#:   list.GetRange(1, 3);
来源：http://yw.newstarts.cn

[D08] 合并两个数组
来源：http://id.yuexingan06.cn

Py:   a + b;  a.extend(b)
来源：http://jr.shtwfgs.cn

PHP:  array_merge($a, $b);
来源：http://ck.chemitech.net.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://og.bookmarksfly.cn

TS:   [...a, ...b];
来源：http://oz.hahajie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kf.colortex.cn

Go:   append(a, b...)
来源：http://qr.huixinmuqiang.cn

Ruby: a + b;  a.concat(b)
来源：http://uj.panjiajie.cn

C#:   a.Concat(b).ToList()
来源：http://em.lnxyls.cn

[D09] 排序（升序）
来源：http://tt.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://op.newstarts.cn

PHP:  sort($arr);
来源：http://by.nicolike.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://is.colortex.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ob.huixiangedu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vm.jctech888.com.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yj.hnjuh.cn

Ruby: arr.sort
来源：http://ik.lnxyls.cn

C#:   list.Sort();
来源：http://gj.muxihuayi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ua.hnjuh.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://by.nicolike.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sl.shxzukj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rr.9csxet.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://iv.9csxet.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://im.bookmarksfly.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zh.jctech888.com.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ib.panjiajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fj.shxzukj.cn

[D11] 反转数组
来源：http://hw.haigaiapp.cn

Py:   arr[::-1];  arr.reverse()
来源：http://vh.521024.cn

PHP:  array_reverse($arr);
来源：http://uh.szxytkj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qg.huanxung.cn

TS:   [...arr].reverse();
来源：http://bj.bookmarksfly.cn

Java: Collections.reverse(list);
来源：http://up.colortex.cn

Go:   slices.Reverse(arr)
来源：http://ys.wgjwhj.cn

Ruby: arr.reverse
来源：http://ue.wgjwhj.cn

C#:   list.Reverse();
来源：http://de.gzmigu.cn

[D12] 查找元素下标
来源：http://kk.yuntaijiaju.cn

Py:   arr.index(x);  x in arr
来源：http://su.colortex.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fo.521024.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://if.yuntaijiaju.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rx.szxytkj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zh.hahajie.cn

Go:   slices.Index(arr, x)
来源：http://xc.jianghongdianzi.cn

Ruby: arr.index(x)
来源：http://ix.lnxyls.cn

C#:   list.IndexOf(x);
来源：http://fx.huanxung.cn

[D13] 过滤（保留满足条件的）
来源：http://ps.asd995.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tx.colortex.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://va.huixinmuqiang.cn

JS:   arr.filter(x => x > 3)
来源：http://aw.gzmigu.cn

TS:   arr.filter(x => x > 3)
来源：http://oy.bjjhwx.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ur.bookmarksfly.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bc.bjjhwx.cn

Ruby: arr.select { |x| x > 3 }
来源：http://it.chemitech.net.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://de.nszjky.cn

[D14] 映射转换（每个元素变形）
来源：http://ra.wgjwhj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://eb.huixinmuqiang.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yp.huixinmuqiang.cn

JS:   arr.map(x => x * 2)
来源：http://qs.muxihuayi.cn

TS:   arr.map(x => x * 2)
来源：http://he.hahajie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://vg.lnxyls.cn

Go:   // 手写循环
来源：http://tb.bjjhwx.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vn.nszjky.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://nb.newstarts.cn

[D15] 去重
来源：http://ja.jianghongdianzi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lp.szsharing.cn

PHP:  array_unique($arr);
来源：http://jr.hahajie.cn

JS:   [...new Set(arr)]
来源：http://gx.9csxet.cn

TS:   [...new Set(arr)]
来源：http://qb.yuexingan06.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://su.chemitech.net.cn

Go:   // 用 map[T]struct{} 手写
来源：http://jo.asd995.cn

Ruby: arr.uniq
来源：http://on.huixinmuqiang.cn

C#:   list.Distinct().ToList()
来源：http://om.muxihuayi.cn

[D16] 求和与平均值
来源：http://ap.hahajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nq.9csxet.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mj.shtwfgs.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bc.huanxung.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yq.chemitech.net.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xh.shxzskj.cn

Go:   // 手写循环累加
来源：http://bu.yuexingan06.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://za.yuexingan06.cn

C#:   list.Sum();  list.Average()
来源：http://kw.wgjwhj.cn

[D17] 最大值与最小值
来源：http://pu.jctech888.com.cn

Py:   max(arr);  min(arr)
来源：http://bd.bjjhwx.cn

PHP:  max($arr);  min($arr);
来源：http://ne.panjiajie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cm.shtwfgs.cn

TS:   Math.max(...arr);
来源：http://ft.colortex.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://sl.jianghongdianzi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://np.panjiajie.cn

Ruby: arr.max;  arr.min
来源：http://vd.panjiajie.cn

C#:   list.Max();  list.Min()
来源：http://qb.nszjky.cn

[D18] 扁平化嵌套数组
来源：http://cg.hnjuh.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kw.521024.cn

PHP:  array_merge(...$nested);
来源：http://ue.hahajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hm.jctech888.com.cn

TS:   nested.flat();
来源：http://yv.newstarts.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dj.szxytkj.cn

Go:   // 手写双层循环
来源：http://ww.szxytkj.cn

Ruby: nested.flatten
来源：http://gb.muxihuayi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://sf.muxihuayi.cn

[D19] 按字段分组
来源：http://dn.9csxet.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ac.jianghongdianzi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ls.haigaiapp.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ry.jctech888.com.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://zf.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gr.jctech888.com.cn

Go:   // 手写 map[string][]T
来源：http://jq.9csxet.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://vq.haigaiapp.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jd.huixiangedu.cn

[D20] 统计每个元素出现次数
来源：http://zb.jctech888.com.cn

Py:   Counter(arr)
来源：http://ar.szxytkj.cn

PHP:  array_count_values($arr);
来源：http://vm.newstarts.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fm.yuexingan06.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://on.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jf.521024.cn

Go:   // 手写 map[T]int
来源：http://ua.wgjwhj.cn

Ruby: arr.tally
来源：http://ti.yuntaijiaju.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rp.521024.cn

[D21] 判断是否包含某元素
来源：http://wm.wgjwhj.cn

Py:   x in arr
来源：http://pg.jctech888.com.cn

PHP:  in_array($x, $arr, true);
来源：http://pg.szxytkj.cn

JS:   arr.includes(x)
来源：http://db.haigaiapp.cn

TS:   arr.includes(x)
来源：http://ff.szsharing.cn

Java: list.contains(x)
来源：http://yy.shxzukj.cn

Go:   slices.Contains(arr, x)
来源：http://cw.wgjwhj.cn

Ruby: arr.include?(x)
来源：http://qo.colortex.cn

C#:   list.Contains(x)
来源：http://cx.lnxyls.cn

[D22] 复制数组（避免共享引用）
来源：http://ub.yuntaijiaju.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://uw.yuntaijiaju.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ag.muxihuayi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jq.shxzskj.cn

TS:   [...arr];
来源：http://qq.szsharing.cn

Java: new ArrayList<>(list);
来源：http://vy.shxzukj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://dx.huanxung.cn

Ruby: arr.dup;  arr.clone
来源：http://ie.asd995.cn

C#:   new List<int>(list);
来源：http://tr.newstarts.cn

[D23] reduce 累积计算
来源：http://if.shtwfgs.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://up.shxzukj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yr.asd995.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mf.huanxung.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uk.shtwfgs.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://bj.wgjwhj.cn

Go:   // 手写循环
来源：http://mg.shxzukj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ft.hahajie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://oi.huixiangedu.cn

[D24] 字典 / Map 基本操作
来源：http://oz.hnjuh.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jt.shxzukj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nl.shxzskj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://or.szsharing.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lp.9csxet.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://sk.bjjhwx.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pj.huanxung.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://iu.chemitech.net.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bs.jctech888.com.cn

[D25] Set 集合去重与交并差
来源：http://bv.panjiajie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jw.muxihuayi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fo.szsharing.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tt.szxytkj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jn.wgjwhj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xh.hahajie.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gv.yuexingan06.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zl.lnxyls.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ck.huanxung.cn

[D26] 数组转字符串
来源：http://kv.newstarts.cn

Py:   ", ".join(map(str, arr))
来源：http://wi.huixinmuqiang.cn

PHP:  implode(", ", $arr);
来源：http://sq.yuexingan06.cn

JS:   arr.join(", ")
来源：http://te.asd995.cn

TS:   arr.join(", ")
来源：http://sl.colortex.cn

Java: String.join(", ", list)
来源：http://ob.huixiangedu.cn

Go:   strings.Join(strs, ", ")
来源：http://gt.hahajie.cn

Ruby: arr.join(", ")
来源：http://an.shxzukj.cn

C#:   string.Join(", ", list)
来源：http://xw.shtwfgs.cn

================================================================================
来源：http://gr.huixiangedu.cn

E. 字符串处理
来源：http://qh.yuntaijiaju.cn

================================================================================
来源：http://zk.yuntaijiaju.cn

[E01] 拼接字符串
来源：http://da.yuexingan06.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zf.521024.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sr.yuntaijiaju.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nb.yuexingan06.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://te.chemitech.net.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pn.yuexingan06.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zc.huixiangedu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zs.shtwfgs.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bi.szsharing.cn

[E02] 重复字符串
来源：http://vb.nszjky.cn

Py:   "ab" * 3
来源：http://zo.hahajie.cn

PHP:  str_repeat("ab", 3);
来源：http://cp.hnjuh.cn

JS:   "ab".repeat(3)
来源：http://ts.yuexingan06.cn

TS:   "ab".repeat(3)
来源：http://bn.colortex.cn

Java: "ab".repeat(3)
来源：http://jf.nszjky.cn

Go:   strings.Repeat("ab", 3)
来源：http://up.shxzukj.cn

Ruby: "ab" * 3
来源：http://zf.jctech888.com.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ev.shxzskj.cn

[E03] 截取子串
来源：http://yq.gzmigu.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qw.chemitech.net.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xl.gzmigu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ur.hahajie.cn

TS:   s.slice(1, 4)
来源：http://je.hnjuh.cn

Java: s.substring(1, 4)
来源：http://my.shxzskj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lu.szsharing.cn

Ruby: s[1, 3];  s[1..3]
来源：http://or.hahajie.cn

C#:   s.Substring(1, 3)
来源：http://bm.shtwfgs.cn

[E04] 查找子串位置
来源：http://ch.nszjky.cn

Py:   s.find("x");  s.index("x")
来源：http://he.shtwfgs.cn

PHP:  strpos($s, "x");
来源：http://oe.shtwfgs.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jg.shxzukj.cn

TS:   s.indexOf("x")
来源：http://lk.huixiangedu.cn

Java: s.indexOf("x")
来源：http://ry.yuntaijiaju.cn

Go:   strings.Index(s, "x")
来源：http://eh.chemitech.net.cn

Ruby: s.index("x")
来源：http://mi.panjiajie.cn

C#:   s.IndexOf("x")
来源：http://wz.huanxung.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://bb.521024.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lf.bookmarksfly.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://an.lnxyls.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nj.haigaiapp.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://tc.bookmarksfly.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ct.huixinmuqiang.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ya.newstarts.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ns.bjjhwx.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lp.colortex.cn

[E06] 替换子串
来源：http://kb.huixinmuqiang.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ct.hahajie.cn

PHP:  str_replace("a", "b", $s);
来源：http://om.hahajie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iy.huixinmuqiang.cn

TS:   s.replaceAll("a", "b")
来源：http://iz.shtwfgs.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://re.nszjky.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://iy.asd995.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bc.huixinmuqiang.cn

C#:   s.Replace("a", "b")
来源：http://cg.jctech888.com.cn

[E07] 按分隔符拆分
来源：http://vt.colortex.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://uw.jctech888.com.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rb.huanxung.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://un.shtwfgs.cn

TS:   s.split(",")
来源：http://lq.yuexingan06.cn

Java: s.split(",");  s.split("\\s+")
来源：http://el.bookmarksfly.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jq.yuntaijiaju.cn

Ruby: s.split(",");  s.split
来源：http://ql.hahajie.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://da.newstarts.cn

[E08] 数组按分隔符合并
来源：http://iq.newstarts.cn

Py:   ",".join(items)
来源：http://nh.newstarts.cn

PHP:  implode(",", $items);
来源：http://wz.9csxet.cn

JS:   items.join(",")
来源：http://kz.gzmigu.cn

TS:   items.join(",")
来源：http://rc.haigaiapp.cn

Java: String.join(",", items)
来源：http://qt.haigaiapp.cn

Go:   strings.Join(items, ",")
来源：http://fw.nszjky.cn

Ruby: items.join(",")
来源：http://pl.shxzskj.cn

C#:   string.Join(",", items)
来源：http://na.szxytkj.cn

[E09] 去除所有空白字符
来源：http://uw.huixinmuqiang.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vy.gzmigu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lf.huixiangedu.cn

JS:   s.replace(/\s+/g, "")
来源：http://dn.hnjuh.cn

TS:   s.replace(/\s+/g, "")
来源：http://mj.lnxyls.cn

Java: s.replaceAll("\\s+", "")
来源：http://ps.yuntaijiaju.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://tr.shtwfgs.cn

Ruby: s.gsub(/\s+/, "")
来源：http://bc.jctech888.com.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rf.szsharing.cn

[E10] 左侧补零 / 定长填充
来源：http://ps.muxihuayi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pw.nicolike.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zi.gzmigu.cn

JS:   "7".padStart(3, "0")
来源：http://em.bjjhwx.cn

TS:   "7".padStart(3, "0")
来源：http://gw.lnxyls.cn

Java: String.format("%03d", 7)
来源：http://hb.bookmarksfly.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://zn.szxytkj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vq.gzmigu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ab.muxihuayi.cn

[E11] 反转字符串
来源：http://dp.wgjwhj.cn

Py:   s[::-1]
来源：http://se.huixiangedu.cn

PHP:  strrev($s);
来源：http://ya.chemitech.net.cn

JS:   [...s].reverse().join("")
来源：http://uw.yuntaijiaju.cn

TS:   [...s].reverse().join("")
来源：http://js.haigaiapp.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wz.hahajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://gk.huanxung.cn

Ruby: s.reverse
来源：http://eu.huixinmuqiang.cn

C#:   new string(s.Reverse().ToArray())
来源：http://rv.yuntaijiaju.cn

[E12] 统计某字符出现次数
来源：http://zx.chemitech.net.cn

Py:   s.count("a")
来源：http://kw.hnjuh.cn

PHP:  substr_count($s, "a");
来源：http://rz.nicolike.cn

JS:   s.split("a").length - 1
来源：http://gp.newstarts.cn

TS:   s.split("a").length - 1
来源：http://ff.hahajie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://du.panjiajie.cn

Go:   strings.Count(s, "a")
来源：http://et.nszjky.cn

Ruby: s.count("a")
来源：http://fh.nszjky.cn

C#:   s.Count(c => c == 'a')
来源：http://cb.9csxet.cn

[E13] 逐字符遍历
来源：http://jk.lnxyls.cn


<!-- 参考信息 -->