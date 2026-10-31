代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lo.lnxyls.cn

TS:   arr.splice(0, 1);
来源：http://ha.shxzukj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lc.nszjky.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zz.colortex.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kj.shxzukj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jj.shtwfgs.cn

[D05] 访问与修改元素
来源：http://nd.huixinmuqiang.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zu.panjiajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vt.nicolike.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://on.jianghongdianzi.cn

TS:   arr[0]; arr.at(-1);
来源：http://kw.bookmarksfly.cn

Java: list.get(0); list.set(0, 9);
来源：http://mm.jctech888.com.cn

Go:   arr[0]; arr[0] = 9
来源：http://lf.chemitech.net.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ll.bjjhwx.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qk.huixiangedu.cn

[D06] 数组长度
来源：http://ah.szsharing.cn

Py:   len(arr)
来源：http://xy.haigaiapp.cn

PHP:  count($arr);
来源：http://ku.szxytkj.cn

JS:   arr.length
来源：http://ny.hnjuh.cn

TS:   arr.length
来源：http://od.colortex.cn

Java: list.size();
来源：http://vz.colortex.cn

Go:   len(arr)
来源：http://mk.jctech888.com.cn

Ruby: arr.length; arr.size
来源：http://ka.huanxung.cn

C#:   list.Count;
来源：http://cc.wgjwhj.cn

[D07] 切片 / 取子数组
来源：http://jg.szsharing.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nw.szsharing.cn

PHP:  array_slice($arr, 1, 3);
来源：http://jh.lnxyls.cn

JS:   arr.slice(1, 4);
来源：http://kr.bookmarksfly.cn

TS:   arr.slice(1, 4);
来源：http://mz.chemitech.net.cn

Java: list.subList(1, 4);
来源：http://eu.nszjky.cn

Go:   arr[1:4]
来源：http://ou.wgjwhj.cn

Ruby: arr[1, 3]
来源：http://xl.jctech888.com.cn

C#:   list.GetRange(1, 3);
来源：http://nj.gzmigu.cn

[D08] 合并两个数组
来源：http://vo.huixinmuqiang.cn

Py:   a + b;  a.extend(b)
来源：http://os.szsharing.cn

PHP:  array_merge($a, $b);
来源：http://zw.gzmigu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://pi.huanxung.cn

TS:   [...a, ...b];
来源：http://mb.chemitech.net.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ey.muxihuayi.cn

Go:   append(a, b...)
来源：http://hf.shxzukj.cn

Ruby: a + b;  a.concat(b)
来源：http://cw.yuntaijiaju.cn

C#:   a.Concat(b).ToList()
来源：http://xt.hahajie.cn

[D09] 排序（升序）
来源：http://he.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://yf.huixiangedu.cn

PHP:  sort($arr);
来源：http://ah.yuexingan06.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sx.bookmarksfly.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://qi.521024.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ir.huanxung.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xh.szsharing.cn

Ruby: arr.sort
来源：http://eh.shxzukj.cn

C#:   list.Sort();
来源：http://ei.jianghongdianzi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://xs.haigaiapp.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pk.muxihuayi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zf.huanxung.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gs.yuexingan06.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://db.szsharing.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wi.szsharing.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yi.wgjwhj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vr.yuntaijiaju.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xf.nicolike.cn

[D11] 反转数组
来源：http://qz.521024.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wa.yuntaijiaju.cn

PHP:  array_reverse($arr);
来源：http://rf.hahajie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pt.colortex.cn

TS:   [...arr].reverse();
来源：http://ro.muxihuayi.cn

Java: Collections.reverse(list);
来源：http://ni.shtwfgs.cn

Go:   slices.Reverse(arr)
来源：http://hw.panjiajie.cn

Ruby: arr.reverse
来源：http://of.nszjky.cn

C#:   list.Reverse();
来源：http://gk.shtwfgs.cn

[D12] 查找元素下标
来源：http://qn.asd995.cn

Py:   arr.index(x);  x in arr
来源：http://ob.lnxyls.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ja.shtwfgs.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tu.asd995.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dr.asd995.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zn.colortex.cn

Go:   slices.Index(arr, x)
来源：http://vj.yuntaijiaju.cn

Ruby: arr.index(x)
来源：http://ml.huanxung.cn

C#:   list.IndexOf(x);
来源：http://uv.bookmarksfly.cn

[D13] 过滤（保留满足条件的）
来源：http://pi.huixiangedu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vv.huixiangedu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vw.szxytkj.cn

JS:   arr.filter(x => x > 3)
来源：http://go.wgjwhj.cn

TS:   arr.filter(x => x > 3)
来源：http://au.szxytkj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://oo.hahajie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kx.yuntaijiaju.cn

Ruby: arr.select { |x| x > 3 }
来源：http://vi.asd995.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://zz.nicolike.cn

[D14] 映射转换（每个元素变形）
来源：http://rx.wgjwhj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qz.wgjwhj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rl.9csxet.cn

JS:   arr.map(x => x * 2)
来源：http://eq.szsharing.cn

TS:   arr.map(x => x * 2)
来源：http://ud.hnjuh.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://mz.gzmigu.cn

Go:   // 手写循环
来源：http://qm.asd995.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fp.wgjwhj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://jt.wgjwhj.cn

[D15] 去重
来源：http://xc.haigaiapp.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rm.wgjwhj.cn

PHP:  array_unique($arr);
来源：http://pq.szxytkj.cn

JS:   [...new Set(arr)]
来源：http://cq.szsharing.cn

TS:   [...new Set(arr)]
来源：http://yj.asd995.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ei.lnxyls.cn

Go:   // 用 map[T]struct{} 手写
来源：http://tn.shxzukj.cn

Ruby: arr.uniq
来源：http://xr.hnjuh.cn

C#:   list.Distinct().ToList()
来源：http://pt.yuexingan06.cn

[D16] 求和与平均值
来源：http://vn.hahajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ig.shxzskj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ld.shtwfgs.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xn.hnjuh.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gf.nszjky.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ck.9csxet.cn

Go:   // 手写循环累加
来源：http://eg.haigaiapp.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://at.panjiajie.cn

C#:   list.Sum();  list.Average()
来源：http://hz.wgjwhj.cn

[D17] 最大值与最小值
来源：http://gz.szsharing.cn

Py:   max(arr);  min(arr)
来源：http://vt.bookmarksfly.cn

PHP:  max($arr);  min($arr);
来源：http://ee.asd995.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pm.huixiangedu.cn

TS:   Math.max(...arr);
来源：http://lg.nicolike.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://af.gzmigu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://my.newstarts.cn

Ruby: arr.max;  arr.min
来源：http://ct.521024.cn

C#:   list.Max();  list.Min()
来源：http://ip.yuexingan06.cn

[D18] 扁平化嵌套数组
来源：http://kz.bookmarksfly.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fv.9csxet.cn

PHP:  array_merge(...$nested);
来源：http://la.nicolike.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mx.bookmarksfly.cn

TS:   nested.flat();
来源：http://ja.chemitech.net.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vh.szsharing.cn

Go:   // 手写双层循环
来源：http://hy.lnxyls.cn

Ruby: nested.flatten
来源：http://en.hnjuh.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ga.gzmigu.cn

[D19] 按字段分组
来源：http://pe.panjiajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ei.huanxung.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rw.9csxet.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://po.lnxyls.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xp.bookmarksfly.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kv.bjjhwx.cn

Go:   // 手写 map[string][]T
来源：http://kz.asd995.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://gh.bookmarksfly.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tx.panjiajie.cn

[D20] 统计每个元素出现次数
来源：http://wr.huixinmuqiang.cn

Py:   Counter(arr)
来源：http://vy.muxihuayi.cn

PHP:  array_count_values($arr);
来源：http://dw.szsharing.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fu.newstarts.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ik.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pq.asd995.cn

Go:   // 手写 map[T]int
来源：http://hf.yuexingan06.cn

Ruby: arr.tally
来源：http://xr.nicolike.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dx.shxzskj.cn

[D21] 判断是否包含某元素
来源：http://mm.jianghongdianzi.cn

Py:   x in arr
来源：http://zu.muxihuayi.cn

PHP:  in_array($x, $arr, true);
来源：http://dc.shtwfgs.cn

JS:   arr.includes(x)
来源：http://yr.bjjhwx.cn

TS:   arr.includes(x)
来源：http://ed.chemitech.net.cn

Java: list.contains(x)
来源：http://oz.yuexingan06.cn

Go:   slices.Contains(arr, x)
来源：http://pj.hnjuh.cn

Ruby: arr.include?(x)
来源：http://wp.9csxet.cn

C#:   list.Contains(x)
来源：http://mz.muxihuayi.cn

[D22] 复制数组（避免共享引用）
来源：http://dd.shxzskj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pr.colortex.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ar.haigaiapp.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hh.shtwfgs.cn

TS:   [...arr];
来源：http://se.muxihuayi.cn

Java: new ArrayList<>(list);
来源：http://jv.jctech888.com.cn

Go:   copied := append([]int(nil), arr...)
来源：http://rh.nszjky.cn

Ruby: arr.dup;  arr.clone
来源：http://cs.shxzukj.cn

C#:   new List<int>(list);
来源：http://bz.wgjwhj.cn

[D23] reduce 累积计算
来源：http://rv.szxytkj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hs.jctech888.com.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qb.szsharing.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nu.9csxet.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nw.9csxet.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://sb.jianghongdianzi.cn

Go:   // 手写循环
来源：http://qs.bjjhwx.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mq.colortex.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ww.nicolike.cn

[D24] 字典 / Map 基本操作
来源：http://xs.shxzukj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vg.haigaiapp.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pd.muxihuayi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jx.nszjky.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zp.bookmarksfly.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://is.jianghongdianzi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lm.nicolike.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ed.shtwfgs.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://md.shxzskj.cn

[D25] Set 集合去重与交并差
来源：http://uo.9csxet.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rb.yuexingan06.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vy.haigaiapp.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xy.521024.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dr.huixinmuqiang.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://et.huixinmuqiang.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ep.hnjuh.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jv.szsharing.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wv.muxihuayi.cn

[D26] 数组转字符串
来源：http://iy.chemitech.net.cn

Py:   ", ".join(map(str, arr))
来源：http://tx.shxzskj.cn

PHP:  implode(", ", $arr);
来源：http://wb.yuntaijiaju.cn

JS:   arr.join(", ")
来源：http://ac.yuntaijiaju.cn

TS:   arr.join(", ")
来源：http://xe.yuntaijiaju.cn

Java: String.join(", ", list)
来源：http://tg.huixiangedu.cn

Go:   strings.Join(strs, ", ")
来源：http://xr.panjiajie.cn

Ruby: arr.join(", ")
来源：http://ke.lnxyls.cn

C#:   string.Join(", ", list)
来源：http://kg.521024.cn

================================================================================
来源：http://ff.jianghongdianzi.cn

E. 字符串处理
来源：http://cn.shxzskj.cn

================================================================================
来源：http://bv.wgjwhj.cn

[E01] 拼接字符串
来源：http://sv.bjjhwx.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sf.nicolike.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sp.jctech888.com.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ug.bookmarksfly.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yk.9csxet.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vg.colortex.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gg.hnjuh.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ns.hahajie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zg.newstarts.cn

[E02] 重复字符串
来源：http://lr.panjiajie.cn

Py:   "ab" * 3
来源：http://fq.hahajie.cn

PHP:  str_repeat("ab", 3);
来源：http://bn.huanxung.cn

JS:   "ab".repeat(3)
来源：http://iu.gzmigu.cn

TS:   "ab".repeat(3)
来源：http://ds.hahajie.cn

Java: "ab".repeat(3)
来源：http://ro.jctech888.com.cn

Go:   strings.Repeat("ab", 3)
来源：http://hr.shtwfgs.cn

Ruby: "ab" * 3
来源：http://ar.asd995.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wo.wgjwhj.cn

[E03] 截取子串
来源：http://xm.shxzukj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://aa.shxzskj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://sk.521024.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fj.haigaiapp.cn

TS:   s.slice(1, 4)
来源：http://pg.chemitech.net.cn

Java: s.substring(1, 4)
来源：http://wy.gzmigu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hd.hahajie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://nz.panjiajie.cn

C#:   s.Substring(1, 3)
来源：http://rz.haigaiapp.cn

[E04] 查找子串位置
来源：http://zx.huixinmuqiang.cn

Py:   s.find("x");  s.index("x")
来源：http://gt.nszjky.cn

PHP:  strpos($s, "x");
来源：http://kj.colortex.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sy.yuntaijiaju.cn

TS:   s.indexOf("x")
来源：http://xd.haigaiapp.cn

Java: s.indexOf("x")
来源：http://cv.hnjuh.cn

Go:   strings.Index(s, "x")
来源：http://dy.shxzukj.cn

Ruby: s.index("x")
来源：http://yo.szsharing.cn

C#:   s.IndexOf("x")
来源：http://ij.jianghongdianzi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://vl.shtwfgs.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bg.shxzukj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pj.colortex.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ju.lnxyls.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://dr.yuntaijiaju.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ej.huixiangedu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gi.521024.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mk.newstarts.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qw.huixiangedu.cn

[E06] 替换子串
来源：http://aj.gzmigu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://uh.bookmarksfly.cn

PHP:  str_replace("a", "b", $s);
来源：http://jk.panjiajie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cb.huixinmuqiang.cn

TS:   s.replaceAll("a", "b")
来源：http://mj.nszjky.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ux.9csxet.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pm.shxzskj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://un.shxzskj.cn

C#:   s.Replace("a", "b")
来源：http://sk.newstarts.cn

[E07] 按分隔符拆分
来源：http://ca.asd995.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://is.shtwfgs.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jr.yuntaijiaju.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://do.szxytkj.cn

TS:   s.split(",")
来源：http://cm.gzmigu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zo.521024.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://eb.bjjhwx.cn

Ruby: s.split(",");  s.split
来源：http://iy.nszjky.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hu.haigaiapp.cn

[E08] 数组按分隔符合并
来源：http://yx.chemitech.net.cn

Py:   ",".join(items)
来源：http://nv.panjiajie.cn

PHP:  implode(",", $items);
来源：http://qf.shtwfgs.cn

JS:   items.join(",")
来源：http://di.521024.cn

TS:   items.join(",")
来源：http://ul.hahajie.cn

Java: String.join(",", items)
来源：http://pj.yuntaijiaju.cn

Go:   strings.Join(items, ",")
来源：http://ao.yuntaijiaju.cn

Ruby: items.join(",")
来源：http://rr.bjjhwx.cn

C#:   string.Join(",", items)
来源：http://dr.521024.cn

[E09] 去除所有空白字符
来源：http://cu.yuexingan06.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ba.yuexingan06.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mi.haigaiapp.cn

JS:   s.replace(/\s+/g, "")
来源：http://yt.muxihuayi.cn

TS:   s.replace(/\s+/g, "")
来源：http://tw.muxihuayi.cn

Java: s.replaceAll("\\s+", "")
来源：http://gz.huixiangedu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://oh.huanxung.cn

Ruby: s.gsub(/\s+/, "")
来源：http://kz.bjjhwx.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uh.gzmigu.cn

[E10] 左侧补零 / 定长填充
来源：http://gc.bjjhwx.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zy.panjiajie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://om.jianghongdianzi.cn

JS:   "7".padStart(3, "0")
来源：http://hn.nszjky.cn

TS:   "7".padStart(3, "0")
来源：http://am.bjjhwx.cn

Java: String.format("%03d", 7)
来源：http://wx.newstarts.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://nk.gzmigu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wp.szxytkj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://uh.szxytkj.cn

[E11] 反转字符串
来源：http://st.colortex.cn

Py:   s[::-1]
来源：http://ez.bjjhwx.cn

PHP:  strrev($s);
来源：http://hu.panjiajie.cn


<!-- 参考信息 -->