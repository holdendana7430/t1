代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://rw.newstarts.cn

Ruby: arr = [1, 2, 3]
来源：http://jv.shxzskj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ht.yuntaijiaju.cn

[D02] 追加元素到末尾
来源：http://sr.shxzskj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ob.bookmarksfly.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hl.asd995.cn

JS:   arr.push(4);
来源：http://fz.colortex.cn

TS:   arr.push(4);
来源：http://eu.lnxyls.cn

Java: list.add(4);
来源：http://wf.521024.cn

Go:   arr = append(arr, 4)
来源：http://et.chemitech.net.cn

Ruby: arr << 4; arr.push(5)
来源：http://dd.shtwfgs.cn

C#:   list.Add(4);
来源：http://ju.muxihuayi.cn

[D03] 在指定位置插入元素
来源：http://al.yuntaijiaju.cn

Py:   arr.insert(0, 0)
来源：http://yz.nicolike.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rn.huanxung.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kg.haigaiapp.cn

TS:   arr.splice(0, 0, 0);
来源：http://ex.wgjwhj.cn

Java: list.add(0, 0);
来源：http://wt.521024.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ks.panjiajie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://op.huixinmuqiang.cn

C#:   list.Insert(0, 0);
来源：http://ag.chemitech.net.cn

[D04] 删除元素
来源：http://tm.hahajie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xb.szxytkj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vk.nszjky.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jv.bookmarksfly.cn

TS:   arr.splice(0, 1);
来源：http://wy.colortex.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nb.huixinmuqiang.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pm.colortex.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://le.jianghongdianzi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://es.szsharing.cn

[D05] 访问与修改元素
来源：http://is.wgjwhj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://og.chemitech.net.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sf.521024.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mk.colortex.cn

TS:   arr[0]; arr.at(-1);
来源：http://gs.521024.cn

Java: list.get(0); list.set(0, 9);
来源：http://mm.szsharing.cn

Go:   arr[0]; arr[0] = 9
来源：http://gz.muxihuayi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wz.shxzukj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://te.huixiangedu.cn

[D06] 数组长度
来源：http://fc.521024.cn

Py:   len(arr)
来源：http://if.bjjhwx.cn

PHP:  count($arr);
来源：http://en.gzmigu.cn

JS:   arr.length
来源：http://qz.asd995.cn

TS:   arr.length
来源：http://cf.hahajie.cn

Java: list.size();
来源：http://bd.gzmigu.cn

Go:   len(arr)
来源：http://cj.9csxet.cn

Ruby: arr.length; arr.size
来源：http://wg.muxihuayi.cn

C#:   list.Count;
来源：http://zo.nicolike.cn

[D07] 切片 / 取子数组
来源：http://bv.yuexingan06.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vo.shtwfgs.cn

PHP:  array_slice($arr, 1, 3);
来源：http://br.nszjky.cn

JS:   arr.slice(1, 4);
来源：http://ax.huixiangedu.cn

TS:   arr.slice(1, 4);
来源：http://mm.shxzukj.cn

Java: list.subList(1, 4);
来源：http://ci.asd995.cn

Go:   arr[1:4]
来源：http://qn.panjiajie.cn

Ruby: arr[1, 3]
来源：http://dx.haigaiapp.cn

C#:   list.GetRange(1, 3);
来源：http://rh.bjjhwx.cn

[D08] 合并两个数组
来源：http://or.huixinmuqiang.cn

Py:   a + b;  a.extend(b)
来源：http://wn.asd995.cn

PHP:  array_merge($a, $b);
来源：http://vv.yuntaijiaju.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://pq.colortex.cn

TS:   [...a, ...b];
来源：http://qh.bjjhwx.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yj.panjiajie.cn

Go:   append(a, b...)
来源：http://uh.lnxyls.cn

Ruby: a + b;  a.concat(b)
来源：http://bo.huixinmuqiang.cn

C#:   a.Concat(b).ToList()
来源：http://qh.wgjwhj.cn

[D09] 排序（升序）
来源：http://bp.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://dz.yuntaijiaju.cn

PHP:  sort($arr);
来源：http://ie.jctech888.com.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tx.asd995.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fi.shtwfgs.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://dv.jctech888.com.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mt.chemitech.net.cn

Ruby: arr.sort
来源：http://ei.yuntaijiaju.cn

C#:   list.Sort();
来源：http://ac.yuntaijiaju.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://it.szsharing.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ab.huixiangedu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://up.haigaiapp.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vl.chemitech.net.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pw.asd995.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kx.yuexingan06.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ri.jctech888.com.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fi.haigaiapp.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://eo.jctech888.com.cn

[D11] 反转数组
来源：http://qr.bjjhwx.cn

Py:   arr[::-1];  arr.reverse()
来源：http://du.newstarts.cn

PHP:  array_reverse($arr);
来源：http://um.wgjwhj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pj.muxihuayi.cn

TS:   [...arr].reverse();
来源：http://ko.jctech888.com.cn

Java: Collections.reverse(list);
来源：http://mj.yuntaijiaju.cn

Go:   slices.Reverse(arr)
来源：http://ux.huanxung.cn

Ruby: arr.reverse
来源：http://by.wgjwhj.cn

C#:   list.Reverse();
来源：http://vx.szsharing.cn

[D12] 查找元素下标
来源：http://bc.shtwfgs.cn

Py:   arr.index(x);  x in arr
来源：http://xj.huixiangedu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kj.newstarts.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wt.lnxyls.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uh.hahajie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lo.jianghongdianzi.cn

Go:   slices.Index(arr, x)
来源：http://hn.asd995.cn

Ruby: arr.index(x)
来源：http://bg.9csxet.cn

C#:   list.IndexOf(x);
来源：http://ze.szsharing.cn

[D13] 过滤（保留满足条件的）
来源：http://mi.gzmigu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://aw.shtwfgs.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nx.haigaiapp.cn

JS:   arr.filter(x => x > 3)
来源：http://sh.szxytkj.cn

TS:   arr.filter(x => x > 3)
来源：http://ug.bookmarksfly.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zj.haigaiapp.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pi.hnjuh.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ec.shtwfgs.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://fq.jctech888.com.cn

[D14] 映射转换（每个元素变形）
来源：http://zz.hahajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yy.hnjuh.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rj.yuexingan06.cn

JS:   arr.map(x => x * 2)
来源：http://jn.shxzskj.cn

TS:   arr.map(x => x * 2)
来源：http://de.haigaiapp.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://bn.asd995.cn

Go:   // 手写循环
来源：http://dc.newstarts.cn

Ruby: arr.map { |x| x * 2 }
来源：http://pd.huixinmuqiang.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://bx.9csxet.cn

[D15] 去重
来源：http://zi.huanxung.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gr.shxzukj.cn

PHP:  array_unique($arr);
来源：http://on.lnxyls.cn

JS:   [...new Set(arr)]
来源：http://fn.jianghongdianzi.cn

TS:   [...new Set(arr)]
来源：http://yc.shxzskj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://oh.huanxung.cn

Go:   // 用 map[T]struct{} 手写
来源：http://nv.bookmarksfly.cn

Ruby: arr.uniq
来源：http://gd.colortex.cn

C#:   list.Distinct().ToList()
来源：http://ll.nicolike.cn

[D16] 求和与平均值
来源：http://hg.szsharing.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://du.wgjwhj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://eb.wgjwhj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zw.jianghongdianzi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xm.szsharing.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gt.haigaiapp.cn

Go:   // 手写循环累加
来源：http://gx.szxytkj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zl.hahajie.cn

C#:   list.Sum();  list.Average()
来源：http://jk.chemitech.net.cn

[D17] 最大值与最小值
来源：http://aa.wgjwhj.cn

Py:   max(arr);  min(arr)
来源：http://tf.gzmigu.cn

PHP:  max($arr);  min($arr);
来源：http://eq.bjjhwx.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nj.bjjhwx.cn

TS:   Math.max(...arr);
来源：http://hq.nszjky.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://lo.haigaiapp.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mo.lnxyls.cn

Ruby: arr.max;  arr.min
来源：http://id.haigaiapp.cn

C#:   list.Max();  list.Min()
来源：http://xp.lnxyls.cn

[D18] 扁平化嵌套数组
来源：http://mo.muxihuayi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ib.hnjuh.cn

PHP:  array_merge(...$nested);
来源：http://cu.shtwfgs.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cv.nicolike.cn

TS:   nested.flat();
来源：http://tp.nicolike.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yl.muxihuayi.cn

Go:   // 手写双层循环
来源：http://wo.wgjwhj.cn

Ruby: nested.flatten
来源：http://qc.wgjwhj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ks.haigaiapp.cn

[D19] 按字段分组
来源：http://we.chemitech.net.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ce.panjiajie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yf.hahajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ar.muxihuayi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://cx.wgjwhj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ws.yuexingan06.cn

Go:   // 手写 map[string][]T
来源：http://kh.chemitech.net.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://vv.gzmigu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bv.yuexingan06.cn

[D20] 统计每个元素出现次数
来源：http://yz.hahajie.cn

Py:   Counter(arr)
来源：http://md.yuexingan06.cn

PHP:  array_count_values($arr);
来源：http://mx.wgjwhj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fl.huanxung.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ud.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://it.yuntaijiaju.cn

Go:   // 手写 map[T]int
来源：http://qh.shxzskj.cn

Ruby: arr.tally
来源：http://ti.haigaiapp.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ya.szsharing.cn

[D21] 判断是否包含某元素
来源：http://aa.nicolike.cn

Py:   x in arr
来源：http://kp.bookmarksfly.cn

PHP:  in_array($x, $arr, true);
来源：http://yk.hahajie.cn

JS:   arr.includes(x)
来源：http://as.bookmarksfly.cn

TS:   arr.includes(x)
来源：http://sf.wgjwhj.cn

Java: list.contains(x)
来源：http://mq.shtwfgs.cn

Go:   slices.Contains(arr, x)
来源：http://ri.hnjuh.cn

Ruby: arr.include?(x)
来源：http://qc.yuexingan06.cn

C#:   list.Contains(x)
来源：http://xf.newstarts.cn

[D22] 复制数组（避免共享引用）
来源：http://hw.521024.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cn.jianghongdianzi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ir.nszjky.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ei.colortex.cn

TS:   [...arr];
来源：http://gy.hnjuh.cn

Java: new ArrayList<>(list);
来源：http://ys.yuexingan06.cn

Go:   copied := append([]int(nil), arr...)
来源：http://kx.521024.cn

Ruby: arr.dup;  arr.clone
来源：http://jk.lnxyls.cn

C#:   new List<int>(list);
来源：http://ew.shtwfgs.cn

[D23] reduce 累积计算
来源：http://ih.jianghongdianzi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bb.huixiangedu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://sm.hahajie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gc.newstarts.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gb.lnxyls.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ju.jctech888.com.cn

Go:   // 手写循环
来源：http://kk.lnxyls.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xb.jctech888.com.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mw.chemitech.net.cn

[D24] 字典 / Map 基本操作
来源：http://gw.yuexingan06.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dz.521024.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ik.bjjhwx.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wr.shxzukj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://la.szxytkj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://of.wgjwhj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://an.gzmigu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gu.nicolike.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jf.nicolike.cn

[D25] Set 集合去重与交并差
来源：http://ux.yuntaijiaju.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fi.szsharing.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fj.hahajie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ls.huixiangedu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://iq.bookmarksfly.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nw.huixiangedu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hd.yuntaijiaju.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qn.shxzskj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tp.haigaiapp.cn

[D26] 数组转字符串
来源：http://pi.nicolike.cn

Py:   ", ".join(map(str, arr))
来源：http://ul.hnjuh.cn

PHP:  implode(", ", $arr);
来源：http://pq.shxzskj.cn

JS:   arr.join(", ")
来源：http://ar.yuntaijiaju.cn

TS:   arr.join(", ")
来源：http://tf.wgjwhj.cn

Java: String.join(", ", list)
来源：http://ql.muxihuayi.cn

Go:   strings.Join(strs, ", ")
来源：http://hy.521024.cn

Ruby: arr.join(", ")
来源：http://zx.szxytkj.cn

C#:   string.Join(", ", list)
来源：http://mn.yuntaijiaju.cn

================================================================================
来源：http://cm.shxzukj.cn

E. 字符串处理
来源：http://yh.newstarts.cn

================================================================================
来源：http://mi.nicolike.cn

[E01] 拼接字符串
来源：http://ds.nicolike.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ie.gzmigu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qp.szsharing.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zt.jianghongdianzi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wz.bookmarksfly.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://se.asd995.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xm.shtwfgs.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ot.panjiajie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vu.nicolike.cn

[E02] 重复字符串
来源：http://db.yuexingan06.cn

Py:   "ab" * 3
来源：http://lc.shxzukj.cn

PHP:  str_repeat("ab", 3);
来源：http://vy.gzmigu.cn

JS:   "ab".repeat(3)
来源：http://is.hahajie.cn

TS:   "ab".repeat(3)
来源：http://rd.panjiajie.cn

Java: "ab".repeat(3)
来源：http://ck.shxzukj.cn

Go:   strings.Repeat("ab", 3)
来源：http://fq.newstarts.cn

Ruby: "ab" * 3
来源：http://nw.yuexingan06.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zb.yuexingan06.cn

[E03] 截取子串
来源：http://ud.bookmarksfly.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ni.yuntaijiaju.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://aw.shxzskj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://js.haigaiapp.cn

TS:   s.slice(1, 4)
来源：http://ei.yuntaijiaju.cn

Java: s.substring(1, 4)
来源：http://rp.gzmigu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bk.hnjuh.cn

Ruby: s[1, 3];  s[1..3]
来源：http://fx.wgjwhj.cn

C#:   s.Substring(1, 3)
来源：http://ev.521024.cn

[E04] 查找子串位置
来源：http://zw.jianghongdianzi.cn

Py:   s.find("x");  s.index("x")
来源：http://ab.yuntaijiaju.cn

PHP:  strpos($s, "x");
来源：http://wh.szxytkj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sj.szsharing.cn

TS:   s.indexOf("x")
来源：http://tj.bookmarksfly.cn

Java: s.indexOf("x")
来源：http://hg.521024.cn

Go:   strings.Index(s, "x")
来源：http://ph.yuntaijiaju.cn

Ruby: s.index("x")
来源：http://yw.bjjhwx.cn

C#:   s.IndexOf("x")
来源：http://hl.asd995.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://nb.panjiajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ue.szsharing.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ue.9csxet.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bt.jianghongdianzi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://rn.szsharing.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nc.chemitech.net.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://oi.huixinmuqiang.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vg.jianghongdianzi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cz.yuexingan06.cn

[E06] 替换子串
来源：http://yd.yuexingan06.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tm.panjiajie.cn

PHP:  str_replace("a", "b", $s);
来源：http://ne.shxzskj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://db.521024.cn

TS:   s.replaceAll("a", "b")
来源：http://em.chemitech.net.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ay.szsharing.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://or.panjiajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bw.bookmarksfly.cn

C#:   s.Replace("a", "b")
来源：http://qz.yuexingan06.cn

[E07] 按分隔符拆分
来源：http://ky.521024.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qj.nicolike.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fj.shxzukj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://hl.haigaiapp.cn

TS:   s.split(",")
来源：http://vu.wgjwhj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://wq.shxzukj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bo.huanxung.cn

Ruby: s.split(",");  s.split
来源：http://ao.shtwfgs.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ko.chemitech.net.cn

[E08] 数组按分隔符合并
来源：http://pi.shxzukj.cn

Py:   ",".join(items)
来源：http://yb.bjjhwx.cn

PHP:  implode(",", $items);
来源：http://xg.bjjhwx.cn

JS:   items.join(",")
来源：http://hc.nicolike.cn

TS:   items.join(",")
来源：http://ei.yuexingan06.cn

Java: String.join(",", items)
来源：http://lu.szxytkj.cn


<!-- 参考信息 -->