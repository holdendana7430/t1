代发 wailian999

[D07] 切片 / 取子数组
来源：http://gy.nicolike.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xq.lnxyls.cn

PHP:  array_slice($arr, 1, 3);
来源：http://bq.jianghongdianzi.cn

JS:   arr.slice(1, 4);
来源：http://rk.nicolike.cn

TS:   arr.slice(1, 4);
来源：http://cj.shxzukj.cn

Java: list.subList(1, 4);
来源：http://th.jctech888.com.cn

Go:   arr[1:4]
来源：http://zg.yuexingan06.cn

Ruby: arr[1, 3]
来源：http://dh.colortex.cn

C#:   list.GetRange(1, 3);
来源：http://jv.yuntaijiaju.cn

[D08] 合并两个数组
来源：http://qe.hahajie.cn

Py:   a + b;  a.extend(b)
来源：http://zy.colortex.cn

PHP:  array_merge($a, $b);
来源：http://nv.nszjky.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://es.yuntaijiaju.cn

TS:   [...a, ...b];
来源：http://nu.hnjuh.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nb.huixiangedu.cn

Go:   append(a, b...)
来源：http://zh.chemitech.net.cn

Ruby: a + b;  a.concat(b)
来源：http://hp.shxzukj.cn

C#:   a.Concat(b).ToList()
来源：http://vh.nszjky.cn

[D09] 排序（升序）
来源：http://td.huixinmuqiang.cn

Py:   sorted(arr);  arr.sort()
来源：http://yy.colortex.cn

PHP:  sort($arr);
来源：http://qk.hnjuh.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vr.shtwfgs.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://qg.newstarts.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://dd.huixinmuqiang.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vp.huixinmuqiang.cn

Ruby: arr.sort
来源：http://gn.bookmarksfly.cn

C#:   list.Sort();
来源：http://po.bjjhwx.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://aj.hahajie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gn.jianghongdianzi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eg.chemitech.net.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jb.muxihuayi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xh.newstarts.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tb.huixinmuqiang.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://th.huanxung.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ny.hnjuh.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lq.hahajie.cn

[D11] 反转数组
来源：http://ii.szxytkj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://lz.huixinmuqiang.cn

PHP:  array_reverse($arr);
来源：http://br.muxihuayi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jh.newstarts.cn

TS:   [...arr].reverse();
来源：http://xb.haigaiapp.cn

Java: Collections.reverse(list);
来源：http://uz.gzmigu.cn

Go:   slices.Reverse(arr)
来源：http://zv.hnjuh.cn

Ruby: arr.reverse
来源：http://tt.haigaiapp.cn

C#:   list.Reverse();
来源：http://ol.lnxyls.cn

[D12] 查找元素下标
来源：http://ck.colortex.cn

Py:   arr.index(x);  x in arr
来源：http://zh.gzmigu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://my.hahajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lx.nszjky.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wv.nicolike.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kp.nszjky.cn

Go:   slices.Index(arr, x)
来源：http://qj.colortex.cn

Ruby: arr.index(x)
来源：http://nw.huanxung.cn

C#:   list.IndexOf(x);
来源：http://qg.jctech888.com.cn

[D13] 过滤（保留满足条件的）
来源：http://ui.wgjwhj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lt.muxihuayi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ok.hahajie.cn

JS:   arr.filter(x => x > 3)
来源：http://xl.panjiajie.cn

TS:   arr.filter(x => x > 3)
来源：http://zn.bookmarksfly.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fv.shxzukj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ep.shtwfgs.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hu.wgjwhj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://kd.panjiajie.cn

[D14] 映射转换（每个元素变形）
来源：http://iu.muxihuayi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jj.shxzskj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cd.shtwfgs.cn

JS:   arr.map(x => x * 2)
来源：http://jz.muxihuayi.cn

TS:   arr.map(x => x * 2)
来源：http://vg.panjiajie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ck.nicolike.cn

Go:   // 手写循环
来源：http://de.shtwfgs.cn

Ruby: arr.map { |x| x * 2 }
来源：http://zn.muxihuayi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://yr.panjiajie.cn

[D15] 去重
来源：http://pn.bookmarksfly.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wu.chemitech.net.cn

PHP:  array_unique($arr);
来源：http://cf.asd995.cn

JS:   [...new Set(arr)]
来源：http://qc.szsharing.cn

TS:   [...new Set(arr)]
来源：http://vo.jianghongdianzi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jr.nicolike.cn

Go:   // 用 map[T]struct{} 手写
来源：http://rz.nszjky.cn

Ruby: arr.uniq
来源：http://ia.bookmarksfly.cn

C#:   list.Distinct().ToList()
来源：http://ps.muxihuayi.cn

[D16] 求和与平均值
来源：http://ni.nszjky.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wn.yuntaijiaju.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yn.chemitech.net.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://eo.lnxyls.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ea.shxzukj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ae.hahajie.cn

Go:   // 手写循环累加
来源：http://my.szsharing.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bq.newstarts.cn

C#:   list.Sum();  list.Average()
来源：http://zb.chemitech.net.cn

[D17] 最大值与最小值
来源：http://dm.muxihuayi.cn

Py:   max(arr);  min(arr)
来源：http://es.bookmarksfly.cn

PHP:  max($arr);  min($arr);
来源：http://nu.bjjhwx.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bw.panjiajie.cn

TS:   Math.max(...arr);
来源：http://ti.9csxet.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://km.9csxet.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://al.shxzskj.cn

Ruby: arr.max;  arr.min
来源：http://wr.shxzskj.cn

C#:   list.Max();  list.Min()
来源：http://fh.panjiajie.cn

[D18] 扁平化嵌套数组
来源：http://hv.shxzukj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zv.yuexingan06.cn

PHP:  array_merge(...$nested);
来源：http://fc.shtwfgs.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ci.asd995.cn

TS:   nested.flat();
来源：http://bu.nszjky.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wl.wgjwhj.cn

Go:   // 手写双层循环
来源：http://lh.shxzukj.cn

Ruby: nested.flatten
来源：http://et.nszjky.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://as.yuexingan06.cn

[D19] 按字段分组
来源：http://is.shxzskj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://po.hahajie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tr.521024.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wj.shtwfgs.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://oo.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://eh.jianghongdianzi.cn

Go:   // 手写 map[string][]T
来源：http://ga.huixinmuqiang.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://km.huanxung.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ar.shxzskj.cn

[D20] 统计每个元素出现次数
来源：http://wx.huanxung.cn

Py:   Counter(arr)
来源：http://gg.shxzskj.cn

PHP:  array_count_values($arr);
来源：http://us.nicolike.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://af.szsharing.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://on.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://aa.gzmigu.cn

Go:   // 手写 map[T]int
来源：http://nx.huixinmuqiang.cn

Ruby: arr.tally
来源：http://wu.nicolike.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ys.haigaiapp.cn

[D21] 判断是否包含某元素
来源：http://pk.chemitech.net.cn

Py:   x in arr
来源：http://dx.wgjwhj.cn

PHP:  in_array($x, $arr, true);
来源：http://nd.9csxet.cn

JS:   arr.includes(x)
来源：http://qu.lnxyls.cn

TS:   arr.includes(x)
来源：http://kp.haigaiapp.cn

Java: list.contains(x)
来源：http://vg.hahajie.cn

Go:   slices.Contains(arr, x)
来源：http://qu.hnjuh.cn

Ruby: arr.include?(x)
来源：http://nu.szsharing.cn

C#:   list.Contains(x)
来源：http://uf.shxzukj.cn

[D22] 复制数组（避免共享引用）
来源：http://do.nszjky.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wj.bookmarksfly.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tg.newstarts.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tw.muxihuayi.cn

TS:   [...arr];
来源：http://kz.jctech888.com.cn

Java: new ArrayList<>(list);
来源：http://jr.shtwfgs.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ie.lnxyls.cn

Ruby: arr.dup;  arr.clone
来源：http://pi.szsharing.cn

C#:   new List<int>(list);
来源：http://kh.hahajie.cn

[D23] reduce 累积计算
来源：http://rd.bookmarksfly.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ev.shxzukj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pi.wgjwhj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pb.bjjhwx.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ds.huixinmuqiang.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://hv.szxytkj.cn

Go:   // 手写循环
来源：http://fr.nszjky.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://le.jianghongdianzi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wf.9csxet.cn

[D24] 字典 / Map 基本操作
来源：http://gp.lnxyls.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ha.szsharing.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hp.9csxet.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mx.colortex.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sz.huixinmuqiang.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ax.lnxyls.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ow.panjiajie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fk.huanxung.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zx.panjiajie.cn

[D25] Set 集合去重与交并差
来源：http://up.panjiajie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://td.newstarts.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lf.muxihuayi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jg.chemitech.net.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://su.newstarts.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fe.huixiangedu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ll.yuntaijiaju.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uu.hahajie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://et.yuntaijiaju.cn

[D26] 数组转字符串
来源：http://sg.shxzukj.cn

Py:   ", ".join(map(str, arr))
来源：http://by.colortex.cn

PHP:  implode(", ", $arr);
来源：http://do.shxzskj.cn

JS:   arr.join(", ")
来源：http://bm.huixiangedu.cn

TS:   arr.join(", ")
来源：http://zz.jianghongdianzi.cn

Java: String.join(", ", list)
来源：http://oc.9csxet.cn

Go:   strings.Join(strs, ", ")
来源：http://hr.lnxyls.cn

Ruby: arr.join(", ")
来源：http://as.nszjky.cn

C#:   string.Join(", ", list)
来源：http://de.haigaiapp.cn

================================================================================
来源：http://sc.bookmarksfly.cn

E. 字符串处理
来源：http://vn.colortex.cn

================================================================================
来源：http://rd.bjjhwx.cn

[E01] 拼接字符串
来源：http://pu.lnxyls.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vd.huixiangedu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xr.lnxyls.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://in.jctech888.com.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ej.panjiajie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sw.chemitech.net.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lx.szxytkj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vi.bjjhwx.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mq.newstarts.cn

[E02] 重复字符串
来源：http://ac.hahajie.cn

Py:   "ab" * 3
来源：http://vn.wgjwhj.cn

PHP:  str_repeat("ab", 3);
来源：http://zy.newstarts.cn

JS:   "ab".repeat(3)
来源：http://yu.nicolike.cn

TS:   "ab".repeat(3)
来源：http://as.panjiajie.cn

Java: "ab".repeat(3)
来源：http://db.nszjky.cn

Go:   strings.Repeat("ab", 3)
来源：http://nq.muxihuayi.cn

Ruby: "ab" * 3
来源：http://sw.shxzukj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vm.panjiajie.cn

[E03] 截取子串
来源：http://nk.gzmigu.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fl.chemitech.net.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dq.chemitech.net.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gw.521024.cn

TS:   s.slice(1, 4)
来源：http://pa.bjjhwx.cn

Java: s.substring(1, 4)
来源：http://cn.lnxyls.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pd.jianghongdianzi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://nb.muxihuayi.cn

C#:   s.Substring(1, 3)
来源：http://qn.gzmigu.cn

[E04] 查找子串位置
来源：http://hh.bookmarksfly.cn

Py:   s.find("x");  s.index("x")
来源：http://sx.lnxyls.cn

PHP:  strpos($s, "x");
来源：http://tk.haigaiapp.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gw.hahajie.cn

TS:   s.indexOf("x")
来源：http://rg.newstarts.cn

Java: s.indexOf("x")
来源：http://mn.szsharing.cn

Go:   strings.Index(s, "x")
来源：http://sr.szxytkj.cn

Ruby: s.index("x")
来源：http://ij.panjiajie.cn

C#:   s.IndexOf("x")
来源：http://df.bjjhwx.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://we.521024.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jy.lnxyls.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rm.muxihuayi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mf.yuexingan06.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://bh.yuexingan06.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nu.yuntaijiaju.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uu.yuexingan06.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pz.yuntaijiaju.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zd.jianghongdianzi.cn

[E06] 替换子串
来源：http://yr.huanxung.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fr.jianghongdianzi.cn

PHP:  str_replace("a", "b", $s);
来源：http://tc.panjiajie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ei.521024.cn

TS:   s.replaceAll("a", "b")
来源：http://ko.gzmigu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fa.muxihuayi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jv.wgjwhj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yq.nszjky.cn

C#:   s.Replace("a", "b")
来源：http://yk.szxytkj.cn

[E07] 按分隔符拆分
来源：http://fh.yuexingan06.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://uh.panjiajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nf.jianghongdianzi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://qz.521024.cn

TS:   s.split(",")
来源：http://hl.9csxet.cn

Java: s.split(",");  s.split("\\s+")
来源：http://la.bookmarksfly.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ps.colortex.cn

Ruby: s.split(",");  s.split
来源：http://ra.szxytkj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bp.jianghongdianzi.cn

[E08] 数组按分隔符合并
来源：http://wz.bjjhwx.cn

Py:   ",".join(items)
来源：http://ks.panjiajie.cn

PHP:  implode(",", $items);
来源：http://vz.nicolike.cn

JS:   items.join(",")
来源：http://zd.hahajie.cn

TS:   items.join(",")
来源：http://bz.hahajie.cn

Java: String.join(",", items)
来源：http://my.panjiajie.cn

Go:   strings.Join(items, ",")
来源：http://ax.huixinmuqiang.cn

Ruby: items.join(",")
来源：http://zz.hnjuh.cn

C#:   string.Join(",", items)
来源：http://xz.newstarts.cn

[E09] 去除所有空白字符
来源：http://ql.muxihuayi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tf.jctech888.com.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jm.szxytkj.cn

JS:   s.replace(/\s+/g, "")
来源：http://ai.huanxung.cn

TS:   s.replace(/\s+/g, "")
来源：http://tk.shxzskj.cn

Java: s.replaceAll("\\s+", "")
来源：http://fv.asd995.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://kz.lnxyls.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ya.asd995.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zo.panjiajie.cn

[E10] 左侧补零 / 定长填充
来源：http://bu.szxytkj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ad.hnjuh.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hl.haigaiapp.cn

JS:   "7".padStart(3, "0")
来源：http://nk.yuexingan06.cn

TS:   "7".padStart(3, "0")
来源：http://ul.9csxet.cn

Java: String.format("%03d", 7)
来源：http://dc.huixinmuqiang.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://tp.jianghongdianzi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://uh.panjiajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bz.muxihuayi.cn

[E11] 反转字符串
来源：http://ms.nszjky.cn

Py:   s[::-1]
来源：http://pq.newstarts.cn

PHP:  strrev($s);
来源：http://na.nszjky.cn

JS:   [...s].reverse().join("")
来源：http://wk.hnjuh.cn

TS:   [...s].reverse().join("")
来源：http://wq.haigaiapp.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://um.nicolike.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://jn.newstarts.cn

Ruby: s.reverse
来源：http://qe.shtwfgs.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ik.muxihuayi.cn

[E12] 统计某字符出现次数
来源：http://lz.gzmigu.cn

Py:   s.count("a")
来源：http://tr.newstarts.cn

PHP:  substr_count($s, "a");
来源：http://fa.huixiangedu.cn

JS:   s.split("a").length - 1
来源：http://xa.nicolike.cn

TS:   s.split("a").length - 1
来源：http://px.yuntaijiaju.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ai.521024.cn

Go:   strings.Count(s, "a")
来源：http://fi.szsharing.cn

Ruby: s.count("a")
来源：http://wy.hnjuh.cn

C#:   s.Count(c => c == 'a')
来源：http://kb.yuexingan06.cn

[E13] 逐字符遍历
来源：http://um.lnxyls.cn

Py:   for ch in s: print(ch)
来源：http://cg.haigaiapp.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ni.asd995.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://iw.521024.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://xt.yuntaijiaju.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://id.lnxyls.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kf.lnxyls.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ny.lnxyls.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kj.521024.cn


<!-- 参考信息 -->