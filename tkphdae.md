代发 wailian999

TS:   arr.slice(1, 4);
来源：http://ss.bjjhwx.cn

Java: list.subList(1, 4);
来源：http://ph.huixiangedu.cn

Go:   arr[1:4]
来源：http://ps.hahajie.cn

Ruby: arr[1, 3]
来源：http://tu.szxytkj.cn

C#:   list.GetRange(1, 3);
来源：http://pl.yuntaijiaju.cn

[D08] 合并两个数组
来源：http://ww.colortex.cn

Py:   a + b;  a.extend(b)
来源：http://si.szsharing.cn

PHP:  array_merge($a, $b);
来源：http://kf.bookmarksfly.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://kn.jctech888.com.cn

TS:   [...a, ...b];
来源：http://zm.colortex.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ng.gzmigu.cn

Go:   append(a, b...)
来源：http://rl.9csxet.cn

Ruby: a + b;  a.concat(b)
来源：http://kb.hahajie.cn

C#:   a.Concat(b).ToList()
来源：http://ej.shxzskj.cn

[D09] 排序（升序）
来源：http://jc.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://cy.muxihuayi.cn

PHP:  sort($arr);
来源：http://dr.lnxyls.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://aq.shtwfgs.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fj.huanxung.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://en.nszjky.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zi.shxzskj.cn

Ruby: arr.sort
来源：http://ju.yuexingan06.cn

C#:   list.Sort();
来源：http://sp.huanxung.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ya.shxzukj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://or.panjiajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yz.huixinmuqiang.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wh.yuntaijiaju.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://sb.nicolike.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ja.lnxyls.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fd.bjjhwx.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pw.shxzskj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mj.gzmigu.cn

[D11] 反转数组
来源：http://ys.panjiajie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://oz.hahajie.cn

PHP:  array_reverse($arr);
来源：http://nj.bjjhwx.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vl.nszjky.cn

TS:   [...arr].reverse();
来源：http://vh.bookmarksfly.cn

Java: Collections.reverse(list);
来源：http://kw.huanxung.cn

Go:   slices.Reverse(arr)
来源：http://hc.jctech888.com.cn

Ruby: arr.reverse
来源：http://nb.panjiajie.cn

C#:   list.Reverse();
来源：http://vs.huanxung.cn

[D12] 查找元素下标
来源：http://rm.hahajie.cn

Py:   arr.index(x);  x in arr
来源：http://ly.hnjuh.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qm.chemitech.net.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rw.jctech888.com.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kp.shtwfgs.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ty.shxzukj.cn

Go:   slices.Index(arr, x)
来源：http://lk.yuntaijiaju.cn

Ruby: arr.index(x)
来源：http://wb.haigaiapp.cn

C#:   list.IndexOf(x);
来源：http://kt.bjjhwx.cn

[D13] 过滤（保留满足条件的）
来源：http://bq.lnxyls.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://al.jctech888.com.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nc.panjiajie.cn

JS:   arr.filter(x => x > 3)
来源：http://ds.bjjhwx.cn

TS:   arr.filter(x => x > 3)
来源：http://di.yuntaijiaju.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ox.haigaiapp.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://to.lnxyls.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wy.hahajie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qa.szsharing.cn

[D14] 映射转换（每个元素变形）
来源：http://ol.haigaiapp.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kx.shtwfgs.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ke.shxzskj.cn

JS:   arr.map(x => x * 2)
来源：http://pa.bjjhwx.cn

TS:   arr.map(x => x * 2)
来源：http://yj.huixiangedu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://wx.huixinmuqiang.cn

Go:   // 手写循环
来源：http://ld.521024.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hw.nicolike.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://lw.shxzskj.cn

[D15] 去重
来源：http://jb.shxzskj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ad.nszjky.cn

PHP:  array_unique($arr);
来源：http://wv.jianghongdianzi.cn

JS:   [...new Set(arr)]
来源：http://fx.asd995.cn

TS:   [...new Set(arr)]
来源：http://ir.nszjky.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vh.panjiajie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ns.chemitech.net.cn

Ruby: arr.uniq
来源：http://xz.jctech888.com.cn

C#:   list.Distinct().ToList()
来源：http://ru.shxzukj.cn

[D16] 求和与平均值
来源：http://ti.newstarts.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ra.9csxet.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rx.yuexingan06.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ak.nicolike.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dd.hnjuh.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ge.wgjwhj.cn

Go:   // 手写循环累加
来源：http://ub.nszjky.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://oh.nszjky.cn

C#:   list.Sum();  list.Average()
来源：http://qb.nszjky.cn

[D17] 最大值与最小值
来源：http://zj.jctech888.com.cn

Py:   max(arr);  min(arr)
来源：http://jw.asd995.cn

PHP:  max($arr);  min($arr);
来源：http://im.hnjuh.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://at.shxzskj.cn

TS:   Math.max(...arr);
来源：http://fs.gzmigu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mn.wgjwhj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vu.nszjky.cn

Ruby: arr.max;  arr.min
来源：http://qe.9csxet.cn

C#:   list.Max();  list.Min()
来源：http://ou.szxytkj.cn

[D18] 扁平化嵌套数组
来源：http://go.chemitech.net.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dq.yuntaijiaju.cn

PHP:  array_merge(...$nested);
来源：http://qq.wgjwhj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kj.chemitech.net.cn

TS:   nested.flat();
来源：http://gv.bjjhwx.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bs.bjjhwx.cn

Go:   // 手写双层循环
来源：http://lx.haigaiapp.cn

Ruby: nested.flatten
来源：http://ff.9csxet.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://wp.gzmigu.cn

[D19] 按字段分组
来源：http://wp.huixiangedu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yy.jctech888.com.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://me.huanxung.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mz.yuntaijiaju.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://la.521024.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://if.gzmigu.cn

Go:   // 手写 map[string][]T
来源：http://hu.shxzskj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ho.gzmigu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dl.jianghongdianzi.cn

[D20] 统计每个元素出现次数
来源：http://pb.shtwfgs.cn

Py:   Counter(arr)
来源：http://ts.bookmarksfly.cn

PHP:  array_count_values($arr);
来源：http://pr.huanxung.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ma.newstarts.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xt.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dv.muxihuayi.cn

Go:   // 手写 map[T]int
来源：http://vi.bjjhwx.cn

Ruby: arr.tally
来源：http://qf.jctech888.com.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ea.nszjky.cn

[D21] 判断是否包含某元素
来源：http://fu.gzmigu.cn

Py:   x in arr
来源：http://uy.nicolike.cn

PHP:  in_array($x, $arr, true);
来源：http://zk.bjjhwx.cn

JS:   arr.includes(x)
来源：http://uj.bjjhwx.cn

TS:   arr.includes(x)
来源：http://ex.bookmarksfly.cn

Java: list.contains(x)
来源：http://gi.shxzukj.cn

Go:   slices.Contains(arr, x)
来源：http://ns.panjiajie.cn

Ruby: arr.include?(x)
来源：http://es.shxzukj.cn

C#:   list.Contains(x)
来源：http://mn.colortex.cn

[D22] 复制数组（避免共享引用）
来源：http://tq.yuntaijiaju.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ax.muxihuayi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ip.bookmarksfly.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ly.shxzukj.cn

TS:   [...arr];
来源：http://vq.huanxung.cn

Java: new ArrayList<>(list);
来源：http://ki.huanxung.cn

Go:   copied := append([]int(nil), arr...)
来源：http://wc.nszjky.cn

Ruby: arr.dup;  arr.clone
来源：http://zb.colortex.cn

C#:   new List<int>(list);
来源：http://fb.yuexingan06.cn

[D23] reduce 累积计算
来源：http://yo.muxihuayi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lx.huixinmuqiang.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://sl.haigaiapp.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yz.bookmarksfly.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tm.newstarts.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://up.haigaiapp.cn

Go:   // 手写循环
来源：http://tq.huanxung.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xi.colortex.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://oy.gzmigu.cn

[D24] 字典 / Map 基本操作
来源：http://xv.yuexingan06.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yh.hnjuh.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://id.panjiajie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://re.huixinmuqiang.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cz.hahajie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dt.shtwfgs.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://op.9csxet.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lf.panjiajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://sq.gzmigu.cn

[D25] Set 集合去重与交并差
来源：http://jb.huixiangedu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vt.huixiangedu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pv.yuexingan06.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jx.jctech888.com.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kc.shxzskj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://go.bookmarksfly.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mc.huixinmuqiang.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uw.bookmarksfly.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qj.asd995.cn

[D26] 数组转字符串
来源：http://id.jctech888.com.cn

Py:   ", ".join(map(str, arr))
来源：http://mu.colortex.cn

PHP:  implode(", ", $arr);
来源：http://zj.bjjhwx.cn

JS:   arr.join(", ")
来源：http://jo.huixiangedu.cn

TS:   arr.join(", ")
来源：http://is.521024.cn

Java: String.join(", ", list)
来源：http://ro.szxytkj.cn

Go:   strings.Join(strs, ", ")
来源：http://lz.wgjwhj.cn

Ruby: arr.join(", ")
来源：http://na.bookmarksfly.cn

C#:   string.Join(", ", list)
来源：http://qx.bjjhwx.cn

================================================================================
来源：http://sw.jctech888.com.cn

E. 字符串处理
来源：http://zz.newstarts.cn

================================================================================
来源：http://lk.yuexingan06.cn

[E01] 拼接字符串
来源：http://wr.newstarts.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ee.huixinmuqiang.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yb.panjiajie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bn.huixinmuqiang.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ed.hnjuh.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ox.521024.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kd.521024.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dk.521024.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://na.panjiajie.cn

[E02] 重复字符串
来源：http://ze.wgjwhj.cn

Py:   "ab" * 3
来源：http://ny.9csxet.cn

PHP:  str_repeat("ab", 3);
来源：http://bv.szxytkj.cn

JS:   "ab".repeat(3)
来源：http://nm.521024.cn

TS:   "ab".repeat(3)
来源：http://ti.bookmarksfly.cn

Java: "ab".repeat(3)
来源：http://rr.shtwfgs.cn

Go:   strings.Repeat("ab", 3)
来源：http://zz.huanxung.cn

Ruby: "ab" * 3
来源：http://vh.chemitech.net.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://es.muxihuayi.cn

[E03] 截取子串
来源：http://ma.newstarts.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jx.521024.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yd.nicolike.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gz.nszjky.cn

TS:   s.slice(1, 4)
来源：http://pd.wgjwhj.cn

Java: s.substring(1, 4)
来源：http://na.521024.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wi.bjjhwx.cn

Ruby: s[1, 3];  s[1..3]
来源：http://py.nicolike.cn

C#:   s.Substring(1, 3)
来源：http://nk.yuntaijiaju.cn

[E04] 查找子串位置
来源：http://dv.jctech888.com.cn

Py:   s.find("x");  s.index("x")
来源：http://lz.szsharing.cn

PHP:  strpos($s, "x");
来源：http://hy.bjjhwx.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qr.chemitech.net.cn

TS:   s.indexOf("x")
来源：http://nk.gzmigu.cn

Java: s.indexOf("x")
来源：http://fb.hnjuh.cn

Go:   strings.Index(s, "x")
来源：http://ai.newstarts.cn

Ruby: s.index("x")
来源：http://nx.gzmigu.cn

C#:   s.IndexOf("x")
来源：http://qs.muxihuayi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://hh.haigaiapp.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vr.yuntaijiaju.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ib.nicolike.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gb.jianghongdianzi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://bn.asd995.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://px.bookmarksfly.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bp.shtwfgs.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wi.panjiajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yp.bjjhwx.cn

[E06] 替换子串
来源：http://kw.wgjwhj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wx.jianghongdianzi.cn

PHP:  str_replace("a", "b", $s);
来源：http://qu.szxytkj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://db.haigaiapp.cn

TS:   s.replaceAll("a", "b")
来源：http://fa.wgjwhj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eh.huixinmuqiang.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ib.jianghongdianzi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nk.yuexingan06.cn

C#:   s.Replace("a", "b")
来源：http://rb.szsharing.cn

[E07] 按分隔符拆分
来源：http://zl.bookmarksfly.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pj.newstarts.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vz.yuntaijiaju.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://up.521024.cn

TS:   s.split(",")
来源：http://ng.jianghongdianzi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://uq.shxzskj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ks.9csxet.cn

Ruby: s.split(",");  s.split
来源：http://sq.huixinmuqiang.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yq.asd995.cn

[E08] 数组按分隔符合并
来源：http://gz.jianghongdianzi.cn

Py:   ",".join(items)
来源：http://uk.jctech888.com.cn

PHP:  implode(",", $items);
来源：http://wy.lnxyls.cn

JS:   items.join(",")
来源：http://eb.lnxyls.cn

TS:   items.join(",")
来源：http://il.shxzukj.cn

Java: String.join(",", items)
来源：http://yt.shxzskj.cn

Go:   strings.Join(items, ",")
来源：http://ot.shxzukj.cn

Ruby: items.join(",")
来源：http://gr.jianghongdianzi.cn

C#:   string.Join(",", items)
来源：http://nq.9csxet.cn

[E09] 去除所有空白字符
来源：http://zn.huanxung.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ek.wgjwhj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lc.hnjuh.cn

JS:   s.replace(/\s+/g, "")
来源：http://fp.521024.cn

TS:   s.replace(/\s+/g, "")
来源：http://co.huixinmuqiang.cn

Java: s.replaceAll("\\s+", "")
来源：http://xw.shxzskj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://kc.huanxung.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ke.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://di.colortex.cn

[E10] 左侧补零 / 定长填充
来源：http://fe.jianghongdianzi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://by.gzmigu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://uq.gzmigu.cn

JS:   "7".padStart(3, "0")
来源：http://qb.newstarts.cn

TS:   "7".padStart(3, "0")
来源：http://ni.gzmigu.cn

Java: String.format("%03d", 7)
来源：http://xi.wgjwhj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://gv.9csxet.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nj.wgjwhj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://so.shxzukj.cn

[E11] 反转字符串
来源：http://rn.521024.cn

Py:   s[::-1]
来源：http://hu.gzmigu.cn

PHP:  strrev($s);
来源：http://xv.szxytkj.cn

JS:   [...s].reverse().join("")
来源：http://mw.hahajie.cn

TS:   [...s].reverse().join("")
来源：http://wr.521024.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ot.huixinmuqiang.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://yr.newstarts.cn

Ruby: s.reverse
来源：http://nx.521024.cn

C#:   new string(s.Reverse().ToArray())
来源：http://br.hnjuh.cn

[E12] 统计某字符出现次数
来源：http://jg.huanxung.cn

Py:   s.count("a")
来源：http://lg.nicolike.cn

PHP:  substr_count($s, "a");
来源：http://wt.muxihuayi.cn

JS:   s.split("a").length - 1
来源：http://rn.gzmigu.cn

TS:   s.split("a").length - 1
来源：http://jp.gzmigu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qe.colortex.cn

Go:   strings.Count(s, "a")
来源：http://aw.newstarts.cn

Ruby: s.count("a")
来源：http://su.bookmarksfly.cn

C#:   s.Count(c => c == 'a')
来源：http://dj.szxytkj.cn

[E13] 逐字符遍历
来源：http://ff.szxytkj.cn

Py:   for ch in s: print(ch)
来源：http://at.szxytkj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cy.huixiangedu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://qk.huixinmuqiang.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ml.shxzskj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xq.newstarts.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zl.yuntaijiaju.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://sj.9csxet.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rq.lnxyls.cn

[E14] URL 编码与 Base64
来源：http://en.jianghongdianzi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://uk.chemitech.net.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ar.colortex.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qe.nicolike.cn


<!-- 参考信息 -->