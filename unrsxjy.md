代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://ts.9csxet.cn

Ruby: arr = [1, 2, 3]
来源：http://oq.yuexingan06.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jo.hnjuh.cn

[D02] 追加元素到末尾
来源：http://kd.asd995.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yh.huixinmuqiang.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xc.nicolike.cn

JS:   arr.push(4);
来源：http://mu.panjiajie.cn

TS:   arr.push(4);
来源：http://kl.lnxyls.cn

Java: list.add(4);
来源：http://jx.szxytkj.cn

Go:   arr = append(arr, 4)
来源：http://hc.jctech888.com.cn

Ruby: arr << 4; arr.push(5)
来源：http://la.shxzukj.cn

C#:   list.Add(4);
来源：http://ox.shxzukj.cn

[D03] 在指定位置插入元素
来源：http://rk.newstarts.cn

Py:   arr.insert(0, 0)
来源：http://cx.huixiangedu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lt.huixinmuqiang.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zt.bookmarksfly.cn

TS:   arr.splice(0, 0, 0);
来源：http://er.huixinmuqiang.cn

Java: list.add(0, 0);
来源：http://tq.colortex.cn

Go:   arr = append([]int{0}, arr...)
来源：http://cc.huixiangedu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://df.haigaiapp.cn

C#:   list.Insert(0, 0);
来源：http://hi.jctech888.com.cn

[D04] 删除元素
来源：http://ty.yuexingan06.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://li.bookmarksfly.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://js.bjjhwx.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wi.shtwfgs.cn

TS:   arr.splice(0, 1);
来源：http://jn.panjiajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fl.shxzskj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://eg.asd995.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ad.hahajie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zs.bjjhwx.cn

[D05] 访问与修改元素
来源：http://vh.yuntaijiaju.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://do.colortex.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://aa.shtwfgs.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://br.haigaiapp.cn

TS:   arr[0]; arr.at(-1);
来源：http://bm.hahajie.cn

Java: list.get(0); list.set(0, 9);
来源：http://na.huanxung.cn

Go:   arr[0]; arr[0] = 9
来源：http://xk.shtwfgs.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gg.szsharing.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ly.521024.cn

[D06] 数组长度
来源：http://fv.jianghongdianzi.cn

Py:   len(arr)
来源：http://dr.huixinmuqiang.cn

PHP:  count($arr);
来源：http://om.shxzskj.cn

JS:   arr.length
来源：http://ll.colortex.cn

TS:   arr.length
来源：http://cw.szsharing.cn

Java: list.size();
来源：http://wj.bjjhwx.cn

Go:   len(arr)
来源：http://vb.huixinmuqiang.cn

Ruby: arr.length; arr.size
来源：http://gl.newstarts.cn

C#:   list.Count;
来源：http://mb.chemitech.net.cn

[D07] 切片 / 取子数组
来源：http://vv.521024.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wi.jianghongdianzi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://mu.shxzskj.cn

JS:   arr.slice(1, 4);
来源：http://yw.bookmarksfly.cn

TS:   arr.slice(1, 4);
来源：http://kd.shxzskj.cn

Java: list.subList(1, 4);
来源：http://kp.gzmigu.cn

Go:   arr[1:4]
来源：http://xo.nicolike.cn

Ruby: arr[1, 3]
来源：http://sq.lnxyls.cn

C#:   list.GetRange(1, 3);
来源：http://nw.chemitech.net.cn

[D08] 合并两个数组
来源：http://hk.newstarts.cn

Py:   a + b;  a.extend(b)
来源：http://fm.521024.cn

PHP:  array_merge($a, $b);
来源：http://ll.nicolike.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://om.szsharing.cn

TS:   [...a, ...b];
来源：http://ie.shtwfgs.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://iq.shxzskj.cn

Go:   append(a, b...)
来源：http://yj.newstarts.cn

Ruby: a + b;  a.concat(b)
来源：http://ab.shxzukj.cn

C#:   a.Concat(b).ToList()
来源：http://sl.szxytkj.cn

[D09] 排序（升序）
来源：http://ko.521024.cn

Py:   sorted(arr);  arr.sort()
来源：http://ee.chemitech.net.cn

PHP:  sort($arr);
来源：http://bc.muxihuayi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tc.lnxyls.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ts.nszjky.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://tw.chemitech.net.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ab.gzmigu.cn

Ruby: arr.sort
来源：http://ug.shxzskj.cn

C#:   list.Sort();
来源：http://fm.colortex.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://cn.huixiangedu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dc.shxzukj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rk.shxzukj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bp.bjjhwx.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hy.lnxyls.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gy.nicolike.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://eb.wgjwhj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ew.nicolike.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://aa.colortex.cn

[D11] 反转数组
来源：http://xs.haigaiapp.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ye.lnxyls.cn

PHP:  array_reverse($arr);
来源：http://wg.jianghongdianzi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qb.hahajie.cn

TS:   [...arr].reverse();
来源：http://ve.bookmarksfly.cn

Java: Collections.reverse(list);
来源：http://ek.jianghongdianzi.cn

Go:   slices.Reverse(arr)
来源：http://ct.huixinmuqiang.cn

Ruby: arr.reverse
来源：http://lv.shxzskj.cn

C#:   list.Reverse();
来源：http://ty.muxihuayi.cn

[D12] 查找元素下标
来源：http://of.huixinmuqiang.cn

Py:   arr.index(x);  x in arr
来源：http://mm.bjjhwx.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pu.muxihuayi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bg.huixiangedu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://id.bjjhwx.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://of.shxzskj.cn

Go:   slices.Index(arr, x)
来源：http://ki.jctech888.com.cn

Ruby: arr.index(x)
来源：http://wl.panjiajie.cn

C#:   list.IndexOf(x);
来源：http://kd.hnjuh.cn

[D13] 过滤（保留满足条件的）
来源：http://bx.gzmigu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pw.shtwfgs.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gy.521024.cn

JS:   arr.filter(x => x > 3)
来源：http://wb.yuexingan06.cn

TS:   arr.filter(x => x > 3)
来源：http://un.nszjky.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://uw.huixinmuqiang.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://br.hnjuh.cn

Ruby: arr.select { |x| x > 3 }
来源：http://mn.panjiajie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ef.shxzskj.cn

[D14] 映射转换（每个元素变形）
来源：http://ig.chemitech.net.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vx.9csxet.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vs.bjjhwx.cn

JS:   arr.map(x => x * 2)
来源：http://fs.shtwfgs.cn

TS:   arr.map(x => x * 2)
来源：http://nv.shxzukj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://nz.bookmarksfly.cn

Go:   // 手写循环
来源：http://pn.haigaiapp.cn

Ruby: arr.map { |x| x * 2 }
来源：http://op.szxytkj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://uh.521024.cn

[D15] 去重
来源：http://qq.newstarts.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xj.newstarts.cn

PHP:  array_unique($arr);
来源：http://nc.jianghongdianzi.cn

JS:   [...new Set(arr)]
来源：http://ci.hahajie.cn

TS:   [...new Set(arr)]
来源：http://vf.haigaiapp.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://di.yuntaijiaju.cn

Go:   // 用 map[T]struct{} 手写
来源：http://yi.nszjky.cn

Ruby: arr.uniq
来源：http://nv.huanxung.cn

C#:   list.Distinct().ToList()
来源：http://oa.9csxet.cn

[D16] 求和与平均值
来源：http://uu.huanxung.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dz.bookmarksfly.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dz.bookmarksfly.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ud.szsharing.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sh.huanxung.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ia.nszjky.cn

Go:   // 手写循环累加
来源：http://ke.jianghongdianzi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lz.huixiangedu.cn

C#:   list.Sum();  list.Average()
来源：http://ec.nicolike.cn

[D17] 最大值与最小值
来源：http://cc.nszjky.cn

Py:   max(arr);  min(arr)
来源：http://yb.9csxet.cn

PHP:  max($arr);  min($arr);
来源：http://jm.jianghongdianzi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ln.bjjhwx.cn

TS:   Math.max(...arr);
来源：http://ji.szxytkj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://pl.huanxung.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wy.szsharing.cn

Ruby: arr.max;  arr.min
来源：http://et.panjiajie.cn

C#:   list.Max();  list.Min()
来源：http://kh.huixiangedu.cn

[D18] 扁平化嵌套数组
来源：http://dl.haigaiapp.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tu.521024.cn

PHP:  array_merge(...$nested);
来源：http://nk.colortex.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://oa.muxihuayi.cn

TS:   nested.flat();
来源：http://xl.jctech888.com.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bm.9csxet.cn

Go:   // 手写双层循环
来源：http://gm.nszjky.cn

Ruby: nested.flatten
来源：http://gp.shxzukj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://rt.colortex.cn

[D19] 按字段分组
来源：http://qo.haigaiapp.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sq.bookmarksfly.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fd.huixiangedu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mw.hnjuh.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://nk.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dm.gzmigu.cn

Go:   // 手写 map[string][]T
来源：http://jh.hahajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://xs.wgjwhj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zo.wgjwhj.cn

[D20] 统计每个元素出现次数
来源：http://zd.shxzskj.cn

Py:   Counter(arr)
来源：http://sn.lnxyls.cn

PHP:  array_count_values($arr);
来源：http://ql.newstarts.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kw.hnjuh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kw.nicolike.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rs.newstarts.cn

Go:   // 手写 map[T]int
来源：http://gl.asd995.cn

Ruby: arr.tally
来源：http://xl.hahajie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://of.panjiajie.cn

[D21] 判断是否包含某元素
来源：http://en.hahajie.cn

Py:   x in arr
来源：http://lp.newstarts.cn

PHP:  in_array($x, $arr, true);
来源：http://cy.9csxet.cn

JS:   arr.includes(x)
来源：http://kj.nszjky.cn

TS:   arr.includes(x)
来源：http://ud.haigaiapp.cn

Java: list.contains(x)
来源：http://ci.szxytkj.cn

Go:   slices.Contains(arr, x)
来源：http://it.muxihuayi.cn

Ruby: arr.include?(x)
来源：http://uk.huanxung.cn

C#:   list.Contains(x)
来源：http://oy.shxzukj.cn

[D22] 复制数组（避免共享引用）
来源：http://po.shxzskj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xg.shxzskj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qm.gzmigu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vu.nicolike.cn

TS:   [...arr];
来源：http://zq.shxzukj.cn

Java: new ArrayList<>(list);
来源：http://tq.huixiangedu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://fi.huixiangedu.cn

Ruby: arr.dup;  arr.clone
来源：http://pt.asd995.cn

C#:   new List<int>(list);
来源：http://sp.szxytkj.cn

[D23] reduce 累积计算
来源：http://gh.szsharing.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fp.szxytkj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dz.nszjky.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://me.bjjhwx.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://va.muxihuayi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://md.haigaiapp.cn

Go:   // 手写循环
来源：http://td.szxytkj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kp.haigaiapp.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sl.muxihuayi.cn

[D24] 字典 / Map 基本操作
来源：http://mc.shtwfgs.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ev.9csxet.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qg.asd995.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ze.bjjhwx.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://or.gzmigu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wo.gzmigu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tf.shxzskj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qs.asd995.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gl.muxihuayi.cn

[D25] Set 集合去重与交并差
来源：http://yh.szxytkj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bk.hnjuh.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mf.521024.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ze.9csxet.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://oq.huixiangedu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kk.hnjuh.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://os.bjjhwx.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tl.gzmigu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mb.bjjhwx.cn

[D26] 数组转字符串
来源：http://xh.bookmarksfly.cn

Py:   ", ".join(map(str, arr))
来源：http://wh.hnjuh.cn

PHP:  implode(", ", $arr);
来源：http://mg.shtwfgs.cn

JS:   arr.join(", ")
来源：http://xi.jianghongdianzi.cn

TS:   arr.join(", ")
来源：http://hq.shtwfgs.cn

Java: String.join(", ", list)
来源：http://pf.huixinmuqiang.cn

Go:   strings.Join(strs, ", ")
来源：http://ua.521024.cn

Ruby: arr.join(", ")
来源：http://jh.9csxet.cn

C#:   string.Join(", ", list)
来源：http://ar.hahajie.cn

================================================================================
来源：http://pk.huixinmuqiang.cn

E. 字符串处理
来源：http://aw.shxzukj.cn

================================================================================
来源：http://uq.szsharing.cn

[E01] 拼接字符串
来源：http://st.huixinmuqiang.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ww.shtwfgs.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://om.chemitech.net.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bz.huixinmuqiang.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dg.jianghongdianzi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tz.huixinmuqiang.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jx.panjiajie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://eh.lnxyls.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kb.huanxung.cn

[E02] 重复字符串
来源：http://ti.jctech888.com.cn

Py:   "ab" * 3
来源：http://pz.bookmarksfly.cn

PHP:  str_repeat("ab", 3);
来源：http://md.shxzskj.cn

JS:   "ab".repeat(3)
来源：http://za.shxzskj.cn

TS:   "ab".repeat(3)
来源：http://im.gzmigu.cn

Java: "ab".repeat(3)
来源：http://ph.hahajie.cn

Go:   strings.Repeat("ab", 3)
来源：http://pr.szxytkj.cn

Ruby: "ab" * 3
来源：http://ys.521024.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ox.colortex.cn

[E03] 截取子串
来源：http://xj.szsharing.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mp.yuntaijiaju.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qw.asd995.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fd.panjiajie.cn

TS:   s.slice(1, 4)
来源：http://av.hnjuh.cn

Java: s.substring(1, 4)
来源：http://lk.jctech888.com.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://km.muxihuayi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ni.bookmarksfly.cn

C#:   s.Substring(1, 3)
来源：http://sb.bookmarksfly.cn

[E04] 查找子串位置
来源：http://qb.szxytkj.cn

Py:   s.find("x");  s.index("x")
来源：http://bq.huanxung.cn

PHP:  strpos($s, "x");
来源：http://dw.szsharing.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://id.shxzukj.cn

TS:   s.indexOf("x")
来源：http://xo.wgjwhj.cn

Java: s.indexOf("x")
来源：http://lh.hahajie.cn

Go:   strings.Index(s, "x")
来源：http://yt.bjjhwx.cn

Ruby: s.index("x")
来源：http://vs.yuntaijiaju.cn

C#:   s.IndexOf("x")
来源：http://nw.nicolike.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://qt.bookmarksfly.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xe.shxzskj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://eg.asd995.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dv.hahajie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://dc.wgjwhj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uo.hahajie.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fl.huanxung.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wd.muxihuayi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dr.nicolike.cn

[E06] 替换子串
来源：http://qg.jianghongdianzi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jq.jianghongdianzi.cn

PHP:  str_replace("a", "b", $s);
来源：http://uq.newstarts.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jw.asd995.cn

TS:   s.replaceAll("a", "b")
来源：http://ux.9csxet.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ft.shxzskj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://je.9csxet.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zm.muxihuayi.cn

C#:   s.Replace("a", "b")
来源：http://lh.hahajie.cn

[E07] 按分隔符拆分
来源：http://mb.szsharing.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ac.hnjuh.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://db.huixinmuqiang.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://hu.jianghongdianzi.cn

TS:   s.split(",")
来源：http://rj.colortex.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ib.shxzukj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mu.shtwfgs.cn

Ruby: s.split(",");  s.split
来源：http://sy.colortex.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jj.jctech888.com.cn

[E08] 数组按分隔符合并
来源：http://ug.huixinmuqiang.cn

Py:   ",".join(items)
来源：http://nc.shtwfgs.cn

PHP:  implode(",", $items);
来源：http://dg.yuexingan06.cn

JS:   items.join(",")
来源：http://wv.jianghongdianzi.cn

TS:   items.join(",")
来源：http://wl.haigaiapp.cn

Java: String.join(",", items)
来源：http://ya.jctech888.com.cn


<!-- 参考信息 -->