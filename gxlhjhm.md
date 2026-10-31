代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://aw.jctech888.com.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sb.haigaiapp.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bl.wgjwhj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rw.9csxet.cn

Go:   arr := []int{1, 2, 3}
来源：http://qz.newstarts.cn

Ruby: arr = [1, 2, 3]
来源：http://qj.yuexingan06.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zx.gzmigu.cn

[D02] 追加元素到末尾
来源：http://va.jctech888.com.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yl.panjiajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gu.yuexingan06.cn

JS:   arr.push(4);
来源：http://fc.shxzskj.cn

TS:   arr.push(4);
来源：http://yi.nszjky.cn

Java: list.add(4);
来源：http://ya.nszjky.cn

Go:   arr = append(arr, 4)
来源：http://ul.panjiajie.cn

Ruby: arr << 4; arr.push(5)
来源：http://yg.bjjhwx.cn

C#:   list.Add(4);
来源：http://vx.lnxyls.cn

[D03] 在指定位置插入元素
来源：http://ap.newstarts.cn

Py:   arr.insert(0, 0)
来源：http://ej.jianghongdianzi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://be.huanxung.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zd.bookmarksfly.cn

TS:   arr.splice(0, 0, 0);
来源：http://ut.nicolike.cn

Java: list.add(0, 0);
来源：http://gz.jianghongdianzi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://iq.jctech888.com.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://eq.nicolike.cn

C#:   list.Insert(0, 0);
来源：http://pu.shxzskj.cn

[D04] 删除元素
来源：http://zt.panjiajie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wq.szsharing.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rb.asd995.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ue.nszjky.cn

TS:   arr.splice(0, 1);
来源：http://kp.shxzukj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yl.huixinmuqiang.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dr.gzmigu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://iy.szsharing.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nb.huixiangedu.cn

[D05] 访问与修改元素
来源：http://jt.szxytkj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hw.asd995.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://at.jianghongdianzi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qz.chemitech.net.cn

TS:   arr[0]; arr.at(-1);
来源：http://hb.szsharing.cn

Java: list.get(0); list.set(0, 9);
来源：http://fi.muxihuayi.cn

Go:   arr[0]; arr[0] = 9
来源：http://av.shtwfgs.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vu.gzmigu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wp.wgjwhj.cn

[D06] 数组长度
来源：http://zu.gzmigu.cn

Py:   len(arr)
来源：http://gu.hnjuh.cn

PHP:  count($arr);
来源：http://vi.szxytkj.cn

JS:   arr.length
来源：http://be.9csxet.cn

TS:   arr.length
来源：http://lv.asd995.cn

Java: list.size();
来源：http://ni.hahajie.cn

Go:   len(arr)
来源：http://yt.chemitech.net.cn

Ruby: arr.length; arr.size
来源：http://wm.muxihuayi.cn

C#:   list.Count;
来源：http://kw.nszjky.cn

[D07] 切片 / 取子数组
来源：http://te.bjjhwx.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ky.521024.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ph.shtwfgs.cn

JS:   arr.slice(1, 4);
来源：http://yo.yuexingan06.cn

TS:   arr.slice(1, 4);
来源：http://ru.huixinmuqiang.cn

Java: list.subList(1, 4);
来源：http://wv.bookmarksfly.cn

Go:   arr[1:4]
来源：http://dj.szxytkj.cn

Ruby: arr[1, 3]
来源：http://ya.chemitech.net.cn

C#:   list.GetRange(1, 3);
来源：http://de.jianghongdianzi.cn

[D08] 合并两个数组
来源：http://lr.szxytkj.cn

Py:   a + b;  a.extend(b)
来源：http://hj.huixiangedu.cn

PHP:  array_merge($a, $b);
来源：http://lw.szsharing.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://cm.newstarts.cn

TS:   [...a, ...b];
来源：http://mg.haigaiapp.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lo.hahajie.cn

Go:   append(a, b...)
来源：http://ll.bjjhwx.cn

Ruby: a + b;  a.concat(b)
来源：http://lp.9csxet.cn

C#:   a.Concat(b).ToList()
来源：http://ac.shxzukj.cn

[D09] 排序（升序）
来源：http://da.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://ty.shxzukj.cn

PHP:  sort($arr);
来源：http://ak.bjjhwx.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dr.nicolike.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://cv.shtwfgs.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://jy.jianghongdianzi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zl.shxzskj.cn

Ruby: arr.sort
来源：http://sa.gzmigu.cn

C#:   list.Sort();
来源：http://kb.nszjky.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://xt.huixinmuqiang.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fb.bookmarksfly.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nh.chemitech.net.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ko.szxytkj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ty.lnxyls.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mt.wgjwhj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hw.szsharing.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kh.shxzukj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vh.asd995.cn

[D11] 反转数组
来源：http://qo.shxzukj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ob.shtwfgs.cn

PHP:  array_reverse($arr);
来源：http://mq.shxzskj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qz.asd995.cn

TS:   [...arr].reverse();
来源：http://ii.nszjky.cn

Java: Collections.reverse(list);
来源：http://tw.bookmarksfly.cn

Go:   slices.Reverse(arr)
来源：http://xq.lnxyls.cn

Ruby: arr.reverse
来源：http://pr.shxzukj.cn

C#:   list.Reverse();
来源：http://ss.nicolike.cn

[D12] 查找元素下标
来源：http://di.szxytkj.cn

Py:   arr.index(x);  x in arr
来源：http://is.huixiangedu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pg.shxzukj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sv.bookmarksfly.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jh.hahajie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ny.shxzukj.cn

Go:   slices.Index(arr, x)
来源：http://ph.jianghongdianzi.cn

Ruby: arr.index(x)
来源：http://wc.huixiangedu.cn

C#:   list.IndexOf(x);
来源：http://zd.colortex.cn

[D13] 过滤（保留满足条件的）
来源：http://ed.shxzskj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ch.hnjuh.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yp.yuexingan06.cn

JS:   arr.filter(x => x > 3)
来源：http://lo.hahajie.cn

TS:   arr.filter(x => x > 3)
来源：http://zr.szsharing.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://et.yuntaijiaju.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://do.lnxyls.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hy.newstarts.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://iz.colortex.cn

[D14] 映射转换（每个元素变形）
来源：http://cs.shtwfgs.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zr.huixiangedu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dj.521024.cn

JS:   arr.map(x => x * 2)
来源：http://xy.chemitech.net.cn

TS:   arr.map(x => x * 2)
来源：http://nt.shtwfgs.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://fw.huixiangedu.cn

Go:   // 手写循环
来源：http://nn.nszjky.cn

Ruby: arr.map { |x| x * 2 }
来源：http://uq.panjiajie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://it.yuexingan06.cn

[D15] 去重
来源：http://za.521024.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ww.hahajie.cn

PHP:  array_unique($arr);
来源：http://ss.shtwfgs.cn

JS:   [...new Set(arr)]
来源：http://dl.jctech888.com.cn

TS:   [...new Set(arr)]
来源：http://se.newstarts.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zj.haigaiapp.cn

Go:   // 用 map[T]struct{} 手写
来源：http://eq.nszjky.cn

Ruby: arr.uniq
来源：http://ky.nszjky.cn

C#:   list.Distinct().ToList()
来源：http://pb.nszjky.cn

[D16] 求和与平均值
来源：http://rl.gzmigu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kn.hnjuh.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://au.521024.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://eo.colortex.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wh.521024.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://au.newstarts.cn

Go:   // 手写循环累加
来源：http://xd.yuntaijiaju.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://sh.9csxet.cn

C#:   list.Sum();  list.Average()
来源：http://xq.szsharing.cn

[D17] 最大值与最小值
来源：http://qs.huanxung.cn

Py:   max(arr);  min(arr)
来源：http://mn.jctech888.com.cn

PHP:  max($arr);  min($arr);
来源：http://hq.huixinmuqiang.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wl.lnxyls.cn

TS:   Math.max(...arr);
来源：http://ux.bjjhwx.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ag.newstarts.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://az.shxzskj.cn

Ruby: arr.max;  arr.min
来源：http://gn.chemitech.net.cn

C#:   list.Max();  list.Min()
来源：http://ln.huixiangedu.cn

[D18] 扁平化嵌套数组
来源：http://wu.shxzukj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kw.chemitech.net.cn

PHP:  array_merge(...$nested);
来源：http://ws.wgjwhj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ua.newstarts.cn

TS:   nested.flat();
来源：http://ot.nicolike.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yv.yuexingan06.cn

Go:   // 手写双层循环
来源：http://jj.lnxyls.cn

Ruby: nested.flatten
来源：http://sx.gzmigu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://as.huanxung.cn

[D19] 按字段分组
来源：http://qi.lnxyls.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xo.jianghongdianzi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kj.jctech888.com.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ol.hahajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://bb.wgjwhj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kq.yuexingan06.cn

Go:   // 手写 map[string][]T
来源：http://iu.panjiajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fm.haigaiapp.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ff.huixinmuqiang.cn

[D20] 统计每个元素出现次数
来源：http://yb.nicolike.cn

Py:   Counter(arr)
来源：http://yw.gzmigu.cn

PHP:  array_count_values($arr);
来源：http://at.colortex.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nv.hahajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zy.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ew.lnxyls.cn

Go:   // 手写 map[T]int
来源：http://pm.nszjky.cn

Ruby: arr.tally
来源：http://bc.huixinmuqiang.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://od.bjjhwx.cn

[D21] 判断是否包含某元素
来源：http://sr.yuntaijiaju.cn

Py:   x in arr
来源：http://ci.szsharing.cn

PHP:  in_array($x, $arr, true);
来源：http://ko.colortex.cn

JS:   arr.includes(x)
来源：http://nk.huixinmuqiang.cn

TS:   arr.includes(x)
来源：http://fo.lnxyls.cn

Java: list.contains(x)
来源：http://fj.bjjhwx.cn

Go:   slices.Contains(arr, x)
来源：http://mq.nicolike.cn

Ruby: arr.include?(x)
来源：http://fc.panjiajie.cn

C#:   list.Contains(x)
来源：http://dg.huanxung.cn

[D22] 复制数组（避免共享引用）
来源：http://da.panjiajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ck.nicolike.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ym.colortex.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mb.yuntaijiaju.cn

TS:   [...arr];
来源：http://wi.gzmigu.cn

Java: new ArrayList<>(list);
来源：http://kx.bjjhwx.cn

Go:   copied := append([]int(nil), arr...)
来源：http://sv.hnjuh.cn

Ruby: arr.dup;  arr.clone
来源：http://rk.nicolike.cn

C#:   new List<int>(list);
来源：http://tk.huixinmuqiang.cn

[D23] reduce 累积计算
来源：http://ei.muxihuayi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ez.521024.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nj.colortex.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ro.huanxung.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dk.hnjuh.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://aw.wgjwhj.cn

Go:   // 手写循环
来源：http://lp.colortex.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hb.hahajie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jb.jctech888.com.cn

[D24] 字典 / Map 基本操作
来源：http://rl.newstarts.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fa.wgjwhj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sy.huanxung.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ll.colortex.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ke.shtwfgs.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zy.jctech888.com.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bp.yuntaijiaju.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ci.bookmarksfly.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jq.panjiajie.cn

[D25] Set 集合去重与交并差
来源：http://gs.muxihuayi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://oq.bookmarksfly.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dd.jctech888.com.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yl.newstarts.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://it.haigaiapp.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ey.huixiangedu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ed.yuntaijiaju.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qc.jctech888.com.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bj.szxytkj.cn

[D26] 数组转字符串
来源：http://hg.wgjwhj.cn

Py:   ", ".join(map(str, arr))
来源：http://bt.chemitech.net.cn

PHP:  implode(", ", $arr);
来源：http://fi.nszjky.cn

JS:   arr.join(", ")
来源：http://yj.shxzskj.cn

TS:   arr.join(", ")
来源：http://pk.wgjwhj.cn

Java: String.join(", ", list)
来源：http://ou.shxzukj.cn

Go:   strings.Join(strs, ", ")
来源：http://wb.jianghongdianzi.cn

Ruby: arr.join(", ")
来源：http://wl.lnxyls.cn

C#:   string.Join(", ", list)
来源：http://eg.wgjwhj.cn

================================================================================
来源：http://ov.panjiajie.cn

E. 字符串处理
来源：http://mu.haigaiapp.cn

================================================================================
来源：http://hf.wgjwhj.cn

[E01] 拼接字符串
来源：http://ai.haigaiapp.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qe.haigaiapp.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ii.gzmigu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uz.lnxyls.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ti.muxihuayi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ad.521024.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vn.521024.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fr.bjjhwx.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://uc.shxzukj.cn

[E02] 重复字符串
来源：http://ni.521024.cn

Py:   "ab" * 3
来源：http://jf.hnjuh.cn

PHP:  str_repeat("ab", 3);
来源：http://ut.hnjuh.cn

JS:   "ab".repeat(3)
来源：http://ev.yuexingan06.cn

TS:   "ab".repeat(3)
来源：http://pd.gzmigu.cn

Java: "ab".repeat(3)
来源：http://mn.gzmigu.cn

Go:   strings.Repeat("ab", 3)
来源：http://ss.newstarts.cn

Ruby: "ab" * 3
来源：http://zz.nicolike.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://eo.nszjky.cn

[E03] 截取子串
来源：http://bf.gzmigu.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://sk.gzmigu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ml.521024.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://do.muxihuayi.cn

TS:   s.slice(1, 4)
来源：http://dn.hahajie.cn

Java: s.substring(1, 4)
来源：http://wp.asd995.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hk.asd995.cn

Ruby: s[1, 3];  s[1..3]
来源：http://cw.asd995.cn

C#:   s.Substring(1, 3)
来源：http://jp.yuexingan06.cn

[E04] 查找子串位置
来源：http://uj.colortex.cn

Py:   s.find("x");  s.index("x")
来源：http://ph.huixiangedu.cn

PHP:  strpos($s, "x");
来源：http://xo.panjiajie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wl.jctech888.com.cn

TS:   s.indexOf("x")
来源：http://tm.521024.cn

Java: s.indexOf("x")
来源：http://jd.yuexingan06.cn

Go:   strings.Index(s, "x")
来源：http://rb.hnjuh.cn

Ruby: s.index("x")
来源：http://bv.newstarts.cn

C#:   s.IndexOf("x")
来源：http://ui.haigaiapp.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://tj.yuexingan06.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vq.nicolike.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://eg.hahajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zx.bjjhwx.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://rc.521024.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://io.asd995.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sg.newstarts.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jj.chemitech.net.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kz.muxihuayi.cn

[E06] 替换子串
来源：http://fw.szsharing.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ho.9csxet.cn

PHP:  str_replace("a", "b", $s);
来源：http://xc.9csxet.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://na.bjjhwx.cn

TS:   s.replaceAll("a", "b")
来源：http://np.jctech888.com.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lg.wgjwhj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://uq.yuexingan06.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://eq.bookmarksfly.cn

C#:   s.Replace("a", "b")
来源：http://qp.szxytkj.cn

[E07] 按分隔符拆分
来源：http://xr.asd995.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sm.jctech888.com.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://va.jianghongdianzi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://rj.wgjwhj.cn

TS:   s.split(",")
来源：http://pg.panjiajie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://de.bjjhwx.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bi.chemitech.net.cn

Ruby: s.split(",");  s.split
来源：http://st.huixinmuqiang.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hv.wgjwhj.cn

[E08] 数组按分隔符合并
来源：http://se.521024.cn

Py:   ",".join(items)
来源：http://nd.yuexingan06.cn


<!-- 参考信息 -->