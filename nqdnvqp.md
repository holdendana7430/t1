代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://uq.huixinmuqiang.cn

Ruby: arr = [1, 2, 3]
来源：http://sq.9csxet.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://za.asd995.cn

[D02] 追加元素到末尾
来源：http://hw.huixiangedu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zk.bjjhwx.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wi.nicolike.cn

JS:   arr.push(4);
来源：http://mp.hnjuh.cn

TS:   arr.push(4);
来源：http://he.yuntaijiaju.cn

Java: list.add(4);
来源：http://jl.chemitech.net.cn

Go:   arr = append(arr, 4)
来源：http://wt.colortex.cn

Ruby: arr << 4; arr.push(5)
来源：http://eu.newstarts.cn

C#:   list.Add(4);
来源：http://um.bjjhwx.cn

[D03] 在指定位置插入元素
来源：http://lt.shtwfgs.cn

Py:   arr.insert(0, 0)
来源：http://zq.szsharing.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bf.muxihuayi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://sh.yuexingan06.cn

TS:   arr.splice(0, 0, 0);
来源：http://lu.hahajie.cn

Java: list.add(0, 0);
来源：http://sh.9csxet.cn

Go:   arr = append([]int{0}, arr...)
来源：http://et.hnjuh.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ug.shtwfgs.cn

C#:   list.Insert(0, 0);
来源：http://gu.shtwfgs.cn

[D04] 删除元素
来源：http://ri.shtwfgs.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ye.szsharing.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uc.lnxyls.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rr.asd995.cn

TS:   arr.splice(0, 1);
来源：http://xt.shtwfgs.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lv.jianghongdianzi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lp.yuntaijiaju.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xo.yuexingan06.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ln.shxzskj.cn

[D05] 访问与修改元素
来源：http://ts.nszjky.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://km.wgjwhj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sk.yuexingan06.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lq.nszjky.cn

TS:   arr[0]; arr.at(-1);
来源：http://uy.huixinmuqiang.cn

Java: list.get(0); list.set(0, 9);
来源：http://kf.szsharing.cn

Go:   arr[0]; arr[0] = 9
来源：http://et.huixinmuqiang.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ko.wgjwhj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ny.gzmigu.cn

[D06] 数组长度
来源：http://sg.shtwfgs.cn

Py:   len(arr)
来源：http://qw.yuexingan06.cn

PHP:  count($arr);
来源：http://wb.521024.cn

JS:   arr.length
来源：http://db.huanxung.cn

TS:   arr.length
来源：http://yb.haigaiapp.cn

Java: list.size();
来源：http://de.nicolike.cn

Go:   len(arr)
来源：http://ch.huixiangedu.cn

Ruby: arr.length; arr.size
来源：http://sw.wgjwhj.cn

C#:   list.Count;
来源：http://gk.muxihuayi.cn

[D07] 切片 / 取子数组
来源：http://vf.colortex.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ni.9csxet.cn

PHP:  array_slice($arr, 1, 3);
来源：http://np.yuexingan06.cn

JS:   arr.slice(1, 4);
来源：http://su.asd995.cn

TS:   arr.slice(1, 4);
来源：http://bb.nicolike.cn

Java: list.subList(1, 4);
来源：http://rc.bookmarksfly.cn

Go:   arr[1:4]
来源：http://sb.shxzskj.cn

Ruby: arr[1, 3]
来源：http://rz.wgjwhj.cn

C#:   list.GetRange(1, 3);
来源：http://mf.9csxet.cn

[D08] 合并两个数组
来源：http://rr.hnjuh.cn

Py:   a + b;  a.extend(b)
来源：http://mg.hnjuh.cn

PHP:  array_merge($a, $b);
来源：http://vl.szsharing.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://kd.yuexingan06.cn

TS:   [...a, ...b];
来源：http://mk.huixiangedu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://le.huixiangedu.cn

Go:   append(a, b...)
来源：http://ic.panjiajie.cn

Ruby: a + b;  a.concat(b)
来源：http://jw.haigaiapp.cn

C#:   a.Concat(b).ToList()
来源：http://qm.hahajie.cn

[D09] 排序（升序）
来源：http://ka.panjiajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://yd.colortex.cn

PHP:  sort($arr);
来源：http://ht.panjiajie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zw.9csxet.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://hy.haigaiapp.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://yz.9csxet.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gm.newstarts.cn

Ruby: arr.sort
来源：http://my.hnjuh.cn

C#:   list.Sort();
来源：http://tt.chemitech.net.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://av.wgjwhj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wc.521024.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tm.yuexingan06.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nc.colortex.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wy.muxihuayi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fj.muxihuayi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://to.newstarts.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://li.asd995.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wc.newstarts.cn

[D11] 反转数组
来源：http://so.huixiangedu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xe.bookmarksfly.cn

PHP:  array_reverse($arr);
来源：http://fl.9csxet.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pd.yuntaijiaju.cn

TS:   [...arr].reverse();
来源：http://ew.muxihuayi.cn

Java: Collections.reverse(list);
来源：http://vv.szsharing.cn

Go:   slices.Reverse(arr)
来源：http://sk.yuexingan06.cn

Ruby: arr.reverse
来源：http://om.panjiajie.cn

C#:   list.Reverse();
来源：http://zj.nicolike.cn

[D12] 查找元素下标
来源：http://qn.nicolike.cn

Py:   arr.index(x);  x in arr
来源：http://hq.521024.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cq.haigaiapp.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ud.haigaiapp.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ja.panjiajie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://et.panjiajie.cn

Go:   slices.Index(arr, x)
来源：http://gh.asd995.cn

Ruby: arr.index(x)
来源：http://fl.bjjhwx.cn

C#:   list.IndexOf(x);
来源：http://md.szsharing.cn

[D13] 过滤（保留满足条件的）
来源：http://pk.shxzskj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ge.bookmarksfly.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://st.newstarts.cn

JS:   arr.filter(x => x > 3)
来源：http://iq.asd995.cn

TS:   arr.filter(x => x > 3)
来源：http://ox.szxytkj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hy.shtwfgs.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ph.jctech888.com.cn

Ruby: arr.select { |x| x > 3 }
来源：http://nb.shxzskj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ow.asd995.cn

[D14] 映射转换（每个元素变形）
来源：http://lb.shxzukj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://va.szxytkj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rw.shxzskj.cn

JS:   arr.map(x => x * 2)
来源：http://pi.hnjuh.cn

TS:   arr.map(x => x * 2)
来源：http://sp.hahajie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ri.yuntaijiaju.cn

Go:   // 手写循环
来源：http://gc.yuntaijiaju.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fy.huanxung.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ko.shtwfgs.cn

[D15] 去重
来源：http://gm.haigaiapp.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nx.szsharing.cn

PHP:  array_unique($arr);
来源：http://as.szxytkj.cn

JS:   [...new Set(arr)]
来源：http://em.lnxyls.cn

TS:   [...new Set(arr)]
来源：http://jj.shxzukj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xg.bjjhwx.cn

Go:   // 用 map[T]struct{} 手写
来源：http://qo.panjiajie.cn

Ruby: arr.uniq
来源：http://yb.yuntaijiaju.cn

C#:   list.Distinct().ToList()
来源：http://kk.huixinmuqiang.cn

[D16] 求和与平均值
来源：http://fw.hnjuh.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://se.wgjwhj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hm.bjjhwx.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ha.newstarts.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lc.shxzskj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jg.wgjwhj.cn

Go:   // 手写循环累加
来源：http://tw.bjjhwx.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zy.lnxyls.cn

C#:   list.Sum();  list.Average()
来源：http://cu.hnjuh.cn

[D17] 最大值与最小值
来源：http://ax.nicolike.cn

Py:   max(arr);  min(arr)
来源：http://vw.wgjwhj.cn

PHP:  max($arr);  min($arr);
来源：http://xi.huanxung.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hl.9csxet.cn

TS:   Math.max(...arr);
来源：http://jv.shxzskj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://lw.9csxet.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vi.shtwfgs.cn

Ruby: arr.max;  arr.min
来源：http://eo.yuntaijiaju.cn

C#:   list.Max();  list.Min()
来源：http://kz.bookmarksfly.cn

[D18] 扁平化嵌套数组
来源：http://ep.shxzukj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cz.lnxyls.cn

PHP:  array_merge(...$nested);
来源：http://bk.hnjuh.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lk.jctech888.com.cn

TS:   nested.flat();
来源：http://ba.huanxung.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ru.panjiajie.cn

Go:   // 手写双层循环
来源：http://vm.nszjky.cn

Ruby: nested.flatten
来源：http://tq.chemitech.net.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://gy.huixiangedu.cn

[D19] 按字段分组
来源：http://iy.jctech888.com.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hw.yuexingan06.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://br.huixiangedu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wy.yuntaijiaju.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://vp.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nh.chemitech.net.cn

Go:   // 手写 map[string][]T
来源：http://hp.szxytkj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ee.nicolike.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://te.hahajie.cn

[D20] 统计每个元素出现次数
来源：http://vt.jctech888.com.cn

Py:   Counter(arr)
来源：http://xs.muxihuayi.cn

PHP:  array_count_values($arr);
来源：http://bg.jianghongdianzi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://me.colortex.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ba.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ov.wgjwhj.cn

Go:   // 手写 map[T]int
来源：http://bz.shtwfgs.cn

Ruby: arr.tally
来源：http://fx.newstarts.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sq.gzmigu.cn

[D21] 判断是否包含某元素
来源：http://qv.lnxyls.cn

Py:   x in arr
来源：http://pm.shxzskj.cn

PHP:  in_array($x, $arr, true);
来源：http://kw.gzmigu.cn

JS:   arr.includes(x)
来源：http://wy.jianghongdianzi.cn

TS:   arr.includes(x)
来源：http://jl.colortex.cn

Java: list.contains(x)
来源：http://gd.521024.cn

Go:   slices.Contains(arr, x)
来源：http://py.nicolike.cn

Ruby: arr.include?(x)
来源：http://cg.bjjhwx.cn

C#:   list.Contains(x)
来源：http://ej.chemitech.net.cn

[D22] 复制数组（避免共享引用）
来源：http://qv.haigaiapp.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kb.jctech888.com.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xr.colortex.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://by.yuexingan06.cn

TS:   [...arr];
来源：http://qo.521024.cn

Java: new ArrayList<>(list);
来源：http://ni.yuexingan06.cn

Go:   copied := append([]int(nil), arr...)
来源：http://zj.shxzskj.cn

Ruby: arr.dup;  arr.clone
来源：http://mf.yuexingan06.cn

C#:   new List<int>(list);
来源：http://oz.shxzskj.cn

[D23] reduce 累积计算
来源：http://mp.colortex.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rg.muxihuayi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ha.hahajie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://be.521024.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://og.szsharing.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://us.yuntaijiaju.cn

Go:   // 手写循环
来源：http://hi.jctech888.com.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ml.gzmigu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://aj.nszjky.cn

[D24] 字典 / Map 基本操作
来源：http://ca.asd995.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vk.wgjwhj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kn.shxzskj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ao.muxihuayi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ff.huixiangedu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://sz.gzmigu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dc.hnjuh.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nm.newstarts.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vi.gzmigu.cn

[D25] Set 集合去重与交并差
来源：http://qs.yuntaijiaju.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wt.asd995.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zt.haigaiapp.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tf.colortex.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tp.hahajie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tk.haigaiapp.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://uo.hahajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zk.521024.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fv.shxzskj.cn

[D26] 数组转字符串
来源：http://gb.yuntaijiaju.cn

Py:   ", ".join(map(str, arr))
来源：http://wr.bjjhwx.cn

PHP:  implode(", ", $arr);
来源：http://bd.newstarts.cn

JS:   arr.join(", ")
来源：http://ni.huixinmuqiang.cn

TS:   arr.join(", ")
来源：http://jd.521024.cn

Java: String.join(", ", list)
来源：http://cc.panjiajie.cn

Go:   strings.Join(strs, ", ")
来源：http://nz.shtwfgs.cn

Ruby: arr.join(", ")
来源：http://hw.521024.cn

C#:   string.Join(", ", list)
来源：http://fl.shtwfgs.cn

================================================================================
来源：http://sv.huanxung.cn

E. 字符串处理
来源：http://lu.nicolike.cn

================================================================================
来源：http://ui.jianghongdianzi.cn

[E01] 拼接字符串
来源：http://sv.asd995.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qx.bjjhwx.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://do.nszjky.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://za.muxihuayi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yo.bjjhwx.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yd.huixinmuqiang.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://og.shtwfgs.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zp.shxzukj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ik.lnxyls.cn

[E02] 重复字符串
来源：http://ma.haigaiapp.cn

Py:   "ab" * 3
来源：http://tx.newstarts.cn

PHP:  str_repeat("ab", 3);
来源：http://qa.bookmarksfly.cn

JS:   "ab".repeat(3)
来源：http://jt.shtwfgs.cn

TS:   "ab".repeat(3)
来源：http://az.huixinmuqiang.cn

Java: "ab".repeat(3)
来源：http://js.shxzukj.cn

Go:   strings.Repeat("ab", 3)
来源：http://cz.yuntaijiaju.cn

Ruby: "ab" * 3
来源：http://cn.huanxung.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ll.bookmarksfly.cn

[E03] 截取子串
来源：http://ke.hahajie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jb.521024.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://la.haigaiapp.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rv.panjiajie.cn

TS:   s.slice(1, 4)
来源：http://qb.szsharing.cn

Java: s.substring(1, 4)
来源：http://hz.asd995.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wz.gzmigu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://wb.521024.cn

C#:   s.Substring(1, 3)
来源：http://ny.muxihuayi.cn

[E04] 查找子串位置
来源：http://sq.szxytkj.cn

Py:   s.find("x");  s.index("x")
来源：http://xe.jctech888.com.cn

PHP:  strpos($s, "x");
来源：http://jy.wgjwhj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ah.gzmigu.cn

TS:   s.indexOf("x")
来源：http://xt.yuntaijiaju.cn

Java: s.indexOf("x")
来源：http://fg.yuntaijiaju.cn

Go:   strings.Index(s, "x")
来源：http://xp.lnxyls.cn

Ruby: s.index("x")
来源：http://vg.nicolike.cn

C#:   s.IndexOf("x")
来源：http://nt.chemitech.net.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://po.muxihuayi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://aj.shxzskj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mr.muxihuayi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oh.nicolike.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://uo.hnjuh.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://za.wgjwhj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bu.shxzskj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kz.asd995.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jw.lnxyls.cn

[E06] 替换子串
来源：http://vg.jctech888.com.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://py.muxihuayi.cn

PHP:  str_replace("a", "b", $s);
来源：http://cp.shxzukj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ow.chemitech.net.cn

TS:   s.replaceAll("a", "b")
来源：http://vp.nicolike.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qw.huixiangedu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wq.lnxyls.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://uy.szxytkj.cn

C#:   s.Replace("a", "b")
来源：http://zl.gzmigu.cn

[E07] 按分隔符拆分
来源：http://ht.huanxung.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tb.jianghongdianzi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yy.szxytkj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://cg.chemitech.net.cn

TS:   s.split(",")
来源：http://sb.szsharing.cn

Java: s.split(",");  s.split("\\s+")
来源：http://vy.shtwfgs.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ev.asd995.cn

Ruby: s.split(",");  s.split
来源：http://ln.newstarts.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tj.szsharing.cn

[E08] 数组按分隔符合并
来源：http://di.yuexingan06.cn

Py:   ",".join(items)
来源：http://jk.9csxet.cn

PHP:  implode(",", $items);
来源：http://yz.huixinmuqiang.cn

JS:   items.join(",")
来源：http://fh.huanxung.cn

TS:   items.join(",")
来源：http://tn.gzmigu.cn

Java: String.join(",", items)
来源：http://rz.bookmarksfly.cn


<!-- 参考信息 -->