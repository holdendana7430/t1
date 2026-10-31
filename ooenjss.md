代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hs.shxzukj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qi.9csxet.cn

JS:   arr.push(4);
来源：http://xt.huixinmuqiang.cn

TS:   arr.push(4);
来源：http://hl.yuntaijiaju.cn

Java: list.add(4);
来源：http://ds.asd995.cn

Go:   arr = append(arr, 4)
来源：http://oo.szxytkj.cn

Ruby: arr << 4; arr.push(5)
来源：http://wb.haigaiapp.cn

C#:   list.Add(4);
来源：http://dj.huanxung.cn

[D03] 在指定位置插入元素
来源：http://xl.lnxyls.cn

Py:   arr.insert(0, 0)
来源：http://qh.muxihuayi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://li.hnjuh.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fn.shxzukj.cn

TS:   arr.splice(0, 0, 0);
来源：http://ik.panjiajie.cn

Java: list.add(0, 0);
来源：http://ia.shxzukj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ee.yuexingan06.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ph.colortex.cn

C#:   list.Insert(0, 0);
来源：http://mx.huixiangedu.cn

[D04] 删除元素
来源：http://rd.lnxyls.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zo.szsharing.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gc.colortex.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xe.gzmigu.cn

TS:   arr.splice(0, 1);
来源：http://zh.muxihuayi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://up.shxzskj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ve.521024.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cv.asd995.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.9csxet.cn

[D05] 访问与修改元素
来源：http://hs.yuntaijiaju.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yl.huanxung.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gx.jianghongdianzi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yu.newstarts.cn

TS:   arr[0]; arr.at(-1);
来源：http://fv.chemitech.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://md.panjiajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://qb.panjiajie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dj.jianghongdianzi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kx.hnjuh.cn

[D06] 数组长度
来源：http://fx.szsharing.cn

Py:   len(arr)
来源：http://bk.szsharing.cn

PHP:  count($arr);
来源：http://wm.gzmigu.cn

JS:   arr.length
来源：http://gp.521024.cn

TS:   arr.length
来源：http://pi.jctech888.com.cn

Java: list.size();
来源：http://nd.yuexingan06.cn

Go:   len(arr)
来源：http://id.jianghongdianzi.cn

Ruby: arr.length; arr.size
来源：http://hh.jianghongdianzi.cn

C#:   list.Count;
来源：http://xj.jctech888.com.cn

[D07] 切片 / 取子数组
来源：http://xw.szsharing.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qf.huixinmuqiang.cn

PHP:  array_slice($arr, 1, 3);
来源：http://jn.shtwfgs.cn

JS:   arr.slice(1, 4);
来源：http://ea.lnxyls.cn

TS:   arr.slice(1, 4);
来源：http://fk.bjjhwx.cn

Java: list.subList(1, 4);
来源：http://bw.huixinmuqiang.cn

Go:   arr[1:4]
来源：http://jy.shxzukj.cn

Ruby: arr[1, 3]
来源：http://xw.nicolike.cn

C#:   list.GetRange(1, 3);
来源：http://rc.huanxung.cn

[D08] 合并两个数组
来源：http://bm.shxzskj.cn

Py:   a + b;  a.extend(b)
来源：http://uq.9csxet.cn

PHP:  array_merge($a, $b);
来源：http://jx.lnxyls.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://or.wgjwhj.cn

TS:   [...a, ...b];
来源：http://jg.jctech888.com.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dy.chemitech.net.cn

Go:   append(a, b...)
来源：http://fi.haigaiapp.cn

Ruby: a + b;  a.concat(b)
来源：http://hw.hnjuh.cn

C#:   a.Concat(b).ToList()
来源：http://fr.yuexingan06.cn

[D09] 排序（升序）
来源：http://wy.huixinmuqiang.cn

Py:   sorted(arr);  arr.sort()
来源：http://bz.bookmarksfly.cn

PHP:  sort($arr);
来源：http://ph.chemitech.net.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://at.521024.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://el.jianghongdianzi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ew.hnjuh.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mo.huanxung.cn

Ruby: arr.sort
来源：http://sc.lnxyls.cn

C#:   list.Sort();
来源：http://hx.jianghongdianzi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://gv.yuntaijiaju.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wm.huixiangedu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://we.jctech888.com.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ta.hnjuh.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gs.wgjwhj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xg.shxzskj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ef.bookmarksfly.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lf.shtwfgs.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vg.nicolike.cn

[D11] 反转数组
来源：http://qk.huixinmuqiang.cn

Py:   arr[::-1];  arr.reverse()
来源：http://tg.jianghongdianzi.cn

PHP:  array_reverse($arr);
来源：http://et.nszjky.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jo.lnxyls.cn

TS:   [...arr].reverse();
来源：http://vd.huixiangedu.cn

Java: Collections.reverse(list);
来源：http://or.panjiajie.cn

Go:   slices.Reverse(arr)
来源：http://sk.huixiangedu.cn

Ruby: arr.reverse
来源：http://ko.bookmarksfly.cn

C#:   list.Reverse();
来源：http://ho.wgjwhj.cn

[D12] 查找元素下标
来源：http://um.bjjhwx.cn

Py:   arr.index(x);  x in arr
来源：http://vj.huixinmuqiang.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ob.gzmigu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bd.hnjuh.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fa.chemitech.net.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://aq.chemitech.net.cn

Go:   slices.Index(arr, x)
来源：http://hq.huixinmuqiang.cn

Ruby: arr.index(x)
来源：http://en.shtwfgs.cn

C#:   list.IndexOf(x);
来源：http://us.nicolike.cn

[D13] 过滤（保留满足条件的）
来源：http://vy.nszjky.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fy.asd995.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kb.shtwfgs.cn

JS:   arr.filter(x => x > 3)
来源：http://gd.bookmarksfly.cn

TS:   arr.filter(x => x > 3)
来源：http://ya.jianghongdianzi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rw.nszjky.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ra.521024.cn

Ruby: arr.select { |x| x > 3 }
来源：http://bb.nszjky.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://gw.521024.cn

[D14] 映射转换（每个元素变形）
来源：http://hq.hnjuh.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ed.shxzukj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xv.muxihuayi.cn

JS:   arr.map(x => x * 2)
来源：http://xq.hahajie.cn

TS:   arr.map(x => x * 2)
来源：http://te.bookmarksfly.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://yn.gzmigu.cn

Go:   // 手写循环
来源：http://ml.shxzukj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jy.9csxet.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://vw.colortex.cn

[D15] 去重
来源：http://hr.muxihuayi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cc.hahajie.cn

PHP:  array_unique($arr);
来源：http://je.newstarts.cn

JS:   [...new Set(arr)]
来源：http://el.nszjky.cn

TS:   [...new Set(arr)]
来源：http://qx.jianghongdianzi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yw.gzmigu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xd.szxytkj.cn

Ruby: arr.uniq
来源：http://ld.chemitech.net.cn

C#:   list.Distinct().ToList()
来源：http://cq.hnjuh.cn

[D16] 求和与平均值
来源：http://ko.jianghongdianzi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://al.nszjky.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wu.huanxung.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ad.jianghongdianzi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://og.shxzskj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zn.wgjwhj.cn

Go:   // 手写循环累加
来源：http://lp.chemitech.net.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dm.panjiajie.cn

C#:   list.Sum();  list.Average()
来源：http://ag.nszjky.cn

[D17] 最大值与最小值
来源：http://bo.gzmigu.cn

Py:   max(arr);  min(arr)
来源：http://kt.huixiangedu.cn

PHP:  max($arr);  min($arr);
来源：http://cu.huixinmuqiang.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jx.colortex.cn

TS:   Math.max(...arr);
来源：http://xx.nicolike.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ze.521024.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qa.shxzukj.cn

Ruby: arr.max;  arr.min
来源：http://nh.newstarts.cn

C#:   list.Max();  list.Min()
来源：http://da.shxzskj.cn

[D18] 扁平化嵌套数组
来源：http://bu.521024.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ju.gzmigu.cn

PHP:  array_merge(...$nested);
来源：http://lt.521024.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yd.jctech888.com.cn

TS:   nested.flat();
来源：http://ox.hahajie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://na.shxzskj.cn

Go:   // 手写双层循环
来源：http://fy.yuntaijiaju.cn

Ruby: nested.flatten
来源：http://ml.haigaiapp.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://sh.muxihuayi.cn

[D19] 按字段分组
来源：http://ww.9csxet.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vk.shxzukj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://df.huixinmuqiang.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bm.nicolike.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://nk.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://aa.asd995.cn

Go:   // 手写 map[string][]T
来源：http://gt.huixinmuqiang.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ku.szsharing.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hq.shxzukj.cn

[D20] 统计每个元素出现次数
来源：http://ts.shtwfgs.cn

Py:   Counter(arr)
来源：http://xp.jctech888.com.cn

PHP:  array_count_values($arr);
来源：http://tt.nicolike.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kw.bjjhwx.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tk.shxzskj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lv.szxytkj.cn

Go:   // 手写 map[T]int
来源：http://qi.nszjky.cn

Ruby: arr.tally
来源：http://ir.521024.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ds.chemitech.net.cn

[D21] 判断是否包含某元素
来源：http://vs.shxzskj.cn

Py:   x in arr
来源：http://nq.yuntaijiaju.cn

PHP:  in_array($x, $arr, true);
来源：http://iz.bookmarksfly.cn

JS:   arr.includes(x)
来源：http://sc.shxzskj.cn

TS:   arr.includes(x)
来源：http://hs.szsharing.cn

Java: list.contains(x)
来源：http://ob.bjjhwx.cn

Go:   slices.Contains(arr, x)
来源：http://bx.huanxung.cn

Ruby: arr.include?(x)
来源：http://kl.colortex.cn

C#:   list.Contains(x)
来源：http://qn.9csxet.cn

[D22] 复制数组（避免共享引用）
来源：http://uc.muxihuayi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zf.panjiajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ht.nicolike.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://db.szxytkj.cn

TS:   [...arr];
来源：http://hz.szxytkj.cn

Java: new ArrayList<>(list);
来源：http://le.jianghongdianzi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ny.jctech888.com.cn

Ruby: arr.dup;  arr.clone
来源：http://vf.huixinmuqiang.cn

C#:   new List<int>(list);
来源：http://yf.shxzukj.cn

[D23] reduce 累积计算
来源：http://ve.shxzskj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://el.asd995.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ym.nszjky.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rl.szxytkj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://in.9csxet.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://kh.gzmigu.cn

Go:   // 手写循环
来源：http://tw.hnjuh.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jg.newstarts.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dk.haigaiapp.cn

[D24] 字典 / Map 基本操作
来源：http://ii.panjiajie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uj.szsharing.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fd.wgjwhj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qd.jianghongdianzi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dw.hnjuh.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://db.szsharing.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://az.chemitech.net.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pz.521024.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ai.yuexingan06.cn

[D25] Set 集合去重与交并差
来源：http://ra.haigaiapp.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hx.shxzukj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vh.chemitech.net.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xk.521024.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ac.muxihuayi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tv.huixinmuqiang.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dl.yuexingan06.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://py.panjiajie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qs.9csxet.cn

[D26] 数组转字符串
来源：http://hc.jianghongdianzi.cn

Py:   ", ".join(map(str, arr))
来源：http://qu.jianghongdianzi.cn

PHP:  implode(", ", $arr);
来源：http://ls.chemitech.net.cn

JS:   arr.join(", ")
来源：http://qa.shxzskj.cn

TS:   arr.join(", ")
来源：http://kl.panjiajie.cn

Java: String.join(", ", list)
来源：http://pc.huixiangedu.cn

Go:   strings.Join(strs, ", ")
来源：http://hv.szxytkj.cn

Ruby: arr.join(", ")
来源：http://ws.asd995.cn

C#:   string.Join(", ", list)
来源：http://oc.hahajie.cn

================================================================================
来源：http://vb.chemitech.net.cn

E. 字符串处理
来源：http://uh.bjjhwx.cn

================================================================================
来源：http://kc.wgjwhj.cn

[E01] 拼接字符串
来源：http://kc.huixinmuqiang.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ou.asd995.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://db.jctech888.com.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fy.gzmigu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://je.9csxet.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kw.9csxet.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ai.bookmarksfly.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ze.asd995.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ci.shxzskj.cn

[E02] 重复字符串
来源：http://sw.gzmigu.cn

Py:   "ab" * 3
来源：http://go.hahajie.cn

PHP:  str_repeat("ab", 3);
来源：http://qe.jianghongdianzi.cn

JS:   "ab".repeat(3)
来源：http://ik.shtwfgs.cn

TS:   "ab".repeat(3)
来源：http://wv.bjjhwx.cn

Java: "ab".repeat(3)
来源：http://pm.lnxyls.cn

Go:   strings.Repeat("ab", 3)
来源：http://sw.szsharing.cn

Ruby: "ab" * 3
来源：http://qz.hahajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ts.jctech888.com.cn

[E03] 截取子串
来源：http://hl.9csxet.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nb.huixinmuqiang.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nu.panjiajie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zz.huixiangedu.cn

TS:   s.slice(1, 4)
来源：http://po.muxihuayi.cn

Java: s.substring(1, 4)
来源：http://yg.jianghongdianzi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://li.newstarts.cn

Ruby: s[1, 3];  s[1..3]
来源：http://su.jianghongdianzi.cn

C#:   s.Substring(1, 3)
来源：http://qs.hahajie.cn

[E04] 查找子串位置
来源：http://sv.521024.cn

Py:   s.find("x");  s.index("x")
来源：http://cb.panjiajie.cn

PHP:  strpos($s, "x");
来源：http://em.newstarts.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vf.szxytkj.cn

TS:   s.indexOf("x")
来源：http://bn.haigaiapp.cn

Java: s.indexOf("x")
来源：http://tn.jianghongdianzi.cn

Go:   strings.Index(s, "x")
来源：http://hz.jianghongdianzi.cn

Ruby: s.index("x")
来源：http://ta.haigaiapp.cn

C#:   s.IndexOf("x")
来源：http://dv.lnxyls.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://dv.9csxet.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pa.newstarts.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://br.shtwfgs.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yh.jctech888.com.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://yq.huanxung.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bz.gzmigu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://le.huixinmuqiang.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vo.shxzskj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mf.gzmigu.cn

[E06] 替换子串
来源：http://gv.asd995.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jy.huanxung.cn

PHP:  str_replace("a", "b", $s);
来源：http://cp.huixinmuqiang.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xo.bookmarksfly.cn

TS:   s.replaceAll("a", "b")
来源：http://ey.hnjuh.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://te.bookmarksfly.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fa.szsharing.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://to.9csxet.cn

C#:   s.Replace("a", "b")
来源：http://do.asd995.cn

[E07] 按分隔符拆分
来源：http://pk.shxzukj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ru.bjjhwx.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://id.jctech888.com.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ez.lnxyls.cn

TS:   s.split(",")
来源：http://df.haigaiapp.cn

Java: s.split(",");  s.split("\\s+")
来源：http://dk.nicolike.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vo.jianghongdianzi.cn

Ruby: s.split(",");  s.split
来源：http://nu.haigaiapp.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://au.yuntaijiaju.cn

[E08] 数组按分隔符合并
来源：http://si.gzmigu.cn

Py:   ",".join(items)
来源：http://wm.newstarts.cn

PHP:  implode(",", $items);
来源：http://th.asd995.cn

JS:   items.join(",")
来源：http://ir.muxihuayi.cn

TS:   items.join(",")
来源：http://ga.yuexingan06.cn

Java: String.join(",", items)
来源：http://ks.szxytkj.cn

Go:   strings.Join(items, ",")
来源：http://mr.hnjuh.cn

Ruby: items.join(",")
来源：http://mt.nszjky.cn

C#:   string.Join(",", items)
来源：http://yj.szxytkj.cn

[E09] 去除所有空白字符
来源：http://qy.newstarts.cn


<!-- 参考信息 -->