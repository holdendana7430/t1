代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ch.panjiajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jt.shtwfgs.cn

JS:   arr.push(4);
来源：http://oc.huixiangedu.cn

TS:   arr.push(4);
来源：http://eb.bjjhwx.cn

Java: list.add(4);
来源：http://lb.shxzskj.cn

Go:   arr = append(arr, 4)
来源：http://kp.shxzskj.cn

Ruby: arr << 4; arr.push(5)
来源：http://oz.bjjhwx.cn

C#:   list.Add(4);
来源：http://ur.muxihuayi.cn

[D03] 在指定位置插入元素
来源：http://ks.hahajie.cn

Py:   arr.insert(0, 0)
来源：http://kn.gzmigu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://uz.panjiajie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://os.szsharing.cn

TS:   arr.splice(0, 0, 0);
来源：http://zl.bjjhwx.cn

Java: list.add(0, 0);
来源：http://ye.shtwfgs.cn

Go:   arr = append([]int{0}, arr...)
来源：http://up.szsharing.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jb.jctech888.com.cn

C#:   list.Insert(0, 0);
来源：http://nt.521024.cn

[D04] 删除元素
来源：http://by.szsharing.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://et.asd995.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ms.shtwfgs.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wd.szxytkj.cn

TS:   arr.splice(0, 1);
来源：http://kb.hahajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pr.hahajie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://so.panjiajie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dc.hahajie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sh.huanxung.cn

[D05] 访问与修改元素
来源：http://lx.szxytkj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kv.bookmarksfly.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ch.shtwfgs.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jw.nicolike.cn

TS:   arr[0]; arr.at(-1);
来源：http://sr.szxytkj.cn

Java: list.get(0); list.set(0, 9);
来源：http://uv.gzmigu.cn

Go:   arr[0]; arr[0] = 9
来源：http://ws.wgjwhj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cc.yuexingan06.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bx.yuexingan06.cn

[D06] 数组长度
来源：http://ln.jctech888.com.cn

Py:   len(arr)
来源：http://qr.lnxyls.cn

PHP:  count($arr);
来源：http://zq.gzmigu.cn

JS:   arr.length
来源：http://lm.chemitech.net.cn

TS:   arr.length
来源：http://oh.haigaiapp.cn

Java: list.size();
来源：http://po.shxzukj.cn

Go:   len(arr)
来源：http://xx.shxzukj.cn

Ruby: arr.length; arr.size
来源：http://tb.bookmarksfly.cn

C#:   list.Count;
来源：http://ol.shxzskj.cn

[D07] 切片 / 取子数组
来源：http://cu.chemitech.net.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mi.nicolike.cn

PHP:  array_slice($arr, 1, 3);
来源：http://mk.yuntaijiaju.cn

JS:   arr.slice(1, 4);
来源：http://qh.gzmigu.cn

TS:   arr.slice(1, 4);
来源：http://vh.lnxyls.cn

Java: list.subList(1, 4);
来源：http://is.huixiangedu.cn

Go:   arr[1:4]
来源：http://za.gzmigu.cn

Ruby: arr[1, 3]
来源：http://qs.gzmigu.cn

C#:   list.GetRange(1, 3);
来源：http://oj.colortex.cn

[D08] 合并两个数组
来源：http://ts.asd995.cn

Py:   a + b;  a.extend(b)
来源：http://iw.huanxung.cn

PHP:  array_merge($a, $b);
来源：http://cn.nszjky.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://kn.szsharing.cn

TS:   [...a, ...b];
来源：http://ra.yuexingan06.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fq.wgjwhj.cn

Go:   append(a, b...)
来源：http://cj.nicolike.cn

Ruby: a + b;  a.concat(b)
来源：http://ty.szxytkj.cn

C#:   a.Concat(b).ToList()
来源：http://xu.wgjwhj.cn

[D09] 排序（升序）
来源：http://pb.huixinmuqiang.cn

Py:   sorted(arr);  arr.sort()
来源：http://xu.521024.cn

PHP:  sort($arr);
来源：http://rx.bjjhwx.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nb.wgjwhj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://sl.bjjhwx.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://od.colortex.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ir.hnjuh.cn

Ruby: arr.sort
来源：http://ec.huixiangedu.cn

C#:   list.Sort();
来源：http://qf.521024.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://lr.9csxet.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cn.hnjuh.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eq.szsharing.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ih.szsharing.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ju.yuntaijiaju.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ko.shxzukj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wv.lnxyls.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kz.9csxet.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ap.jianghongdianzi.cn

[D11] 反转数组
来源：http://yc.panjiajie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xg.bookmarksfly.cn

PHP:  array_reverse($arr);
来源：http://fi.panjiajie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ac.lnxyls.cn

TS:   [...arr].reverse();
来源：http://zb.lnxyls.cn

Java: Collections.reverse(list);
来源：http://lr.shtwfgs.cn

Go:   slices.Reverse(arr)
来源：http://oz.bookmarksfly.cn

Ruby: arr.reverse
来源：http://jr.yuntaijiaju.cn

C#:   list.Reverse();
来源：http://nn.gzmigu.cn

[D12] 查找元素下标
来源：http://cp.yuexingan06.cn

Py:   arr.index(x);  x in arr
来源：http://lb.shxzukj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ch.colortex.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gk.yuntaijiaju.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fo.hahajie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yc.colortex.cn

Go:   slices.Index(arr, x)
来源：http://tj.newstarts.cn

Ruby: arr.index(x)
来源：http://hf.panjiajie.cn

C#:   list.IndexOf(x);
来源：http://ej.hahajie.cn

[D13] 过滤（保留满足条件的）
来源：http://fe.chemitech.net.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tg.hnjuh.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tw.shxzukj.cn

JS:   arr.filter(x => x > 3)
来源：http://vg.newstarts.cn

TS:   arr.filter(x => x > 3)
来源：http://xa.shxzukj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zd.szsharing.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yp.colortex.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fo.huixinmuqiang.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://oj.muxihuayi.cn

[D14] 映射转换（每个元素变形）
来源：http://bq.yuntaijiaju.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gb.szxytkj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qm.shxzskj.cn

JS:   arr.map(x => x * 2)
来源：http://dg.bookmarksfly.cn

TS:   arr.map(x => x * 2)
来源：http://xt.bjjhwx.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://vl.bookmarksfly.cn

Go:   // 手写循环
来源：http://nc.colortex.cn

Ruby: arr.map { |x| x * 2 }
来源：http://kz.gzmigu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://uf.szxytkj.cn

[D15] 去重
来源：http://kd.huixiangedu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ku.asd995.cn

PHP:  array_unique($arr);
来源：http://tp.bookmarksfly.cn

JS:   [...new Set(arr)]
来源：http://hv.yuexingan06.cn

TS:   [...new Set(arr)]
来源：http://al.szsharing.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wz.hnjuh.cn

Go:   // 用 map[T]struct{} 手写
来源：http://um.nicolike.cn

Ruby: arr.uniq
来源：http://hj.hahajie.cn

C#:   list.Distinct().ToList()
来源：http://vy.colortex.cn

[D16] 求和与平均值
来源：http://ou.wgjwhj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qz.asd995.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wj.szsharing.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ds.chemitech.net.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kf.shtwfgs.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hd.shxzukj.cn

Go:   // 手写循环累加
来源：http://cp.9csxet.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fb.hahajie.cn

C#:   list.Sum();  list.Average()
来源：http://ot.shxzskj.cn

[D17] 最大值与最小值
来源：http://fr.9csxet.cn

Py:   max(arr);  min(arr)
来源：http://td.newstarts.cn

PHP:  max($arr);  min($arr);
来源：http://wl.shxzskj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gu.chemitech.net.cn

TS:   Math.max(...arr);
来源：http://hp.panjiajie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://rp.asd995.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://du.wgjwhj.cn

Ruby: arr.max;  arr.min
来源：http://au.wgjwhj.cn

C#:   list.Max();  list.Min()
来源：http://nm.huanxung.cn

[D18] 扁平化嵌套数组
来源：http://ob.bjjhwx.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gc.hnjuh.cn

PHP:  array_merge(...$nested);
来源：http://gy.nicolike.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zb.hnjuh.cn

TS:   nested.flat();
来源：http://bs.huixiangedu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yd.nszjky.cn

Go:   // 手写双层循环
来源：http://oz.asd995.cn

Ruby: nested.flatten
来源：http://vo.bookmarksfly.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hd.hnjuh.cn

[D19] 按字段分组
来源：http://zq.9csxet.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://le.colortex.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://em.asd995.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ia.wgjwhj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://hu.hahajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ez.hahajie.cn

Go:   // 手写 map[string][]T
来源：http://qr.nicolike.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://gb.bjjhwx.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ja.yuntaijiaju.cn

[D20] 统计每个元素出现次数
来源：http://di.wgjwhj.cn

Py:   Counter(arr)
来源：http://st.szsharing.cn

PHP:  array_count_values($arr);
来源：http://hy.hahajie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sn.panjiajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pn.huixinmuqiang.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://be.shxzskj.cn

Go:   // 手写 map[T]int
来源：http://iy.bjjhwx.cn

Ruby: arr.tally
来源：http://cl.szxytkj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vx.bjjhwx.cn

[D21] 判断是否包含某元素
来源：http://xh.haigaiapp.cn

Py:   x in arr
来源：http://vd.huixinmuqiang.cn

PHP:  in_array($x, $arr, true);
来源：http://vh.9csxet.cn

JS:   arr.includes(x)
来源：http://et.lnxyls.cn

TS:   arr.includes(x)
来源：http://hk.shtwfgs.cn

Java: list.contains(x)
来源：http://dp.huanxung.cn

Go:   slices.Contains(arr, x)
来源：http://jh.521024.cn

Ruby: arr.include?(x)
来源：http://jz.shtwfgs.cn

C#:   list.Contains(x)
来源：http://qy.szsharing.cn

[D22] 复制数组（避免共享引用）
来源：http://ne.chemitech.net.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yr.huixiangedu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rg.nicolike.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fg.muxihuayi.cn

TS:   [...arr];
来源：http://xm.chemitech.net.cn

Java: new ArrayList<>(list);
来源：http://ux.jianghongdianzi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://bh.panjiajie.cn

Ruby: arr.dup;  arr.clone
来源：http://bl.szxytkj.cn

C#:   new List<int>(list);
来源：http://zd.wgjwhj.cn

[D23] reduce 累积计算
来源：http://qp.yuexingan06.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://as.chemitech.net.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ez.shxzukj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kg.521024.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ng.9csxet.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://so.jianghongdianzi.cn

Go:   // 手写循环
来源：http://xs.hahajie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uh.jctech888.com.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lv.huixinmuqiang.cn

[D24] 字典 / Map 基本操作
来源：http://nd.muxihuayi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bz.shxzskj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dm.wgjwhj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://me.nicolike.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nk.bookmarksfly.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xc.521024.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://iz.haigaiapp.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kc.jctech888.com.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://df.yuntaijiaju.cn

[D25] Set 集合去重与交并差
来源：http://rv.shxzukj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://sa.haigaiapp.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pw.huanxung.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ic.nicolike.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gy.newstarts.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zi.9csxet.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bw.shxzskj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://oz.huixiangedu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dt.wgjwhj.cn

[D26] 数组转字符串
来源：http://cb.gzmigu.cn

Py:   ", ".join(map(str, arr))
来源：http://ay.newstarts.cn

PHP:  implode(", ", $arr);
来源：http://qj.521024.cn

JS:   arr.join(", ")
来源：http://as.muxihuayi.cn

TS:   arr.join(", ")
来源：http://fa.shtwfgs.cn

Java: String.join(", ", list)
来源：http://ts.huanxung.cn

Go:   strings.Join(strs, ", ")
来源：http://iv.haigaiapp.cn

Ruby: arr.join(", ")
来源：http://tp.bjjhwx.cn

C#:   string.Join(", ", list)
来源：http://ml.huanxung.cn

================================================================================
来源：http://oc.yuexingan06.cn

E. 字符串处理
来源：http://bp.nicolike.cn

================================================================================
来源：http://dx.szxytkj.cn

[E01] 拼接字符串
来源：http://ze.newstarts.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ep.lnxyls.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jm.yuntaijiaju.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://sm.huanxung.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pm.wgjwhj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hg.szxytkj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://st.asd995.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kr.nszjky.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ri.shxzukj.cn

[E02] 重复字符串
来源：http://tt.yuntaijiaju.cn

Py:   "ab" * 3
来源：http://sc.nicolike.cn

PHP:  str_repeat("ab", 3);
来源：http://zf.yuntaijiaju.cn

JS:   "ab".repeat(3)
来源：http://cc.bjjhwx.cn

TS:   "ab".repeat(3)
来源：http://zt.szxytkj.cn

Java: "ab".repeat(3)
来源：http://fb.shxzskj.cn

Go:   strings.Repeat("ab", 3)
来源：http://ot.szsharing.cn

Ruby: "ab" * 3
来源：http://da.szxytkj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yo.huanxung.cn

[E03] 截取子串
来源：http://fs.chemitech.net.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ur.shxzukj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tf.panjiajie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qc.jctech888.com.cn

TS:   s.slice(1, 4)
来源：http://da.9csxet.cn

Java: s.substring(1, 4)
来源：http://ke.colortex.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://au.yuexingan06.cn

Ruby: s[1, 3];  s[1..3]
来源：http://tc.muxihuayi.cn

C#:   s.Substring(1, 3)
来源：http://px.panjiajie.cn

[E04] 查找子串位置
来源：http://ir.asd995.cn

Py:   s.find("x");  s.index("x")
来源：http://ad.szsharing.cn

PHP:  strpos($s, "x");
来源：http://ub.szsharing.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cp.521024.cn

TS:   s.indexOf("x")
来源：http://ha.hahajie.cn

Java: s.indexOf("x")
来源：http://ot.gzmigu.cn

Go:   strings.Index(s, "x")
来源：http://fb.yuntaijiaju.cn

Ruby: s.index("x")
来源：http://hh.shtwfgs.cn

C#:   s.IndexOf("x")
来源：http://om.wgjwhj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xc.huixiangedu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zd.huanxung.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ud.shxzukj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ad.huixiangedu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://mo.szsharing.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ho.nszjky.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://al.lnxyls.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ps.muxihuayi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vs.shxzukj.cn

[E06] 替换子串
来源：http://ek.jianghongdianzi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xj.shxzukj.cn

PHP:  str_replace("a", "b", $s);
来源：http://so.shxzskj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oc.huixiangedu.cn

TS:   s.replaceAll("a", "b")
来源：http://tb.521024.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vg.szxytkj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sl.newstarts.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://oe.bookmarksfly.cn

C#:   s.Replace("a", "b")
来源：http://sm.huixiangedu.cn

[E07] 按分隔符拆分
来源：http://cc.hnjuh.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ie.shxzskj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zk.szxytkj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://dg.yuntaijiaju.cn

TS:   s.split(",")
来源：http://ba.wgjwhj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://er.bjjhwx.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://st.hahajie.cn

Ruby: s.split(",");  s.split
来源：http://jy.newstarts.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kd.lnxyls.cn

[E08] 数组按分隔符合并
来源：http://id.chemitech.net.cn

Py:   ",".join(items)
来源：http://bx.bjjhwx.cn

PHP:  implode(",", $items);
来源：http://rx.9csxet.cn

JS:   items.join(",")
来源：http://cb.huixiangedu.cn

TS:   items.join(",")
来源：http://jd.huixinmuqiang.cn

Java: String.join(",", items)
来源：http://bp.haigaiapp.cn

Go:   strings.Join(items, ",")
来源：http://eo.szxytkj.cn

Ruby: items.join(",")
来源：http://fp.huixinmuqiang.cn

C#:   string.Join(",", items)
来源：http://hz.shxzskj.cn

[E09] 去除所有空白字符
来源：http://hp.yuntaijiaju.cn


<!-- 参考信息 -->