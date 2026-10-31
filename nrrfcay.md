代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://rk.lnxyls.cn

C#:   a.Concat(b).ToList()
来源：http://oe.shxzukj.cn

[D09] 排序（升序）
来源：http://ew.panjiajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://hk.nszjky.cn

PHP:  sort($arr);
来源：http://vy.huanxung.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tj.gzmigu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ia.jianghongdianzi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ld.huixiangedu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gl.shtwfgs.cn

Ruby: arr.sort
来源：http://qr.szxytkj.cn

C#:   list.Sort();
来源：http://oc.bookmarksfly.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://xf.hahajie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mt.szsharing.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rk.bookmarksfly.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lf.hnjuh.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zg.asd995.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ig.shxzskj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gx.bjjhwx.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://in.wgjwhj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rk.huixinmuqiang.cn

[D11] 反转数组
来源：http://xx.521024.cn

Py:   arr[::-1];  arr.reverse()
来源：http://eq.shxzukj.cn

PHP:  array_reverse($arr);
来源：http://nr.521024.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://iv.shxzukj.cn

TS:   [...arr].reverse();
来源：http://jh.bookmarksfly.cn

Java: Collections.reverse(list);
来源：http://vb.asd995.cn

Go:   slices.Reverse(arr)
来源：http://yv.colortex.cn

Ruby: arr.reverse
来源：http://wj.hnjuh.cn

C#:   list.Reverse();
来源：http://th.colortex.cn

[D12] 查找元素下标
来源：http://em.muxihuayi.cn

Py:   arr.index(x);  x in arr
来源：http://yu.9csxet.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uj.jianghongdianzi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ot.asd995.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://io.yuexingan06.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wd.521024.cn

Go:   slices.Index(arr, x)
来源：http://zv.jianghongdianzi.cn

Ruby: arr.index(x)
来源：http://it.shtwfgs.cn

C#:   list.IndexOf(x);
来源：http://db.colortex.cn

[D13] 过滤（保留满足条件的）
来源：http://sk.nszjky.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://is.nicolike.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qz.bookmarksfly.cn

JS:   arr.filter(x => x > 3)
来源：http://ck.gzmigu.cn

TS:   arr.filter(x => x > 3)
来源：http://oz.huanxung.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://az.jianghongdianzi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wn.bookmarksfly.cn

Ruby: arr.select { |x| x > 3 }
来源：http://va.shtwfgs.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://rk.szsharing.cn

[D14] 映射转换（每个元素变形）
来源：http://zr.huanxung.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ac.gzmigu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://oc.haigaiapp.cn

JS:   arr.map(x => x * 2)
来源：http://xr.bjjhwx.cn

TS:   arr.map(x => x * 2)
来源：http://gk.huixiangedu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://wf.yuexingan06.cn

Go:   // 手写循环
来源：http://zf.yuntaijiaju.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hh.yuntaijiaju.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://td.shtwfgs.cn

[D15] 去重
来源：http://de.muxihuayi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://he.bjjhwx.cn

PHP:  array_unique($arr);
来源：http://wk.muxihuayi.cn

JS:   [...new Set(arr)]
来源：http://hg.lnxyls.cn

TS:   [...new Set(arr)]
来源：http://qz.yuntaijiaju.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ev.szxytkj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zi.jianghongdianzi.cn

Ruby: arr.uniq
来源：http://ec.9csxet.cn

C#:   list.Distinct().ToList()
来源：http://pc.gzmigu.cn

[D16] 求和与平均值
来源：http://oy.huixinmuqiang.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rb.muxihuayi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cq.jianghongdianzi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://le.yuexingan06.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rt.colortex.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bz.bookmarksfly.cn

Go:   // 手写循环累加
来源：http://wv.yuexingan06.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ri.shxzukj.cn

C#:   list.Sum();  list.Average()
来源：http://ya.jianghongdianzi.cn

[D17] 最大值与最小值
来源：http://nk.gzmigu.cn

Py:   max(arr);  min(arr)
来源：http://ve.huanxung.cn

PHP:  max($arr);  min($arr);
来源：http://qk.gzmigu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zf.lnxyls.cn

TS:   Math.max(...arr);
来源：http://mf.jianghongdianzi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ix.huixiangedu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xq.jianghongdianzi.cn

Ruby: arr.max;  arr.min
来源：http://kj.muxihuayi.cn

C#:   list.Max();  list.Min()
来源：http://sd.nicolike.cn

[D18] 扁平化嵌套数组
来源：http://uk.nicolike.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bh.gzmigu.cn

PHP:  array_merge(...$nested);
来源：http://fe.jianghongdianzi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hm.jianghongdianzi.cn

TS:   nested.flat();
来源：http://lt.521024.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ue.yuexingan06.cn

Go:   // 手写双层循环
来源：http://mo.nicolike.cn

Ruby: nested.flatten
来源：http://vl.shtwfgs.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://vl.chemitech.net.cn

[D19] 按字段分组
来源：http://av.lnxyls.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vc.shtwfgs.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dy.bjjhwx.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://eh.huixiangedu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ak.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qr.521024.cn

Go:   // 手写 map[string][]T
来源：http://an.jianghongdianzi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fc.newstarts.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tz.szxytkj.cn

[D20] 统计每个元素出现次数
来源：http://qr.muxihuayi.cn

Py:   Counter(arr)
来源：http://as.newstarts.cn

PHP:  array_count_values($arr);
来源：http://kk.szsharing.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nk.521024.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cn.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xa.asd995.cn

Go:   // 手写 map[T]int
来源：http://mw.gzmigu.cn

Ruby: arr.tally
来源：http://zp.huixiangedu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lk.panjiajie.cn

[D21] 判断是否包含某元素
来源：http://da.huixinmuqiang.cn

Py:   x in arr
来源：http://sm.lnxyls.cn

PHP:  in_array($x, $arr, true);
来源：http://eh.bookmarksfly.cn

JS:   arr.includes(x)
来源：http://kh.huixiangedu.cn

TS:   arr.includes(x)
来源：http://co.haigaiapp.cn

Java: list.contains(x)
来源：http://dz.muxihuayi.cn

Go:   slices.Contains(arr, x)
来源：http://fx.jctech888.com.cn

Ruby: arr.include?(x)
来源：http://af.newstarts.cn

C#:   list.Contains(x)
来源：http://jr.jctech888.com.cn

[D22] 复制数组（避免共享引用）
来源：http://ma.lnxyls.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yu.hahajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wz.bjjhwx.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cj.jianghongdianzi.cn

TS:   [...arr];
来源：http://lp.haigaiapp.cn

Java: new ArrayList<>(list);
来源：http://ov.huanxung.cn

Go:   copied := append([]int(nil), arr...)
来源：http://dm.nicolike.cn

Ruby: arr.dup;  arr.clone
来源：http://xs.panjiajie.cn

C#:   new List<int>(list);
来源：http://nc.jctech888.com.cn

[D23] reduce 累积计算
来源：http://cy.yuexingan06.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wn.muxihuayi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xq.colortex.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gi.huanxung.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fk.521024.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://pb.muxihuayi.cn

Go:   // 手写循环
来源：http://or.jctech888.com.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tk.colortex.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kf.haigaiapp.cn

[D24] 字典 / Map 基本操作
来源：http://vw.chemitech.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ww.bjjhwx.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ve.gzmigu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://yl.yuexingan06.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nh.nszjky.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gg.yuexingan06.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ln.huixinmuqiang.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mb.hnjuh.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dg.gzmigu.cn

[D25] Set 集合去重与交并差
来源：http://lp.huixiangedu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://la.haigaiapp.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wf.shxzskj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hl.huanxung.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://km.asd995.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ip.haigaiapp.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ef.shxzukj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qr.huanxung.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jt.bjjhwx.cn

[D26] 数组转字符串
来源：http://ip.yuntaijiaju.cn

Py:   ", ".join(map(str, arr))
来源：http://im.nicolike.cn

PHP:  implode(", ", $arr);
来源：http://rp.huixinmuqiang.cn

JS:   arr.join(", ")
来源：http://nz.jctech888.com.cn

TS:   arr.join(", ")
来源：http://ut.huixinmuqiang.cn

Java: String.join(", ", list)
来源：http://mf.521024.cn

Go:   strings.Join(strs, ", ")
来源：http://pr.yuntaijiaju.cn

Ruby: arr.join(", ")
来源：http://xj.szxytkj.cn

C#:   string.Join(", ", list)
来源：http://ga.huixinmuqiang.cn

================================================================================
来源：http://ia.jctech888.com.cn

E. 字符串处理
来源：http://bc.huanxung.cn

================================================================================
来源：http://fc.muxihuayi.cn

[E01] 拼接字符串
来源：http://vg.shxzukj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://te.huixinmuqiang.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nr.521024.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ok.gzmigu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://be.bookmarksfly.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mb.jctech888.com.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mt.huixiangedu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rn.jctech888.com.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fl.chemitech.net.cn

[E02] 重复字符串
来源：http://hl.chemitech.net.cn

Py:   "ab" * 3
来源：http://jx.chemitech.net.cn

PHP:  str_repeat("ab", 3);
来源：http://pq.jianghongdianzi.cn

JS:   "ab".repeat(3)
来源：http://lo.asd995.cn

TS:   "ab".repeat(3)
来源：http://zx.jctech888.com.cn

Java: "ab".repeat(3)
来源：http://yo.huanxung.cn

Go:   strings.Repeat("ab", 3)
来源：http://ym.newstarts.cn

Ruby: "ab" * 3
来源：http://pk.panjiajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hh.nszjky.cn

[E03] 截取子串
来源：http://iw.nszjky.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vr.chemitech.net.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://sq.szsharing.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bv.panjiajie.cn

TS:   s.slice(1, 4)
来源：http://ex.panjiajie.cn

Java: s.substring(1, 4)
来源：http://eg.jianghongdianzi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ul.shtwfgs.cn

Ruby: s[1, 3];  s[1..3]
来源：http://by.hahajie.cn

C#:   s.Substring(1, 3)
来源：http://ht.muxihuayi.cn

[E04] 查找子串位置
来源：http://et.hnjuh.cn

Py:   s.find("x");  s.index("x")
来源：http://rr.jianghongdianzi.cn

PHP:  strpos($s, "x");
来源：http://oe.muxihuayi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cb.nicolike.cn

TS:   s.indexOf("x")
来源：http://la.bjjhwx.cn

Java: s.indexOf("x")
来源：http://ff.shxzskj.cn

Go:   strings.Index(s, "x")
来源：http://xx.huixiangedu.cn

Ruby: s.index("x")
来源：http://cu.asd995.cn

C#:   s.IndexOf("x")
来源：http://pp.nszjky.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://br.panjiajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ez.nicolike.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ej.jctech888.com.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ne.shxzskj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xj.panjiajie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ki.gzmigu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pv.521024.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zf.9csxet.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bd.hnjuh.cn

[E06] 替换子串
来源：http://ag.jianghongdianzi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ih.panjiajie.cn

PHP:  str_replace("a", "b", $s);
来源：http://xi.szsharing.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gc.panjiajie.cn

TS:   s.replaceAll("a", "b")
来源：http://xx.muxihuayi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bo.bjjhwx.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://uu.nszjky.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://le.hahajie.cn

C#:   s.Replace("a", "b")
来源：http://bt.bookmarksfly.cn

[E07] 按分隔符拆分
来源：http://ni.lnxyls.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jk.wgjwhj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ki.nicolike.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://gp.hahajie.cn

TS:   s.split(",")
来源：http://tc.haigaiapp.cn

Java: s.split(",");  s.split("\\s+")
来源：http://he.asd995.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jq.bookmarksfly.cn

Ruby: s.split(",");  s.split
来源：http://rr.shxzskj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ap.shtwfgs.cn

[E08] 数组按分隔符合并
来源：http://zu.nicolike.cn

Py:   ",".join(items)
来源：http://ih.yuexingan06.cn

PHP:  implode(",", $items);
来源：http://iu.jctech888.com.cn

JS:   items.join(",")
来源：http://ka.panjiajie.cn

TS:   items.join(",")
来源：http://ve.hnjuh.cn

Java: String.join(",", items)
来源：http://lj.yuexingan06.cn

Go:   strings.Join(items, ",")
来源：http://at.bjjhwx.cn

Ruby: items.join(",")
来源：http://ac.gzmigu.cn

C#:   string.Join(",", items)
来源：http://tl.huanxung.cn

[E09] 去除所有空白字符
来源：http://cp.szxytkj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rc.chemitech.net.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jt.hnjuh.cn

JS:   s.replace(/\s+/g, "")
来源：http://nf.huixiangedu.cn

TS:   s.replace(/\s+/g, "")
来源：http://nf.shxzukj.cn

Java: s.replaceAll("\\s+", "")
来源：http://vx.9csxet.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://fe.nszjky.cn

Ruby: s.gsub(/\s+/, "")
来源：http://cj.newstarts.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cu.shxzskj.cn

[E10] 左侧补零 / 定长填充
来源：http://xs.hahajie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gp.jianghongdianzi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jx.nicolike.cn

JS:   "7".padStart(3, "0")
来源：http://pw.jianghongdianzi.cn

TS:   "7".padStart(3, "0")
来源：http://nb.haigaiapp.cn

Java: String.format("%03d", 7)
来源：http://gv.shxzukj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://gu.muxihuayi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qu.shtwfgs.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jy.nicolike.cn

[E11] 反转字符串
来源：http://dq.shxzukj.cn

Py:   s[::-1]
来源：http://vk.yuntaijiaju.cn

PHP:  strrev($s);
来源：http://xq.nszjky.cn

JS:   [...s].reverse().join("")
来源：http://ho.yuexingan06.cn

TS:   [...s].reverse().join("")
来源：http://nm.lnxyls.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ms.muxihuayi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://so.newstarts.cn

Ruby: s.reverse
来源：http://hf.hahajie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://eb.haigaiapp.cn

[E12] 统计某字符出现次数
来源：http://zo.bjjhwx.cn

Py:   s.count("a")
来源：http://ee.9csxet.cn

PHP:  substr_count($s, "a");
来源：http://be.colortex.cn

JS:   s.split("a").length - 1
来源：http://ro.nszjky.cn

TS:   s.split("a").length - 1
来源：http://qt.huanxung.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mm.shxzskj.cn

Go:   strings.Count(s, "a")
来源：http://pn.panjiajie.cn

Ruby: s.count("a")
来源：http://in.yuexingan06.cn

C#:   s.Count(c => c == 'a')
来源：http://ow.9csxet.cn

[E13] 逐字符遍历
来源：http://td.huixinmuqiang.cn

Py:   for ch in s: print(ch)
来源：http://uj.shtwfgs.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mj.shtwfgs.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://fs.colortex.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://lh.haigaiapp.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qc.lnxyls.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ao.huixiangedu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ym.huixinmuqiang.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gq.bjjhwx.cn

[E14] URL 编码与 Base64
来源：http://jq.nszjky.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://co.bookmarksfly.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://gt.huixinmuqiang.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lh.yuexingan06.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://so.yuexingan06.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pb.hahajie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kf.colortex.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kn.muxihuayi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ta.hahajie.cn

[E15] HTML 转义 / 反转义
来源：http://zq.bookmarksfly.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ep.muxihuayi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sg.521024.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nf.szxytkj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://sj.huixiangedu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jo.haigaiapp.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mm.bjjhwx.cn


<!-- 参考信息 -->