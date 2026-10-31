代发 wailian999

D. 数组 / 列表 / 集合
来源：http://bq.nszjky.cn

================================================================================
来源：http://eb.chemitech.net.cn

[D01] 创建数组 / 列表
来源：http://iv.chemitech.net.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://yv.huixiangedu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xy.haigaiapp.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rp.szxytkj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ic.huanxung.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yg.jctech888.com.cn

Go:   arr := []int{1, 2, 3}
来源：http://kn.nszjky.cn

Ruby: arr = [1, 2, 3]
来源：http://bm.bookmarksfly.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ng.panjiajie.cn

[D02] 追加元素到末尾
来源：http://yk.nszjky.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dg.huixiangedu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vq.yuntaijiaju.cn

JS:   arr.push(4);
来源：http://um.wgjwhj.cn

TS:   arr.push(4);
来源：http://wv.bookmarksfly.cn

Java: list.add(4);
来源：http://sr.bookmarksfly.cn

Go:   arr = append(arr, 4)
来源：http://uu.wgjwhj.cn

Ruby: arr << 4; arr.push(5)
来源：http://ms.shxzukj.cn

C#:   list.Add(4);
来源：http://rd.yuntaijiaju.cn

[D03] 在指定位置插入元素
来源：http://qz.nicolike.cn

Py:   arr.insert(0, 0)
来源：http://pi.jianghongdianzi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://na.lnxyls.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gr.huanxung.cn

TS:   arr.splice(0, 0, 0);
来源：http://ly.shtwfgs.cn

Java: list.add(0, 0);
来源：http://jm.lnxyls.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ov.hnjuh.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uz.hahajie.cn

C#:   list.Insert(0, 0);
来源：http://gb.asd995.cn

[D04] 删除元素
来源：http://tc.wgjwhj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://em.huixinmuqiang.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xr.lnxyls.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fy.9csxet.cn

TS:   arr.splice(0, 1);
来源：http://sf.lnxyls.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jy.huixinmuqiang.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gi.szxytkj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dl.yuntaijiaju.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://eh.yuexingan06.cn

[D05] 访问与修改元素
来源：http://kv.colortex.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jm.szsharing.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vf.jctech888.com.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nk.nicolike.cn

TS:   arr[0]; arr.at(-1);
来源：http://hx.hnjuh.cn

Java: list.get(0); list.set(0, 9);
来源：http://vo.newstarts.cn

Go:   arr[0]; arr[0] = 9
来源：http://eb.gzmigu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jx.9csxet.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://if.huanxung.cn

[D06] 数组长度
来源：http://wt.huixiangedu.cn

Py:   len(arr)
来源：http://wz.shxzukj.cn

PHP:  count($arr);
来源：http://ll.muxihuayi.cn

JS:   arr.length
来源：http://ix.muxihuayi.cn

TS:   arr.length
来源：http://cs.shxzukj.cn

Java: list.size();
来源：http://mu.521024.cn

Go:   len(arr)
来源：http://vi.huixiangedu.cn

Ruby: arr.length; arr.size
来源：http://ee.wgjwhj.cn

C#:   list.Count;
来源：http://bn.wgjwhj.cn

[D07] 切片 / 取子数组
来源：http://gm.lnxyls.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nr.9csxet.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ul.9csxet.cn

JS:   arr.slice(1, 4);
来源：http://vq.jianghongdianzi.cn

TS:   arr.slice(1, 4);
来源：http://ml.muxihuayi.cn

Java: list.subList(1, 4);
来源：http://de.shtwfgs.cn

Go:   arr[1:4]
来源：http://po.lnxyls.cn

Ruby: arr[1, 3]
来源：http://km.9csxet.cn

C#:   list.GetRange(1, 3);
来源：http://rq.haigaiapp.cn

[D08] 合并两个数组
来源：http://kh.9csxet.cn

Py:   a + b;  a.extend(b)
来源：http://po.shtwfgs.cn

PHP:  array_merge($a, $b);
来源：http://hs.huixiangedu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://fs.newstarts.cn

TS:   [...a, ...b];
来源：http://tt.panjiajie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://br.asd995.cn

Go:   append(a, b...)
来源：http://vz.muxihuayi.cn

Ruby: a + b;  a.concat(b)
来源：http://mg.shtwfgs.cn

C#:   a.Concat(b).ToList()
来源：http://yb.bookmarksfly.cn

[D09] 排序（升序）
来源：http://iv.szxytkj.cn

Py:   sorted(arr);  arr.sort()
来源：http://ke.panjiajie.cn

PHP:  sort($arr);
来源：http://oh.yuntaijiaju.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zc.haigaiapp.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://pa.huixiangedu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://oj.yuntaijiaju.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://as.bjjhwx.cn

Ruby: arr.sort
来源：http://nq.chemitech.net.cn

C#:   list.Sort();
来源：http://ji.szxytkj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://sa.asd995.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qx.chemitech.net.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jx.shtwfgs.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rf.hnjuh.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://va.huixiangedu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hs.shxzukj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yz.muxihuayi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://my.hahajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://it.yuntaijiaju.cn

[D11] 反转数组
来源：http://nk.huixiangedu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://cv.bookmarksfly.cn

PHP:  array_reverse($arr);
来源：http://zf.haigaiapp.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nb.jianghongdianzi.cn

TS:   [...arr].reverse();
来源：http://dn.hahajie.cn

Java: Collections.reverse(list);
来源：http://qi.hnjuh.cn

Go:   slices.Reverse(arr)
来源：http://yv.huixiangedu.cn

Ruby: arr.reverse
来源：http://on.huixinmuqiang.cn

C#:   list.Reverse();
来源：http://jt.colortex.cn

[D12] 查找元素下标
来源：http://fg.9csxet.cn

Py:   arr.index(x);  x in arr
来源：http://aq.chemitech.net.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uy.wgjwhj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://py.nicolike.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bl.wgjwhj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://om.huixiangedu.cn

Go:   slices.Index(arr, x)
来源：http://uz.shxzukj.cn

Ruby: arr.index(x)
来源：http://xh.asd995.cn

C#:   list.IndexOf(x);
来源：http://pb.nicolike.cn

[D13] 过滤（保留满足条件的）
来源：http://eo.shxzskj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cb.huixiangedu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cf.colortex.cn

JS:   arr.filter(x => x > 3)
来源：http://ba.huanxung.cn

TS:   arr.filter(x => x > 3)
来源：http://gl.nicolike.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cz.nszjky.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tt.hahajie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://vo.hnjuh.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://no.jianghongdianzi.cn

[D14] 映射转换（每个元素变形）
来源：http://ok.nicolike.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rg.nszjky.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bw.9csxet.cn

JS:   arr.map(x => x * 2)
来源：http://ov.newstarts.cn

TS:   arr.map(x => x * 2)
来源：http://pj.gzmigu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://nz.huixinmuqiang.cn

Go:   // 手写循环
来源：http://rf.jctech888.com.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jh.yuntaijiaju.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qx.521024.cn

[D15] 去重
来源：http://dm.huixiangedu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ka.newstarts.cn

PHP:  array_unique($arr);
来源：http://xm.shxzukj.cn

JS:   [...new Set(arr)]
来源：http://nf.hnjuh.cn

TS:   [...new Set(arr)]
来源：http://dt.chemitech.net.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kb.newstarts.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vt.huixiangedu.cn

Ruby: arr.uniq
来源：http://ve.jianghongdianzi.cn

C#:   list.Distinct().ToList()
来源：http://ik.haigaiapp.cn

[D16] 求和与平均值
来源：http://wv.521024.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bk.9csxet.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ul.huixinmuqiang.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zg.huanxung.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fs.panjiajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://te.lnxyls.cn

Go:   // 手写循环累加
来源：http://lk.shtwfgs.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ny.hahajie.cn

C#:   list.Sum();  list.Average()
来源：http://gh.nicolike.cn

[D17] 最大值与最小值
来源：http://bl.huixiangedu.cn

Py:   max(arr);  min(arr)
来源：http://dz.huanxung.cn

PHP:  max($arr);  min($arr);
来源：http://rk.nszjky.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://he.jctech888.com.cn

TS:   Math.max(...arr);
来源：http://dq.newstarts.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gg.gzmigu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bh.chemitech.net.cn

Ruby: arr.max;  arr.min
来源：http://ze.haigaiapp.cn

C#:   list.Max();  list.Min()
来源：http://hf.yuexingan06.cn

[D18] 扁平化嵌套数组
来源：http://lr.shxzukj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wv.gzmigu.cn

PHP:  array_merge(...$nested);
来源：http://cd.asd995.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rf.chemitech.net.cn

TS:   nested.flat();
来源：http://ay.panjiajie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pk.shxzukj.cn

Go:   // 手写双层循环
来源：http://kp.huanxung.cn

Ruby: nested.flatten
来源：http://uw.bookmarksfly.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://pb.lnxyls.cn

[D19] 按字段分组
来源：http://zx.newstarts.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xc.yuntaijiaju.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nz.huanxung.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fc.wgjwhj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://hc.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ar.huanxung.cn

Go:   // 手写 map[string][]T
来源：http://hi.colortex.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://db.yuexingan06.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ww.muxihuayi.cn

[D20] 统计每个元素出现次数
来源：http://mm.yuexingan06.cn

Py:   Counter(arr)
来源：http://we.hnjuh.cn

PHP:  array_count_values($arr);
来源：http://fj.shxzskj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rl.yuntaijiaju.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dw.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xs.wgjwhj.cn

Go:   // 手写 map[T]int
来源：http://ag.huixinmuqiang.cn

Ruby: arr.tally
来源：http://fs.haigaiapp.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kx.hnjuh.cn

[D21] 判断是否包含某元素
来源：http://ye.haigaiapp.cn

Py:   x in arr
来源：http://bt.jctech888.com.cn

PHP:  in_array($x, $arr, true);
来源：http://zy.huanxung.cn

JS:   arr.includes(x)
来源：http://gy.hahajie.cn

TS:   arr.includes(x)
来源：http://aq.szsharing.cn

Java: list.contains(x)
来源：http://wp.huixinmuqiang.cn

Go:   slices.Contains(arr, x)
来源：http://cm.jianghongdianzi.cn

Ruby: arr.include?(x)
来源：http://nl.gzmigu.cn

C#:   list.Contains(x)
来源：http://rw.jianghongdianzi.cn

[D22] 复制数组（避免共享引用）
来源：http://ys.muxihuayi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nk.asd995.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lv.nicolike.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xs.hahajie.cn

TS:   [...arr];
来源：http://er.jianghongdianzi.cn

Java: new ArrayList<>(list);
来源：http://py.nicolike.cn

Go:   copied := append([]int(nil), arr...)
来源：http://sx.shtwfgs.cn

Ruby: arr.dup;  arr.clone
来源：http://vy.nicolike.cn

C#:   new List<int>(list);
来源：http://bf.shxzukj.cn

[D23] reduce 累积计算
来源：http://xf.bookmarksfly.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kd.shxzskj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://eq.huixinmuqiang.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://du.yuntaijiaju.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wx.jctech888.com.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://al.nszjky.cn

Go:   // 手写循环
来源：http://jg.bookmarksfly.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://me.panjiajie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dm.nszjky.cn

[D24] 字典 / Map 基本操作
来源：http://vu.wgjwhj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ea.nszjky.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ce.yuntaijiaju.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ty.gzmigu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bg.huixinmuqiang.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cs.shtwfgs.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cx.jianghongdianzi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lw.huanxung.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jj.yuexingan06.cn

[D25] Set 集合去重与交并差
来源：http://pz.nicolike.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ks.jctech888.com.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zf.hnjuh.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pb.gzmigu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zd.nicolike.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mw.nicolike.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://au.nicolike.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://md.nicolike.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ao.chemitech.net.cn

[D26] 数组转字符串
来源：http://gy.shxzskj.cn

Py:   ", ".join(map(str, arr))
来源：http://rb.colortex.cn

PHP:  implode(", ", $arr);
来源：http://lh.huixinmuqiang.cn

JS:   arr.join(", ")
来源：http://ex.huixinmuqiang.cn

TS:   arr.join(", ")
来源：http://at.shtwfgs.cn

Java: String.join(", ", list)
来源：http://hi.huanxung.cn

Go:   strings.Join(strs, ", ")
来源：http://bf.jianghongdianzi.cn

Ruby: arr.join(", ")
来源：http://sv.szsharing.cn

C#:   string.Join(", ", list)
来源：http://ad.colortex.cn

================================================================================
来源：http://py.chemitech.net.cn

E. 字符串处理
来源：http://us.chemitech.net.cn

================================================================================
来源：http://xs.gzmigu.cn

[E01] 拼接字符串
来源：http://ro.szxytkj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xm.hnjuh.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://su.gzmigu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pw.chemitech.net.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nj.colortex.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://uo.lnxyls.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uq.huixiangedu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hb.shtwfgs.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dn.nicolike.cn

[E02] 重复字符串
来源：http://qo.yuexingan06.cn

Py:   "ab" * 3
来源：http://qf.bookmarksfly.cn

PHP:  str_repeat("ab", 3);
来源：http://zg.wgjwhj.cn

JS:   "ab".repeat(3)
来源：http://ib.yuntaijiaju.cn

TS:   "ab".repeat(3)
来源：http://dh.hnjuh.cn

Java: "ab".repeat(3)
来源：http://bv.huanxung.cn

Go:   strings.Repeat("ab", 3)
来源：http://mf.muxihuayi.cn

Ruby: "ab" * 3
来源：http://on.huanxung.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://az.9csxet.cn

[E03] 截取子串
来源：http://bb.lnxyls.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jq.huixiangedu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wv.szsharing.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gg.huanxung.cn

TS:   s.slice(1, 4)
来源：http://oe.newstarts.cn

Java: s.substring(1, 4)
来源：http://xj.9csxet.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ry.haigaiapp.cn

Ruby: s[1, 3];  s[1..3]
来源：http://xn.shxzskj.cn

C#:   s.Substring(1, 3)
来源：http://hy.szsharing.cn

[E04] 查找子串位置
来源：http://tw.asd995.cn

Py:   s.find("x");  s.index("x")
来源：http://mn.hnjuh.cn

PHP:  strpos($s, "x");
来源：http://ie.asd995.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ab.bjjhwx.cn

TS:   s.indexOf("x")
来源：http://vs.bjjhwx.cn

Java: s.indexOf("x")
来源：http://vl.bjjhwx.cn

Go:   strings.Index(s, "x")
来源：http://ng.hnjuh.cn

Ruby: s.index("x")
来源：http://az.jctech888.com.cn

C#:   s.IndexOf("x")
来源：http://wr.521024.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://mn.colortex.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kq.hahajie.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zx.asd995.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ki.colortex.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://vl.hnjuh.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ms.hnjuh.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xh.wgjwhj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rd.bjjhwx.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ys.huixiangedu.cn

[E06] 替换子串
来源：http://ky.jctech888.com.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://es.asd995.cn

PHP:  str_replace("a", "b", $s);
来源：http://qw.bjjhwx.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bq.521024.cn

TS:   s.replaceAll("a", "b")
来源：http://zq.shtwfgs.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yw.huanxung.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ja.lnxyls.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gm.9csxet.cn

C#:   s.Replace("a", "b")
来源：http://mt.wgjwhj.cn

[E07] 按分隔符拆分
来源：http://nh.asd995.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mo.jctech888.com.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ce.gzmigu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://mv.asd995.cn

TS:   s.split(",")
来源：http://ui.asd995.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ry.bjjhwx.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jd.huixiangedu.cn


<!-- 参考信息 -->