代发 wailian999

Java: list.add(4);
来源：http://ek.colortex.cn

Go:   arr = append(arr, 4)
来源：http://oh.szsharing.cn

Ruby: arr << 4; arr.push(5)
来源：http://id.szxytkj.cn

C#:   list.Add(4);
来源：http://nm.huixiangedu.cn

[D03] 在指定位置插入元素
来源：http://ph.chemitech.net.cn

Py:   arr.insert(0, 0)
来源：http://em.hahajie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lm.huanxung.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://sq.newstarts.cn

TS:   arr.splice(0, 0, 0);
来源：http://fw.wgjwhj.cn

Java: list.add(0, 0);
来源：http://up.gzmigu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vl.haigaiapp.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ag.muxihuayi.cn

C#:   list.Insert(0, 0);
来源：http://dm.newstarts.cn

[D04] 删除元素
来源：http://rv.muxihuayi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qd.jctech888.com.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vu.huixiangedu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://os.szxytkj.cn

TS:   arr.splice(0, 1);
来源：http://rg.gzmigu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gt.huixinmuqiang.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cu.szsharing.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ql.gzmigu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hk.huixiangedu.cn

[D05] 访问与修改元素
来源：http://cb.521024.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vp.huanxung.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fr.shtwfgs.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nu.bjjhwx.cn

TS:   arr[0]; arr.at(-1);
来源：http://ip.hahajie.cn

Java: list.get(0); list.set(0, 9);
来源：http://za.newstarts.cn

Go:   arr[0]; arr[0] = 9
来源：http://qu.gzmigu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qg.shtwfgs.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zt.jctech888.com.cn

[D06] 数组长度
来源：http://zd.jctech888.com.cn

Py:   len(arr)
来源：http://ew.bookmarksfly.cn

PHP:  count($arr);
来源：http://iu.szsharing.cn

JS:   arr.length
来源：http://db.521024.cn

TS:   arr.length
来源：http://qq.jctech888.com.cn

Java: list.size();
来源：http://lq.nicolike.cn

Go:   len(arr)
来源：http://ch.bjjhwx.cn

Ruby: arr.length; arr.size
来源：http://op.lnxyls.cn

C#:   list.Count;
来源：http://ka.9csxet.cn

[D07] 切片 / 取子数组
来源：http://pv.bookmarksfly.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rs.newstarts.cn

PHP:  array_slice($arr, 1, 3);
来源：http://mh.bookmarksfly.cn

JS:   arr.slice(1, 4);
来源：http://wx.jctech888.com.cn

TS:   arr.slice(1, 4);
来源：http://cb.521024.cn

Java: list.subList(1, 4);
来源：http://tu.shxzukj.cn

Go:   arr[1:4]
来源：http://rb.jianghongdianzi.cn

Ruby: arr[1, 3]
来源：http://og.asd995.cn

C#:   list.GetRange(1, 3);
来源：http://ua.nicolike.cn

[D08] 合并两个数组
来源：http://ep.yuntaijiaju.cn

Py:   a + b;  a.extend(b)
来源：http://zf.huixinmuqiang.cn

PHP:  array_merge($a, $b);
来源：http://oh.chemitech.net.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ai.nszjky.cn

TS:   [...a, ...b];
来源：http://oh.huixiangedu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sp.colortex.cn

Go:   append(a, b...)
来源：http://qx.yuntaijiaju.cn

Ruby: a + b;  a.concat(b)
来源：http://ph.szxytkj.cn

C#:   a.Concat(b).ToList()
来源：http://bf.shxzskj.cn

[D09] 排序（升序）
来源：http://zo.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://rb.wgjwhj.cn

PHP:  sort($arr);
来源：http://zr.shxzskj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ag.newstarts.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tw.9csxet.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://bd.shtwfgs.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hi.asd995.cn

Ruby: arr.sort
来源：http://qr.bookmarksfly.cn

C#:   list.Sort();
来源：http://yi.gzmigu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://pw.haigaiapp.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qy.nicolike.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mj.chemitech.net.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qc.panjiajie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://td.huixiangedu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vy.9csxet.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rd.gzmigu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ta.colortex.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://sa.yuntaijiaju.cn

[D11] 反转数组
来源：http://gd.hnjuh.cn

Py:   arr[::-1];  arr.reverse()
来源：http://vz.shxzukj.cn

PHP:  array_reverse($arr);
来源：http://vp.jianghongdianzi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xy.asd995.cn

TS:   [...arr].reverse();
来源：http://tt.9csxet.cn

Java: Collections.reverse(list);
来源：http://wx.shxzskj.cn

Go:   slices.Reverse(arr)
来源：http://ww.hnjuh.cn

Ruby: arr.reverse
来源：http://uf.chemitech.net.cn

C#:   list.Reverse();
来源：http://nx.nicolike.cn

[D12] 查找元素下标
来源：http://nj.9csxet.cn

Py:   arr.index(x);  x in arr
来源：http://gj.yuntaijiaju.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bj.lnxyls.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ov.shtwfgs.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://my.asd995.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mm.jianghongdianzi.cn

Go:   slices.Index(arr, x)
来源：http://bw.chemitech.net.cn

Ruby: arr.index(x)
来源：http://gj.shtwfgs.cn

C#:   list.IndexOf(x);
来源：http://mv.huixiangedu.cn

[D13] 过滤（保留满足条件的）
来源：http://bv.szxytkj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gk.lnxyls.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kd.nicolike.cn

JS:   arr.filter(x => x > 3)
来源：http://xr.muxihuayi.cn

TS:   arr.filter(x => x > 3)
来源：http://ry.shxzukj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://co.shtwfgs.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dq.szsharing.cn

Ruby: arr.select { |x| x > 3 }
来源：http://mo.yuntaijiaju.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://cr.szxytkj.cn

[D14] 映射转换（每个元素变形）
来源：http://ca.asd995.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pn.szxytkj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yx.haigaiapp.cn

JS:   arr.map(x => x * 2)
来源：http://lx.nszjky.cn

TS:   arr.map(x => x * 2)
来源：http://au.bjjhwx.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://tt.nicolike.cn

Go:   // 手写循环
来源：http://ym.colortex.cn

Ruby: arr.map { |x| x * 2 }
来源：http://xd.huixinmuqiang.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://fy.hnjuh.cn

[D15] 去重
来源：http://al.colortex.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ja.wgjwhj.cn

PHP:  array_unique($arr);
来源：http://er.hnjuh.cn

JS:   [...new Set(arr)]
来源：http://bd.colortex.cn

TS:   [...new Set(arr)]
来源：http://go.asd995.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gn.shxzukj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://eq.asd995.cn

Ruby: arr.uniq
来源：http://bu.hnjuh.cn

C#:   list.Distinct().ToList()
来源：http://gx.jctech888.com.cn

[D16] 求和与平均值
来源：http://dh.shxzukj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ef.lnxyls.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://te.bjjhwx.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xj.gzmigu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://st.yuexingan06.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lx.nszjky.cn

Go:   // 手写循环累加
来源：http://hc.521024.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pl.newstarts.cn

C#:   list.Sum();  list.Average()
来源：http://iu.wgjwhj.cn

[D17] 最大值与最小值
来源：http://rq.hnjuh.cn

Py:   max(arr);  min(arr)
来源：http://zw.bjjhwx.cn

PHP:  max($arr);  min($arr);
来源：http://yp.newstarts.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hg.nszjky.cn

TS:   Math.max(...arr);
来源：http://ip.yuntaijiaju.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://bv.wgjwhj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://sv.521024.cn

Ruby: arr.max;  arr.min
来源：http://ub.bjjhwx.cn

C#:   list.Max();  list.Min()
来源：http://ar.huanxung.cn

[D18] 扁平化嵌套数组
来源：http://hm.521024.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tf.szxytkj.cn

PHP:  array_merge(...$nested);
来源：http://ez.panjiajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wi.lnxyls.cn

TS:   nested.flat();
来源：http://hy.shxzukj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cv.asd995.cn

Go:   // 手写双层循环
来源：http://qo.shxzskj.cn

Ruby: nested.flatten
来源：http://pl.newstarts.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hf.szsharing.cn

[D19] 按字段分组
来源：http://yn.shxzskj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://an.colortex.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ii.huanxung.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://sn.panjiajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://vy.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qj.chemitech.net.cn

Go:   // 手写 map[string][]T
来源：http://gz.wgjwhj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://qu.colortex.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cs.hahajie.cn

[D20] 统计每个元素出现次数
来源：http://oi.yuexingan06.cn

Py:   Counter(arr)
来源：http://jc.bookmarksfly.cn

PHP:  array_count_values($arr);
来源：http://ud.colortex.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://go.bookmarksfly.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qe.hahajie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tt.gzmigu.cn

Go:   // 手写 map[T]int
来源：http://kd.panjiajie.cn

Ruby: arr.tally
来源：http://ih.jctech888.com.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sb.panjiajie.cn

[D21] 判断是否包含某元素
来源：http://oe.shxzukj.cn

Py:   x in arr
来源：http://yk.nszjky.cn

PHP:  in_array($x, $arr, true);
来源：http://or.shtwfgs.cn

JS:   arr.includes(x)
来源：http://db.hahajie.cn

TS:   arr.includes(x)
来源：http://pf.yuntaijiaju.cn

Java: list.contains(x)
来源：http://gp.huanxung.cn

Go:   slices.Contains(arr, x)
来源：http://dr.shxzukj.cn

Ruby: arr.include?(x)
来源：http://ua.muxihuayi.cn

C#:   list.Contains(x)
来源：http://mr.hahajie.cn

[D22] 复制数组（避免共享引用）
来源：http://ib.newstarts.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hn.huixinmuqiang.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bu.szxytkj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rm.shxzukj.cn

TS:   [...arr];
来源：http://hv.huanxung.cn

Java: new ArrayList<>(list);
来源：http://sm.huixiangedu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://th.bjjhwx.cn

Ruby: arr.dup;  arr.clone
来源：http://dl.panjiajie.cn

C#:   new List<int>(list);
来源：http://gx.huixiangedu.cn

[D23] reduce 累积计算
来源：http://wh.yuexingan06.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gb.9csxet.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bp.asd995.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wm.szsharing.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nf.shxzukj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://jc.chemitech.net.cn

Go:   // 手写循环
来源：http://cd.jctech888.com.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fm.jianghongdianzi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ro.nszjky.cn

[D24] 字典 / Map 基本操作
来源：http://ur.yuexingan06.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ow.asd995.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ja.521024.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://he.huixinmuqiang.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lw.szxytkj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ce.jianghongdianzi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hy.521024.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ue.lnxyls.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://sv.panjiajie.cn

[D25] Set 集合去重与交并差
来源：http://jc.jianghongdianzi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dq.shxzskj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ee.yuntaijiaju.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ds.wgjwhj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bk.huanxung.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lj.muxihuayi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cc.shxzskj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pg.9csxet.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://du.panjiajie.cn

[D26] 数组转字符串
来源：http://xp.huixinmuqiang.cn

Py:   ", ".join(map(str, arr))
来源：http://ci.shxzukj.cn

PHP:  implode(", ", $arr);
来源：http://dr.huixinmuqiang.cn

JS:   arr.join(", ")
来源：http://ym.wgjwhj.cn

TS:   arr.join(", ")
来源：http://cg.9csxet.cn

Java: String.join(", ", list)
来源：http://or.chemitech.net.cn

Go:   strings.Join(strs, ", ")
来源：http://vn.newstarts.cn

Ruby: arr.join(", ")
来源：http://ek.jctech888.com.cn

C#:   string.Join(", ", list)
来源：http://ac.521024.cn

================================================================================
来源：http://bl.yuexingan06.cn

E. 字符串处理
来源：http://vl.9csxet.cn

================================================================================
来源：http://ye.lnxyls.cn

[E01] 拼接字符串
来源：http://bc.bjjhwx.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://it.gzmigu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mh.521024.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://eh.lnxyls.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://oi.9csxet.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ic.521024.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vw.yuntaijiaju.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rq.bookmarksfly.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zp.chemitech.net.cn

[E02] 重复字符串
来源：http://em.huixinmuqiang.cn

Py:   "ab" * 3
来源：http://bb.newstarts.cn

PHP:  str_repeat("ab", 3);
来源：http://xj.shxzukj.cn

JS:   "ab".repeat(3)
来源：http://qq.gzmigu.cn

TS:   "ab".repeat(3)
来源：http://jv.nszjky.cn

Java: "ab".repeat(3)
来源：http://dt.panjiajie.cn

Go:   strings.Repeat("ab", 3)
来源：http://ab.wgjwhj.cn

Ruby: "ab" * 3
来源：http://jq.colortex.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gx.panjiajie.cn

[E03] 截取子串
来源：http://qe.yuexingan06.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jg.huixinmuqiang.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fp.chemitech.net.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://uj.colortex.cn

TS:   s.slice(1, 4)
来源：http://gm.chemitech.net.cn

Java: s.substring(1, 4)
来源：http://mw.asd995.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tn.muxihuayi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://um.hnjuh.cn

C#:   s.Substring(1, 3)
来源：http://xc.yuexingan06.cn

[E04] 查找子串位置
来源：http://fo.newstarts.cn

Py:   s.find("x");  s.index("x")
来源：http://nu.9csxet.cn

PHP:  strpos($s, "x");
来源：http://dd.hnjuh.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pr.bjjhwx.cn

TS:   s.indexOf("x")
来源：http://aw.shxzskj.cn

Java: s.indexOf("x")
来源：http://zv.colortex.cn

Go:   strings.Index(s, "x")
来源：http://fb.nicolike.cn

Ruby: s.index("x")
来源：http://et.szsharing.cn

C#:   s.IndexOf("x")
来源：http://ev.lnxyls.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://il.asd995.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dg.nszjky.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sg.hnjuh.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ay.yuntaijiaju.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://kn.szxytkj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://se.huixiangedu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qi.haigaiapp.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fy.lnxyls.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gt.bookmarksfly.cn

[E06] 替换子串
来源：http://tv.nszjky.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wz.szsharing.cn

PHP:  str_replace("a", "b", $s);
来源：http://gb.9csxet.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iw.chemitech.net.cn

TS:   s.replaceAll("a", "b")
来源：http://op.shtwfgs.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yg.shxzskj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bb.nszjky.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mq.hnjuh.cn

C#:   s.Replace("a", "b")
来源：http://wn.yuntaijiaju.cn

[E07] 按分隔符拆分
来源：http://xb.hahajie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gs.hahajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://eg.wgjwhj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://lw.muxihuayi.cn

TS:   s.split(",")
来源：http://lc.muxihuayi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://sz.huanxung.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ri.huanxung.cn

Ruby: s.split(",");  s.split
来源：http://me.colortex.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://oj.wgjwhj.cn

[E08] 数组按分隔符合并
来源：http://wy.hahajie.cn

Py:   ",".join(items)
来源：http://ux.shxzukj.cn

PHP:  implode(",", $items);
来源：http://gv.asd995.cn

JS:   items.join(",")
来源：http://fs.jianghongdianzi.cn

TS:   items.join(",")
来源：http://yb.shxzukj.cn

Java: String.join(",", items)
来源：http://pu.9csxet.cn

Go:   strings.Join(items, ",")
来源：http://ui.nszjky.cn

Ruby: items.join(",")
来源：http://ka.bjjhwx.cn

C#:   string.Join(",", items)
来源：http://fw.huanxung.cn

[E09] 去除所有空白字符
来源：http://ln.jctech888.com.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://oa.nszjky.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ap.huixiangedu.cn

JS:   s.replace(/\s+/g, "")
来源：http://jt.jianghongdianzi.cn

TS:   s.replace(/\s+/g, "")
来源：http://xw.bjjhwx.cn


<!-- 参考信息 -->