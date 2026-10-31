代发 wailian999

[D03] 在指定位置插入元素
来源：http://kr.521024.cn

Py:   arr.insert(0, 0)
来源：http://qr.hnjuh.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://es.nszjky.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mc.yuexingan06.cn

TS:   arr.splice(0, 0, 0);
来源：http://lp.huixinmuqiang.cn

Java: list.add(0, 0);
来源：http://ao.shxzskj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://zf.yuexingan06.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uq.nszjky.cn

C#:   list.Insert(0, 0);
来源：http://mj.panjiajie.cn

[D04] 删除元素
来源：http://dj.yuexingan06.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uo.hnjuh.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://du.asd995.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vc.hnjuh.cn

TS:   arr.splice(0, 1);
来源：http://fa.hahajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jy.colortex.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://so.jianghongdianzi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pc.shxzukj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://iu.szsharing.cn

[D05] 访问与修改元素
来源：http://pd.hahajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xp.lnxyls.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wj.jctech888.com.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ml.lnxyls.cn

TS:   arr[0]; arr.at(-1);
来源：http://oc.panjiajie.cn

Java: list.get(0); list.set(0, 9);
来源：http://zb.huixiangedu.cn

Go:   arr[0]; arr[0] = 9
来源：http://cs.chemitech.net.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pe.bookmarksfly.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kt.521024.cn

[D06] 数组长度
来源：http://pm.jianghongdianzi.cn

Py:   len(arr)
来源：http://qx.nicolike.cn

PHP:  count($arr);
来源：http://uc.bookmarksfly.cn

JS:   arr.length
来源：http://px.huixinmuqiang.cn

TS:   arr.length
来源：http://hi.hahajie.cn

Java: list.size();
来源：http://ve.muxihuayi.cn

Go:   len(arr)
来源：http://hu.haigaiapp.cn

Ruby: arr.length; arr.size
来源：http://su.nszjky.cn

C#:   list.Count;
来源：http://zr.shtwfgs.cn

[D07] 切片 / 取子数组
来源：http://bj.nszjky.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dd.huixinmuqiang.cn

PHP:  array_slice($arr, 1, 3);
来源：http://fw.huanxung.cn

JS:   arr.slice(1, 4);
来源：http://ib.wgjwhj.cn

TS:   arr.slice(1, 4);
来源：http://sk.yuexingan06.cn

Java: list.subList(1, 4);
来源：http://ud.muxihuayi.cn

Go:   arr[1:4]
来源：http://wp.chemitech.net.cn

Ruby: arr[1, 3]
来源：http://do.muxihuayi.cn

C#:   list.GetRange(1, 3);
来源：http://sb.jianghongdianzi.cn

[D08] 合并两个数组
来源：http://mr.jctech888.com.cn

Py:   a + b;  a.extend(b)
来源：http://dh.nicolike.cn

PHP:  array_merge($a, $b);
来源：http://wb.jctech888.com.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://cs.huanxung.cn

TS:   [...a, ...b];
来源：http://ek.szsharing.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rx.bookmarksfly.cn

Go:   append(a, b...)
来源：http://cd.gzmigu.cn

Ruby: a + b;  a.concat(b)
来源：http://cy.huixinmuqiang.cn

C#:   a.Concat(b).ToList()
来源：http://hd.newstarts.cn

[D09] 排序（升序）
来源：http://ob.huixiangedu.cn

Py:   sorted(arr);  arr.sort()
来源：http://iy.newstarts.cn

PHP:  sort($arr);
来源：http://nq.shxzukj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://im.colortex.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://by.hahajie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://yj.bjjhwx.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ly.bookmarksfly.cn

Ruby: arr.sort
来源：http://km.haigaiapp.cn

C#:   list.Sort();
来源：http://pb.szsharing.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://wa.huixinmuqiang.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dt.jianghongdianzi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wy.colortex.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://de.szsharing.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mz.bookmarksfly.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mp.9csxet.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ht.shxzskj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lf.bookmarksfly.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://es.nicolike.cn

[D11] 反转数组
来源：http://tz.newstarts.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ky.bookmarksfly.cn

PHP:  array_reverse($arr);
来源：http://sq.colortex.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kp.szsharing.cn

TS:   [...arr].reverse();
来源：http://ea.muxihuayi.cn

Java: Collections.reverse(list);
来源：http://wv.newstarts.cn

Go:   slices.Reverse(arr)
来源：http://mu.yuexingan06.cn

Ruby: arr.reverse
来源：http://bz.hnjuh.cn

C#:   list.Reverse();
来源：http://pg.bjjhwx.cn

[D12] 查找元素下标
来源：http://ku.521024.cn

Py:   arr.index(x);  x in arr
来源：http://xt.hnjuh.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://sb.jctech888.com.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ro.szsharing.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oa.muxihuayi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ao.chemitech.net.cn

Go:   slices.Index(arr, x)
来源：http://ib.shxzukj.cn

Ruby: arr.index(x)
来源：http://bo.jianghongdianzi.cn

C#:   list.IndexOf(x);
来源：http://ag.muxihuayi.cn

[D13] 过滤（保留满足条件的）
来源：http://iu.hahajie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wl.newstarts.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hh.newstarts.cn

JS:   arr.filter(x => x > 3)
来源：http://uo.huixiangedu.cn

TS:   arr.filter(x => x > 3)
来源：http://lo.hnjuh.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fk.jianghongdianzi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://up.shxzskj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://jc.shxzukj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://im.shxzskj.cn

[D14] 映射转换（每个元素变形）
来源：http://pc.chemitech.net.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tj.huixiangedu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lq.jctech888.com.cn

JS:   arr.map(x => x * 2)
来源：http://zn.wgjwhj.cn

TS:   arr.map(x => x * 2)
来源：http://mx.hnjuh.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://xj.asd995.cn

Go:   // 手写循环
来源：http://ku.yuexingan06.cn

Ruby: arr.map { |x| x * 2 }
来源：http://aq.colortex.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ps.newstarts.cn

[D15] 去重
来源：http://tb.szxytkj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://in.huanxung.cn

PHP:  array_unique($arr);
来源：http://qx.shxzskj.cn

JS:   [...new Set(arr)]
来源：http://tk.szxytkj.cn

TS:   [...new Set(arr)]
来源：http://bq.hnjuh.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vd.hnjuh.cn

Go:   // 用 map[T]struct{} 手写
来源：http://hg.wgjwhj.cn

Ruby: arr.uniq
来源：http://ng.gzmigu.cn

C#:   list.Distinct().ToList()
来源：http://ly.panjiajie.cn

[D16] 求和与平均值
来源：http://yg.shtwfgs.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nv.szxytkj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fe.9csxet.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://df.muxihuayi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tu.colortex.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://oc.gzmigu.cn

Go:   // 手写循环累加
来源：http://uy.newstarts.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://si.hnjuh.cn

C#:   list.Sum();  list.Average()
来源：http://ug.panjiajie.cn

[D17] 最大值与最小值
来源：http://rl.huixiangedu.cn

Py:   max(arr);  min(arr)
来源：http://kr.newstarts.cn

PHP:  max($arr);  min($arr);
来源：http://ih.szxytkj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rq.szsharing.cn

TS:   Math.max(...arr);
来源：http://pm.gzmigu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://lx.huixinmuqiang.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zg.hahajie.cn

Ruby: arr.max;  arr.min
来源：http://bf.yuexingan06.cn

C#:   list.Max();  list.Min()
来源：http://ct.panjiajie.cn

[D18] 扁平化嵌套数组
来源：http://yw.szsharing.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ii.szsharing.cn

PHP:  array_merge(...$nested);
来源：http://vz.gzmigu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wa.asd995.cn

TS:   nested.flat();
来源：http://bj.newstarts.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://uw.newstarts.cn

Go:   // 手写双层循环
来源：http://da.9csxet.cn

Ruby: nested.flatten
来源：http://gd.huixinmuqiang.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ku.shxzukj.cn

[D19] 按字段分组
来源：http://lo.huixiangedu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yz.bookmarksfly.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://db.asd995.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dl.huixinmuqiang.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ih.huixinmuqiang.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gb.asd995.cn

Go:   // 手写 map[string][]T
来源：http://is.9csxet.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://pe.shxzukj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ou.jianghongdianzi.cn

[D20] 统计每个元素出现次数
来源：http://jb.chemitech.net.cn

Py:   Counter(arr)
来源：http://ob.nicolike.cn

PHP:  array_count_values($arr);
来源：http://sh.nszjky.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ie.haigaiapp.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xz.szxytkj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bd.gzmigu.cn

Go:   // 手写 map[T]int
来源：http://ba.shtwfgs.cn

Ruby: arr.tally
来源：http://nb.wgjwhj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sf.chemitech.net.cn

[D21] 判断是否包含某元素
来源：http://on.szsharing.cn

Py:   x in arr
来源：http://xz.lnxyls.cn

PHP:  in_array($x, $arr, true);
来源：http://vp.newstarts.cn

JS:   arr.includes(x)
来源：http://rn.colortex.cn

TS:   arr.includes(x)
来源：http://jf.bookmarksfly.cn

Java: list.contains(x)
来源：http://hn.huixinmuqiang.cn

Go:   slices.Contains(arr, x)
来源：http://ki.wgjwhj.cn

Ruby: arr.include?(x)
来源：http://dg.szxytkj.cn

C#:   list.Contains(x)
来源：http://dp.nicolike.cn

[D22] 复制数组（避免共享引用）
来源：http://zg.gzmigu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nm.lnxyls.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yn.nszjky.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tl.jctech888.com.cn

TS:   [...arr];
来源：http://db.bjjhwx.cn

Java: new ArrayList<>(list);
来源：http://fm.muxihuayi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://pw.bjjhwx.cn

Ruby: arr.dup;  arr.clone
来源：http://me.jianghongdianzi.cn

C#:   new List<int>(list);
来源：http://uo.chemitech.net.cn

[D23] reduce 累积计算
来源：http://gn.nszjky.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bv.newstarts.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nx.bjjhwx.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ov.chemitech.net.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ap.gzmigu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://tt.wgjwhj.cn

Go:   // 手写循环
来源：http://bs.gzmigu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fv.yuexingan06.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nt.bjjhwx.cn

[D24] 字典 / Map 基本操作
来源：http://hr.shxzskj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rp.shxzukj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ux.shtwfgs.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ax.huixiangedu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://th.shtwfgs.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nq.huixinmuqiang.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wr.haigaiapp.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://sd.huanxung.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mb.szsharing.cn

[D25] Set 集合去重与交并差
来源：http://ss.chemitech.net.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xw.hahajie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rg.colortex.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yy.asd995.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://up.huanxung.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xi.nicolike.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://uj.jctech888.com.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ge.nszjky.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vs.huixiangedu.cn

[D26] 数组转字符串
来源：http://gd.wgjwhj.cn

Py:   ", ".join(map(str, arr))
来源：http://cx.wgjwhj.cn

PHP:  implode(", ", $arr);
来源：http://gr.szsharing.cn

JS:   arr.join(", ")
来源：http://sj.huixinmuqiang.cn

TS:   arr.join(", ")
来源：http://cq.jctech888.com.cn

Java: String.join(", ", list)
来源：http://xk.shxzskj.cn

Go:   strings.Join(strs, ", ")
来源：http://al.521024.cn

Ruby: arr.join(", ")
来源：http://tf.chemitech.net.cn

C#:   string.Join(", ", list)
来源：http://tk.bookmarksfly.cn

================================================================================
来源：http://bi.nicolike.cn

E. 字符串处理
来源：http://us.newstarts.cn

================================================================================
来源：http://ou.hahajie.cn

[E01] 拼接字符串
来源：http://hy.newstarts.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nh.newstarts.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sl.shtwfgs.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cf.newstarts.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ih.nicolike.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gc.521024.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dw.chemitech.net.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wr.jctech888.com.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kn.shtwfgs.cn

[E02] 重复字符串
来源：http://rc.huixiangedu.cn

Py:   "ab" * 3
来源：http://us.szsharing.cn

PHP:  str_repeat("ab", 3);
来源：http://ld.newstarts.cn

JS:   "ab".repeat(3)
来源：http://az.9csxet.cn

TS:   "ab".repeat(3)
来源：http://fd.9csxet.cn

Java: "ab".repeat(3)
来源：http://ro.szsharing.cn

Go:   strings.Repeat("ab", 3)
来源：http://bq.newstarts.cn

Ruby: "ab" * 3
来源：http://jc.nszjky.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://od.huixiangedu.cn

[E03] 截取子串
来源：http://il.muxihuayi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bi.lnxyls.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ju.szsharing.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://az.wgjwhj.cn

TS:   s.slice(1, 4)
来源：http://op.9csxet.cn

Java: s.substring(1, 4)
来源：http://ov.huixinmuqiang.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ye.jctech888.com.cn

Ruby: s[1, 3];  s[1..3]
来源：http://fl.wgjwhj.cn

C#:   s.Substring(1, 3)
来源：http://ds.huixinmuqiang.cn

[E04] 查找子串位置
来源：http://pi.shtwfgs.cn

Py:   s.find("x");  s.index("x")
来源：http://bh.shtwfgs.cn

PHP:  strpos($s, "x");
来源：http://sa.szsharing.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ja.wgjwhj.cn

TS:   s.indexOf("x")
来源：http://gx.newstarts.cn

Java: s.indexOf("x")
来源：http://uk.panjiajie.cn

Go:   strings.Index(s, "x")
来源：http://vl.jctech888.com.cn

Ruby: s.index("x")
来源：http://ap.yuntaijiaju.cn

C#:   s.IndexOf("x")
来源：http://mc.szxytkj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://he.yuexingan06.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://db.muxihuayi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rp.wgjwhj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ln.nszjky.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hr.wgjwhj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://by.yuexingan06.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cp.muxihuayi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zz.jianghongdianzi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://an.newstarts.cn

[E06] 替换子串
来源：http://ob.bookmarksfly.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cc.haigaiapp.cn

PHP:  str_replace("a", "b", $s);
来源：http://bv.asd995.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wp.jctech888.com.cn

TS:   s.replaceAll("a", "b")
来源：http://me.hnjuh.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ex.bjjhwx.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sb.bjjhwx.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zt.newstarts.cn

C#:   s.Replace("a", "b")
来源：http://al.nicolike.cn

[E07] 按分隔符拆分
来源：http://ic.jianghongdianzi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xt.newstarts.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tg.huixiangedu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://fx.shxzukj.cn

TS:   s.split(",")
来源：http://ga.panjiajie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://yz.hahajie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hv.huixiangedu.cn

Ruby: s.split(",");  s.split
来源：http://ls.gzmigu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://at.yuexingan06.cn

[E08] 数组按分隔符合并
来源：http://ct.muxihuayi.cn

Py:   ",".join(items)
来源：http://qc.lnxyls.cn

PHP:  implode(",", $items);
来源：http://qo.chemitech.net.cn

JS:   items.join(",")
来源：http://an.nicolike.cn

TS:   items.join(",")
来源：http://mr.chemitech.net.cn

Java: String.join(",", items)
来源：http://cm.jctech888.com.cn

Go:   strings.Join(items, ",")
来源：http://cj.nszjky.cn

Ruby: items.join(",")
来源：http://ut.newstarts.cn

C#:   string.Join(",", items)
来源：http://vx.shxzskj.cn

[E09] 去除所有空白字符
来源：http://sp.wgjwhj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nj.bookmarksfly.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://iy.nszjky.cn

JS:   s.replace(/\s+/g, "")
来源：http://jy.panjiajie.cn

TS:   s.replace(/\s+/g, "")
来源：http://iw.nicolike.cn

Java: s.replaceAll("\\s+", "")
来源：http://px.muxihuayi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://si.szsharing.cn

Ruby: s.gsub(/\s+/, "")
来源：http://hl.nicolike.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ax.bjjhwx.cn


<!-- 参考信息 -->