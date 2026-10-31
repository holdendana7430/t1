代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kz.bookmarksfly.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://al.9csxet.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://oo.huixinmuqiang.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ai.szsharing.cn

Go:   arr := []int{1, 2, 3}
来源：http://qz.jctech888.com.cn

Ruby: arr = [1, 2, 3]
来源：http://te.shxzukj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tv.jctech888.com.cn

[D02] 追加元素到末尾
来源：http://kb.bjjhwx.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ls.nicolike.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gy.jctech888.com.cn

JS:   arr.push(4);
来源：http://xh.huixinmuqiang.cn

TS:   arr.push(4);
来源：http://bs.bookmarksfly.cn

Java: list.add(4);
来源：http://rv.521024.cn

Go:   arr = append(arr, 4)
来源：http://vr.muxihuayi.cn

Ruby: arr << 4; arr.push(5)
来源：http://mk.lnxyls.cn

C#:   list.Add(4);
来源：http://yx.yuntaijiaju.cn

[D03] 在指定位置插入元素
来源：http://ii.panjiajie.cn

Py:   arr.insert(0, 0)
来源：http://gv.haigaiapp.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rp.lnxyls.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kx.yuntaijiaju.cn

TS:   arr.splice(0, 0, 0);
来源：http://rt.nicolike.cn

Java: list.add(0, 0);
来源：http://wy.bookmarksfly.cn

Go:   arr = append([]int{0}, arr...)
来源：http://pt.jianghongdianzi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bk.hahajie.cn

C#:   list.Insert(0, 0);
来源：http://ky.shxzukj.cn

[D04] 删除元素
来源：http://nl.huanxung.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vm.chemitech.net.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fh.jctech888.com.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://db.9csxet.cn

TS:   arr.splice(0, 1);
来源：http://pg.szsharing.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bu.chemitech.net.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gd.szsharing.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qn.bjjhwx.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ew.hahajie.cn

[D05] 访问与修改元素
来源：http://nf.panjiajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://du.szsharing.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://my.muxihuayi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cx.nicolike.cn

TS:   arr[0]; arr.at(-1);
来源：http://ff.haigaiapp.cn

Java: list.get(0); list.set(0, 9);
来源：http://ke.lnxyls.cn

Go:   arr[0]; arr[0] = 9
来源：http://xz.shtwfgs.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xs.yuntaijiaju.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://co.shtwfgs.cn

[D06] 数组长度
来源：http://rl.yuexingan06.cn

Py:   len(arr)
来源：http://kt.szxytkj.cn

PHP:  count($arr);
来源：http://hr.chemitech.net.cn

JS:   arr.length
来源：http://lk.9csxet.cn

TS:   arr.length
来源：http://do.shxzskj.cn

Java: list.size();
来源：http://az.huixinmuqiang.cn

Go:   len(arr)
来源：http://po.colortex.cn

Ruby: arr.length; arr.size
来源：http://qm.hahajie.cn

C#:   list.Count;
来源：http://wd.yuexingan06.cn

[D07] 切片 / 取子数组
来源：http://uc.yuntaijiaju.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yf.hahajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://va.huixiangedu.cn

JS:   arr.slice(1, 4);
来源：http://ih.huixiangedu.cn

TS:   arr.slice(1, 4);
来源：http://om.huixinmuqiang.cn

Java: list.subList(1, 4);
来源：http://jd.hahajie.cn

Go:   arr[1:4]
来源：http://gq.nszjky.cn

Ruby: arr[1, 3]
来源：http://wi.haigaiapp.cn

C#:   list.GetRange(1, 3);
来源：http://gi.szsharing.cn

[D08] 合并两个数组
来源：http://gk.nszjky.cn

Py:   a + b;  a.extend(b)
来源：http://op.newstarts.cn

PHP:  array_merge($a, $b);
来源：http://nw.bookmarksfly.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ak.panjiajie.cn

TS:   [...a, ...b];
来源：http://sa.szxytkj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kc.jianghongdianzi.cn

Go:   append(a, b...)
来源：http://pu.yuexingan06.cn

Ruby: a + b;  a.concat(b)
来源：http://gh.newstarts.cn

C#:   a.Concat(b).ToList()
来源：http://mw.bookmarksfly.cn

[D09] 排序（升序）
来源：http://cd.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://qp.szsharing.cn

PHP:  sort($arr);
来源：http://xm.bjjhwx.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://uy.jctech888.com.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://js.bookmarksfly.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://yh.colortex.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tu.521024.cn

Ruby: arr.sort
来源：http://cu.nicolike.cn

C#:   list.Sort();
来源：http://vj.shxzskj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qf.nszjky.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sb.hahajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dd.jianghongdianzi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://an.bookmarksfly.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bv.hnjuh.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ij.9csxet.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ug.yuexingan06.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://au.colortex.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vp.yuexingan06.cn

[D11] 反转数组
来源：http://qw.521024.cn

Py:   arr[::-1];  arr.reverse()
来源：http://li.huixiangedu.cn

PHP:  array_reverse($arr);
来源：http://ui.huixiangedu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wl.bookmarksfly.cn

TS:   [...arr].reverse();
来源：http://di.yuexingan06.cn

Java: Collections.reverse(list);
来源：http://af.muxihuayi.cn

Go:   slices.Reverse(arr)
来源：http://wq.haigaiapp.cn

Ruby: arr.reverse
来源：http://pg.shtwfgs.cn

C#:   list.Reverse();
来源：http://dz.nszjky.cn

[D12] 查找元素下标
来源：http://zw.yuexingan06.cn

Py:   arr.index(x);  x in arr
来源：http://vh.huixinmuqiang.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://sn.asd995.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wz.asd995.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wo.bjjhwx.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hi.muxihuayi.cn

Go:   slices.Index(arr, x)
来源：http://jp.asd995.cn

Ruby: arr.index(x)
来源：http://cp.nicolike.cn

C#:   list.IndexOf(x);
来源：http://er.newstarts.cn

[D13] 过滤（保留满足条件的）
来源：http://ql.muxihuayi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jx.9csxet.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xx.szsharing.cn

JS:   arr.filter(x => x > 3)
来源：http://dd.panjiajie.cn

TS:   arr.filter(x => x > 3)
来源：http://ut.colortex.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tv.jianghongdianzi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dd.szxytkj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://zo.bookmarksfly.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://se.gzmigu.cn

[D14] 映射转换（每个元素变形）
来源：http://ye.huixinmuqiang.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ic.chemitech.net.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ru.hnjuh.cn

JS:   arr.map(x => x * 2)
来源：http://yr.haigaiapp.cn

TS:   arr.map(x => x * 2)
来源：http://yo.colortex.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://vu.huanxung.cn

Go:   // 手写循环
来源：http://sl.shtwfgs.cn

Ruby: arr.map { |x| x * 2 }
来源：http://rx.jianghongdianzi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://dk.szsharing.cn

[D15] 去重
来源：http://ji.newstarts.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rr.panjiajie.cn

PHP:  array_unique($arr);
来源：http://bq.asd995.cn

JS:   [...new Set(arr)]
来源：http://au.nszjky.cn

TS:   [...new Set(arr)]
来源：http://og.szsharing.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jt.shxzskj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://pw.muxihuayi.cn

Ruby: arr.uniq
来源：http://wg.lnxyls.cn

C#:   list.Distinct().ToList()
来源：http://gc.huixinmuqiang.cn

[D16] 求和与平均值
来源：http://mt.szxytkj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://po.szsharing.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fr.shtwfgs.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mz.yuexingan06.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dm.huixiangedu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ge.yuexingan06.cn

Go:   // 手写循环累加
来源：http://xz.haigaiapp.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qi.yuntaijiaju.cn

C#:   list.Sum();  list.Average()
来源：http://vp.hnjuh.cn

[D17] 最大值与最小值
来源：http://ja.panjiajie.cn

Py:   max(arr);  min(arr)
来源：http://pq.yuntaijiaju.cn

PHP:  max($arr);  min($arr);
来源：http://rw.bjjhwx.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ya.jianghongdianzi.cn

TS:   Math.max(...arr);
来源：http://zf.shxzskj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://tu.yuexingan06.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fn.bookmarksfly.cn

Ruby: arr.max;  arr.min
来源：http://xe.szsharing.cn

C#:   list.Max();  list.Min()
来源：http://kh.newstarts.cn

[D18] 扁平化嵌套数组
来源：http://vp.shxzukj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ez.bjjhwx.cn

PHP:  array_merge(...$nested);
来源：http://dy.szsharing.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mw.bjjhwx.cn

TS:   nested.flat();
来源：http://tc.bjjhwx.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lc.shtwfgs.cn

Go:   // 手写双层循环
来源：http://gy.huixiangedu.cn

Ruby: nested.flatten
来源：http://xy.gzmigu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hg.wgjwhj.cn

[D19] 按字段分组
来源：http://vz.jctech888.com.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gn.9csxet.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ix.shxzukj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dp.newstarts.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://gf.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hc.nszjky.cn

Go:   // 手写 map[string][]T
来源：http://ik.shxzskj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://lx.521024.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vq.muxihuayi.cn

[D20] 统计每个元素出现次数
来源：http://nn.shxzskj.cn

Py:   Counter(arr)
来源：http://nz.muxihuayi.cn

PHP:  array_count_values($arr);
来源：http://nd.jctech888.com.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ww.asd995.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ji.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dx.muxihuayi.cn

Go:   // 手写 map[T]int
来源：http://dy.jctech888.com.cn

Ruby: arr.tally
来源：http://nf.521024.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ak.wgjwhj.cn

[D21] 判断是否包含某元素
来源：http://tm.huixinmuqiang.cn

Py:   x in arr
来源：http://qy.szxytkj.cn

PHP:  in_array($x, $arr, true);
来源：http://tj.shtwfgs.cn

JS:   arr.includes(x)
来源：http://sf.jctech888.com.cn

TS:   arr.includes(x)
来源：http://to.jianghongdianzi.cn

Java: list.contains(x)
来源：http://lj.shxzukj.cn

Go:   slices.Contains(arr, x)
来源：http://rs.bjjhwx.cn

Ruby: arr.include?(x)
来源：http://qn.szxytkj.cn

C#:   list.Contains(x)
来源：http://fl.panjiajie.cn

[D22] 复制数组（避免共享引用）
来源：http://os.asd995.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lq.shtwfgs.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yv.shxzskj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://er.jctech888.com.cn

TS:   [...arr];
来源：http://xa.szxytkj.cn

Java: new ArrayList<>(list);
来源：http://zr.muxihuayi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://mb.yuexingan06.cn

Ruby: arr.dup;  arr.clone
来源：http://rf.shtwfgs.cn

C#:   new List<int>(list);
来源：http://vr.huixiangedu.cn

[D23] reduce 累积计算
来源：http://zv.huixiangedu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mg.asd995.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xg.shxzskj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dw.lnxyls.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nh.bjjhwx.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://sc.521024.cn

Go:   // 手写循环
来源：http://xp.shxzukj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://be.szxytkj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yo.bookmarksfly.cn

[D24] 字典 / Map 基本操作
来源：http://wx.newstarts.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gu.colortex.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gw.hahajie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://om.9csxet.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ha.yuntaijiaju.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://oz.nszjky.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://me.lnxyls.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pr.asd995.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kt.9csxet.cn

[D25] Set 集合去重与交并差
来源：http://wx.hnjuh.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lv.hnjuh.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ue.szxytkj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cy.lnxyls.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ck.chemitech.net.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ck.jctech888.com.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nc.haigaiapp.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://va.szxytkj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://do.haigaiapp.cn

[D26] 数组转字符串
来源：http://co.gzmigu.cn

Py:   ", ".join(map(str, arr))
来源：http://jn.huanxung.cn

PHP:  implode(", ", $arr);
来源：http://lm.newstarts.cn

JS:   arr.join(", ")
来源：http://mf.gzmigu.cn

TS:   arr.join(", ")
来源：http://fk.haigaiapp.cn

Java: String.join(", ", list)
来源：http://fj.huixiangedu.cn

Go:   strings.Join(strs, ", ")
来源：http://hc.newstarts.cn

Ruby: arr.join(", ")
来源：http://cj.hnjuh.cn

C#:   string.Join(", ", list)
来源：http://cf.9csxet.cn

================================================================================
来源：http://hd.hnjuh.cn

E. 字符串处理
来源：http://rn.shxzskj.cn

================================================================================
来源：http://fp.gzmigu.cn

[E01] 拼接字符串
来源：http://ij.jianghongdianzi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yd.jianghongdianzi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fn.haigaiapp.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nx.muxihuayi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pr.bookmarksfly.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lx.hahajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uk.panjiajie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cg.bjjhwx.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jg.jctech888.com.cn

[E02] 重复字符串
来源：http://ko.huixinmuqiang.cn

Py:   "ab" * 3
来源：http://yt.huixinmuqiang.cn

PHP:  str_repeat("ab", 3);
来源：http://bo.shxzskj.cn

JS:   "ab".repeat(3)
来源：http://de.huixiangedu.cn

TS:   "ab".repeat(3)
来源：http://vl.gzmigu.cn

Java: "ab".repeat(3)
来源：http://dk.gzmigu.cn

Go:   strings.Repeat("ab", 3)
来源：http://xv.szxytkj.cn

Ruby: "ab" * 3
来源：http://aa.huixiangedu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ji.szxytkj.cn

[E03] 截取子串
来源：http://ib.bookmarksfly.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kj.muxihuayi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ap.521024.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ez.lnxyls.cn

TS:   s.slice(1, 4)
来源：http://vw.yuntaijiaju.cn

Java: s.substring(1, 4)
来源：http://qo.nicolike.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ba.newstarts.cn

Ruby: s[1, 3];  s[1..3]
来源：http://kt.jianghongdianzi.cn

C#:   s.Substring(1, 3)
来源：http://em.521024.cn

[E04] 查找子串位置
来源：http://wc.muxihuayi.cn

Py:   s.find("x");  s.index("x")
来源：http://kj.asd995.cn

PHP:  strpos($s, "x");
来源：http://hp.bjjhwx.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://io.szsharing.cn

TS:   s.indexOf("x")
来源：http://ld.chemitech.net.cn

Java: s.indexOf("x")
来源：http://rw.hnjuh.cn

Go:   strings.Index(s, "x")
来源：http://qa.hahajie.cn

Ruby: s.index("x")
来源：http://hy.wgjwhj.cn

C#:   s.IndexOf("x")
来源：http://ot.521024.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://td.huixiangedu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gs.yuntaijiaju.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://me.colortex.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://op.bjjhwx.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://bo.shxzskj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://eo.gzmigu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zk.newstarts.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gw.lnxyls.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vq.yuexingan06.cn

[E06] 替换子串
来源：http://on.hahajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cw.wgjwhj.cn

PHP:  str_replace("a", "b", $s);
来源：http://mz.9csxet.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rv.huanxung.cn

TS:   s.replaceAll("a", "b")
来源：http://zy.chemitech.net.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uj.panjiajie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://no.lnxyls.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nl.huixinmuqiang.cn

C#:   s.Replace("a", "b")
来源：http://jv.9csxet.cn

[E07] 按分隔符拆分
来源：http://bu.newstarts.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://he.colortex.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ej.wgjwhj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://bl.szxytkj.cn

TS:   s.split(",")
来源：http://bj.bjjhwx.cn

Java: s.split(",");  s.split("\\s+")
来源：http://bc.gzmigu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://eg.hnjuh.cn

Ruby: s.split(",");  s.split
来源：http://mp.yuntaijiaju.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://on.yuntaijiaju.cn

[E08] 数组按分隔符合并
来源：http://zy.szxytkj.cn

Py:   ",".join(items)
来源：http://xn.jianghongdianzi.cn


<!-- 参考信息 -->