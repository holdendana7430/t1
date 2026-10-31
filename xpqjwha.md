代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dm.newstarts.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ol.newstarts.cn

JS:   arr.push(4);
来源：http://dq.nszjky.cn

TS:   arr.push(4);
来源：http://th.521024.cn

Java: list.add(4);
来源：http://yf.muxihuayi.cn

Go:   arr = append(arr, 4)
来源：http://am.chemitech.net.cn

Ruby: arr << 4; arr.push(5)
来源：http://pt.jianghongdianzi.cn

C#:   list.Add(4);
来源：http://rr.yuexingan06.cn

[D03] 在指定位置插入元素
来源：http://wy.huixiangedu.cn

Py:   arr.insert(0, 0)
来源：http://pe.colortex.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mj.hahajie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ol.szxytkj.cn

TS:   arr.splice(0, 0, 0);
来源：http://zh.szsharing.cn

Java: list.add(0, 0);
来源：http://ry.gzmigu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://bg.szxytkj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kq.asd995.cn

C#:   list.Insert(0, 0);
来源：http://ta.521024.cn

[D04] 删除元素
来源：http://qz.szsharing.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hm.jctech888.com.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zw.hahajie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qw.521024.cn

TS:   arr.splice(0, 1);
来源：http://vb.newstarts.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dx.newstarts.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mb.szxytkj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lm.asd995.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uk.gzmigu.cn

[D05] 访问与修改元素
来源：http://lv.hnjuh.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wp.9csxet.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gu.huixiangedu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mq.newstarts.cn

TS:   arr[0]; arr.at(-1);
来源：http://vh.szxytkj.cn

Java: list.get(0); list.set(0, 9);
来源：http://sl.colortex.cn

Go:   arr[0]; arr[0] = 9
来源：http://ay.nszjky.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ji.bookmarksfly.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://uj.9csxet.cn

[D06] 数组长度
来源：http://wf.shtwfgs.cn

Py:   len(arr)
来源：http://qv.shxzskj.cn

PHP:  count($arr);
来源：http://py.shxzukj.cn

JS:   arr.length
来源：http://zn.lnxyls.cn

TS:   arr.length
来源：http://zp.gzmigu.cn

Java: list.size();
来源：http://pp.muxihuayi.cn

Go:   len(arr)
来源：http://oi.9csxet.cn

Ruby: arr.length; arr.size
来源：http://qg.asd995.cn

C#:   list.Count;
来源：http://sw.bjjhwx.cn

[D07] 切片 / 取子数组
来源：http://lv.hahajie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ii.chemitech.net.cn

PHP:  array_slice($arr, 1, 3);
来源：http://eo.panjiajie.cn

JS:   arr.slice(1, 4);
来源：http://ej.szsharing.cn

TS:   arr.slice(1, 4);
来源：http://jm.hahajie.cn

Java: list.subList(1, 4);
来源：http://jh.nszjky.cn

Go:   arr[1:4]
来源：http://cn.huixiangedu.cn

Ruby: arr[1, 3]
来源：http://mv.bjjhwx.cn

C#:   list.GetRange(1, 3);
来源：http://vz.chemitech.net.cn

[D08] 合并两个数组
来源：http://zd.hahajie.cn

Py:   a + b;  a.extend(b)
来源：http://jo.szsharing.cn

PHP:  array_merge($a, $b);
来源：http://qa.haigaiapp.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://xv.wgjwhj.cn

TS:   [...a, ...b];
来源：http://wy.asd995.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sp.gzmigu.cn

Go:   append(a, b...)
来源：http://ca.newstarts.cn

Ruby: a + b;  a.concat(b)
来源：http://gm.yuexingan06.cn

C#:   a.Concat(b).ToList()
来源：http://gg.hahajie.cn

[D09] 排序（升序）
来源：http://yc.chemitech.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://ar.panjiajie.cn

PHP:  sort($arr);
来源：http://mb.9csxet.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sx.asd995.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://pt.szsharing.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://qh.huanxung.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fj.haigaiapp.cn

Ruby: arr.sort
来源：http://iz.521024.cn

C#:   list.Sort();
来源：http://os.nicolike.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://tg.hahajie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ly.shxzskj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://im.jctech888.com.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ws.newstarts.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://oj.huixinmuqiang.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nu.521024.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dz.nicolike.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rs.shxzskj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rj.bookmarksfly.cn

[D11] 反转数组
来源：http://ir.panjiajie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qu.jianghongdianzi.cn

PHP:  array_reverse($arr);
来源：http://oy.asd995.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://be.chemitech.net.cn

TS:   [...arr].reverse();
来源：http://ia.bookmarksfly.cn

Java: Collections.reverse(list);
来源：http://ps.yuexingan06.cn

Go:   slices.Reverse(arr)
来源：http://vz.yuexingan06.cn

Ruby: arr.reverse
来源：http://tf.panjiajie.cn

C#:   list.Reverse();
来源：http://mc.nicolike.cn

[D12] 查找元素下标
来源：http://yx.bookmarksfly.cn

Py:   arr.index(x);  x in arr
来源：http://gp.szxytkj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://sm.yuexingan06.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ft.bjjhwx.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ho.szsharing.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ed.nszjky.cn

Go:   slices.Index(arr, x)
来源：http://kp.hnjuh.cn

Ruby: arr.index(x)
来源：http://cq.huixiangedu.cn

C#:   list.IndexOf(x);
来源：http://bz.chemitech.net.cn

[D13] 过滤（保留满足条件的）
来源：http://ql.haigaiapp.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ea.haigaiapp.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fi.hahajie.cn

JS:   arr.filter(x => x > 3)
来源：http://zs.huixiangedu.cn

TS:   arr.filter(x => x > 3)
来源：http://op.jianghongdianzi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ob.shxzukj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tl.shxzukj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://vd.szsharing.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://gx.szsharing.cn

[D14] 映射转换（每个元素变形）
来源：http://go.huanxung.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yd.panjiajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gu.hahajie.cn

JS:   arr.map(x => x * 2)
来源：http://he.shxzskj.cn

TS:   arr.map(x => x * 2)
来源：http://yt.szsharing.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://es.hahajie.cn

Go:   // 手写循环
来源：http://lj.colortex.cn

Ruby: arr.map { |x| x * 2 }
来源：http://mj.haigaiapp.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://sl.huixinmuqiang.cn

[D15] 去重
来源：http://hx.shxzukj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://im.shxzukj.cn

PHP:  array_unique($arr);
来源：http://yd.nicolike.cn

JS:   [...new Set(arr)]
来源：http://xw.shtwfgs.cn

TS:   [...new Set(arr)]
来源：http://sh.jianghongdianzi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ip.9csxet.cn

Go:   // 用 map[T]struct{} 手写
来源：http://lu.jctech888.com.cn

Ruby: arr.uniq
来源：http://kj.nszjky.cn

C#:   list.Distinct().ToList()
来源：http://fr.bjjhwx.cn

[D16] 求和与平均值
来源：http://he.hnjuh.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vf.hahajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bz.yuntaijiaju.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://th.colortex.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kj.bookmarksfly.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://va.muxihuayi.cn

Go:   // 手写循环累加
来源：http://fi.hahajie.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gv.colortex.cn

C#:   list.Sum();  list.Average()
来源：http://qa.shtwfgs.cn

[D17] 最大值与最小值
来源：http://bj.wgjwhj.cn

Py:   max(arr);  min(arr)
来源：http://wy.nicolike.cn

PHP:  max($arr);  min($arr);
来源：http://be.huanxung.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hl.bjjhwx.cn

TS:   Math.max(...arr);
来源：http://ot.lnxyls.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://pc.nicolike.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lo.nszjky.cn

Ruby: arr.max;  arr.min
来源：http://xm.muxihuayi.cn

C#:   list.Max();  list.Min()
来源：http://ix.nszjky.cn

[D18] 扁平化嵌套数组
来源：http://td.shtwfgs.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nu.huixiangedu.cn

PHP:  array_merge(...$nested);
来源：http://zv.panjiajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rv.wgjwhj.cn

TS:   nested.flat();
来源：http://zu.bookmarksfly.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wb.yuexingan06.cn

Go:   // 手写双层循环
来源：http://fn.asd995.cn

Ruby: nested.flatten
来源：http://yz.shxzskj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ne.shxzskj.cn

[D19] 按字段分组
来源：http://ag.asd995.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mr.huixinmuqiang.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kh.yuntaijiaju.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ax.panjiajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://fj.bookmarksfly.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ps.chemitech.net.cn

Go:   // 手写 map[string][]T
来源：http://oa.shtwfgs.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://cn.muxihuayi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://do.shxzskj.cn

[D20] 统计每个元素出现次数
来源：http://wn.yuntaijiaju.cn

Py:   Counter(arr)
来源：http://cf.521024.cn

PHP:  array_count_values($arr);
来源：http://qv.521024.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gd.chemitech.net.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yo.nicolike.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qg.muxihuayi.cn

Go:   // 手写 map[T]int
来源：http://jx.colortex.cn

Ruby: arr.tally
来源：http://jk.szxytkj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tt.hnjuh.cn

[D21] 判断是否包含某元素
来源：http://lv.muxihuayi.cn

Py:   x in arr
来源：http://zw.gzmigu.cn

PHP:  in_array($x, $arr, true);
来源：http://ov.wgjwhj.cn

JS:   arr.includes(x)
来源：http://lw.hnjuh.cn

TS:   arr.includes(x)
来源：http://vh.huixinmuqiang.cn

Java: list.contains(x)
来源：http://yy.szsharing.cn

Go:   slices.Contains(arr, x)
来源：http://kz.asd995.cn

Ruby: arr.include?(x)
来源：http://qi.szxytkj.cn

C#:   list.Contains(x)
来源：http://cd.bjjhwx.cn

[D22] 复制数组（避免共享引用）
来源：http://og.huanxung.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://za.bjjhwx.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gb.huixinmuqiang.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zl.521024.cn

TS:   [...arr];
来源：http://rc.asd995.cn

Java: new ArrayList<>(list);
来源：http://zt.9csxet.cn

Go:   copied := append([]int(nil), arr...)
来源：http://tk.bjjhwx.cn

Ruby: arr.dup;  arr.clone
来源：http://ou.yuexingan06.cn

C#:   new List<int>(list);
来源：http://zw.chemitech.net.cn

[D23] reduce 累积计算
来源：http://ey.shxzukj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jc.shtwfgs.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mp.haigaiapp.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sh.colortex.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nm.shxzskj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://nb.yuntaijiaju.cn

Go:   // 手写循环
来源：http://ak.nicolike.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://oa.lnxyls.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ib.yuexingan06.cn

[D24] 字典 / Map 基本操作
来源：http://ib.nicolike.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nl.gzmigu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gm.haigaiapp.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nj.colortex.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tm.newstarts.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qy.asd995.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pc.shtwfgs.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pp.hnjuh.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ft.521024.cn

[D25] Set 集合去重与交并差
来源：http://jn.huanxung.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dy.haigaiapp.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://oq.gzmigu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://sd.9csxet.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ny.colortex.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://am.hnjuh.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pj.szsharing.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://se.huixinmuqiang.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://sh.shxzskj.cn

[D26] 数组转字符串
来源：http://iz.9csxet.cn

Py:   ", ".join(map(str, arr))
来源：http://ek.yuexingan06.cn

PHP:  implode(", ", $arr);
来源：http://rg.shxzskj.cn

JS:   arr.join(", ")
来源：http://ha.521024.cn

TS:   arr.join(", ")
来源：http://ok.wgjwhj.cn

Java: String.join(", ", list)
来源：http://ax.yuexingan06.cn

Go:   strings.Join(strs, ", ")
来源：http://cz.yuexingan06.cn

Ruby: arr.join(", ")
来源：http://vo.huixinmuqiang.cn

C#:   string.Join(", ", list)
来源：http://ef.wgjwhj.cn

================================================================================
来源：http://bq.huixinmuqiang.cn

E. 字符串处理
来源：http://tu.yuntaijiaju.cn

================================================================================
来源：http://em.muxihuayi.cn

[E01] 拼接字符串
来源：http://pn.huixinmuqiang.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://am.nszjky.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://my.yuntaijiaju.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wo.huixiangedu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qn.bjjhwx.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dd.wgjwhj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ap.newstarts.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ls.colortex.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sr.huanxung.cn

[E02] 重复字符串
来源：http://bu.bjjhwx.cn

Py:   "ab" * 3
来源：http://qp.shtwfgs.cn

PHP:  str_repeat("ab", 3);
来源：http://yp.jianghongdianzi.cn

JS:   "ab".repeat(3)
来源：http://jr.hahajie.cn

TS:   "ab".repeat(3)
来源：http://vt.bjjhwx.cn

Java: "ab".repeat(3)
来源：http://dp.newstarts.cn

Go:   strings.Repeat("ab", 3)
来源：http://za.newstarts.cn

Ruby: "ab" * 3
来源：http://bw.jianghongdianzi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kn.gzmigu.cn

[E03] 截取子串
来源：http://kr.newstarts.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rl.bookmarksfly.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://uj.bookmarksfly.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dz.szxytkj.cn

TS:   s.slice(1, 4)
来源：http://yo.huixiangedu.cn

Java: s.substring(1, 4)
来源：http://kv.muxihuayi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gf.521024.cn

Ruby: s[1, 3];  s[1..3]
来源：http://gi.bjjhwx.cn

C#:   s.Substring(1, 3)
来源：http://yh.lnxyls.cn

[E04] 查找子串位置
来源：http://ht.wgjwhj.cn

Py:   s.find("x");  s.index("x")
来源：http://iz.asd995.cn

PHP:  strpos($s, "x");
来源：http://yk.jianghongdianzi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mn.shxzukj.cn

TS:   s.indexOf("x")
来源：http://oj.yuexingan06.cn

Java: s.indexOf("x")
来源：http://jz.hahajie.cn

Go:   strings.Index(s, "x")
来源：http://sn.hnjuh.cn

Ruby: s.index("x")
来源：http://xf.huixiangedu.cn

C#:   s.IndexOf("x")
来源：http://po.shtwfgs.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://pu.hnjuh.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://up.shtwfgs.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://df.huixiangedu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pe.jctech888.com.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://yk.jctech888.com.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fz.shxzskj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wn.huixinmuqiang.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xk.chemitech.net.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ew.nicolike.cn

[E06] 替换子串
来源：http://yd.szsharing.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://er.haigaiapp.cn

PHP:  str_replace("a", "b", $s);
来源：http://ic.nicolike.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jc.nszjky.cn

TS:   s.replaceAll("a", "b")
来源：http://cl.yuexingan06.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ms.yuntaijiaju.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xk.gzmigu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ja.shxzskj.cn

C#:   s.Replace("a", "b")
来源：http://qh.muxihuayi.cn

[E07] 按分隔符拆分
来源：http://ue.bjjhwx.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fp.newstarts.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hm.yuexingan06.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://gg.nszjky.cn

TS:   s.split(",")
来源：http://km.nszjky.cn

Java: s.split(",");  s.split("\\s+")
来源：http://mt.jianghongdianzi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ka.wgjwhj.cn

Ruby: s.split(",");  s.split
来源：http://cq.hnjuh.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ut.szsharing.cn

[E08] 数组按分隔符合并
来源：http://bx.szxytkj.cn

Py:   ",".join(items)
来源：http://rw.bookmarksfly.cn

PHP:  implode(",", $items);
来源：http://bt.gzmigu.cn

JS:   items.join(",")
来源：http://aa.newstarts.cn

TS:   items.join(",")
来源：http://cp.muxihuayi.cn

Java: String.join(",", items)
来源：http://tn.huanxung.cn

Go:   strings.Join(items, ",")
来源：http://se.jctech888.com.cn

Ruby: items.join(",")
来源：http://zg.huanxung.cn

C#:   string.Join(",", items)
来源：http://kw.521024.cn

[E09] 去除所有空白字符
来源：http://zg.nszjky.cn


<!-- 参考信息 -->