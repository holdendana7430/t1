代发 wailian999

C#:   list.Insert(0, 0);
来源：http://ae.yuexingan06.cn

[D04] 删除元素
来源：http://yb.hnjuh.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vf.muxihuayi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ut.hnjuh.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ed.yuntaijiaju.cn

TS:   arr.splice(0, 1);
来源：http://dy.newstarts.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ed.huixiangedu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pi.chemitech.net.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wa.hnjuh.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://oo.hahajie.cn

[D05] 访问与修改元素
来源：http://hr.shxzskj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nr.lnxyls.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://oy.haigaiapp.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xh.jianghongdianzi.cn

TS:   arr[0]; arr.at(-1);
来源：http://ri.jctech888.com.cn

Java: list.get(0); list.set(0, 9);
来源：http://rk.nszjky.cn

Go:   arr[0]; arr[0] = 9
来源：http://ze.nicolike.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nk.9csxet.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vr.jctech888.com.cn

[D06] 数组长度
来源：http://al.shxzskj.cn

Py:   len(arr)
来源：http://xf.huanxung.cn

PHP:  count($arr);
来源：http://na.asd995.cn

JS:   arr.length
来源：http://ec.huanxung.cn

TS:   arr.length
来源：http://rn.shxzskj.cn

Java: list.size();
来源：http://jk.yuntaijiaju.cn

Go:   len(arr)
来源：http://la.jctech888.com.cn

Ruby: arr.length; arr.size
来源：http://yh.wgjwhj.cn

C#:   list.Count;
来源：http://vu.bjjhwx.cn

[D07] 切片 / 取子数组
来源：http://sa.shxzskj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jo.hahajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://wk.yuexingan06.cn

JS:   arr.slice(1, 4);
来源：http://ut.asd995.cn

TS:   arr.slice(1, 4);
来源：http://ck.asd995.cn

Java: list.subList(1, 4);
来源：http://dl.szxytkj.cn

Go:   arr[1:4]
来源：http://vj.bjjhwx.cn

Ruby: arr[1, 3]
来源：http://bb.jianghongdianzi.cn

C#:   list.GetRange(1, 3);
来源：http://gl.muxihuayi.cn

[D08] 合并两个数组
来源：http://hu.szsharing.cn

Py:   a + b;  a.extend(b)
来源：http://tg.shxzukj.cn

PHP:  array_merge($a, $b);
来源：http://yh.newstarts.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://mf.yuntaijiaju.cn

TS:   [...a, ...b];
来源：http://hk.haigaiapp.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ae.bjjhwx.cn

Go:   append(a, b...)
来源：http://vr.colortex.cn

Ruby: a + b;  a.concat(b)
来源：http://pm.nicolike.cn

C#:   a.Concat(b).ToList()
来源：http://ly.9csxet.cn

[D09] 排序（升序）
来源：http://rz.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://wt.shtwfgs.cn

PHP:  sort($arr);
来源：http://es.newstarts.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ld.szxytkj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://in.panjiajie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://pp.shxzukj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://iy.asd995.cn

Ruby: arr.sort
来源：http://ft.shxzskj.cn

C#:   list.Sort();
来源：http://vr.huixiangedu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://nk.yuntaijiaju.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vl.haigaiapp.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oa.shxzukj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hh.haigaiapp.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ef.szxytkj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://sm.muxihuayi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ta.nicolike.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vg.hahajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://sa.muxihuayi.cn

[D11] 反转数组
来源：http://uz.huanxung.cn

Py:   arr[::-1];  arr.reverse()
来源：http://si.bookmarksfly.cn

PHP:  array_reverse($arr);
来源：http://wg.bookmarksfly.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xk.nszjky.cn

TS:   [...arr].reverse();
来源：http://ec.colortex.cn

Java: Collections.reverse(list);
来源：http://ap.chemitech.net.cn

Go:   slices.Reverse(arr)
来源：http://cb.yuexingan06.cn

Ruby: arr.reverse
来源：http://ke.yuexingan06.cn

C#:   list.Reverse();
来源：http://aw.szsharing.cn

[D12] 查找元素下标
来源：http://cv.shtwfgs.cn

Py:   arr.index(x);  x in arr
来源：http://pa.haigaiapp.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ol.bookmarksfly.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rn.shtwfgs.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qs.szsharing.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gq.huixiangedu.cn

Go:   slices.Index(arr, x)
来源：http://sm.chemitech.net.cn

Ruby: arr.index(x)
来源：http://be.newstarts.cn

C#:   list.IndexOf(x);
来源：http://dd.szsharing.cn

[D13] 过滤（保留满足条件的）
来源：http://jc.asd995.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xm.shtwfgs.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qu.nicolike.cn

JS:   arr.filter(x => x > 3)
来源：http://em.shxzukj.cn

TS:   arr.filter(x => x > 3)
来源：http://hh.nszjky.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://as.huixinmuqiang.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vz.521024.cn

Ruby: arr.select { |x| x > 3 }
来源：http://tk.shxzukj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://pg.nicolike.cn

[D14] 映射转换（每个元素变形）
来源：http://yq.hnjuh.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gk.huixiangedu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://io.shxzukj.cn

JS:   arr.map(x => x * 2)
来源：http://nn.chemitech.net.cn

TS:   arr.map(x => x * 2)
来源：http://ms.jianghongdianzi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://lg.bjjhwx.cn

Go:   // 手写循环
来源：http://ca.shxzskj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://th.panjiajie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://tn.chemitech.net.cn

[D15] 去重
来源：http://ln.huixinmuqiang.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yx.szxytkj.cn

PHP:  array_unique($arr);
来源：http://vc.nicolike.cn

JS:   [...new Set(arr)]
来源：http://nc.huixinmuqiang.cn

TS:   [...new Set(arr)]
来源：http://nq.panjiajie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fh.hahajie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://jk.hahajie.cn

Ruby: arr.uniq
来源：http://xj.muxihuayi.cn

C#:   list.Distinct().ToList()
来源：http://zq.szxytkj.cn

[D16] 求和与平均值
来源：http://cu.huixinmuqiang.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qo.newstarts.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pi.521024.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lm.jianghongdianzi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ds.bjjhwx.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kv.huixiangedu.cn

Go:   // 手写循环累加
来源：http://mq.huixiangedu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ee.shxzskj.cn

C#:   list.Sum();  list.Average()
来源：http://to.nszjky.cn

[D17] 最大值与最小值
来源：http://gg.muxihuayi.cn

Py:   max(arr);  min(arr)
来源：http://zh.huixinmuqiang.cn

PHP:  max($arr);  min($arr);
来源：http://as.bookmarksfly.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ez.szsharing.cn

TS:   Math.max(...arr);
来源：http://ve.jianghongdianzi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://cp.jctech888.com.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ld.bjjhwx.cn

Ruby: arr.max;  arr.min
来源：http://mh.bjjhwx.cn

C#:   list.Max();  list.Min()
来源：http://lt.asd995.cn

[D18] 扁平化嵌套数组
来源：http://qw.nszjky.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yh.9csxet.cn

PHP:  array_merge(...$nested);
来源：http://mg.nszjky.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://og.yuntaijiaju.cn

TS:   nested.flat();
来源：http://uh.nicolike.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gv.panjiajie.cn

Go:   // 手写双层循环
来源：http://cb.bjjhwx.cn

Ruby: nested.flatten
来源：http://ev.gzmigu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zj.newstarts.cn

[D19] 按字段分组
来源：http://qi.bjjhwx.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zw.nszjky.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://an.shxzskj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hj.9csxet.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ht.huixinmuqiang.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mb.bookmarksfly.cn

Go:   // 手写 map[string][]T
来源：http://dx.panjiajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://wl.shxzukj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nz.yuexingan06.cn

[D20] 统计每个元素出现次数
来源：http://iw.shtwfgs.cn

Py:   Counter(arr)
来源：http://cp.chemitech.net.cn

PHP:  array_count_values($arr);
来源：http://ku.shtwfgs.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zr.lnxyls.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kl.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dq.huanxung.cn

Go:   // 手写 map[T]int
来源：http://tj.asd995.cn

Ruby: arr.tally
来源：http://hw.huixiangedu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zb.haigaiapp.cn

[D21] 判断是否包含某元素
来源：http://xe.muxihuayi.cn

Py:   x in arr
来源：http://wb.521024.cn

PHP:  in_array($x, $arr, true);
来源：http://zu.szxytkj.cn

JS:   arr.includes(x)
来源：http://nc.haigaiapp.cn

TS:   arr.includes(x)
来源：http://nb.hahajie.cn

Java: list.contains(x)
来源：http://hx.bjjhwx.cn

Go:   slices.Contains(arr, x)
来源：http://zq.colortex.cn

Ruby: arr.include?(x)
来源：http://ww.nszjky.cn

C#:   list.Contains(x)
来源：http://wu.jctech888.com.cn

[D22] 复制数组（避免共享引用）
来源：http://po.lnxyls.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kk.chemitech.net.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://am.shtwfgs.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yi.huanxung.cn

TS:   [...arr];
来源：http://jh.jctech888.com.cn

Java: new ArrayList<>(list);
来源：http://ki.9csxet.cn

Go:   copied := append([]int(nil), arr...)
来源：http://uj.huixiangedu.cn

Ruby: arr.dup;  arr.clone
来源：http://vv.panjiajie.cn

C#:   new List<int>(list);
来源：http://hv.nicolike.cn

[D23] reduce 累积计算
来源：http://lj.colortex.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bq.bookmarksfly.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ei.hnjuh.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://be.lnxyls.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ia.jctech888.com.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xl.huixiangedu.cn

Go:   // 手写循环
来源：http://bw.colortex.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ue.shxzukj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mh.lnxyls.cn

[D24] 字典 / Map 基本操作
来源：http://vi.asd995.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ye.hahajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://py.yuntaijiaju.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xk.bjjhwx.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://is.bjjhwx.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://at.newstarts.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dz.yuexingan06.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ck.szxytkj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://eq.newstarts.cn

[D25] Set 集合去重与交并差
来源：http://el.jctech888.com.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qv.9csxet.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qr.huixiangedu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nn.asd995.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://be.jianghongdianzi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ac.colortex.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vy.panjiajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gg.yuntaijiaju.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qs.newstarts.cn

[D26] 数组转字符串
来源：http://xt.wgjwhj.cn

Py:   ", ".join(map(str, arr))
来源：http://ht.asd995.cn

PHP:  implode(", ", $arr);
来源：http://sy.shxzukj.cn

JS:   arr.join(", ")
来源：http://gm.yuntaijiaju.cn

TS:   arr.join(", ")
来源：http://si.muxihuayi.cn

Java: String.join(", ", list)
来源：http://hm.haigaiapp.cn

Go:   strings.Join(strs, ", ")
来源：http://qp.wgjwhj.cn

Ruby: arr.join(", ")
来源：http://vh.colortex.cn

C#:   string.Join(", ", list)
来源：http://hp.jctech888.com.cn

================================================================================
来源：http://dy.yuntaijiaju.cn

E. 字符串处理
来源：http://zj.jctech888.com.cn

================================================================================
来源：http://fw.shxzukj.cn

[E01] 拼接字符串
来源：http://bl.huixiangedu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://by.muxihuayi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yt.shtwfgs.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cs.hahajie.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yn.jctech888.com.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://px.newstarts.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ke.shxzskj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jp.panjiajie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bm.521024.cn

[E02] 重复字符串
来源：http://rk.huixinmuqiang.cn

Py:   "ab" * 3
来源：http://um.shtwfgs.cn

PHP:  str_repeat("ab", 3);
来源：http://zs.chemitech.net.cn

JS:   "ab".repeat(3)
来源：http://gs.colortex.cn

TS:   "ab".repeat(3)
来源：http://ab.shtwfgs.cn

Java: "ab".repeat(3)
来源：http://aw.chemitech.net.cn

Go:   strings.Repeat("ab", 3)
来源：http://ct.haigaiapp.cn

Ruby: "ab" * 3
来源：http://ls.haigaiapp.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cy.9csxet.cn

[E03] 截取子串
来源：http://zb.huixinmuqiang.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nv.bookmarksfly.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zl.jctech888.com.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://li.hahajie.cn

TS:   s.slice(1, 4)
来源：http://kn.jctech888.com.cn

Java: s.substring(1, 4)
来源：http://hu.yuntaijiaju.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fv.gzmigu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://bt.shtwfgs.cn

C#:   s.Substring(1, 3)
来源：http://fc.chemitech.net.cn

[E04] 查找子串位置
来源：http://nb.wgjwhj.cn

Py:   s.find("x");  s.index("x")
来源：http://mf.jctech888.com.cn

PHP:  strpos($s, "x");
来源：http://dr.jctech888.com.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tw.gzmigu.cn

TS:   s.indexOf("x")
来源：http://ri.9csxet.cn

Java: s.indexOf("x")
来源：http://od.nszjky.cn

Go:   strings.Index(s, "x")
来源：http://il.hahajie.cn

Ruby: s.index("x")
来源：http://ep.panjiajie.cn

C#:   s.IndexOf("x")
来源：http://ob.521024.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://sy.hnjuh.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rl.hnjuh.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://oy.521024.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://iz.newstarts.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://yb.asd995.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xy.9csxet.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://za.9csxet.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://os.chemitech.net.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ko.chemitech.net.cn

[E06] 替换子串
来源：http://ig.jianghongdianzi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wj.hnjuh.cn

PHP:  str_replace("a", "b", $s);
来源：http://qq.szsharing.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ns.szsharing.cn

TS:   s.replaceAll("a", "b")
来源：http://nf.newstarts.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fj.shtwfgs.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://it.chemitech.net.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ue.9csxet.cn

C#:   s.Replace("a", "b")
来源：http://nf.lnxyls.cn

[E07] 按分隔符拆分
来源：http://co.nicolike.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://uj.asd995.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hg.haigaiapp.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://je.bookmarksfly.cn

TS:   s.split(",")
来源：http://hn.jctech888.com.cn

Java: s.split(",");  s.split("\\s+")
来源：http://em.shxzskj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yf.colortex.cn

Ruby: s.split(",");  s.split
来源：http://jc.chemitech.net.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bt.huixiangedu.cn

[E08] 数组按分隔符合并
来源：http://tm.nszjky.cn

Py:   ",".join(items)
来源：http://on.chemitech.net.cn

PHP:  implode(",", $items);
来源：http://wv.521024.cn

JS:   items.join(",")
来源：http://zw.hahajie.cn

TS:   items.join(",")
来源：http://wg.jctech888.com.cn

Java: String.join(",", items)
来源：http://ty.szsharing.cn

Go:   strings.Join(items, ",")
来源：http://cg.shtwfgs.cn

Ruby: items.join(",")
来源：http://ix.colortex.cn

C#:   string.Join(",", items)
来源：http://ha.shtwfgs.cn

[E09] 去除所有空白字符
来源：http://ze.shtwfgs.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://re.shtwfgs.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pw.szsharing.cn

JS:   s.replace(/\s+/g, "")
来源：http://ee.9csxet.cn

TS:   s.replace(/\s+/g, "")
来源：http://vx.shtwfgs.cn

Java: s.replaceAll("\\s+", "")
来源：http://rm.huanxung.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ip.colortex.cn

Ruby: s.gsub(/\s+/, "")
来源：http://hc.haigaiapp.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kc.colortex.cn

[E10] 左侧补零 / 定长填充
来源：http://wf.lnxyls.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dx.521024.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nb.yuntaijiaju.cn

JS:   "7".padStart(3, "0")
来源：http://dj.shxzskj.cn

TS:   "7".padStart(3, "0")
来源：http://ty.nszjky.cn

Java: String.format("%03d", 7)
来源：http://rb.gzmigu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://mp.haigaiapp.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://he.huanxung.cn


<!-- 参考信息 -->