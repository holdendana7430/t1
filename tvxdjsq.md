代发 wailian999

Java: list.size();
来源：http://ie.colortex.cn

Go:   len(arr)
来源：http://ga.shxzskj.cn

Ruby: arr.length; arr.size
来源：http://bi.haigaiapp.cn

C#:   list.Count;
来源：http://gl.huixinmuqiang.cn

[D07] 切片 / 取子数组
来源：http://pi.yuexingan06.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ss.jianghongdianzi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ts.shxzskj.cn

JS:   arr.slice(1, 4);
来源：http://tm.gzmigu.cn

TS:   arr.slice(1, 4);
来源：http://cc.yuntaijiaju.cn

Java: list.subList(1, 4);
来源：http://qm.yuntaijiaju.cn

Go:   arr[1:4]
来源：http://la.muxihuayi.cn

Ruby: arr[1, 3]
来源：http://jm.9csxet.cn

C#:   list.GetRange(1, 3);
来源：http://oj.chemitech.net.cn

[D08] 合并两个数组
来源：http://pp.yuexingan06.cn

Py:   a + b;  a.extend(b)
来源：http://ib.521024.cn

PHP:  array_merge($a, $b);
来源：http://qc.szxytkj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://kv.colortex.cn

TS:   [...a, ...b];
来源：http://il.asd995.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ik.bjjhwx.cn

Go:   append(a, b...)
来源：http://bb.muxihuayi.cn

Ruby: a + b;  a.concat(b)
来源：http://rr.huanxung.cn

C#:   a.Concat(b).ToList()
来源：http://qr.gzmigu.cn

[D09] 排序（升序）
来源：http://sr.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://mo.yuexingan06.cn

PHP:  sort($arr);
来源：http://zr.bookmarksfly.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sq.jianghongdianzi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fs.lnxyls.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://uq.lnxyls.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://un.nszjky.cn

Ruby: arr.sort
来源：http://mm.yuntaijiaju.cn

C#:   list.Sort();
来源：http://fn.szxytkj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://cb.jctech888.com.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://of.jianghongdianzi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ac.huixiangedu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qa.jctech888.com.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xo.jianghongdianzi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fr.hahajie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://oq.521024.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ce.hahajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bt.yuntaijiaju.cn

[D11] 反转数组
来源：http://fm.jctech888.com.cn

Py:   arr[::-1];  arr.reverse()
来源：http://al.shxzskj.cn

PHP:  array_reverse($arr);
来源：http://jv.szxytkj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nf.haigaiapp.cn

TS:   [...arr].reverse();
来源：http://pb.shxzskj.cn

Java: Collections.reverse(list);
来源：http://bh.newstarts.cn

Go:   slices.Reverse(arr)
来源：http://ad.wgjwhj.cn

Ruby: arr.reverse
来源：http://xs.bjjhwx.cn

C#:   list.Reverse();
来源：http://jm.521024.cn

[D12] 查找元素下标
来源：http://yq.jianghongdianzi.cn

Py:   arr.index(x);  x in arr
来源：http://sw.yuexingan06.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fc.wgjwhj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yj.huixiangedu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gt.9csxet.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ek.shxzukj.cn

Go:   slices.Index(arr, x)
来源：http://eq.szxytkj.cn

Ruby: arr.index(x)
来源：http://ob.huixiangedu.cn

C#:   list.IndexOf(x);
来源：http://yz.wgjwhj.cn

[D13] 过滤（保留满足条件的）
来源：http://ke.gzmigu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zl.huanxung.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xf.szxytkj.cn

JS:   arr.filter(x => x > 3)
来源：http://uw.panjiajie.cn

TS:   arr.filter(x => x > 3)
来源：http://mt.asd995.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jj.newstarts.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://om.colortex.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ra.jianghongdianzi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ze.yuntaijiaju.cn

[D14] 映射转换（每个元素变形）
来源：http://cx.szsharing.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hu.shtwfgs.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://su.hahajie.cn

JS:   arr.map(x => x * 2)
来源：http://fd.haigaiapp.cn

TS:   arr.map(x => x * 2)
来源：http://ow.huixiangedu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://nd.shtwfgs.cn

Go:   // 手写循环
来源：http://eg.gzmigu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vb.nicolike.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://vx.asd995.cn

[D15] 去重
来源：http://cv.9csxet.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cp.shxzukj.cn

PHP:  array_unique($arr);
来源：http://hy.shtwfgs.cn

JS:   [...new Set(arr)]
来源：http://tx.huanxung.cn

TS:   [...new Set(arr)]
来源：http://an.yuexingan06.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://le.muxihuayi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://fb.haigaiapp.cn

Ruby: arr.uniq
来源：http://iw.panjiajie.cn

C#:   list.Distinct().ToList()
来源：http://ki.shxzskj.cn

[D16] 求和与平均值
来源：http://ys.jianghongdianzi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dw.haigaiapp.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://oy.yuntaijiaju.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ey.shxzskj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fk.hnjuh.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://db.wgjwhj.cn

Go:   // 手写循环累加
来源：http://gg.shxzukj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yd.yuntaijiaju.cn

C#:   list.Sum();  list.Average()
来源：http://qd.hahajie.cn

[D17] 最大值与最小值
来源：http://re.bookmarksfly.cn

Py:   max(arr);  min(arr)
来源：http://ij.szxytkj.cn

PHP:  max($arr);  min($arr);
来源：http://tn.gzmigu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ll.newstarts.cn

TS:   Math.max(...arr);
来源：http://vc.lnxyls.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gg.nszjky.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://sw.hahajie.cn

Ruby: arr.max;  arr.min
来源：http://od.shtwfgs.cn

C#:   list.Max();  list.Min()
来源：http://yj.shtwfgs.cn

[D18] 扁平化嵌套数组
来源：http://bw.shxzskj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cd.huixinmuqiang.cn

PHP:  array_merge(...$nested);
来源：http://qy.muxihuayi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vr.lnxyls.cn

TS:   nested.flat();
来源：http://sn.shxzukj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://le.bjjhwx.cn

Go:   // 手写双层循环
来源：http://db.huixiangedu.cn

Ruby: nested.flatten
来源：http://kq.nszjky.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ne.jianghongdianzi.cn

[D19] 按字段分组
来源：http://or.jctech888.com.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wa.nicolike.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xs.hahajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dm.hnjuh.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://pl.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://el.panjiajie.cn

Go:   // 手写 map[string][]T
来源：http://hs.lnxyls.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rn.yuntaijiaju.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wk.haigaiapp.cn

[D20] 统计每个元素出现次数
来源：http://ne.panjiajie.cn

Py:   Counter(arr)
来源：http://dw.lnxyls.cn

PHP:  array_count_values($arr);
来源：http://zt.bookmarksfly.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yi.hahajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qe.bookmarksfly.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mf.9csxet.cn

Go:   // 手写 map[T]int
来源：http://gk.yuntaijiaju.cn

Ruby: arr.tally
来源：http://ob.jctech888.com.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qa.jctech888.com.cn

[D21] 判断是否包含某元素
来源：http://xt.yuexingan06.cn

Py:   x in arr
来源：http://vr.gzmigu.cn

PHP:  in_array($x, $arr, true);
来源：http://xf.bjjhwx.cn

JS:   arr.includes(x)
来源：http://ch.huixiangedu.cn

TS:   arr.includes(x)
来源：http://cs.panjiajie.cn

Java: list.contains(x)
来源：http://yv.jctech888.com.cn

Go:   slices.Contains(arr, x)
来源：http://yn.shxzskj.cn

Ruby: arr.include?(x)
来源：http://tf.chemitech.net.cn

C#:   list.Contains(x)
来源：http://eo.colortex.cn

[D22] 复制数组（避免共享引用）
来源：http://yd.lnxyls.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xx.haigaiapp.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lf.shtwfgs.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ql.huixinmuqiang.cn

TS:   [...arr];
来源：http://hf.shxzskj.cn

Java: new ArrayList<>(list);
来源：http://hr.huanxung.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cu.haigaiapp.cn

Ruby: arr.dup;  arr.clone
来源：http://ow.lnxyls.cn

C#:   new List<int>(list);
来源：http://sx.shxzukj.cn

[D23] reduce 累积计算
来源：http://eq.newstarts.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gk.nszjky.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jx.colortex.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mm.asd995.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nq.szxytkj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://yi.nicolike.cn

Go:   // 手写循环
来源：http://oq.bjjhwx.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yf.colortex.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vm.panjiajie.cn

[D24] 字典 / Map 基本操作
来源：http://np.yuntaijiaju.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wl.bjjhwx.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jx.huixinmuqiang.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://yv.shtwfgs.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dj.colortex.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dv.asd995.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bz.muxihuayi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bh.hahajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zh.yuntaijiaju.cn

[D25] Set 集合去重与交并差
来源：http://jg.jianghongdianzi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qd.shxzskj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vm.shxzskj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://iz.huanxung.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ro.muxihuayi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ea.gzmigu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ag.huixiangedu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hg.panjiajie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://oh.szxytkj.cn

[D26] 数组转字符串
来源：http://wd.szsharing.cn

Py:   ", ".join(map(str, arr))
来源：http://sr.shtwfgs.cn

PHP:  implode(", ", $arr);
来源：http://im.colortex.cn

JS:   arr.join(", ")
来源：http://lh.muxihuayi.cn

TS:   arr.join(", ")
来源：http://ic.jianghongdianzi.cn

Java: String.join(", ", list)
来源：http://cd.gzmigu.cn

Go:   strings.Join(strs, ", ")
来源：http://ug.hahajie.cn

Ruby: arr.join(", ")
来源：http://qt.szsharing.cn

C#:   string.Join(", ", list)
来源：http://gf.shxzukj.cn

================================================================================
来源：http://ad.wgjwhj.cn

E. 字符串处理
来源：http://ia.gzmigu.cn

================================================================================
来源：http://mq.haigaiapp.cn

[E01] 拼接字符串
来源：http://za.jianghongdianzi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ng.haigaiapp.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dc.wgjwhj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dn.huanxung.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vi.lnxyls.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dj.shxzukj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pi.9csxet.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ws.yuntaijiaju.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ox.colortex.cn

[E02] 重复字符串
来源：http://wp.shtwfgs.cn

Py:   "ab" * 3
来源：http://vf.panjiajie.cn

PHP:  str_repeat("ab", 3);
来源：http://ks.bjjhwx.cn

JS:   "ab".repeat(3)
来源：http://wg.bookmarksfly.cn

TS:   "ab".repeat(3)
来源：http://rl.colortex.cn

Java: "ab".repeat(3)
来源：http://qk.haigaiapp.cn

Go:   strings.Repeat("ab", 3)
来源：http://ma.szxytkj.cn

Ruby: "ab" * 3
来源：http://mh.wgjwhj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xs.9csxet.cn

[E03] 截取子串
来源：http://lx.huixiangedu.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://so.yuexingan06.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ut.newstarts.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ee.haigaiapp.cn

TS:   s.slice(1, 4)
来源：http://xn.nszjky.cn

Java: s.substring(1, 4)
来源：http://vj.newstarts.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nc.hnjuh.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ei.9csxet.cn

C#:   s.Substring(1, 3)
来源：http://lt.nicolike.cn

[E04] 查找子串位置
来源：http://tq.szxytkj.cn

Py:   s.find("x");  s.index("x")
来源：http://iw.jianghongdianzi.cn

PHP:  strpos($s, "x");
来源：http://ad.muxihuayi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mv.yuntaijiaju.cn

TS:   s.indexOf("x")
来源：http://ez.yuexingan06.cn

Java: s.indexOf("x")
来源：http://ey.bookmarksfly.cn

Go:   strings.Index(s, "x")
来源：http://jm.szsharing.cn

Ruby: s.index("x")
来源：http://kd.muxihuayi.cn

C#:   s.IndexOf("x")
来源：http://ao.yuntaijiaju.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://pv.9csxet.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pf.huixinmuqiang.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dt.huanxung.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ir.newstarts.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ty.bjjhwx.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sr.panjiajie.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ct.bjjhwx.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://os.521024.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tq.bookmarksfly.cn

[E06] 替换子串
来源：http://vv.gzmigu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nc.shxzskj.cn

PHP:  str_replace("a", "b", $s);
来源：http://sv.shtwfgs.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zo.shxzukj.cn

TS:   s.replaceAll("a", "b")
来源：http://mg.nszjky.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mt.nszjky.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qk.muxihuayi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vh.panjiajie.cn

C#:   s.Replace("a", "b")
来源：http://li.521024.cn

[E07] 按分隔符拆分
来源：http://pd.yuexingan06.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bx.jctech888.com.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zp.521024.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://bk.lnxyls.cn

TS:   s.split(",")
来源：http://tg.shxzukj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ff.huixinmuqiang.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://is.yuexingan06.cn

Ruby: s.split(",");  s.split
来源：http://vg.bookmarksfly.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vl.huixinmuqiang.cn

[E08] 数组按分隔符合并
来源：http://xr.colortex.cn

Py:   ",".join(items)
来源：http://bn.huixiangedu.cn

PHP:  implode(",", $items);
来源：http://pm.yuexingan06.cn

JS:   items.join(",")
来源：http://la.szsharing.cn

TS:   items.join(",")
来源：http://sw.shxzukj.cn

Java: String.join(",", items)
来源：http://qp.jctech888.com.cn

Go:   strings.Join(items, ",")
来源：http://gp.9csxet.cn

Ruby: items.join(",")
来源：http://mf.yuntaijiaju.cn

C#:   string.Join(",", items)
来源：http://ot.yuntaijiaju.cn

[E09] 去除所有空白字符
来源：http://np.hnjuh.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ao.newstarts.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://sn.bookmarksfly.cn

JS:   s.replace(/\s+/g, "")
来源：http://bm.hahajie.cn

TS:   s.replace(/\s+/g, "")
来源：http://qg.9csxet.cn

Java: s.replaceAll("\\s+", "")
来源：http://yv.chemitech.net.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ek.muxihuayi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ax.yuntaijiaju.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uy.szxytkj.cn

[E10] 左侧补零 / 定长填充
来源：http://sg.jctech888.com.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kn.yuntaijiaju.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xz.521024.cn

JS:   "7".padStart(3, "0")
来源：http://tm.gzmigu.cn

TS:   "7".padStart(3, "0")
来源：http://si.jctech888.com.cn

Java: String.format("%03d", 7)
来源：http://mu.colortex.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://mv.muxihuayi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rv.szxytkj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bi.newstarts.cn

[E11] 反转字符串
来源：http://na.9csxet.cn

Py:   s[::-1]
来源：http://kg.521024.cn

PHP:  strrev($s);
来源：http://at.hahajie.cn

JS:   [...s].reverse().join("")
来源：http://ms.szsharing.cn

TS:   [...s].reverse().join("")
来源：http://nc.shtwfgs.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://fa.shxzukj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://go.asd995.cn

Ruby: s.reverse
来源：http://ch.gzmigu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://bf.szxytkj.cn

[E12] 统计某字符出现次数
来源：http://ww.colortex.cn

Py:   s.count("a")
来源：http://ap.huixiangedu.cn

PHP:  substr_count($s, "a");
来源：http://qq.gzmigu.cn

JS:   s.split("a").length - 1
来源：http://vl.hnjuh.cn

TS:   s.split("a").length - 1
来源：http://jo.huanxung.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vi.szxytkj.cn

Go:   strings.Count(s, "a")
来源：http://hx.wgjwhj.cn

Ruby: s.count("a")
来源：http://da.haigaiapp.cn

C#:   s.Count(c => c == 'a')
来源：http://ge.yuexingan06.cn

[E13] 逐字符遍历
来源：http://lo.bjjhwx.cn

Py:   for ch in s: print(ch)
来源：http://ey.muxihuayi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://eu.asd995.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://yx.9csxet.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://zw.huixiangedu.cn


<!-- 参考信息 -->