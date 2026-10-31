代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://nc.szxytkj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hq.haigaiapp.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cd.shxzskj.cn

[D06] 数组长度
来源：http://gg.huixiangedu.cn

Py:   len(arr)
来源：http://na.shtwfgs.cn

PHP:  count($arr);
来源：http://yz.jianghongdianzi.cn

JS:   arr.length
来源：http://xq.gzmigu.cn

TS:   arr.length
来源：http://gx.jctech888.com.cn

Java: list.size();
来源：http://zz.nszjky.cn

Go:   len(arr)
来源：http://ku.szxytkj.cn

Ruby: arr.length; arr.size
来源：http://dz.bookmarksfly.cn

C#:   list.Count;
来源：http://yj.jianghongdianzi.cn

[D07] 切片 / 取子数组
来源：http://sw.521024.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vm.muxihuayi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://zz.bjjhwx.cn

JS:   arr.slice(1, 4);
来源：http://oj.521024.cn

TS:   arr.slice(1, 4);
来源：http://sr.bookmarksfly.cn

Java: list.subList(1, 4);
来源：http://fp.bookmarksfly.cn

Go:   arr[1:4]
来源：http://le.hahajie.cn

Ruby: arr[1, 3]
来源：http://pi.szsharing.cn

C#:   list.GetRange(1, 3);
来源：http://fc.bookmarksfly.cn

[D08] 合并两个数组
来源：http://de.shtwfgs.cn

Py:   a + b;  a.extend(b)
来源：http://ez.huixiangedu.cn

PHP:  array_merge($a, $b);
来源：http://si.panjiajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ri.shtwfgs.cn

TS:   [...a, ...b];
来源：http://km.muxihuayi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ot.newstarts.cn

Go:   append(a, b...)
来源：http://hz.huixinmuqiang.cn

Ruby: a + b;  a.concat(b)
来源：http://ne.huixiangedu.cn

C#:   a.Concat(b).ToList()
来源：http://ar.nszjky.cn

[D09] 排序（升序）
来源：http://gh.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://xu.shtwfgs.cn

PHP:  sort($arr);
来源：http://cg.huanxung.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://en.yuexingan06.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://km.shtwfgs.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://qt.nszjky.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xh.hnjuh.cn

Ruby: arr.sort
来源：http://au.bookmarksfly.cn

C#:   list.Sort();
来源：http://yh.huanxung.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mj.lnxyls.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://by.asd995.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zv.panjiajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dm.shxzskj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ag.chemitech.net.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ak.yuexingan06.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xm.chemitech.net.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mx.lnxyls.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qo.wgjwhj.cn

[D11] 反转数组
来源：http://pv.huixinmuqiang.cn

Py:   arr[::-1];  arr.reverse()
来源：http://je.newstarts.cn

PHP:  array_reverse($arr);
来源：http://ye.huanxung.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vc.huanxung.cn

TS:   [...arr].reverse();
来源：http://mz.shxzukj.cn

Java: Collections.reverse(list);
来源：http://ok.asd995.cn

Go:   slices.Reverse(arr)
来源：http://ir.bookmarksfly.cn

Ruby: arr.reverse
来源：http://qw.chemitech.net.cn

C#:   list.Reverse();
来源：http://vb.shxzukj.cn

[D12] 查找元素下标
来源：http://om.jianghongdianzi.cn

Py:   arr.index(x);  x in arr
来源：http://gt.bookmarksfly.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pj.9csxet.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qg.yuexingan06.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://us.bookmarksfly.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wa.shxzukj.cn

Go:   slices.Index(arr, x)
来源：http://il.haigaiapp.cn

Ruby: arr.index(x)
来源：http://do.yuexingan06.cn

C#:   list.IndexOf(x);
来源：http://vn.colortex.cn

[D13] 过滤（保留满足条件的）
来源：http://zm.nszjky.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bs.huixinmuqiang.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://io.shtwfgs.cn

JS:   arr.filter(x => x > 3)
来源：http://qx.huixiangedu.cn

TS:   arr.filter(x => x > 3)
来源：http://bv.panjiajie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lr.gzmigu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mv.asd995.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ed.szsharing.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://tn.bookmarksfly.cn

[D14] 映射转换（每个元素变形）
来源：http://tp.szsharing.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://is.9csxet.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zh.szxytkj.cn

JS:   arr.map(x => x * 2)
来源：http://ud.colortex.cn

TS:   arr.map(x => x * 2)
来源：http://ng.jianghongdianzi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://gh.hahajie.cn

Go:   // 手写循环
来源：http://xv.szxytkj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://rh.shxzukj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://bh.gzmigu.cn

[D15] 去重
来源：http://iw.hnjuh.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zt.521024.cn

PHP:  array_unique($arr);
来源：http://rm.huixinmuqiang.cn

JS:   [...new Set(arr)]
来源：http://tt.panjiajie.cn

TS:   [...new Set(arr)]
来源：http://kc.lnxyls.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xa.shxzukj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zk.nicolike.cn

Ruby: arr.uniq
来源：http://mz.9csxet.cn

C#:   list.Distinct().ToList()
来源：http://qe.9csxet.cn

[D16] 求和与平均值
来源：http://xv.huixinmuqiang.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tn.colortex.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yz.521024.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zq.huixiangedu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vl.lnxyls.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://su.bjjhwx.cn

Go:   // 手写循环累加
来源：http://at.hahajie.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ty.9csxet.cn

C#:   list.Sum();  list.Average()
来源：http://uu.muxihuayi.cn

[D17] 最大值与最小值
来源：http://me.shxzukj.cn

Py:   max(arr);  min(arr)
来源：http://sd.jianghongdianzi.cn

PHP:  max($arr);  min($arr);
来源：http://ne.huixiangedu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ih.huanxung.cn

TS:   Math.max(...arr);
来源：http://dk.yuexingan06.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://bh.lnxyls.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vm.huanxung.cn

Ruby: arr.max;  arr.min
来源：http://zi.lnxyls.cn

C#:   list.Max();  list.Min()
来源：http://il.521024.cn

[D18] 扁平化嵌套数组
来源：http://qx.yuntaijiaju.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kj.shxzskj.cn

PHP:  array_merge(...$nested);
来源：http://mt.jctech888.com.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wj.wgjwhj.cn

TS:   nested.flat();
来源：http://hl.jctech888.com.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ra.wgjwhj.cn

Go:   // 手写双层循环
来源：http://oz.wgjwhj.cn

Ruby: nested.flatten
来源：http://ra.asd995.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zh.nicolike.cn

[D19] 按字段分组
来源：http://wx.shxzskj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xe.huanxung.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ei.newstarts.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wu.wgjwhj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://yg.muxihuayi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zj.muxihuayi.cn

Go:   // 手写 map[string][]T
来源：http://tc.huixiangedu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://sn.hahajie.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ft.colortex.cn

[D20] 统计每个元素出现次数
来源：http://uz.huixinmuqiang.cn

Py:   Counter(arr)
来源：http://ta.asd995.cn

PHP:  array_count_values($arr);
来源：http://ps.nicolike.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ji.bjjhwx.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://db.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xr.muxihuayi.cn

Go:   // 手写 map[T]int
来源：http://jz.asd995.cn

Ruby: arr.tally
来源：http://es.szsharing.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://on.huixinmuqiang.cn

[D21] 判断是否包含某元素
来源：http://iw.chemitech.net.cn

Py:   x in arr
来源：http://bm.huanxung.cn

PHP:  in_array($x, $arr, true);
来源：http://cx.nicolike.cn

JS:   arr.includes(x)
来源：http://hb.colortex.cn

TS:   arr.includes(x)
来源：http://xu.huixinmuqiang.cn

Java: list.contains(x)
来源：http://ld.hnjuh.cn

Go:   slices.Contains(arr, x)
来源：http://ap.shxzukj.cn

Ruby: arr.include?(x)
来源：http://xa.gzmigu.cn

C#:   list.Contains(x)
来源：http://km.hahajie.cn

[D22] 复制数组（避免共享引用）
来源：http://ha.shtwfgs.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ng.haigaiapp.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hx.9csxet.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://oh.521024.cn

TS:   [...arr];
来源：http://yp.szxytkj.cn

Java: new ArrayList<>(list);
来源：http://cz.shtwfgs.cn

Go:   copied := append([]int(nil), arr...)
来源：http://vq.bookmarksfly.cn

Ruby: arr.dup;  arr.clone
来源：http://fm.shxzskj.cn

C#:   new List<int>(list);
来源：http://my.521024.cn

[D23] reduce 累积计算
来源：http://ko.huanxung.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sa.lnxyls.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tt.panjiajie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ma.nszjky.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://td.colortex.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://gk.colortex.cn

Go:   // 手写循环
来源：http://fo.szxytkj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://er.nszjky.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cx.szsharing.cn

[D24] 字典 / Map 基本操作
来源：http://za.hnjuh.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ze.colortex.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://um.huixinmuqiang.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fk.hahajie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ej.jctech888.com.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hw.shxzukj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://va.bookmarksfly.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xc.yuntaijiaju.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qu.jctech888.com.cn

[D25] Set 集合去重与交并差
来源：http://qe.szxytkj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ba.huixinmuqiang.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://oa.yuexingan06.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kb.muxihuayi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cs.shxzskj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jw.bjjhwx.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xl.hnjuh.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vh.newstarts.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://be.huanxung.cn

[D26] 数组转字符串
来源：http://he.jianghongdianzi.cn

Py:   ", ".join(map(str, arr))
来源：http://qb.jianghongdianzi.cn

PHP:  implode(", ", $arr);
来源：http://pk.bookmarksfly.cn

JS:   arr.join(", ")
来源：http://xi.colortex.cn

TS:   arr.join(", ")
来源：http://qb.hahajie.cn

Java: String.join(", ", list)
来源：http://nx.yuexingan06.cn

Go:   strings.Join(strs, ", ")
来源：http://ec.shxzskj.cn

Ruby: arr.join(", ")
来源：http://gd.panjiajie.cn

C#:   string.Join(", ", list)
来源：http://qr.huanxung.cn

================================================================================
来源：http://mt.nszjky.cn

E. 字符串处理
来源：http://zj.hnjuh.cn

================================================================================
来源：http://hy.yuexingan06.cn

[E01] 拼接字符串
来源：http://jp.haigaiapp.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hq.shxzukj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wx.szxytkj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hl.bookmarksfly.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qq.521024.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ft.yuexingan06.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zn.wgjwhj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wf.chemitech.net.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ph.bookmarksfly.cn

[E02] 重复字符串
来源：http://kf.colortex.cn

Py:   "ab" * 3
来源：http://ku.nszjky.cn

PHP:  str_repeat("ab", 3);
来源：http://wz.521024.cn

JS:   "ab".repeat(3)
来源：http://rp.szxytkj.cn

TS:   "ab".repeat(3)
来源：http://sc.nszjky.cn

Java: "ab".repeat(3)
来源：http://im.panjiajie.cn

Go:   strings.Repeat("ab", 3)
来源：http://ci.huanxung.cn

Ruby: "ab" * 3
来源：http://aw.asd995.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dv.lnxyls.cn

[E03] 截取子串
来源：http://xw.jianghongdianzi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xv.asd995.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tr.wgjwhj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mg.9csxet.cn

TS:   s.slice(1, 4)
来源：http://ht.shxzukj.cn

Java: s.substring(1, 4)
来源：http://ce.panjiajie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pg.chemitech.net.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ol.panjiajie.cn

C#:   s.Substring(1, 3)
来源：http://nu.yuexingan06.cn

[E04] 查找子串位置
来源：http://hu.asd995.cn

Py:   s.find("x");  s.index("x")
来源：http://gy.9csxet.cn

PHP:  strpos($s, "x");
来源：http://do.hnjuh.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pb.yuntaijiaju.cn

TS:   s.indexOf("x")
来源：http://fd.szxytkj.cn

Java: s.indexOf("x")
来源：http://al.9csxet.cn

Go:   strings.Index(s, "x")
来源：http://oj.shtwfgs.cn

Ruby: s.index("x")
来源：http://iu.yuexingan06.cn

C#:   s.IndexOf("x")
来源：http://ka.chemitech.net.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://og.asd995.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://yw.szsharing.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ih.lnxyls.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://se.haigaiapp.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://si.hnjuh.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jx.hahajie.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sy.chemitech.net.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ql.muxihuayi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://oj.wgjwhj.cn

[E06] 替换子串
来源：http://kk.nszjky.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dn.jianghongdianzi.cn

PHP:  str_replace("a", "b", $s);
来源：http://xh.bookmarksfly.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zn.yuntaijiaju.cn

TS:   s.replaceAll("a", "b")
来源：http://gs.shxzskj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bv.chemitech.net.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tz.gzmigu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nv.nicolike.cn

C#:   s.Replace("a", "b")
来源：http://zx.szxytkj.cn

[E07] 按分隔符拆分
来源：http://zr.bjjhwx.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gz.huanxung.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://sh.szsharing.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://xc.shtwfgs.cn

TS:   s.split(",")
来源：http://og.lnxyls.cn

Java: s.split(",");  s.split("\\s+")
来源：http://rc.colortex.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rn.muxihuayi.cn

Ruby: s.split(",");  s.split
来源：http://yw.jianghongdianzi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xi.asd995.cn

[E08] 数组按分隔符合并
来源：http://dw.muxihuayi.cn

Py:   ",".join(items)
来源：http://rl.huixiangedu.cn

PHP:  implode(",", $items);
来源：http://jr.bjjhwx.cn

JS:   items.join(",")
来源：http://yv.bookmarksfly.cn

TS:   items.join(",")
来源：http://xx.shxzukj.cn

Java: String.join(",", items)
来源：http://od.521024.cn

Go:   strings.Join(items, ",")
来源：http://yl.asd995.cn

Ruby: items.join(",")
来源：http://nr.szxytkj.cn

C#:   string.Join(",", items)
来源：http://lx.yuexingan06.cn

[E09] 去除所有空白字符
来源：http://ib.hnjuh.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ov.jctech888.com.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ro.bjjhwx.cn

JS:   s.replace(/\s+/g, "")
来源：http://uo.shxzskj.cn

TS:   s.replace(/\s+/g, "")
来源：http://ya.szxytkj.cn

Java: s.replaceAll("\\s+", "")
来源：http://sj.huixiangedu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://tf.chemitech.net.cn

Ruby: s.gsub(/\s+/, "")
来源：http://gr.nszjky.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sl.panjiajie.cn

[E10] 左侧补零 / 定长填充
来源：http://hq.jctech888.com.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tj.szsharing.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://uv.jctech888.com.cn

JS:   "7".padStart(3, "0")
来源：http://pg.chemitech.net.cn

TS:   "7".padStart(3, "0")
来源：http://ep.haigaiapp.cn

Java: String.format("%03d", 7)
来源：http://dx.colortex.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://um.bookmarksfly.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://id.huixiangedu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xo.huanxung.cn

[E11] 反转字符串
来源：http://gp.szxytkj.cn

Py:   s[::-1]
来源：http://iq.nicolike.cn

PHP:  strrev($s);
来源：http://fo.hnjuh.cn

JS:   [...s].reverse().join("")
来源：http://wn.huixinmuqiang.cn

TS:   [...s].reverse().join("")
来源：http://jh.wgjwhj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://iv.gzmigu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://cx.newstarts.cn

Ruby: s.reverse
来源：http://kx.9csxet.cn

C#:   new string(s.Reverse().ToArray())
来源：http://nl.chemitech.net.cn

[E12] 统计某字符出现次数
来源：http://ez.shtwfgs.cn

Py:   s.count("a")
来源：http://ku.bookmarksfly.cn

PHP:  substr_count($s, "a");
来源：http://dk.chemitech.net.cn

JS:   s.split("a").length - 1
来源：http://gt.521024.cn

TS:   s.split("a").length - 1
来源：http://bs.szsharing.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jq.panjiajie.cn


<!-- 参考信息 -->