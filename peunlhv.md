代发 wailian999

Java: list.size();
来源：http://vw.haigaiapp.cn

Go:   len(arr)
来源：http://xr.huixiangedu.cn

Ruby: arr.length; arr.size
来源：http://jb.gzmigu.cn

C#:   list.Count;
来源：http://bz.bjjhwx.cn

[D07] 切片 / 取子数组
来源：http://gv.haigaiapp.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ex.muxihuayi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ol.wgjwhj.cn

JS:   arr.slice(1, 4);
来源：http://zs.shxzskj.cn

TS:   arr.slice(1, 4);
来源：http://ri.yuntaijiaju.cn

Java: list.subList(1, 4);
来源：http://em.gzmigu.cn

Go:   arr[1:4]
来源：http://jo.shxzskj.cn

Ruby: arr[1, 3]
来源：http://hw.hahajie.cn

C#:   list.GetRange(1, 3);
来源：http://ny.haigaiapp.cn

[D08] 合并两个数组
来源：http://xz.9csxet.cn

Py:   a + b;  a.extend(b)
来源：http://bd.jctech888.com.cn

PHP:  array_merge($a, $b);
来源：http://oz.asd995.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://oe.nicolike.cn

TS:   [...a, ...b];
来源：http://ea.szsharing.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rs.szxytkj.cn

Go:   append(a, b...)
来源：http://tv.haigaiapp.cn

Ruby: a + b;  a.concat(b)
来源：http://ql.chemitech.net.cn

C#:   a.Concat(b).ToList()
来源：http://sh.chemitech.net.cn

[D09] 排序（升序）
来源：http://uu.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://nz.szsharing.cn

PHP:  sort($arr);
来源：http://kr.wgjwhj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xi.huixiangedu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://dr.9csxet.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vj.huixiangedu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ab.nicolike.cn

Ruby: arr.sort
来源：http://lh.hnjuh.cn

C#:   list.Sort();
来源：http://sq.newstarts.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://py.newstarts.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xc.shxzskj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wm.hnjuh.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gk.lnxyls.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gd.jctech888.com.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zc.shxzskj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gx.hahajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mb.hnjuh.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bg.wgjwhj.cn

[D11] 反转数组
来源：http://bo.521024.cn

Py:   arr[::-1];  arr.reverse()
来源：http://hi.9csxet.cn

PHP:  array_reverse($arr);
来源：http://ls.shxzskj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jl.huanxung.cn

TS:   [...arr].reverse();
来源：http://bl.colortex.cn

Java: Collections.reverse(list);
来源：http://py.gzmigu.cn

Go:   slices.Reverse(arr)
来源：http://re.yuexingan06.cn

Ruby: arr.reverse
来源：http://rg.asd995.cn

C#:   list.Reverse();
来源：http://cs.wgjwhj.cn

[D12] 查找元素下标
来源：http://jt.lnxyls.cn

Py:   arr.index(x);  x in arr
来源：http://iq.colortex.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yl.newstarts.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sv.huanxung.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cs.szsharing.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sz.huanxung.cn

Go:   slices.Index(arr, x)
来源：http://gj.szxytkj.cn

Ruby: arr.index(x)
来源：http://nr.bjjhwx.cn

C#:   list.IndexOf(x);
来源：http://fo.yuexingan06.cn

[D13] 过滤（保留满足条件的）
来源：http://xg.hnjuh.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ei.szsharing.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://el.szxytkj.cn

JS:   arr.filter(x => x > 3)
来源：http://oh.521024.cn

TS:   arr.filter(x => x > 3)
来源：http://hq.szxytkj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nl.hahajie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://iz.muxihuayi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hb.shxzskj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ge.szxytkj.cn

[D14] 映射转换（每个元素变形）
来源：http://im.colortex.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://at.wgjwhj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zs.shxzukj.cn

JS:   arr.map(x => x * 2)
来源：http://kx.hnjuh.cn

TS:   arr.map(x => x * 2)
来源：http://mc.huixiangedu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ik.asd995.cn

Go:   // 手写循环
来源：http://xl.shxzukj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ne.jianghongdianzi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://dd.hahajie.cn

[D15] 去重
来源：http://sg.bookmarksfly.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://md.hnjuh.cn

PHP:  array_unique($arr);
来源：http://em.9csxet.cn

JS:   [...new Set(arr)]
来源：http://np.shtwfgs.cn

TS:   [...new Set(arr)]
来源：http://tn.jianghongdianzi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ou.gzmigu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://tv.9csxet.cn

Ruby: arr.uniq
来源：http://lg.nicolike.cn

C#:   list.Distinct().ToList()
来源：http://dh.yuntaijiaju.cn

[D16] 求和与平均值
来源：http://pp.hahajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ha.chemitech.net.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ur.asd995.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ng.9csxet.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wy.chemitech.net.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://id.hnjuh.cn

Go:   // 手写循环累加
来源：http://fj.asd995.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ic.shtwfgs.cn

C#:   list.Sum();  list.Average()
来源：http://uj.asd995.cn

[D17] 最大值与最小值
来源：http://hz.huixiangedu.cn

Py:   max(arr);  min(arr)
来源：http://ff.wgjwhj.cn

PHP:  max($arr);  min($arr);
来源：http://lf.haigaiapp.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zr.shtwfgs.cn

TS:   Math.max(...arr);
来源：http://qh.yuntaijiaju.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://yi.jianghongdianzi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ya.bjjhwx.cn

Ruby: arr.max;  arr.min
来源：http://im.asd995.cn

C#:   list.Max();  list.Min()
来源：http://og.jianghongdianzi.cn

[D18] 扁平化嵌套数组
来源：http://yq.newstarts.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mw.jctech888.com.cn

PHP:  array_merge(...$nested);
来源：http://ni.bookmarksfly.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zp.szxytkj.cn

TS:   nested.flat();
来源：http://nt.muxihuayi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cc.wgjwhj.cn

Go:   // 手写双层循环
来源：http://jv.panjiajie.cn

Ruby: nested.flatten
来源：http://dt.shxzukj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://gl.nszjky.cn

[D19] 按字段分组
来源：http://nz.yuexingan06.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ua.gzmigu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tt.bookmarksfly.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kk.gzmigu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://os.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xk.yuntaijiaju.cn

Go:   // 手写 map[string][]T
来源：http://os.nszjky.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://lt.asd995.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://sf.colortex.cn

[D20] 统计每个元素出现次数
来源：http://mu.shxzskj.cn

Py:   Counter(arr)
来源：http://wq.jctech888.com.cn

PHP:  array_count_values($arr);
来源：http://cx.huanxung.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qw.colortex.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oy.lnxyls.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vn.nicolike.cn

Go:   // 手写 map[T]int
来源：http://be.jctech888.com.cn

Ruby: arr.tally
来源：http://ce.yuexingan06.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ys.asd995.cn

[D21] 判断是否包含某元素
来源：http://pf.huixiangedu.cn

Py:   x in arr
来源：http://ac.huixiangedu.cn

PHP:  in_array($x, $arr, true);
来源：http://lv.wgjwhj.cn

JS:   arr.includes(x)
来源：http://pe.huanxung.cn

TS:   arr.includes(x)
来源：http://ev.wgjwhj.cn

Java: list.contains(x)
来源：http://ll.szsharing.cn

Go:   slices.Contains(arr, x)
来源：http://xy.haigaiapp.cn

Ruby: arr.include?(x)
来源：http://ou.chemitech.net.cn

C#:   list.Contains(x)
来源：http://yl.yuntaijiaju.cn

[D22] 复制数组（避免共享引用）
来源：http://zl.panjiajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://af.bjjhwx.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://or.asd995.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dw.shxzskj.cn

TS:   [...arr];
来源：http://ua.jianghongdianzi.cn

Java: new ArrayList<>(list);
来源：http://gp.newstarts.cn

Go:   copied := append([]int(nil), arr...)
来源：http://wb.hnjuh.cn

Ruby: arr.dup;  arr.clone
来源：http://ni.haigaiapp.cn

C#:   new List<int>(list);
来源：http://rp.szsharing.cn

[D23] reduce 累积计算
来源：http://tp.jctech888.com.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ju.jianghongdianzi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jd.jctech888.com.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zd.szxytkj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hm.521024.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://nt.lnxyls.cn

Go:   // 手写循环
来源：http://bj.chemitech.net.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tc.jianghongdianzi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zk.asd995.cn

[D24] 字典 / Map 基本操作
来源：http://eb.huixiangedu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ms.huixinmuqiang.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bj.521024.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ea.hahajie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wt.haigaiapp.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mn.colortex.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gq.bookmarksfly.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kq.yuexingan06.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hl.jctech888.com.cn

[D25] Set 集合去重与交并差
来源：http://ly.asd995.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rb.shxzukj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kw.yuexingan06.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rp.huixinmuqiang.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://iz.wgjwhj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tf.bookmarksfly.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://so.shxzskj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rb.huixinmuqiang.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kb.bookmarksfly.cn

[D26] 数组转字符串
来源：http://vg.9csxet.cn

Py:   ", ".join(map(str, arr))
来源：http://do.nicolike.cn

PHP:  implode(", ", $arr);
来源：http://vj.szxytkj.cn

JS:   arr.join(", ")
来源：http://md.9csxet.cn

TS:   arr.join(", ")
来源：http://uz.jctech888.com.cn

Java: String.join(", ", list)
来源：http://rw.szsharing.cn

Go:   strings.Join(strs, ", ")
来源：http://bu.nicolike.cn

Ruby: arr.join(", ")
来源：http://uy.9csxet.cn

C#:   string.Join(", ", list)
来源：http://wg.9csxet.cn

================================================================================
来源：http://tl.huanxung.cn

E. 字符串处理
来源：http://tc.haigaiapp.cn

================================================================================
来源：http://bz.bookmarksfly.cn

[E01] 拼接字符串
来源：http://mh.nicolike.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bp.asd995.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pz.shxzukj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cq.nszjky.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yn.nicolike.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ah.yuexingan06.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pb.jctech888.com.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sf.newstarts.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wq.panjiajie.cn

[E02] 重复字符串
来源：http://pj.huixiangedu.cn

Py:   "ab" * 3
来源：http://sy.shxzukj.cn

PHP:  str_repeat("ab", 3);
来源：http://nt.chemitech.net.cn

JS:   "ab".repeat(3)
来源：http://hb.nicolike.cn

TS:   "ab".repeat(3)
来源：http://ta.bookmarksfly.cn

Java: "ab".repeat(3)
来源：http://gg.huanxung.cn

Go:   strings.Repeat("ab", 3)
来源：http://gp.colortex.cn

Ruby: "ab" * 3
来源：http://rg.nicolike.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sa.jianghongdianzi.cn

[E03] 截取子串
来源：http://ro.wgjwhj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://iy.yuexingan06.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ze.bookmarksfly.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tc.hahajie.cn

TS:   s.slice(1, 4)
来源：http://az.huanxung.cn

Java: s.substring(1, 4)
来源：http://ak.nicolike.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bh.jianghongdianzi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://fd.huixinmuqiang.cn

C#:   s.Substring(1, 3)
来源：http://tw.hahajie.cn

[E04] 查找子串位置
来源：http://kr.nszjky.cn

Py:   s.find("x");  s.index("x")
来源：http://ud.panjiajie.cn

PHP:  strpos($s, "x");
来源：http://nf.shtwfgs.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dz.yuntaijiaju.cn

TS:   s.indexOf("x")
来源：http://xo.huixinmuqiang.cn

Java: s.indexOf("x")
来源：http://ww.nicolike.cn

Go:   strings.Index(s, "x")
来源：http://fl.wgjwhj.cn

Ruby: s.index("x")
来源：http://cz.shxzukj.cn

C#:   s.IndexOf("x")
来源：http://oa.huixiangedu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://nf.haigaiapp.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pg.9csxet.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://el.haigaiapp.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ea.panjiajie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://bp.nszjky.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kl.shtwfgs.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zk.nszjky.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gc.huixiangedu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ty.newstarts.cn

[E06] 替换子串
来源：http://kj.asd995.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dp.asd995.cn

PHP:  str_replace("a", "b", $s);
来源：http://me.muxihuayi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vw.shtwfgs.cn

TS:   s.replaceAll("a", "b")
来源：http://cm.yuntaijiaju.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gh.wgjwhj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://km.nicolike.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hm.jianghongdianzi.cn

C#:   s.Replace("a", "b")
来源：http://lv.jianghongdianzi.cn

[E07] 按分隔符拆分
来源：http://cp.chemitech.net.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mp.bookmarksfly.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mi.wgjwhj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://qp.panjiajie.cn

TS:   s.split(",")
来源：http://vm.jianghongdianzi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://gd.nicolike.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xh.panjiajie.cn

Ruby: s.split(",");  s.split
来源：http://ml.521024.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xf.yuntaijiaju.cn

[E08] 数组按分隔符合并
来源：http://le.521024.cn

Py:   ",".join(items)
来源：http://dg.shtwfgs.cn

PHP:  implode(",", $items);
来源：http://ic.bjjhwx.cn

JS:   items.join(",")
来源：http://py.9csxet.cn

TS:   items.join(",")
来源：http://qw.shxzukj.cn

Java: String.join(",", items)
来源：http://hl.chemitech.net.cn

Go:   strings.Join(items, ",")
来源：http://vy.yuntaijiaju.cn

Ruby: items.join(",")
来源：http://dp.asd995.cn

C#:   string.Join(",", items)
来源：http://vs.shxzukj.cn

[E09] 去除所有空白字符
来源：http://yb.huanxung.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bu.wgjwhj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pr.nicolike.cn

JS:   s.replace(/\s+/g, "")
来源：http://hi.yuntaijiaju.cn

TS:   s.replace(/\s+/g, "")
来源：http://wc.muxihuayi.cn

Java: s.replaceAll("\\s+", "")
来源：http://qy.wgjwhj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://oa.bjjhwx.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ty.bjjhwx.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pz.hnjuh.cn

[E10] 左侧补零 / 定长填充
来源：http://qb.szsharing.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://me.jctech888.com.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hc.chemitech.net.cn

JS:   "7".padStart(3, "0")
来源：http://es.huixiangedu.cn

TS:   "7".padStart(3, "0")
来源：http://qh.szxytkj.cn

Java: String.format("%03d", 7)
来源：http://gu.colortex.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://nb.panjiajie.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://th.hahajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://li.newstarts.cn

[E11] 反转字符串
来源：http://xm.newstarts.cn

Py:   s[::-1]
来源：http://dw.nicolike.cn

PHP:  strrev($s);
来源：http://hh.hahajie.cn

JS:   [...s].reverse().join("")
来源：http://tu.szsharing.cn

TS:   [...s].reverse().join("")
来源：http://mc.bookmarksfly.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ju.shxzukj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ex.hahajie.cn

Ruby: s.reverse
来源：http://ik.jctech888.com.cn

C#:   new string(s.Reverse().ToArray())
来源：http://nf.jctech888.com.cn

[E12] 统计某字符出现次数
来源：http://fu.shxzskj.cn

Py:   s.count("a")
来源：http://ov.newstarts.cn

PHP:  substr_count($s, "a");
来源：http://yq.shxzskj.cn

JS:   s.split("a").length - 1
来源：http://dp.lnxyls.cn

TS:   s.split("a").length - 1
来源：http://xv.hahajie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://js.521024.cn

Go:   strings.Count(s, "a")
来源：http://ji.yuntaijiaju.cn

Ruby: s.count("a")
来源：http://ig.521024.cn

C#:   s.Count(c => c == 'a')
来源：http://wp.yuexingan06.cn

[E13] 逐字符遍历
来源：http://yj.muxihuayi.cn

Py:   for ch in s: print(ch)
来源：http://st.bookmarksfly.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ik.nicolike.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://hr.huixinmuqiang.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ts.newstarts.cn


<!-- 参考信息 -->