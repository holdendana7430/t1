代发 wailian999

Java: list.add(4);
来源：http://kp.shxzskj.cn

Go:   arr = append(arr, 4)
来源：http://wo.colortex.cn

Ruby: arr << 4; arr.push(5)
来源：http://xz.lnxyls.cn

C#:   list.Add(4);
来源：http://io.521024.cn

[D03] 在指定位置插入元素
来源：http://sg.asd995.cn

Py:   arr.insert(0, 0)
来源：http://kj.szxytkj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mc.shtwfgs.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kk.bookmarksfly.cn

TS:   arr.splice(0, 0, 0);
来源：http://we.521024.cn

Java: list.add(0, 0);
来源：http://zw.shxzskj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://lz.muxihuayi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xj.bookmarksfly.cn

C#:   list.Insert(0, 0);
来源：http://hf.9csxet.cn

[D04] 删除元素
来源：http://xt.jianghongdianzi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nu.bjjhwx.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tq.panjiajie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wz.yuexingan06.cn

TS:   arr.splice(0, 1);
来源：http://fi.hahajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hh.lnxyls.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://za.hahajie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://je.shtwfgs.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ms.bjjhwx.cn

[D05] 访问与修改元素
来源：http://hu.lnxyls.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mk.shtwfgs.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ur.shtwfgs.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://iy.hnjuh.cn

TS:   arr[0]; arr.at(-1);
来源：http://dn.szsharing.cn

Java: list.get(0); list.set(0, 9);
来源：http://yx.panjiajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://iw.muxihuayi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pz.asd995.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bm.shxzskj.cn

[D06] 数组长度
来源：http://rb.huanxung.cn

Py:   len(arr)
来源：http://sx.nicolike.cn

PHP:  count($arr);
来源：http://ev.szxytkj.cn

JS:   arr.length
来源：http://yd.newstarts.cn

TS:   arr.length
来源：http://bg.szsharing.cn

Java: list.size();
来源：http://ve.lnxyls.cn

Go:   len(arr)
来源：http://ym.bookmarksfly.cn

Ruby: arr.length; arr.size
来源：http://wp.huixinmuqiang.cn

C#:   list.Count;
来源：http://gp.jianghongdianzi.cn

[D07] 切片 / 取子数组
来源：http://ku.yuexingan06.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hw.jianghongdianzi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ij.521024.cn

JS:   arr.slice(1, 4);
来源：http://gv.jianghongdianzi.cn

TS:   arr.slice(1, 4);
来源：http://sf.shxzukj.cn

Java: list.subList(1, 4);
来源：http://cn.hahajie.cn

Go:   arr[1:4]
来源：http://yr.bookmarksfly.cn

Ruby: arr[1, 3]
来源：http://ag.bjjhwx.cn

C#:   list.GetRange(1, 3);
来源：http://te.chemitech.net.cn

[D08] 合并两个数组
来源：http://bj.shxzukj.cn

Py:   a + b;  a.extend(b)
来源：http://jn.panjiajie.cn

PHP:  array_merge($a, $b);
来源：http://el.haigaiapp.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://jt.jianghongdianzi.cn

TS:   [...a, ...b];
来源：http://ij.yuexingan06.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://be.muxihuayi.cn

Go:   append(a, b...)
来源：http://nf.asd995.cn

Ruby: a + b;  a.concat(b)
来源：http://us.huixinmuqiang.cn

C#:   a.Concat(b).ToList()
来源：http://qq.nicolike.cn

[D09] 排序（升序）
来源：http://xg.yuntaijiaju.cn

Py:   sorted(arr);  arr.sort()
来源：http://or.bookmarksfly.cn

PHP:  sort($arr);
来源：http://xi.colortex.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fu.shxzskj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xl.shtwfgs.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://pu.hahajie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ed.haigaiapp.cn

Ruby: arr.sort
来源：http://fp.haigaiapp.cn

C#:   list.Sort();
来源：http://mu.gzmigu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://nm.gzmigu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gi.shxzukj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ha.nicolike.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://eo.gzmigu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ju.huixinmuqiang.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ro.nicolike.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://li.nszjky.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xp.huixinmuqiang.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bw.nicolike.cn

[D11] 反转数组
来源：http://nk.nszjky.cn

Py:   arr[::-1];  arr.reverse()
来源：http://rs.jianghongdianzi.cn

PHP:  array_reverse($arr);
来源：http://vi.yuexingan06.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yz.hnjuh.cn

TS:   [...arr].reverse();
来源：http://vh.9csxet.cn

Java: Collections.reverse(list);
来源：http://rx.jctech888.com.cn

Go:   slices.Reverse(arr)
来源：http://zf.jianghongdianzi.cn

Ruby: arr.reverse
来源：http://gc.haigaiapp.cn

C#:   list.Reverse();
来源：http://vi.chemitech.net.cn

[D12] 查找元素下标
来源：http://zc.jctech888.com.cn

Py:   arr.index(x);  x in arr
来源：http://ca.hahajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mu.bjjhwx.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ib.huanxung.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bn.szxytkj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ej.colortex.cn

Go:   slices.Index(arr, x)
来源：http://ok.gzmigu.cn

Ruby: arr.index(x)
来源：http://av.asd995.cn

C#:   list.IndexOf(x);
来源：http://oo.panjiajie.cn

[D13] 过滤（保留满足条件的）
来源：http://ox.panjiajie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ip.colortex.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ai.huixiangedu.cn

JS:   arr.filter(x => x > 3)
来源：http://ri.huixiangedu.cn

TS:   arr.filter(x => x > 3)
来源：http://us.szsharing.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qz.9csxet.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fs.wgjwhj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qf.gzmigu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ut.shxzskj.cn

[D14] 映射转换（每个元素变形）
来源：http://uv.szsharing.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ra.bookmarksfly.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ru.hnjuh.cn

JS:   arr.map(x => x * 2)
来源：http://ya.521024.cn

TS:   arr.map(x => x * 2)
来源：http://vo.shtwfgs.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ni.521024.cn

Go:   // 手写循环
来源：http://gn.chemitech.net.cn

Ruby: arr.map { |x| x * 2 }
来源：http://bb.bookmarksfly.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://uy.shtwfgs.cn

[D15] 去重
来源：http://zq.yuexingan06.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://si.bjjhwx.cn

PHP:  array_unique($arr);
来源：http://jm.shtwfgs.cn

JS:   [...new Set(arr)]
来源：http://lb.shtwfgs.cn

TS:   [...new Set(arr)]
来源：http://hd.jctech888.com.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ka.shxzukj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://pw.jctech888.com.cn

Ruby: arr.uniq
来源：http://ge.bjjhwx.cn

C#:   list.Distinct().ToList()
来源：http://rr.muxihuayi.cn

[D16] 求和与平均值
来源：http://je.newstarts.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ba.lnxyls.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jj.huixiangedu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vs.jianghongdianzi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tu.nszjky.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jt.jctech888.com.cn

Go:   // 手写循环累加
来源：http://ig.bookmarksfly.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://sq.bjjhwx.cn

C#:   list.Sum();  list.Average()
来源：http://kd.nszjky.cn

[D17] 最大值与最小值
来源：http://nn.panjiajie.cn

Py:   max(arr);  min(arr)
来源：http://hz.szsharing.cn

PHP:  max($arr);  min($arr);
来源：http://yx.nicolike.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://el.shtwfgs.cn

TS:   Math.max(...arr);
来源：http://xv.yuntaijiaju.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ho.shxzskj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jd.newstarts.cn

Ruby: arr.max;  arr.min
来源：http://pd.shxzukj.cn

C#:   list.Max();  list.Min()
来源：http://er.bjjhwx.cn

[D18] 扁平化嵌套数组
来源：http://oq.szxytkj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ny.shxzskj.cn

PHP:  array_merge(...$nested);
来源：http://eb.nicolike.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fq.chemitech.net.cn

TS:   nested.flat();
来源：http://gi.hahajie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dg.huixinmuqiang.cn

Go:   // 手写双层循环
来源：http://oa.colortex.cn

Ruby: nested.flatten
来源：http://qb.gzmigu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hv.hnjuh.cn

[D19] 按字段分组
来源：http://tv.nszjky.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fo.bookmarksfly.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://uw.huanxung.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vg.wgjwhj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ku.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ta.chemitech.net.cn

Go:   // 手写 map[string][]T
来源：http://tt.panjiajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ng.shxzskj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gr.shxzskj.cn

[D20] 统计每个元素出现次数
来源：http://kk.nszjky.cn

Py:   Counter(arr)
来源：http://aq.shxzukj.cn

PHP:  array_count_values($arr);
来源：http://vz.521024.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zb.bjjhwx.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gk.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://be.haigaiapp.cn

Go:   // 手写 map[T]int
来源：http://sq.shxzskj.cn

Ruby: arr.tally
来源：http://sh.szxytkj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://iv.9csxet.cn

[D21] 判断是否包含某元素
来源：http://rh.muxihuayi.cn

Py:   x in arr
来源：http://oj.newstarts.cn

PHP:  in_array($x, $arr, true);
来源：http://lb.nicolike.cn

JS:   arr.includes(x)
来源：http://ij.newstarts.cn

TS:   arr.includes(x)
来源：http://oe.9csxet.cn

Java: list.contains(x)
来源：http://rq.shxzskj.cn

Go:   slices.Contains(arr, x)
来源：http://tt.shtwfgs.cn

Ruby: arr.include?(x)
来源：http://db.szxytkj.cn

C#:   list.Contains(x)
来源：http://va.yuntaijiaju.cn

[D22] 复制数组（避免共享引用）
来源：http://kv.szxytkj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qp.shxzskj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pv.9csxet.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zj.gzmigu.cn

TS:   [...arr];
来源：http://hy.colortex.cn

Java: new ArrayList<>(list);
来源：http://ky.shxzskj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://mz.colortex.cn

Ruby: arr.dup;  arr.clone
来源：http://aw.shtwfgs.cn

C#:   new List<int>(list);
来源：http://ih.yuexingan06.cn

[D23] reduce 累积计算
来源：http://zg.szxytkj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fz.bjjhwx.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xl.gzmigu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wg.jianghongdianzi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qn.shxzskj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://hk.huixinmuqiang.cn

Go:   // 手写循环
来源：http://nl.jianghongdianzi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ue.bookmarksfly.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gy.panjiajie.cn

[D24] 字典 / Map 基本操作
来源：http://xx.huixiangedu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gw.hahajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sn.yuexingan06.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lj.haigaiapp.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zw.shtwfgs.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tw.9csxet.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ud.haigaiapp.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ik.colortex.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gl.muxihuayi.cn

[D25] Set 集合去重与交并差
来源：http://rg.wgjwhj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kp.lnxyls.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gb.huixiangedu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ld.nszjky.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zb.jctech888.com.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sk.jctech888.com.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tq.shxzukj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ow.nicolike.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nh.colortex.cn

[D26] 数组转字符串
来源：http://gp.colortex.cn

Py:   ", ".join(map(str, arr))
来源：http://yb.nicolike.cn

PHP:  implode(", ", $arr);
来源：http://am.shxzukj.cn

JS:   arr.join(", ")
来源：http://sc.nicolike.cn

TS:   arr.join(", ")
来源：http://wa.haigaiapp.cn

Java: String.join(", ", list)
来源：http://ch.yuntaijiaju.cn

Go:   strings.Join(strs, ", ")
来源：http://su.muxihuayi.cn

Ruby: arr.join(", ")
来源：http://az.colortex.cn

C#:   string.Join(", ", list)
来源：http://ma.bookmarksfly.cn

================================================================================
来源：http://wo.hahajie.cn

E. 字符串处理
来源：http://we.shxzskj.cn

================================================================================
来源：http://sa.colortex.cn

[E01] 拼接字符串
来源：http://la.wgjwhj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://se.nszjky.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qp.bookmarksfly.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bf.haigaiapp.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zg.jctech888.com.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cd.huanxung.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nt.szxytkj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://es.jianghongdianzi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ov.szxytkj.cn

[E02] 重复字符串
来源：http://hy.shxzukj.cn

Py:   "ab" * 3
来源：http://gn.muxihuayi.cn

PHP:  str_repeat("ab", 3);
来源：http://wg.asd995.cn

JS:   "ab".repeat(3)
来源：http://ch.shtwfgs.cn

TS:   "ab".repeat(3)
来源：http://ix.yuntaijiaju.cn

Java: "ab".repeat(3)
来源：http://wl.haigaiapp.cn

Go:   strings.Repeat("ab", 3)
来源：http://xb.jianghongdianzi.cn

Ruby: "ab" * 3
来源：http://mc.9csxet.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uw.muxihuayi.cn

[E03] 截取子串
来源：http://zr.lnxyls.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pl.huixiangedu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hk.huixiangedu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ji.huixinmuqiang.cn

TS:   s.slice(1, 4)
来源：http://ro.wgjwhj.cn

Java: s.substring(1, 4)
来源：http://vj.huanxung.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ts.huixiangedu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://tn.colortex.cn

C#:   s.Substring(1, 3)
来源：http://yj.asd995.cn

[E04] 查找子串位置
来源：http://ls.shxzskj.cn

Py:   s.find("x");  s.index("x")
来源：http://xp.chemitech.net.cn

PHP:  strpos($s, "x");
来源：http://tu.9csxet.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lv.gzmigu.cn

TS:   s.indexOf("x")
来源：http://dc.huixiangedu.cn

Java: s.indexOf("x")
来源：http://yv.jctech888.com.cn

Go:   strings.Index(s, "x")
来源：http://ju.yuexingan06.cn

Ruby: s.index("x")
来源：http://ud.haigaiapp.cn

C#:   s.IndexOf("x")
来源：http://nr.gzmigu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://rq.asd995.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nv.hnjuh.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dp.huanxung.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bt.jctech888.com.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://wq.haigaiapp.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zq.muxihuayi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gn.bookmarksfly.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nc.shxzskj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vs.shtwfgs.cn

[E06] 替换子串
来源：http://lo.jctech888.com.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nv.haigaiapp.cn

PHP:  str_replace("a", "b", $s);
来源：http://vx.nicolike.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ug.huanxung.cn

TS:   s.replaceAll("a", "b")
来源：http://yg.colortex.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://co.yuexingan06.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jr.nszjky.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://en.shtwfgs.cn

C#:   s.Replace("a", "b")
来源：http://ue.yuexingan06.cn

[E07] 按分隔符拆分
来源：http://nt.colortex.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vn.newstarts.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wi.huixinmuqiang.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://gw.asd995.cn

TS:   s.split(",")
来源：http://rt.9csxet.cn

Java: s.split(",");  s.split("\\s+")
来源：http://lr.chemitech.net.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ip.muxihuayi.cn

Ruby: s.split(",");  s.split
来源：http://ye.hahajie.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wr.nicolike.cn

[E08] 数组按分隔符合并
来源：http://bd.yuntaijiaju.cn

Py:   ",".join(items)
来源：http://bb.huixiangedu.cn

PHP:  implode(",", $items);
来源：http://dc.gzmigu.cn

JS:   items.join(",")
来源：http://jw.hahajie.cn

TS:   items.join(",")
来源：http://pw.hnjuh.cn

Java: String.join(",", items)
来源：http://lj.yuexingan06.cn

Go:   strings.Join(items, ",")
来源：http://hh.yuntaijiaju.cn

Ruby: items.join(",")
来源：http://qe.muxihuayi.cn

C#:   string.Join(",", items)
来源：http://ce.wgjwhj.cn

[E09] 去除所有空白字符
来源：http://nx.shxzukj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ag.hahajie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yr.jianghongdianzi.cn

JS:   s.replace(/\s+/g, "")
来源：http://nj.bookmarksfly.cn

TS:   s.replace(/\s+/g, "")
来源：http://hi.521024.cn


<!-- 参考信息 -->