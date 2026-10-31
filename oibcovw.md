代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://ot.lnxyls.cn

Ruby: arr = [1, 2, 3]
来源：http://zf.lnxyls.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qs.yuexingan06.cn

[D02] 追加元素到末尾
来源：http://ny.jctech888.com.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mc.panjiajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wb.yuexingan06.cn

JS:   arr.push(4);
来源：http://be.chemitech.net.cn

TS:   arr.push(4);
来源：http://jm.lnxyls.cn

Java: list.add(4);
来源：http://ur.shxzukj.cn

Go:   arr = append(arr, 4)
来源：http://ai.bjjhwx.cn

Ruby: arr << 4; arr.push(5)
来源：http://ad.szxytkj.cn

C#:   list.Add(4);
来源：http://qs.jianghongdianzi.cn

[D03] 在指定位置插入元素
来源：http://yr.521024.cn

Py:   arr.insert(0, 0)
来源：http://gq.huixinmuqiang.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://je.yuexingan06.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gx.jianghongdianzi.cn

TS:   arr.splice(0, 0, 0);
来源：http://bg.jianghongdianzi.cn

Java: list.add(0, 0);
来源：http://mc.521024.cn

Go:   arr = append([]int{0}, arr...)
来源：http://at.huixiangedu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ak.huixinmuqiang.cn

C#:   list.Insert(0, 0);
来源：http://oy.huanxung.cn

[D04] 删除元素
来源：http://nf.jctech888.com.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://oq.shtwfgs.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://av.shxzukj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ub.chemitech.net.cn

TS:   arr.splice(0, 1);
来源：http://vx.szxytkj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hu.lnxyls.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://iw.newstarts.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jo.muxihuayi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wh.yuntaijiaju.cn

[D05] 访问与修改元素
来源：http://vn.shxzskj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yb.bookmarksfly.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pz.colortex.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nz.nicolike.cn

TS:   arr[0]; arr.at(-1);
来源：http://ou.gzmigu.cn

Java: list.get(0); list.set(0, 9);
来源：http://jf.yuntaijiaju.cn

Go:   arr[0]; arr[0] = 9
来源：http://er.huixiangedu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gn.yuexingan06.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ym.bookmarksfly.cn

[D06] 数组长度
来源：http://au.shxzskj.cn

Py:   len(arr)
来源：http://qo.shxzskj.cn

PHP:  count($arr);
来源：http://bb.asd995.cn

JS:   arr.length
来源：http://ip.shxzukj.cn

TS:   arr.length
来源：http://gi.huanxung.cn

Java: list.size();
来源：http://nh.jctech888.com.cn

Go:   len(arr)
来源：http://wx.hahajie.cn

Ruby: arr.length; arr.size
来源：http://tx.szxytkj.cn

C#:   list.Count;
来源：http://af.shxzukj.cn

[D07] 切片 / 取子数组
来源：http://zn.hnjuh.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mr.hnjuh.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ac.shtwfgs.cn

JS:   arr.slice(1, 4);
来源：http://je.newstarts.cn

TS:   arr.slice(1, 4);
来源：http://yd.wgjwhj.cn

Java: list.subList(1, 4);
来源：http://vu.yuexingan06.cn

Go:   arr[1:4]
来源：http://my.lnxyls.cn

Ruby: arr[1, 3]
来源：http://gf.shxzukj.cn

C#:   list.GetRange(1, 3);
来源：http://xb.huixinmuqiang.cn

[D08] 合并两个数组
来源：http://fc.muxihuayi.cn

Py:   a + b;  a.extend(b)
来源：http://rq.yuexingan06.cn

PHP:  array_merge($a, $b);
来源：http://ji.bookmarksfly.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://er.wgjwhj.cn

TS:   [...a, ...b];
来源：http://qa.huanxung.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://di.9csxet.cn

Go:   append(a, b...)
来源：http://ph.hnjuh.cn

Ruby: a + b;  a.concat(b)
来源：http://so.gzmigu.cn

C#:   a.Concat(b).ToList()
来源：http://er.muxihuayi.cn

[D09] 排序（升序）
来源：http://hv.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://dx.jianghongdianzi.cn

PHP:  sort($arr);
来源：http://rg.wgjwhj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mp.haigaiapp.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://na.nicolike.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://qr.muxihuayi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dn.colortex.cn

Ruby: arr.sort
来源：http://ce.jctech888.com.cn

C#:   list.Sort();
来源：http://xu.huixinmuqiang.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://av.bookmarksfly.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vc.huixiangedu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kn.huanxung.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jl.hahajie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xq.gzmigu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://eg.szsharing.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dq.9csxet.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fg.lnxyls.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ex.shxzskj.cn

[D11] 反转数组
来源：http://av.shtwfgs.cn

Py:   arr[::-1];  arr.reverse()
来源：http://cm.shxzukj.cn

PHP:  array_reverse($arr);
来源：http://ap.asd995.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nu.521024.cn

TS:   [...arr].reverse();
来源：http://pr.hahajie.cn

Java: Collections.reverse(list);
来源：http://ly.9csxet.cn

Go:   slices.Reverse(arr)
来源：http://xv.shxzukj.cn

Ruby: arr.reverse
来源：http://eh.yuntaijiaju.cn

C#:   list.Reverse();
来源：http://mt.panjiajie.cn

[D12] 查找元素下标
来源：http://rn.jctech888.com.cn

Py:   arr.index(x);  x in arr
来源：http://uv.9csxet.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fn.huanxung.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xc.newstarts.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sn.bookmarksfly.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ex.szsharing.cn

Go:   slices.Index(arr, x)
来源：http://le.jianghongdianzi.cn

Ruby: arr.index(x)
来源：http://tg.huixinmuqiang.cn

C#:   list.IndexOf(x);
来源：http://yd.jctech888.com.cn

[D13] 过滤（保留满足条件的）
来源：http://qr.chemitech.net.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zd.huixiangedu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gv.huixinmuqiang.cn

JS:   arr.filter(x => x > 3)
来源：http://ks.521024.cn

TS:   arr.filter(x => x > 3)
来源：http://ut.muxihuayi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://iv.haigaiapp.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xu.szxytkj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xp.panjiajie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://xc.521024.cn

[D14] 映射转换（每个元素变形）
来源：http://ql.szxytkj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pg.chemitech.net.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xb.asd995.cn

JS:   arr.map(x => x * 2)
来源：http://lx.hnjuh.cn

TS:   arr.map(x => x * 2)
来源：http://sr.asd995.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://dt.9csxet.cn

Go:   // 手写循环
来源：http://ia.wgjwhj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://rd.hnjuh.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qf.yuexingan06.cn

[D15] 去重
来源：http://oq.wgjwhj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wq.szxytkj.cn

PHP:  array_unique($arr);
来源：http://zm.hnjuh.cn

JS:   [...new Set(arr)]
来源：http://un.szsharing.cn

TS:   [...new Set(arr)]
来源：http://oo.szxytkj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bk.shxzukj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://hk.521024.cn

Ruby: arr.uniq
来源：http://qz.szsharing.cn

C#:   list.Distinct().ToList()
来源：http://yd.huixinmuqiang.cn

[D16] 求和与平均值
来源：http://kq.szsharing.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dc.yuexingan06.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://up.huixinmuqiang.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://uy.lnxyls.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lx.gzmigu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gf.asd995.cn

Go:   // 手写循环累加
来源：http://dw.colortex.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hh.nicolike.cn

C#:   list.Sum();  list.Average()
来源：http://rw.haigaiapp.cn

[D17] 最大值与最小值
来源：http://kx.szsharing.cn

Py:   max(arr);  min(arr)
来源：http://qb.panjiajie.cn

PHP:  max($arr);  min($arr);
来源：http://du.szxytkj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dl.gzmigu.cn

TS:   Math.max(...arr);
来源：http://ml.asd995.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://uz.hahajie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qe.shtwfgs.cn

Ruby: arr.max;  arr.min
来源：http://zt.yuexingan06.cn

C#:   list.Max();  list.Min()
来源：http://dl.shxzukj.cn

[D18] 扁平化嵌套数组
来源：http://gz.hnjuh.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bi.yuntaijiaju.cn

PHP:  array_merge(...$nested);
来源：http://ho.yuexingan06.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yl.lnxyls.cn

TS:   nested.flat();
来源：http://hs.shxzukj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ji.wgjwhj.cn

Go:   // 手写双层循环
来源：http://gc.colortex.cn

Ruby: nested.flatten
来源：http://ng.lnxyls.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://pr.bookmarksfly.cn

[D19] 按字段分组
来源：http://zs.szsharing.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jk.521024.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://te.wgjwhj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pa.huixinmuqiang.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://li.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ba.colortex.cn

Go:   // 手写 map[string][]T
来源：http://fg.chemitech.net.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://bz.newstarts.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hm.shxzskj.cn

[D20] 统计每个元素出现次数
来源：http://bt.shxzskj.cn

Py:   Counter(arr)
来源：http://wv.panjiajie.cn

PHP:  array_count_values($arr);
来源：http://lp.newstarts.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dr.yuntaijiaju.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nh.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lz.lnxyls.cn

Go:   // 手写 map[T]int
来源：http://oe.nicolike.cn

Ruby: arr.tally
来源：http://xq.muxihuayi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nz.bookmarksfly.cn

[D21] 判断是否包含某元素
来源：http://xn.muxihuayi.cn

Py:   x in arr
来源：http://bz.nicolike.cn

PHP:  in_array($x, $arr, true);
来源：http://se.newstarts.cn

JS:   arr.includes(x)
来源：http://na.szsharing.cn

TS:   arr.includes(x)
来源：http://vv.newstarts.cn

Java: list.contains(x)
来源：http://rp.nicolike.cn

Go:   slices.Contains(arr, x)
来源：http://sd.shxzskj.cn

Ruby: arr.include?(x)
来源：http://rx.nicolike.cn

C#:   list.Contains(x)
来源：http://ys.hahajie.cn

[D22] 复制数组（避免共享引用）
来源：http://og.9csxet.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rb.nszjky.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://da.panjiajie.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xd.szsharing.cn

TS:   [...arr];
来源：http://zz.bjjhwx.cn

Java: new ArrayList<>(list);
来源：http://ne.hnjuh.cn

Go:   copied := append([]int(nil), arr...)
来源：http://yx.asd995.cn

Ruby: arr.dup;  arr.clone
来源：http://gr.chemitech.net.cn

C#:   new List<int>(list);
来源：http://hr.szsharing.cn

[D23] reduce 累积计算
来源：http://qs.hnjuh.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zi.shxzukj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pn.9csxet.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yd.huixiangedu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pz.521024.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://aa.521024.cn

Go:   // 手写循环
来源：http://cz.newstarts.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://km.szsharing.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zt.huanxung.cn

[D24] 字典 / Map 基本操作
来源：http://ka.9csxet.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tw.wgjwhj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://el.bookmarksfly.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://or.jianghongdianzi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://on.wgjwhj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://by.521024.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ni.muxihuayi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ph.jianghongdianzi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tt.bookmarksfly.cn

[D25] Set 集合去重与交并差
来源：http://lq.nszjky.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yc.9csxet.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lq.nicolike.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yw.huixiangedu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kp.haigaiapp.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ft.jianghongdianzi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tm.szxytkj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wu.huanxung.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rt.muxihuayi.cn

[D26] 数组转字符串
来源：http://cy.jianghongdianzi.cn

Py:   ", ".join(map(str, arr))
来源：http://wh.gzmigu.cn

PHP:  implode(", ", $arr);
来源：http://rc.gzmigu.cn

JS:   arr.join(", ")
来源：http://ec.hahajie.cn

TS:   arr.join(", ")
来源：http://jl.huanxung.cn

Java: String.join(", ", list)
来源：http://jk.yuntaijiaju.cn

Go:   strings.Join(strs, ", ")
来源：http://qv.szsharing.cn

Ruby: arr.join(", ")
来源：http://jx.521024.cn

C#:   string.Join(", ", list)
来源：http://fa.panjiajie.cn

================================================================================
来源：http://kv.hnjuh.cn

E. 字符串处理
来源：http://af.shxzukj.cn

================================================================================
来源：http://wv.nicolike.cn

[E01] 拼接字符串
来源：http://mo.9csxet.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yh.shtwfgs.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rc.yuexingan06.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lx.huixinmuqiang.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bw.gzmigu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://uk.szxytkj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yd.bookmarksfly.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://id.chemitech.net.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cd.jctech888.com.cn

[E02] 重复字符串
来源：http://hr.haigaiapp.cn

Py:   "ab" * 3
来源：http://ju.chemitech.net.cn

PHP:  str_repeat("ab", 3);
来源：http://kp.nszjky.cn

JS:   "ab".repeat(3)
来源：http://gm.shtwfgs.cn

TS:   "ab".repeat(3)
来源：http://hh.shtwfgs.cn

Java: "ab".repeat(3)
来源：http://zx.panjiajie.cn

Go:   strings.Repeat("ab", 3)
来源：http://qn.hnjuh.cn

Ruby: "ab" * 3
来源：http://sw.jianghongdianzi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://oi.521024.cn

[E03] 截取子串
来源：http://vv.shtwfgs.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bt.shtwfgs.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ik.hahajie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ea.lnxyls.cn

TS:   s.slice(1, 4)
来源：http://cs.muxihuayi.cn

Java: s.substring(1, 4)
来源：http://jn.chemitech.net.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wd.chemitech.net.cn

Ruby: s[1, 3];  s[1..3]
来源：http://qr.huixiangedu.cn

C#:   s.Substring(1, 3)
来源：http://pm.huanxung.cn

[E04] 查找子串位置
来源：http://fo.colortex.cn

Py:   s.find("x");  s.index("x")
来源：http://yh.huixinmuqiang.cn

PHP:  strpos($s, "x");
来源：http://mb.bjjhwx.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ej.shxzukj.cn

TS:   s.indexOf("x")
来源：http://sp.yuntaijiaju.cn

Java: s.indexOf("x")
来源：http://mh.chemitech.net.cn

Go:   strings.Index(s, "x")
来源：http://sk.shtwfgs.cn

Ruby: s.index("x")
来源：http://nn.shtwfgs.cn

C#:   s.IndexOf("x")
来源：http://la.panjiajie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://du.bookmarksfly.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cw.shxzukj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://gc.yuexingan06.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gv.shtwfgs.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://yv.muxihuayi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wy.szsharing.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ay.huixinmuqiang.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gn.asd995.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://aw.bookmarksfly.cn

[E06] 替换子串
来源：http://nl.521024.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mj.huixiangedu.cn

PHP:  str_replace("a", "b", $s);
来源：http://vr.szxytkj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hv.wgjwhj.cn

TS:   s.replaceAll("a", "b")
来源：http://qk.shxzukj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tg.yuntaijiaju.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lu.521024.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hk.bookmarksfly.cn

C#:   s.Replace("a", "b")
来源：http://hu.colortex.cn

[E07] 按分隔符拆分
来源：http://ff.9csxet.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dh.jctech888.com.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://af.nicolike.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://vs.panjiajie.cn

TS:   s.split(",")
来源：http://fv.shxzskj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://uu.szxytkj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ll.shtwfgs.cn

Ruby: s.split(",");  s.split
来源：http://nw.haigaiapp.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gy.muxihuayi.cn

[E08] 数组按分隔符合并
来源：http://dr.shtwfgs.cn

Py:   ",".join(items)
来源：http://gq.9csxet.cn

PHP:  implode(",", $items);
来源：http://ru.muxihuayi.cn

JS:   items.join(",")
来源：http://sx.asd995.cn

TS:   items.join(",")
来源：http://eb.nszjky.cn

Java: String.join(",", items)
来源：http://tg.shtwfgs.cn


<!-- 参考信息 -->