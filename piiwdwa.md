代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://ad.wgjwhj.cn

Ruby: arr = [1, 2, 3]
来源：http://sz.colortex.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wf.nicolike.cn

[D02] 追加元素到末尾
来源：http://yu.shxzskj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fr.521024.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ls.9csxet.cn

JS:   arr.push(4);
来源：http://us.asd995.cn

TS:   arr.push(4);
来源：http://nw.huanxung.cn

Java: list.add(4);
来源：http://sp.asd995.cn

Go:   arr = append(arr, 4)
来源：http://rm.nicolike.cn

Ruby: arr << 4; arr.push(5)
来源：http://kn.szsharing.cn

C#:   list.Add(4);
来源：http://wi.szxytkj.cn

[D03] 在指定位置插入元素
来源：http://io.huanxung.cn

Py:   arr.insert(0, 0)
来源：http://fn.bjjhwx.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dr.panjiajie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kq.9csxet.cn

TS:   arr.splice(0, 0, 0);
来源：http://ym.nicolike.cn

Java: list.add(0, 0);
来源：http://vj.bjjhwx.cn

Go:   arr = append([]int{0}, arr...)
来源：http://qb.9csxet.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xs.asd995.cn

C#:   list.Insert(0, 0);
来源：http://bw.bjjhwx.cn

[D04] 删除元素
来源：http://mc.szxytkj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://km.nicolike.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://va.jctech888.com.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yw.shxzukj.cn

TS:   arr.splice(0, 1);
来源：http://do.jianghongdianzi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jo.shtwfgs.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xg.jctech888.com.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vx.wgjwhj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ow.haigaiapp.cn

[D05] 访问与修改元素
来源：http://ji.szxytkj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pc.shtwfgs.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://on.chemitech.net.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://oe.lnxyls.cn

TS:   arr[0]; arr.at(-1);
来源：http://rl.9csxet.cn

Java: list.get(0); list.set(0, 9);
来源：http://ge.521024.cn

Go:   arr[0]; arr[0] = 9
来源：http://lu.9csxet.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pv.bjjhwx.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bi.shxzskj.cn

[D06] 数组长度
来源：http://vn.newstarts.cn

Py:   len(arr)
来源：http://cj.bjjhwx.cn

PHP:  count($arr);
来源：http://cy.huixiangedu.cn

JS:   arr.length
来源：http://vz.haigaiapp.cn

TS:   arr.length
来源：http://ug.huixiangedu.cn

Java: list.size();
来源：http://lw.colortex.cn

Go:   len(arr)
来源：http://ey.lnxyls.cn

Ruby: arr.length; arr.size
来源：http://qz.chemitech.net.cn

C#:   list.Count;
来源：http://px.lnxyls.cn

[D07] 切片 / 取子数组
来源：http://ah.muxihuayi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nf.lnxyls.cn

PHP:  array_slice($arr, 1, 3);
来源：http://zy.muxihuayi.cn

JS:   arr.slice(1, 4);
来源：http://gj.jctech888.com.cn

TS:   arr.slice(1, 4);
来源：http://av.chemitech.net.cn

Java: list.subList(1, 4);
来源：http://xv.jianghongdianzi.cn

Go:   arr[1:4]
来源：http://mc.lnxyls.cn

Ruby: arr[1, 3]
来源：http://ms.chemitech.net.cn

C#:   list.GetRange(1, 3);
来源：http://io.szsharing.cn

[D08] 合并两个数组
来源：http://zr.muxihuayi.cn

Py:   a + b;  a.extend(b)
来源：http://um.521024.cn

PHP:  array_merge($a, $b);
来源：http://qs.bookmarksfly.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://tg.yuntaijiaju.cn

TS:   [...a, ...b];
来源：http://ne.chemitech.net.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xc.muxihuayi.cn

Go:   append(a, b...)
来源：http://vw.wgjwhj.cn

Ruby: a + b;  a.concat(b)
来源：http://ba.9csxet.cn

C#:   a.Concat(b).ToList()
来源：http://yk.panjiajie.cn

[D09] 排序（升序）
来源：http://qk.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://wx.huixiangedu.cn

PHP:  sort($arr);
来源：http://hn.newstarts.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hw.gzmigu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://qt.huixiangedu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://tc.shtwfgs.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hl.yuexingan06.cn

Ruby: arr.sort
来源：http://ch.521024.cn

C#:   list.Sort();
来源：http://ry.szsharing.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://vs.wgjwhj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vi.lnxyls.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pm.huixiangedu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kq.gzmigu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pc.521024.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ke.jctech888.com.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ga.hahajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://et.shxzukj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://so.newstarts.cn

[D11] 反转数组
来源：http://qd.shxzukj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://yc.muxihuayi.cn

PHP:  array_reverse($arr);
来源：http://so.hahajie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hh.panjiajie.cn

TS:   [...arr].reverse();
来源：http://zb.colortex.cn

Java: Collections.reverse(list);
来源：http://bd.asd995.cn

Go:   slices.Reverse(arr)
来源：http://wj.521024.cn

Ruby: arr.reverse
来源：http://az.szxytkj.cn

C#:   list.Reverse();
来源：http://mz.huixinmuqiang.cn

[D12] 查找元素下标
来源：http://ys.gzmigu.cn

Py:   arr.index(x);  x in arr
来源：http://gu.yuexingan06.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yj.panjiajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nv.yuexingan06.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://st.yuntaijiaju.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lu.muxihuayi.cn

Go:   slices.Index(arr, x)
来源：http://ub.chemitech.net.cn

Ruby: arr.index(x)
来源：http://hf.wgjwhj.cn

C#:   list.IndexOf(x);
来源：http://qt.nicolike.cn

[D13] 过滤（保留满足条件的）
来源：http://lq.jctech888.com.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qg.chemitech.net.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qm.hnjuh.cn

JS:   arr.filter(x => x > 3)
来源：http://jr.nszjky.cn

TS:   arr.filter(x => x > 3)
来源：http://pi.bjjhwx.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lk.szsharing.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://eu.huanxung.cn

Ruby: arr.select { |x| x > 3 }
来源：http://be.huixiangedu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://av.yuexingan06.cn

[D14] 映射转换（每个元素变形）
来源：http://sn.gzmigu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dx.gzmigu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wl.huixinmuqiang.cn

JS:   arr.map(x => x * 2)
来源：http://jq.bjjhwx.cn

TS:   arr.map(x => x * 2)
来源：http://ag.521024.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://pk.hnjuh.cn

Go:   // 手写循环
来源：http://mo.huixiangedu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ky.wgjwhj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://cf.9csxet.cn

[D15] 去重
来源：http://zi.newstarts.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zh.huixiangedu.cn

PHP:  array_unique($arr);
来源：http://sj.bookmarksfly.cn

JS:   [...new Set(arr)]
来源：http://gi.shxzukj.cn

TS:   [...new Set(arr)]
来源：http://jt.newstarts.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bv.szxytkj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://jn.newstarts.cn

Ruby: arr.uniq
来源：http://jp.lnxyls.cn

C#:   list.Distinct().ToList()
来源：http://vn.nicolike.cn

[D16] 求和与平均值
来源：http://ab.lnxyls.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ts.chemitech.net.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dq.shxzukj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://th.nszjky.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fy.colortex.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qg.shtwfgs.cn

Go:   // 手写循环累加
来源：http://hu.bookmarksfly.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jw.jctech888.com.cn

C#:   list.Sum();  list.Average()
来源：http://kn.jianghongdianzi.cn

[D17] 最大值与最小值
来源：http://zm.gzmigu.cn

Py:   max(arr);  min(arr)
来源：http://nc.muxihuayi.cn

PHP:  max($arr);  min($arr);
来源：http://nt.szsharing.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mi.panjiajie.cn

TS:   Math.max(...arr);
来源：http://cw.hahajie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ym.chemitech.net.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vu.shxzukj.cn

Ruby: arr.max;  arr.min
来源：http://lg.asd995.cn

C#:   list.Max();  list.Min()
来源：http://of.chemitech.net.cn

[D18] 扁平化嵌套数组
来源：http://ha.9csxet.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rt.hahajie.cn

PHP:  array_merge(...$nested);
来源：http://tu.jctech888.com.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yq.colortex.cn

TS:   nested.flat();
来源：http://gj.9csxet.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zd.wgjwhj.cn

Go:   // 手写双层循环
来源：http://ce.nszjky.cn

Ruby: nested.flatten
来源：http://ut.nicolike.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://za.shxzukj.cn

[D19] 按字段分组
来源：http://br.jianghongdianzi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xk.muxihuayi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fb.asd995.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qq.jianghongdianzi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://kz.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ky.colortex.cn

Go:   // 手写 map[string][]T
来源：http://cx.shtwfgs.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://iu.huixiangedu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pe.9csxet.cn

[D20] 统计每个元素出现次数
来源：http://dh.521024.cn

Py:   Counter(arr)
来源：http://lo.asd995.cn

PHP:  array_count_values($arr);
来源：http://tv.colortex.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hu.shtwfgs.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ke.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wj.yuntaijiaju.cn

Go:   // 手写 map[T]int
来源：http://hh.9csxet.cn

Ruby: arr.tally
来源：http://xf.panjiajie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sc.huanxung.cn

[D21] 判断是否包含某元素
来源：http://cl.nicolike.cn

Py:   x in arr
来源：http://fh.521024.cn

PHP:  in_array($x, $arr, true);
来源：http://js.hnjuh.cn

JS:   arr.includes(x)
来源：http://yx.wgjwhj.cn

TS:   arr.includes(x)
来源：http://np.jianghongdianzi.cn

Java: list.contains(x)
来源：http://mv.newstarts.cn

Go:   slices.Contains(arr, x)
来源：http://kn.lnxyls.cn

Ruby: arr.include?(x)
来源：http://nb.huanxung.cn

C#:   list.Contains(x)
来源：http://td.521024.cn

[D22] 复制数组（避免共享引用）
来源：http://vz.panjiajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xe.huixinmuqiang.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://me.yuexingan06.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ey.szxytkj.cn

TS:   [...arr];
来源：http://rd.newstarts.cn

Java: new ArrayList<>(list);
来源：http://ht.muxihuayi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://kd.muxihuayi.cn

Ruby: arr.dup;  arr.clone
来源：http://eq.szxytkj.cn

C#:   new List<int>(list);
来源：http://pt.asd995.cn

[D23] reduce 累积计算
来源：http://ja.jianghongdianzi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gv.gzmigu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hx.huixinmuqiang.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vz.nicolike.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ct.gzmigu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xh.bookmarksfly.cn

Go:   // 手写循环
来源：http://ar.asd995.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pc.chemitech.net.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://od.newstarts.cn

[D24] 字典 / Map 基本操作
来源：http://sm.hahajie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xv.yuexingan06.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kb.lnxyls.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mi.hnjuh.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ww.szxytkj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zz.huanxung.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kh.lnxyls.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://iu.jianghongdianzi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tx.haigaiapp.cn

[D25] Set 集合去重与交并差
来源：http://xv.newstarts.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cd.jianghongdianzi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qr.hahajie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ci.gzmigu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gj.haigaiapp.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ah.bookmarksfly.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xj.panjiajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qj.panjiajie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://au.chemitech.net.cn

[D26] 数组转字符串
来源：http://nj.gzmigu.cn

Py:   ", ".join(map(str, arr))
来源：http://gd.gzmigu.cn

PHP:  implode(", ", $arr);
来源：http://gs.shtwfgs.cn

JS:   arr.join(", ")
来源：http://vc.panjiajie.cn

TS:   arr.join(", ")
来源：http://pu.szxytkj.cn

Java: String.join(", ", list)
来源：http://rl.szxytkj.cn

Go:   strings.Join(strs, ", ")
来源：http://pa.newstarts.cn

Ruby: arr.join(", ")
来源：http://vw.bjjhwx.cn

C#:   string.Join(", ", list)
来源：http://iw.shxzskj.cn

================================================================================
来源：http://bg.szsharing.cn

E. 字符串处理
来源：http://si.panjiajie.cn

================================================================================
来源：http://ry.huanxung.cn

[E01] 拼接字符串
来源：http://hb.shxzukj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qv.newstarts.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bt.9csxet.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ir.shxzukj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kf.gzmigu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ft.colortex.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ko.newstarts.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yx.jianghongdianzi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kw.asd995.cn

[E02] 重复字符串
来源：http://cb.jianghongdianzi.cn

Py:   "ab" * 3
来源：http://gf.bookmarksfly.cn

PHP:  str_repeat("ab", 3);
来源：http://lm.muxihuayi.cn

JS:   "ab".repeat(3)
来源：http://sd.lnxyls.cn

TS:   "ab".repeat(3)
来源：http://rv.9csxet.cn

Java: "ab".repeat(3)
来源：http://st.shxzukj.cn

Go:   strings.Repeat("ab", 3)
来源：http://bx.panjiajie.cn

Ruby: "ab" * 3
来源：http://ab.521024.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rk.hahajie.cn

[E03] 截取子串
来源：http://vt.chemitech.net.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qh.nicolike.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fv.huixiangedu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ta.chemitech.net.cn

TS:   s.slice(1, 4)
来源：http://ke.panjiajie.cn

Java: s.substring(1, 4)
来源：http://ps.newstarts.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ll.hahajie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://eh.9csxet.cn

C#:   s.Substring(1, 3)
来源：http://df.shxzskj.cn

[E04] 查找子串位置
来源：http://sv.nszjky.cn

Py:   s.find("x");  s.index("x")
来源：http://fs.521024.cn

PHP:  strpos($s, "x");
来源：http://lt.muxihuayi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lz.szxytkj.cn

TS:   s.indexOf("x")
来源：http://df.huixiangedu.cn

Java: s.indexOf("x")
来源：http://fz.huixinmuqiang.cn

Go:   strings.Index(s, "x")
来源：http://jg.9csxet.cn

Ruby: s.index("x")
来源：http://am.shxzukj.cn

C#:   s.IndexOf("x")
来源：http://nf.huixiangedu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://jd.gzmigu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mn.shtwfgs.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jn.shxzukj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ys.gzmigu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://yq.yuexingan06.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ix.shxzukj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sg.bookmarksfly.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ef.colortex.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ba.huixiangedu.cn

[E06] 替换子串
来源：http://eo.jianghongdianzi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ob.wgjwhj.cn

PHP:  str_replace("a", "b", $s);
来源：http://wf.huixinmuqiang.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qt.szxytkj.cn

TS:   s.replaceAll("a", "b")
来源：http://ye.yuexingan06.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ek.521024.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bj.shxzukj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wq.panjiajie.cn

C#:   s.Replace("a", "b")
来源：http://zy.huixinmuqiang.cn

[E07] 按分隔符拆分
来源：http://xg.szxytkj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wi.nicolike.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://su.hahajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://hj.muxihuayi.cn

TS:   s.split(",")
来源：http://by.colortex.cn

Java: s.split(",");  s.split("\\s+")
来源：http://pn.huixiangedu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jo.szxytkj.cn

Ruby: s.split(",");  s.split
来源：http://pn.521024.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fd.shxzukj.cn

[E08] 数组按分隔符合并
来源：http://qr.521024.cn

Py:   ",".join(items)
来源：http://gq.asd995.cn

PHP:  implode(",", $items);
来源：http://rj.jianghongdianzi.cn

JS:   items.join(",")
来源：http://nq.shxzskj.cn

TS:   items.join(",")
来源：http://tg.lnxyls.cn

Java: String.join(",", items)
来源：http://vx.hahajie.cn


<!-- 参考信息 -->