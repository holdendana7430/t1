代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nc.haigaiapp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tb.haigaiapp.cn

JS:   arr.push(4);
来源：http://od.wgjwhj.cn

TS:   arr.push(4);
来源：http://ha.huanxung.cn

Java: list.add(4);
来源：http://mz.muxihuayi.cn

Go:   arr = append(arr, 4)
来源：http://gk.gzmigu.cn

Ruby: arr << 4; arr.push(5)
来源：http://de.huixinmuqiang.cn

C#:   list.Add(4);
来源：http://qv.nicolike.cn

[D03] 在指定位置插入元素
来源：http://sp.jianghongdianzi.cn

Py:   arr.insert(0, 0)
来源：http://qm.huixiangedu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ax.shxzukj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://iu.huixinmuqiang.cn

TS:   arr.splice(0, 0, 0);
来源：http://zb.colortex.cn

Java: list.add(0, 0);
来源：http://qc.bookmarksfly.cn

Go:   arr = append([]int{0}, arr...)
来源：http://cr.szxytkj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ct.szxytkj.cn

C#:   list.Insert(0, 0);
来源：http://sp.muxihuayi.cn

[D04] 删除元素
来源：http://wf.huanxung.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hv.asd995.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lk.shxzukj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xu.bjjhwx.cn

TS:   arr.splice(0, 1);
来源：http://tw.jctech888.com.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gf.szxytkj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gq.wgjwhj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ab.asd995.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ql.shxzukj.cn

[D05] 访问与修改元素
来源：http://ic.huixiangedu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://km.asd995.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xv.yuexingan06.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tm.nicolike.cn

TS:   arr[0]; arr.at(-1);
来源：http://si.lnxyls.cn

Java: list.get(0); list.set(0, 9);
来源：http://as.lnxyls.cn

Go:   arr[0]; arr[0] = 9
来源：http://tf.lnxyls.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ow.colortex.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://tb.haigaiapp.cn

[D06] 数组长度
来源：http://hf.shxzukj.cn

Py:   len(arr)
来源：http://tg.shxzskj.cn

PHP:  count($arr);
来源：http://zp.nszjky.cn

JS:   arr.length
来源：http://wh.yuntaijiaju.cn

TS:   arr.length
来源：http://ml.nszjky.cn

Java: list.size();
来源：http://uf.huixiangedu.cn

Go:   len(arr)
来源：http://tg.jianghongdianzi.cn

Ruby: arr.length; arr.size
来源：http://ov.nszjky.cn

C#:   list.Count;
来源：http://pd.szsharing.cn

[D07] 切片 / 取子数组
来源：http://qd.szsharing.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pg.shxzskj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hx.nicolike.cn

JS:   arr.slice(1, 4);
来源：http://tl.huixinmuqiang.cn

TS:   arr.slice(1, 4);
来源：http://jz.colortex.cn

Java: list.subList(1, 4);
来源：http://fe.jianghongdianzi.cn

Go:   arr[1:4]
来源：http://xf.shxzukj.cn

Ruby: arr[1, 3]
来源：http://iz.521024.cn

C#:   list.GetRange(1, 3);
来源：http://mz.huixinmuqiang.cn

[D08] 合并两个数组
来源：http://sz.521024.cn

Py:   a + b;  a.extend(b)
来源：http://bc.shtwfgs.cn

PHP:  array_merge($a, $b);
来源：http://fy.nicolike.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://aa.panjiajie.cn

TS:   [...a, ...b];
来源：http://kr.9csxet.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fg.yuntaijiaju.cn

Go:   append(a, b...)
来源：http://kp.szxytkj.cn

Ruby: a + b;  a.concat(b)
来源：http://gb.9csxet.cn

C#:   a.Concat(b).ToList()
来源：http://na.bookmarksfly.cn

[D09] 排序（升序）
来源：http://wo.wgjwhj.cn

Py:   sorted(arr);  arr.sort()
来源：http://np.shtwfgs.cn

PHP:  sort($arr);
来源：http://wh.nicolike.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kj.wgjwhj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://md.521024.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://eo.9csxet.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gq.nszjky.cn

Ruby: arr.sort
来源：http://zb.shxzukj.cn

C#:   list.Sort();
来源：http://gf.bookmarksfly.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://zo.huixinmuqiang.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wg.wgjwhj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fz.hahajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xb.panjiajie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lo.asd995.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yv.bookmarksfly.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wg.chemitech.net.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.chemitech.net.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mx.yuntaijiaju.cn

[D11] 反转数组
来源：http://zc.huixinmuqiang.cn

Py:   arr[::-1];  arr.reverse()
来源：http://kh.nicolike.cn

PHP:  array_reverse($arr);
来源：http://za.nicolike.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gg.jctech888.com.cn

TS:   [...arr].reverse();
来源：http://yq.9csxet.cn

Java: Collections.reverse(list);
来源：http://qc.huixiangedu.cn

Go:   slices.Reverse(arr)
来源：http://ib.huanxung.cn

Ruby: arr.reverse
来源：http://ew.9csxet.cn

C#:   list.Reverse();
来源：http://gl.chemitech.net.cn

[D12] 查找元素下标
来源：http://st.gzmigu.cn

Py:   arr.index(x);  x in arr
来源：http://kd.521024.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://va.bjjhwx.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://to.nszjky.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wh.colortex.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yw.hnjuh.cn

Go:   slices.Index(arr, x)
来源：http://ju.huixiangedu.cn

Ruby: arr.index(x)
来源：http://jj.nszjky.cn

C#:   list.IndexOf(x);
来源：http://gm.panjiajie.cn

[D13] 过滤（保留满足条件的）
来源：http://so.nszjky.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pm.colortex.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fl.hnjuh.cn

JS:   arr.filter(x => x > 3)
来源：http://eg.newstarts.cn

TS:   arr.filter(x => x > 3)
来源：http://sj.shxzukj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ti.nicolike.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wp.bookmarksfly.cn

Ruby: arr.select { |x| x > 3 }
来源：http://za.jctech888.com.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://jd.wgjwhj.cn

[D14] 映射转换（每个元素变形）
来源：http://xn.lnxyls.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rw.bjjhwx.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ix.wgjwhj.cn

JS:   arr.map(x => x * 2)
来源：http://qo.521024.cn

TS:   arr.map(x => x * 2)
来源：http://io.haigaiapp.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ya.521024.cn

Go:   // 手写循环
来源：http://xg.yuexingan06.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qf.nicolike.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://dl.asd995.cn

[D15] 去重
来源：http://mr.huanxung.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kv.jianghongdianzi.cn

PHP:  array_unique($arr);
来源：http://pz.wgjwhj.cn

JS:   [...new Set(arr)]
来源：http://bf.hahajie.cn

TS:   [...new Set(arr)]
来源：http://kt.9csxet.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qd.asd995.cn

Go:   // 用 map[T]struct{} 手写
来源：http://pb.jianghongdianzi.cn

Ruby: arr.uniq
来源：http://wj.wgjwhj.cn

C#:   list.Distinct().ToList()
来源：http://du.haigaiapp.cn

[D16] 求和与平均值
来源：http://nh.huixiangedu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://la.muxihuayi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://je.nszjky.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qt.huixinmuqiang.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rm.wgjwhj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gr.9csxet.cn

Go:   // 手写循环累加
来源：http://sd.chemitech.net.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ja.shxzskj.cn

C#:   list.Sum();  list.Average()
来源：http://ft.bookmarksfly.cn

[D17] 最大值与最小值
来源：http://fo.szxytkj.cn

Py:   max(arr);  min(arr)
来源：http://bp.lnxyls.cn

PHP:  max($arr);  min($arr);
来源：http://cs.bjjhwx.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gl.szsharing.cn

TS:   Math.max(...arr);
来源：http://ii.panjiajie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ml.jctech888.com.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zy.szxytkj.cn

Ruby: arr.max;  arr.min
来源：http://lf.wgjwhj.cn

C#:   list.Max();  list.Min()
来源：http://yu.bjjhwx.cn

[D18] 扁平化嵌套数组
来源：http://ik.shtwfgs.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tx.haigaiapp.cn

PHP:  array_merge(...$nested);
来源：http://so.521024.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sd.muxihuayi.cn

TS:   nested.flat();
来源：http://mh.yuntaijiaju.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ob.shtwfgs.cn

Go:   // 手写双层循环
来源：http://sr.yuexingan06.cn

Ruby: nested.flatten
来源：http://bt.hnjuh.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xo.jctech888.com.cn

[D19] 按字段分组
来源：http://jc.newstarts.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fc.newstarts.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pq.wgjwhj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qi.521024.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://dy.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sn.hnjuh.cn

Go:   // 手写 map[string][]T
来源：http://sg.jctech888.com.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ua.panjiajie.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lm.bjjhwx.cn

[D20] 统计每个元素出现次数
来源：http://ae.wgjwhj.cn

Py:   Counter(arr)
来源：http://dx.hnjuh.cn

PHP:  array_count_values($arr);
来源：http://vs.shtwfgs.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xb.bookmarksfly.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ou.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jc.huanxung.cn

Go:   // 手写 map[T]int
来源：http://hz.nicolike.cn

Ruby: arr.tally
来源：http://wz.shxzskj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zf.jianghongdianzi.cn

[D21] 判断是否包含某元素
来源：http://mf.huixiangedu.cn

Py:   x in arr
来源：http://mk.szxytkj.cn

PHP:  in_array($x, $arr, true);
来源：http://ty.panjiajie.cn

JS:   arr.includes(x)
来源：http://fq.yuexingan06.cn

TS:   arr.includes(x)
来源：http://kc.asd995.cn

Java: list.contains(x)
来源：http://sm.szxytkj.cn

Go:   slices.Contains(arr, x)
来源：http://xk.bjjhwx.cn

Ruby: arr.include?(x)
来源：http://nt.shtwfgs.cn

C#:   list.Contains(x)
来源：http://zu.bookmarksfly.cn

[D22] 复制数组（避免共享引用）
来源：http://rn.9csxet.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://df.lnxyls.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xs.hnjuh.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dd.shxzskj.cn

TS:   [...arr];
来源：http://hx.hnjuh.cn

Java: new ArrayList<>(list);
来源：http://vr.nicolike.cn

Go:   copied := append([]int(nil), arr...)
来源：http://am.lnxyls.cn

Ruby: arr.dup;  arr.clone
来源：http://rp.colortex.cn

C#:   new List<int>(list);
来源：http://ti.szxytkj.cn

[D23] reduce 累积计算
来源：http://ie.nszjky.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ap.nszjky.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wt.huixiangedu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pt.muxihuayi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wh.shtwfgs.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://tq.haigaiapp.cn

Go:   // 手写循环
来源：http://tq.hahajie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wv.jctech888.com.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ou.newstarts.cn

[D24] 字典 / Map 基本操作
来源：http://xo.lnxyls.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xu.huixinmuqiang.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://us.gzmigu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ww.yuntaijiaju.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://we.yuntaijiaju.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vf.bjjhwx.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ya.huanxung.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qc.yuntaijiaju.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lq.panjiajie.cn

[D25] Set 集合去重与交并差
来源：http://ng.gzmigu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ff.jctech888.com.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bp.huixinmuqiang.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pi.colortex.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kc.szxytkj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dl.nicolike.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bk.jctech888.com.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vl.nicolike.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rj.szxytkj.cn

[D26] 数组转字符串
来源：http://pe.yuexingan06.cn

Py:   ", ".join(map(str, arr))
来源：http://he.chemitech.net.cn

PHP:  implode(", ", $arr);
来源：http://gt.9csxet.cn

JS:   arr.join(", ")
来源：http://tl.huixiangedu.cn

TS:   arr.join(", ")
来源：http://ts.asd995.cn

Java: String.join(", ", list)
来源：http://dr.gzmigu.cn

Go:   strings.Join(strs, ", ")
来源：http://lx.colortex.cn

Ruby: arr.join(", ")
来源：http://sv.huixinmuqiang.cn

C#:   string.Join(", ", list)
来源：http://yg.shxzukj.cn

================================================================================
来源：http://cs.szsharing.cn

E. 字符串处理
来源：http://tw.huanxung.cn

================================================================================
来源：http://ek.521024.cn

[E01] 拼接字符串
来源：http://tz.wgjwhj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xd.521024.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ml.bookmarksfly.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jx.bookmarksfly.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dy.muxihuayi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wx.yuntaijiaju.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kw.bjjhwx.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wm.colortex.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://un.shxzukj.cn

[E02] 重复字符串
来源：http://ig.shtwfgs.cn

Py:   "ab" * 3
来源：http://fv.asd995.cn

PHP:  str_repeat("ab", 3);
来源：http://jc.hnjuh.cn

JS:   "ab".repeat(3)
来源：http://jx.bjjhwx.cn

TS:   "ab".repeat(3)
来源：http://mt.shxzukj.cn

Java: "ab".repeat(3)
来源：http://wf.muxihuayi.cn

Go:   strings.Repeat("ab", 3)
来源：http://ix.521024.cn

Ruby: "ab" * 3
来源：http://qa.yuexingan06.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mq.jianghongdianzi.cn

[E03] 截取子串
来源：http://km.jctech888.com.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lf.hnjuh.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ng.9csxet.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dd.lnxyls.cn

TS:   s.slice(1, 4)
来源：http://et.gzmigu.cn

Java: s.substring(1, 4)
来源：http://hl.szsharing.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sf.bjjhwx.cn

Ruby: s[1, 3];  s[1..3]
来源：http://gb.shxzukj.cn

C#:   s.Substring(1, 3)
来源：http://yo.lnxyls.cn

[E04] 查找子串位置
来源：http://ay.9csxet.cn

Py:   s.find("x");  s.index("x")
来源：http://mx.szsharing.cn

PHP:  strpos($s, "x");
来源：http://lv.yuntaijiaju.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wz.shtwfgs.cn

TS:   s.indexOf("x")
来源：http://ey.yuexingan06.cn

Java: s.indexOf("x")
来源：http://uf.colortex.cn

Go:   strings.Index(s, "x")
来源：http://cq.lnxyls.cn

Ruby: s.index("x")
来源：http://iu.newstarts.cn

C#:   s.IndexOf("x")
来源：http://sa.huanxung.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ah.chemitech.net.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xk.haigaiapp.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ci.colortex.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kx.huixinmuqiang.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ta.shxzukj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gt.shtwfgs.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xb.lnxyls.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ci.hnjuh.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mx.521024.cn

[E06] 替换子串
来源：http://rj.gzmigu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://an.asd995.cn

PHP:  str_replace("a", "b", $s);
来源：http://ps.521024.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ev.bjjhwx.cn

TS:   s.replaceAll("a", "b")
来源：http://ez.9csxet.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gw.szsharing.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lk.lnxyls.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mr.lnxyls.cn

C#:   s.Replace("a", "b")
来源：http://pw.bjjhwx.cn

[E07] 按分隔符拆分
来源：http://jn.jianghongdianzi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qt.hnjuh.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://iw.jianghongdianzi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://lj.yuexingan06.cn

TS:   s.split(",")
来源：http://gx.haigaiapp.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zf.chemitech.net.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xl.colortex.cn

Ruby: s.split(",");  s.split
来源：http://yo.lnxyls.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pj.jctech888.com.cn

[E08] 数组按分隔符合并
来源：http://rd.huanxung.cn

Py:   ",".join(items)
来源：http://tq.szsharing.cn

PHP:  implode(",", $items);
来源：http://xk.nicolike.cn

JS:   items.join(",")
来源：http://rb.shxzukj.cn

TS:   items.join(",")
来源：http://pn.huanxung.cn

Java: String.join(",", items)
来源：http://xx.huixiangedu.cn

Go:   strings.Join(items, ",")
来源：http://zs.szsharing.cn

Ruby: items.join(",")
来源：http://vu.chemitech.net.cn

C#:   string.Join(",", items)
来源：http://cq.huixinmuqiang.cn

[E09] 去除所有空白字符
来源：http://gz.muxihuayi.cn


<!-- 参考信息 -->