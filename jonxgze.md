代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://ng.yuntaijiaju.cn

C#:   a.Concat(b).ToList()
来源：http://vm.lnxyls.cn

[D09] 排序（升序）
来源：http://lu.gzmigu.cn

Py:   sorted(arr);  arr.sort()
来源：http://ff.huanxung.cn

PHP:  sort($arr);
来源：http://dz.hahajie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wa.hnjuh.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fh.szxytkj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://rx.shxzskj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rv.jianghongdianzi.cn

Ruby: arr.sort
来源：http://uh.muxihuayi.cn

C#:   list.Sort();
来源：http://mn.yuntaijiaju.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://pv.shxzskj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lf.panjiajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wg.521024.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sf.huixinmuqiang.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://px.jianghongdianzi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ii.gzmigu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zi.9csxet.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fj.lnxyls.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vf.panjiajie.cn

[D11] 反转数组
来源：http://rj.haigaiapp.cn

Py:   arr[::-1];  arr.reverse()
来源：http://aw.gzmigu.cn

PHP:  array_reverse($arr);
来源：http://df.asd995.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ir.wgjwhj.cn

TS:   [...arr].reverse();
来源：http://lp.yuexingan06.cn

Java: Collections.reverse(list);
来源：http://pi.521024.cn

Go:   slices.Reverse(arr)
来源：http://dg.bjjhwx.cn

Ruby: arr.reverse
来源：http://oj.haigaiapp.cn

C#:   list.Reverse();
来源：http://ee.haigaiapp.cn

[D12] 查找元素下标
来源：http://ev.wgjwhj.cn

Py:   arr.index(x);  x in arr
来源：http://ib.yuexingan06.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pq.asd995.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eu.asd995.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nq.panjiajie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dv.hahajie.cn

Go:   slices.Index(arr, x)
来源：http://eq.panjiajie.cn

Ruby: arr.index(x)
来源：http://hu.hnjuh.cn

C#:   list.IndexOf(x);
来源：http://iy.hahajie.cn

[D13] 过滤（保留满足条件的）
来源：http://oj.huixinmuqiang.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ej.jctech888.com.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ue.jianghongdianzi.cn

JS:   arr.filter(x => x > 3)
来源：http://jl.bjjhwx.cn

TS:   arr.filter(x => x > 3)
来源：http://rn.yuexingan06.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hd.szsharing.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dj.jctech888.com.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wo.huixiangedu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://fu.panjiajie.cn

[D14] 映射转换（每个元素变形）
来源：http://as.bjjhwx.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sr.jctech888.com.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ae.huixinmuqiang.cn

JS:   arr.map(x => x * 2)
来源：http://zl.muxihuayi.cn

TS:   arr.map(x => x * 2)
来源：http://cc.nszjky.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://fv.panjiajie.cn

Go:   // 手写循环
来源：http://hv.newstarts.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ed.yuntaijiaju.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://jc.haigaiapp.cn

[D15] 去重
来源：http://wc.521024.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bn.shtwfgs.cn

PHP:  array_unique($arr);
来源：http://yd.chemitech.net.cn

JS:   [...new Set(arr)]
来源：http://ei.szsharing.cn

TS:   [...new Set(arr)]
来源：http://ut.newstarts.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ro.9csxet.cn

Go:   // 用 map[T]struct{} 手写
来源：http://in.jctech888.com.cn

Ruby: arr.uniq
来源：http://fo.chemitech.net.cn

C#:   list.Distinct().ToList()
来源：http://cl.jctech888.com.cn

[D16] 求和与平均值
来源：http://bj.nszjky.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ge.shxzskj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://lc.huixiangedu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pl.hahajie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://du.yuntaijiaju.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pk.hahajie.cn

Go:   // 手写循环累加
来源：http://iw.gzmigu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://sd.9csxet.cn

C#:   list.Sum();  list.Average()
来源：http://uo.asd995.cn

[D17] 最大值与最小值
来源：http://ij.huixinmuqiang.cn

Py:   max(arr);  min(arr)
来源：http://zd.shxzukj.cn

PHP:  max($arr);  min($arr);
来源：http://ze.huixiangedu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.521024.cn

TS:   Math.max(...arr);
来源：http://zz.szxytkj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://zt.asd995.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wn.shtwfgs.cn

Ruby: arr.max;  arr.min
来源：http://ck.9csxet.cn

C#:   list.Max();  list.Min()
来源：http://pp.lnxyls.cn

[D18] 扁平化嵌套数组
来源：http://hu.nicolike.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rs.panjiajie.cn

PHP:  array_merge(...$nested);
来源：http://vt.szsharing.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qy.nszjky.cn

TS:   nested.flat();
来源：http://im.szxytkj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://he.hahajie.cn

Go:   // 手写双层循环
来源：http://sp.yuexingan06.cn

Ruby: nested.flatten
来源：http://ou.huanxung.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zs.huixinmuqiang.cn

[D19] 按字段分组
来源：http://nt.huanxung.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://js.shxzskj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jk.shxzukj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fi.haigaiapp.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://dy.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://me.szxytkj.cn

Go:   // 手写 map[string][]T
来源：http://vo.hahajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://xq.gzmigu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ll.szxytkj.cn

[D20] 统计每个元素出现次数
来源：http://ci.haigaiapp.cn

Py:   Counter(arr)
来源：http://wl.gzmigu.cn

PHP:  array_count_values($arr);
来源：http://gg.haigaiapp.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rd.yuntaijiaju.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wn.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vc.9csxet.cn

Go:   // 手写 map[T]int
来源：http://mb.hnjuh.cn

Ruby: arr.tally
来源：http://rg.wgjwhj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ng.asd995.cn

[D21] 判断是否包含某元素
来源：http://up.hahajie.cn

Py:   x in arr
来源：http://ss.hahajie.cn

PHP:  in_array($x, $arr, true);
来源：http://go.9csxet.cn

JS:   arr.includes(x)
来源：http://ea.gzmigu.cn

TS:   arr.includes(x)
来源：http://zp.huixiangedu.cn

Java: list.contains(x)
来源：http://qq.szxytkj.cn

Go:   slices.Contains(arr, x)
来源：http://xz.hahajie.cn

Ruby: arr.include?(x)
来源：http://mf.nicolike.cn

C#:   list.Contains(x)
来源：http://dn.haigaiapp.cn

[D22] 复制数组（避免共享引用）
来源：http://yf.muxihuayi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://sm.bookmarksfly.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jy.bjjhwx.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ou.nicolike.cn

TS:   [...arr];
来源：http://wd.521024.cn

Java: new ArrayList<>(list);
来源：http://ym.huanxung.cn

Go:   copied := append([]int(nil), arr...)
来源：http://rr.jctech888.com.cn

Ruby: arr.dup;  arr.clone
来源：http://li.hnjuh.cn

C#:   new List<int>(list);
来源：http://az.521024.cn

[D23] reduce 累积计算
来源：http://cd.newstarts.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qh.colortex.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hw.haigaiapp.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gj.lnxyls.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uj.wgjwhj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://hb.huixinmuqiang.cn

Go:   // 手写循环
来源：http://wh.shtwfgs.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bk.huixiangedu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://br.9csxet.cn

[D24] 字典 / Map 基本操作
来源：http://il.521024.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pw.huanxung.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://td.521024.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://je.muxihuayi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://uy.9csxet.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ts.jianghongdianzi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vh.szxytkj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ip.haigaiapp.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hs.hahajie.cn

[D25] Set 集合去重与交并差
来源：http://tt.bjjhwx.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zz.jctech888.com.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zh.szxytkj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mt.colortex.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://px.bjjhwx.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vd.haigaiapp.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://og.colortex.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ry.bookmarksfly.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jz.szsharing.cn

[D26] 数组转字符串
来源：http://dx.muxihuayi.cn

Py:   ", ".join(map(str, arr))
来源：http://tf.jctech888.com.cn

PHP:  implode(", ", $arr);
来源：http://df.shtwfgs.cn

JS:   arr.join(", ")
来源：http://db.bjjhwx.cn

TS:   arr.join(", ")
来源：http://ej.panjiajie.cn

Java: String.join(", ", list)
来源：http://co.huanxung.cn

Go:   strings.Join(strs, ", ")
来源：http://xu.hnjuh.cn

Ruby: arr.join(", ")
来源：http://ok.nszjky.cn

C#:   string.Join(", ", list)
来源：http://cj.szsharing.cn

================================================================================
来源：http://dr.jctech888.com.cn

E. 字符串处理
来源：http://kf.bookmarksfly.cn

================================================================================
来源：http://pw.wgjwhj.cn

[E01] 拼接字符串
来源：http://zi.chemitech.net.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rw.szxytkj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://iy.jianghongdianzi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vv.huixinmuqiang.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sn.asd995.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nj.panjiajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jx.muxihuayi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gn.yuexingan06.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wx.jianghongdianzi.cn

[E02] 重复字符串
来源：http://jw.panjiajie.cn

Py:   "ab" * 3
来源：http://ax.huanxung.cn

PHP:  str_repeat("ab", 3);
来源：http://pp.newstarts.cn

JS:   "ab".repeat(3)
来源：http://th.huixiangedu.cn

TS:   "ab".repeat(3)
来源：http://fq.szxytkj.cn

Java: "ab".repeat(3)
来源：http://gh.szsharing.cn

Go:   strings.Repeat("ab", 3)
来源：http://tm.jctech888.com.cn

Ruby: "ab" * 3
来源：http://og.shxzskj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ph.hahajie.cn

[E03] 截取子串
来源：http://vs.bookmarksfly.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xg.yuexingan06.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bq.bjjhwx.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cu.hnjuh.cn

TS:   s.slice(1, 4)
来源：http://fd.nicolike.cn

Java: s.substring(1, 4)
来源：http://wp.lnxyls.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://oc.newstarts.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ia.newstarts.cn

C#:   s.Substring(1, 3)
来源：http://qe.colortex.cn

[E04] 查找子串位置
来源：http://fh.shxzukj.cn

Py:   s.find("x");  s.index("x")
来源：http://xv.szsharing.cn

PHP:  strpos($s, "x");
来源：http://mi.chemitech.net.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ik.bjjhwx.cn

TS:   s.indexOf("x")
来源：http://cq.shxzukj.cn

Java: s.indexOf("x")
来源：http://bu.muxihuayi.cn

Go:   strings.Index(s, "x")
来源：http://wk.huixiangedu.cn

Ruby: s.index("x")
来源：http://vs.wgjwhj.cn

C#:   s.IndexOf("x")
来源：http://kz.wgjwhj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://vr.asd995.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://do.huanxung.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tq.hahajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wi.wgjwhj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hr.hahajie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pz.panjiajie.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pd.jctech888.com.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vg.9csxet.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://uz.szxytkj.cn

[E06] 替换子串
来源：http://lf.521024.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ip.521024.cn

PHP:  str_replace("a", "b", $s);
来源：http://jd.panjiajie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xk.yuntaijiaju.cn

TS:   s.replaceAll("a", "b")
来源：http://tr.chemitech.net.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ct.huanxung.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xn.shxzukj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qx.huixiangedu.cn

C#:   s.Replace("a", "b")
来源：http://jc.yuntaijiaju.cn

[E07] 按分隔符拆分
来源：http://uf.chemitech.net.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://on.huanxung.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nh.lnxyls.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://tr.newstarts.cn

TS:   s.split(",")
来源：http://zg.chemitech.net.cn

Java: s.split(",");  s.split("\\s+")
来源：http://pa.colortex.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hj.bookmarksfly.cn

Ruby: s.split(",");  s.split
来源：http://ft.yuexingan06.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bo.shtwfgs.cn

[E08] 数组按分隔符合并
来源：http://yi.hahajie.cn

Py:   ",".join(items)
来源：http://ll.huixinmuqiang.cn

PHP:  implode(",", $items);
来源：http://dj.panjiajie.cn

JS:   items.join(",")
来源：http://hn.huixinmuqiang.cn

TS:   items.join(",")
来源：http://lp.bookmarksfly.cn

Java: String.join(",", items)
来源：http://za.newstarts.cn

Go:   strings.Join(items, ",")
来源：http://ze.yuntaijiaju.cn

Ruby: items.join(",")
来源：http://qt.shxzskj.cn

C#:   string.Join(",", items)
来源：http://fi.yuexingan06.cn

[E09] 去除所有空白字符
来源：http://yr.bookmarksfly.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ln.newstarts.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zt.nicolike.cn

JS:   s.replace(/\s+/g, "")
来源：http://uj.nszjky.cn

TS:   s.replace(/\s+/g, "")
来源：http://nv.szxytkj.cn

Java: s.replaceAll("\\s+", "")
来源：http://cs.nszjky.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://fa.gzmigu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://vz.shxzukj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://il.haigaiapp.cn

[E10] 左侧补零 / 定长填充
来源：http://zx.haigaiapp.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wc.wgjwhj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hc.colortex.cn

JS:   "7".padStart(3, "0")
来源：http://ck.huanxung.cn

TS:   "7".padStart(3, "0")
来源：http://wd.colortex.cn

Java: String.format("%03d", 7)
来源：http://jd.szxytkj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://fp.asd995.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ty.haigaiapp.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ml.shxzukj.cn

[E11] 反转字符串
来源：http://pm.lnxyls.cn

Py:   s[::-1]
来源：http://qn.wgjwhj.cn

PHP:  strrev($s);
来源：http://nh.lnxyls.cn

JS:   [...s].reverse().join("")
来源：http://mm.yuntaijiaju.cn

TS:   [...s].reverse().join("")
来源：http://lm.jctech888.com.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://tt.bjjhwx.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://dt.wgjwhj.cn

Ruby: s.reverse
来源：http://tt.9csxet.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ow.shxzukj.cn

[E12] 统计某字符出现次数
来源：http://gg.huixinmuqiang.cn

Py:   s.count("a")
来源：http://sh.521024.cn

PHP:  substr_count($s, "a");
来源：http://nc.shxzskj.cn

JS:   s.split("a").length - 1
来源：http://pd.newstarts.cn

TS:   s.split("a").length - 1
来源：http://eq.newstarts.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nv.nicolike.cn

Go:   strings.Count(s, "a")
来源：http://nh.muxihuayi.cn

Ruby: s.count("a")
来源：http://id.hahajie.cn

C#:   s.Count(c => c == 'a')
来源：http://xs.newstarts.cn

[E13] 逐字符遍历
来源：http://lz.jianghongdianzi.cn

Py:   for ch in s: print(ch)
来源：http://hz.muxihuayi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fo.jianghongdianzi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xl.huixiangedu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://xw.shtwfgs.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gb.hnjuh.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ma.yuntaijiaju.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vp.szsharing.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cm.chemitech.net.cn

[E14] URL 编码与 Base64
来源：http://yj.jctech888.com.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bp.jianghongdianzi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://nr.shtwfgs.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xh.nicolike.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yq.hnjuh.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jm.jianghongdianzi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ai.newstarts.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ib.colortex.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ya.szxytkj.cn

[E15] HTML 转义 / 反转义
来源：http://er.shxzukj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://kw.jianghongdianzi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ne.jctech888.com.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qj.wgjwhj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://re.haigaiapp.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mb.huanxung.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ax.lnxyls.cn


<!-- 参考信息 -->