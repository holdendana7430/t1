代发 wailian999

C#:   list.Insert(0, 0);
来源：http://qw.yuntaijiaju.cn

[D04] 删除元素
来源：http://rs.bjjhwx.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pd.yuexingan06.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xn.hahajie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zp.nszjky.cn

TS:   arr.splice(0, 1);
来源：http://ma.bookmarksfly.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gc.lnxyls.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dx.shtwfgs.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qi.szsharing.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cg.jctech888.com.cn

[D05] 访问与修改元素
来源：http://nd.szsharing.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qp.shxzskj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vg.muxihuayi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fo.asd995.cn

TS:   arr[0]; arr.at(-1);
来源：http://wz.muxihuayi.cn

Java: list.get(0); list.set(0, 9);
来源：http://gt.jianghongdianzi.cn

Go:   arr[0]; arr[0] = 9
来源：http://xa.newstarts.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wj.521024.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zh.521024.cn

[D06] 数组长度
来源：http://ei.newstarts.cn

Py:   len(arr)
来源：http://yt.521024.cn

PHP:  count($arr);
来源：http://hv.shxzukj.cn

JS:   arr.length
来源：http://xv.yuntaijiaju.cn

TS:   arr.length
来源：http://ri.szsharing.cn

Java: list.size();
来源：http://mo.521024.cn

Go:   len(arr)
来源：http://pg.gzmigu.cn

Ruby: arr.length; arr.size
来源：http://ek.wgjwhj.cn

C#:   list.Count;
来源：http://cg.haigaiapp.cn

[D07] 切片 / 取子数组
来源：http://hb.yuexingan06.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zq.colortex.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qa.huixinmuqiang.cn

JS:   arr.slice(1, 4);
来源：http://ze.lnxyls.cn

TS:   arr.slice(1, 4);
来源：http://fr.hnjuh.cn

Java: list.subList(1, 4);
来源：http://sw.szxytkj.cn

Go:   arr[1:4]
来源：http://qa.muxihuayi.cn

Ruby: arr[1, 3]
来源：http://vw.haigaiapp.cn

C#:   list.GetRange(1, 3);
来源：http://dl.muxihuayi.cn

[D08] 合并两个数组
来源：http://en.yuntaijiaju.cn

Py:   a + b;  a.extend(b)
来源：http://xa.jianghongdianzi.cn

PHP:  array_merge($a, $b);
来源：http://eg.wgjwhj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://re.bjjhwx.cn

TS:   [...a, ...b];
来源：http://rb.gzmigu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xx.521024.cn

Go:   append(a, b...)
来源：http://ju.huixinmuqiang.cn

Ruby: a + b;  a.concat(b)
来源：http://ht.hnjuh.cn

C#:   a.Concat(b).ToList()
来源：http://ij.szsharing.cn

[D09] 排序（升序）
来源：http://zb.jianghongdianzi.cn

Py:   sorted(arr);  arr.sort()
来源：http://xe.nszjky.cn

PHP:  sort($arr);
来源：http://zf.huixiangedu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ca.shxzukj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://us.yuntaijiaju.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://uu.asd995.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ti.asd995.cn

Ruby: arr.sort
来源：http://of.wgjwhj.cn

C#:   list.Sort();
来源：http://up.huixinmuqiang.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qi.gzmigu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ye.haigaiapp.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ej.asd995.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://he.gzmigu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://aa.yuexingan06.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vm.huanxung.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xo.chemitech.net.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jt.nszjky.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ys.huanxung.cn

[D11] 反转数组
来源：http://yk.gzmigu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://my.nicolike.cn

PHP:  array_reverse($arr);
来源：http://aa.bjjhwx.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rh.newstarts.cn

TS:   [...arr].reverse();
来源：http://lg.colortex.cn

Java: Collections.reverse(list);
来源：http://nk.haigaiapp.cn

Go:   slices.Reverse(arr)
来源：http://gq.asd995.cn

Ruby: arr.reverse
来源：http://tu.chemitech.net.cn

C#:   list.Reverse();
来源：http://jw.shtwfgs.cn

[D12] 查找元素下标
来源：http://ti.shxzukj.cn

Py:   arr.index(x);  x in arr
来源：http://pz.asd995.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gv.9csxet.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uq.bjjhwx.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ru.gzmigu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zf.chemitech.net.cn

Go:   slices.Index(arr, x)
来源：http://zi.panjiajie.cn

Ruby: arr.index(x)
来源：http://zm.huixiangedu.cn

C#:   list.IndexOf(x);
来源：http://tg.hahajie.cn

[D13] 过滤（保留满足条件的）
来源：http://jj.yuexingan06.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dl.huixinmuqiang.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://oz.hnjuh.cn

JS:   arr.filter(x => x > 3)
来源：http://mo.jianghongdianzi.cn

TS:   arr.filter(x => x > 3)
来源：http://ly.hnjuh.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://by.szxytkj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lr.wgjwhj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://kr.lnxyls.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://xl.panjiajie.cn

[D14] 映射转换（每个元素变形）
来源：http://hc.colortex.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vg.asd995.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lr.nicolike.cn

JS:   arr.map(x => x * 2)
来源：http://ky.szsharing.cn

TS:   arr.map(x => x * 2)
来源：http://ol.hahajie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ca.shxzskj.cn

Go:   // 手写循环
来源：http://mo.shtwfgs.cn

Ruby: arr.map { |x| x * 2 }
来源：http://mm.chemitech.net.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://vq.haigaiapp.cn

[D15] 去重
来源：http://wx.newstarts.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ub.huixiangedu.cn

PHP:  array_unique($arr);
来源：http://zn.haigaiapp.cn

JS:   [...new Set(arr)]
来源：http://dr.bookmarksfly.cn

TS:   [...new Set(arr)]
来源：http://rz.muxihuayi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nz.gzmigu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://bf.shxzukj.cn

Ruby: arr.uniq
来源：http://yi.nszjky.cn

C#:   list.Distinct().ToList()
来源：http://ht.gzmigu.cn

[D16] 求和与平均值
来源：http://yo.newstarts.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fl.jctech888.com.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://an.szsharing.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ot.newstarts.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dh.hahajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wh.asd995.cn

Go:   // 手写循环累加
来源：http://cs.bookmarksfly.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pf.shxzskj.cn

C#:   list.Sum();  list.Average()
来源：http://ji.hahajie.cn

[D17] 最大值与最小值
来源：http://ff.shxzukj.cn

Py:   max(arr);  min(arr)
来源：http://al.asd995.cn

PHP:  max($arr);  min($arr);
来源：http://xp.asd995.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wo.chemitech.net.cn

TS:   Math.max(...arr);
来源：http://el.chemitech.net.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ab.bjjhwx.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zw.wgjwhj.cn

Ruby: arr.max;  arr.min
来源：http://cm.yuntaijiaju.cn

C#:   list.Max();  list.Min()
来源：http://zu.wgjwhj.cn

[D18] 扁平化嵌套数组
来源：http://sr.hnjuh.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xy.shxzskj.cn

PHP:  array_merge(...$nested);
来源：http://mr.haigaiapp.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ua.huixiangedu.cn

TS:   nested.flat();
来源：http://lg.bookmarksfly.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ao.yuntaijiaju.cn

Go:   // 手写双层循环
来源：http://gq.shtwfgs.cn

Ruby: nested.flatten
来源：http://tf.szsharing.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://jz.colortex.cn

[D19] 按字段分组
来源：http://qn.asd995.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qn.bjjhwx.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nc.nszjky.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://sj.hnjuh.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://yo.hahajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xw.huixinmuqiang.cn

Go:   // 手写 map[string][]T
来源：http://vc.muxihuayi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://bk.huixiangedu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mt.gzmigu.cn

[D20] 统计每个元素出现次数
来源：http://sk.wgjwhj.cn

Py:   Counter(arr)
来源：http://lq.gzmigu.cn

PHP:  array_count_values($arr);
来源：http://vt.shxzskj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oq.yuexingan06.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wt.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wp.hahajie.cn

Go:   // 手写 map[T]int
来源：http://lv.gzmigu.cn

Ruby: arr.tally
来源：http://ee.shxzskj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tk.szsharing.cn

[D21] 判断是否包含某元素
来源：http://oq.huixinmuqiang.cn

Py:   x in arr
来源：http://wl.nicolike.cn

PHP:  in_array($x, $arr, true);
来源：http://rp.wgjwhj.cn

JS:   arr.includes(x)
来源：http://sz.hnjuh.cn

TS:   arr.includes(x)
来源：http://ls.hnjuh.cn

Java: list.contains(x)
来源：http://yg.newstarts.cn

Go:   slices.Contains(arr, x)
来源：http://pz.szxytkj.cn

Ruby: arr.include?(x)
来源：http://fz.haigaiapp.cn

C#:   list.Contains(x)
来源：http://yj.szxytkj.cn

[D22] 复制数组（避免共享引用）
来源：http://nc.haigaiapp.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pq.yuexingan06.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qx.hnjuh.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xl.jctech888.com.cn

TS:   [...arr];
来源：http://fz.hnjuh.cn

Java: new ArrayList<>(list);
来源：http://to.9csxet.cn

Go:   copied := append([]int(nil), arr...)
来源：http://zx.huixiangedu.cn

Ruby: arr.dup;  arr.clone
来源：http://xj.hnjuh.cn

C#:   new List<int>(list);
来源：http://qv.chemitech.net.cn

[D23] reduce 累积计算
来源：http://wq.lnxyls.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ta.nicolike.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://in.hahajie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://al.nicolike.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ow.hahajie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://zp.newstarts.cn

Go:   // 手写循环
来源：http://dv.lnxyls.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wu.panjiajie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://of.colortex.cn

[D24] 字典 / Map 基本操作
来源：http://ow.521024.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vl.shxzskj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mr.haigaiapp.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://iy.wgjwhj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ua.asd995.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nk.hnjuh.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yx.521024.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://il.panjiajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ey.lnxyls.cn

[D25] Set 集合去重与交并差
来源：http://ij.yuexingan06.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tt.huixiangedu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xp.huanxung.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ng.huanxung.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://au.huanxung.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bz.9csxet.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bx.bookmarksfly.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bd.shtwfgs.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fr.yuntaijiaju.cn

[D26] 数组转字符串
来源：http://ub.yuexingan06.cn

Py:   ", ".join(map(str, arr))
来源：http://it.huixinmuqiang.cn

PHP:  implode(", ", $arr);
来源：http://se.huanxung.cn

JS:   arr.join(", ")
来源：http://ms.huixinmuqiang.cn

TS:   arr.join(", ")
来源：http://ns.shxzukj.cn

Java: String.join(", ", list)
来源：http://jl.jctech888.com.cn

Go:   strings.Join(strs, ", ")
来源：http://hr.shxzskj.cn

Ruby: arr.join(", ")
来源：http://pe.yuexingan06.cn

C#:   string.Join(", ", list)
来源：http://je.muxihuayi.cn

================================================================================
来源：http://lw.jianghongdianzi.cn

E. 字符串处理
来源：http://mh.jctech888.com.cn

================================================================================
来源：http://nf.haigaiapp.cn

[E01] 拼接字符串
来源：http://xt.nszjky.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ul.nszjky.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xp.nszjky.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gs.newstarts.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xe.jianghongdianzi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xb.nszjky.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uz.yuexingan06.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://iy.bookmarksfly.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://uh.szxytkj.cn

[E02] 重复字符串
来源：http://bs.wgjwhj.cn

Py:   "ab" * 3
来源：http://uq.huixinmuqiang.cn

PHP:  str_repeat("ab", 3);
来源：http://qu.huixiangedu.cn

JS:   "ab".repeat(3)
来源：http://bs.szsharing.cn

TS:   "ab".repeat(3)
来源：http://wq.szxytkj.cn

Java: "ab".repeat(3)
来源：http://gs.bjjhwx.cn

Go:   strings.Repeat("ab", 3)
来源：http://lw.huanxung.cn

Ruby: "ab" * 3
来源：http://ek.lnxyls.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cl.wgjwhj.cn

[E03] 截取子串
来源：http://tn.muxihuayi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wv.hnjuh.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://la.nicolike.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ke.szxytkj.cn

TS:   s.slice(1, 4)
来源：http://ow.szsharing.cn

Java: s.substring(1, 4)
来源：http://ly.jctech888.com.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://eh.newstarts.cn

Ruby: s[1, 3];  s[1..3]
来源：http://tr.jctech888.com.cn

C#:   s.Substring(1, 3)
来源：http://gp.jianghongdianzi.cn

[E04] 查找子串位置
来源：http://eq.hahajie.cn

Py:   s.find("x");  s.index("x")
来源：http://uy.wgjwhj.cn

PHP:  strpos($s, "x");
来源：http://hs.hahajie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cv.shtwfgs.cn

TS:   s.indexOf("x")
来源：http://cu.jianghongdianzi.cn

Java: s.indexOf("x")
来源：http://hf.hahajie.cn

Go:   strings.Index(s, "x")
来源：http://qq.colortex.cn

Ruby: s.index("x")
来源：http://av.bookmarksfly.cn

C#:   s.IndexOf("x")
来源：http://ax.haigaiapp.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xg.jianghongdianzi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://km.hahajie.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pe.hahajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ki.colortex.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://op.jctech888.com.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xy.bjjhwx.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mt.hahajie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yx.shtwfgs.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bf.haigaiapp.cn

[E06] 替换子串
来源：http://zm.asd995.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kx.bjjhwx.cn

PHP:  str_replace("a", "b", $s);
来源：http://ky.huixinmuqiang.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nj.szxytkj.cn

TS:   s.replaceAll("a", "b")
来源：http://xj.newstarts.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lt.hnjuh.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://se.huixiangedu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vz.chemitech.net.cn

C#:   s.Replace("a", "b")
来源：http://pw.panjiajie.cn

[E07] 按分隔符拆分
来源：http://gs.shxzukj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dy.newstarts.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jp.szsharing.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://jd.huixiangedu.cn

TS:   s.split(",")
来源：http://in.chemitech.net.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xd.wgjwhj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bp.wgjwhj.cn

Ruby: s.split(",");  s.split
来源：http://cl.521024.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tb.lnxyls.cn

[E08] 数组按分隔符合并
来源：http://mc.shxzukj.cn

Py:   ",".join(items)
来源：http://ex.yuexingan06.cn

PHP:  implode(",", $items);
来源：http://hz.chemitech.net.cn

JS:   items.join(",")
来源：http://dr.521024.cn

TS:   items.join(",")
来源：http://mu.yuexingan06.cn

Java: String.join(",", items)
来源：http://rt.9csxet.cn

Go:   strings.Join(items, ",")
来源：http://ah.colortex.cn

Ruby: items.join(",")
来源：http://ao.panjiajie.cn

C#:   string.Join(",", items)
来源：http://ri.jianghongdianzi.cn

[E09] 去除所有空白字符
来源：http://wh.szxytkj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ll.jianghongdianzi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ah.jctech888.com.cn

JS:   s.replace(/\s+/g, "")
来源：http://pr.9csxet.cn

TS:   s.replace(/\s+/g, "")
来源：http://jk.panjiajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://fh.shxzskj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ni.bjjhwx.cn

Ruby: s.gsub(/\s+/, "")
来源：http://zs.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cc.panjiajie.cn

[E10] 左侧补零 / 定长填充
来源：http://gs.shxzukj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ks.shxzukj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ku.huanxung.cn

JS:   "7".padStart(3, "0")
来源：http://vj.hahajie.cn

TS:   "7".padStart(3, "0")
来源：http://np.yuntaijiaju.cn

Java: String.format("%03d", 7)
来源：http://gb.bookmarksfly.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://yr.huixinmuqiang.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cw.huanxung.cn


<!-- 参考信息 -->