代发 wailian999

D. 数组 / 列表 / 集合
来源：http://yr.newstarts.cn

================================================================================
来源：http://px.huixiangedu.cn

[D01] 创建数组 / 列表
来源：http://aw.yuexingan06.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mv.yuntaijiaju.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gh.521024.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gl.shxzskj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://zn.panjiajie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://am.jianghongdianzi.cn

Go:   arr := []int{1, 2, 3}
来源：http://lg.newstarts.cn

Ruby: arr = [1, 2, 3]
来源：http://vm.shxzskj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nn.yuexingan06.cn

[D02] 追加元素到末尾
来源：http://bz.yuntaijiaju.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ht.hnjuh.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ie.9csxet.cn

JS:   arr.push(4);
来源：http://hl.jctech888.com.cn

TS:   arr.push(4);
来源：http://pw.bjjhwx.cn

Java: list.add(4);
来源：http://zg.asd995.cn

Go:   arr = append(arr, 4)
来源：http://ho.panjiajie.cn

Ruby: arr << 4; arr.push(5)
来源：http://re.colortex.cn

C#:   list.Add(4);
来源：http://kn.colortex.cn

[D03] 在指定位置插入元素
来源：http://km.huixiangedu.cn

Py:   arr.insert(0, 0)
来源：http://nn.gzmigu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ry.jctech888.com.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://my.nicolike.cn

TS:   arr.splice(0, 0, 0);
来源：http://mf.huanxung.cn

Java: list.add(0, 0);
来源：http://tl.colortex.cn

Go:   arr = append([]int{0}, arr...)
来源：http://za.lnxyls.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gi.nszjky.cn

C#:   list.Insert(0, 0);
来源：http://cy.shxzskj.cn

[D04] 删除元素
来源：http://yu.nszjky.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ux.jctech888.com.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ha.szsharing.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xl.wgjwhj.cn

TS:   arr.splice(0, 1);
来源：http://yb.jctech888.com.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ge.colortex.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://df.wgjwhj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vn.jctech888.com.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zl.chemitech.net.cn

[D05] 访问与修改元素
来源：http://wo.muxihuayi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cl.bjjhwx.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://np.huanxung.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cn.huixiangedu.cn

TS:   arr[0]; arr.at(-1);
来源：http://yc.szsharing.cn

Java: list.get(0); list.set(0, 9);
来源：http://em.jctech888.com.cn

Go:   arr[0]; arr[0] = 9
来源：http://uo.gzmigu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://as.szsharing.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qp.haigaiapp.cn

[D06] 数组长度
来源：http://db.nszjky.cn

Py:   len(arr)
来源：http://su.muxihuayi.cn

PHP:  count($arr);
来源：http://fy.colortex.cn

JS:   arr.length
来源：http://xq.asd995.cn

TS:   arr.length
来源：http://jb.jianghongdianzi.cn

Java: list.size();
来源：http://eq.haigaiapp.cn

Go:   len(arr)
来源：http://ba.shtwfgs.cn

Ruby: arr.length; arr.size
来源：http://cj.yuexingan06.cn

C#:   list.Count;
来源：http://gq.bookmarksfly.cn

[D07] 切片 / 取子数组
来源：http://ru.huixiangedu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yw.szxytkj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://pc.wgjwhj.cn

JS:   arr.slice(1, 4);
来源：http://wz.jctech888.com.cn

TS:   arr.slice(1, 4);
来源：http://il.wgjwhj.cn

Java: list.subList(1, 4);
来源：http://ba.lnxyls.cn

Go:   arr[1:4]
来源：http://oi.huanxung.cn

Ruby: arr[1, 3]
来源：http://wc.szxytkj.cn

C#:   list.GetRange(1, 3);
来源：http://ln.jctech888.com.cn

[D08] 合并两个数组
来源：http://qw.szxytkj.cn

Py:   a + b;  a.extend(b)
来源：http://lb.521024.cn

PHP:  array_merge($a, $b);
来源：http://ed.szxytkj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://op.9csxet.cn

TS:   [...a, ...b];
来源：http://iu.huixinmuqiang.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hp.colortex.cn

Go:   append(a, b...)
来源：http://im.colortex.cn

Ruby: a + b;  a.concat(b)
来源：http://rs.hahajie.cn

C#:   a.Concat(b).ToList()
来源：http://rs.nicolike.cn

[D09] 排序（升序）
来源：http://db.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://lv.newstarts.cn

PHP:  sort($arr);
来源：http://bg.asd995.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wf.huixinmuqiang.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://yl.lnxyls.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://kl.huixiangedu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://po.szxytkj.cn

Ruby: arr.sort
来源：http://df.nicolike.cn

C#:   list.Sort();
来源：http://it.nicolike.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://hw.gzmigu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://py.jianghongdianzi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ql.muxihuayi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gj.wgjwhj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ax.shxzukj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://oa.shtwfgs.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tt.shtwfgs.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tf.asd995.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://od.lnxyls.cn

[D11] 反转数组
来源：http://fb.yuexingan06.cn

Py:   arr[::-1];  arr.reverse()
来源：http://rg.yuexingan06.cn

PHP:  array_reverse($arr);
来源：http://gb.hnjuh.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://sr.lnxyls.cn

TS:   [...arr].reverse();
来源：http://os.gzmigu.cn

Java: Collections.reverse(list);
来源：http://ws.hahajie.cn

Go:   slices.Reverse(arr)
来源：http://bz.lnxyls.cn

Ruby: arr.reverse
来源：http://ad.wgjwhj.cn

C#:   list.Reverse();
来源：http://zo.muxihuayi.cn

[D12] 查找元素下标
来源：http://af.9csxet.cn

Py:   arr.index(x);  x in arr
来源：http://jf.huixiangedu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kb.hahajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ru.lnxyls.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uq.chemitech.net.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kc.yuexingan06.cn

Go:   slices.Index(arr, x)
来源：http://vt.chemitech.net.cn

Ruby: arr.index(x)
来源：http://yq.szsharing.cn

C#:   list.IndexOf(x);
来源：http://cm.colortex.cn

[D13] 过滤（保留满足条件的）
来源：http://st.hahajie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qs.shxzukj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://au.shxzukj.cn

JS:   arr.filter(x => x > 3)
来源：http://lj.hnjuh.cn

TS:   arr.filter(x => x > 3)
来源：http://dj.nszjky.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ow.chemitech.net.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://uk.jianghongdianzi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hb.szsharing.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://um.lnxyls.cn

[D14] 映射转换（每个元素变形）
来源：http://yw.szsharing.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tn.bjjhwx.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://eh.shxzskj.cn

JS:   arr.map(x => x * 2)
来源：http://me.521024.cn

TS:   arr.map(x => x * 2)
来源：http://cb.shxzukj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://vt.nicolike.cn

Go:   // 手写循环
来源：http://mk.521024.cn

Ruby: arr.map { |x| x * 2 }
来源：http://eq.muxihuayi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://fs.haigaiapp.cn

[D15] 去重
来源：http://pf.shxzukj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qd.muxihuayi.cn

PHP:  array_unique($arr);
来源：http://wr.szsharing.cn

JS:   [...new Set(arr)]
来源：http://fl.jctech888.com.cn

TS:   [...new Set(arr)]
来源：http://ir.9csxet.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dc.colortex.cn

Go:   // 用 map[T]struct{} 手写
来源：http://do.huanxung.cn

Ruby: arr.uniq
来源：http://vh.huanxung.cn

C#:   list.Distinct().ToList()
来源：http://hz.gzmigu.cn

[D16] 求和与平均值
来源：http://sz.nszjky.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yp.chemitech.net.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kf.huixiangedu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://am.szsharing.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sa.huixiangedu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bs.jianghongdianzi.cn

Go:   // 手写循环累加
来源：http://lc.yuexingan06.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ai.haigaiapp.cn

C#:   list.Sum();  list.Average()
来源：http://og.colortex.cn

[D17] 最大值与最小值
来源：http://xq.chemitech.net.cn

Py:   max(arr);  min(arr)
来源：http://lh.jctech888.com.cn

PHP:  max($arr);  min($arr);
来源：http://lr.colortex.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mu.asd995.cn

TS:   Math.max(...arr);
来源：http://so.9csxet.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://hb.newstarts.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zu.hnjuh.cn

Ruby: arr.max;  arr.min
来源：http://jv.huixiangedu.cn

C#:   list.Max();  list.Min()
来源：http://fx.521024.cn

[D18] 扁平化嵌套数组
来源：http://wd.gzmigu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xa.panjiajie.cn

PHP:  array_merge(...$nested);
来源：http://es.lnxyls.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fl.szxytkj.cn

TS:   nested.flat();
来源：http://hu.jianghongdianzi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kx.shxzskj.cn

Go:   // 手写双层循环
来源：http://rn.szxytkj.cn

Ruby: nested.flatten
来源：http://gl.shxzskj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://th.521024.cn

[D19] 按字段分组
来源：http://kb.yuexingan06.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wt.chemitech.net.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ag.muxihuayi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gi.panjiajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://no.gzmigu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yq.asd995.cn

Go:   // 手写 map[string][]T
来源：http://bn.huixinmuqiang.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://za.asd995.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xu.shxzukj.cn

[D20] 统计每个元素出现次数
来源：http://xf.szxytkj.cn

Py:   Counter(arr)
来源：http://vl.shxzskj.cn

PHP:  array_count_values($arr);
来源：http://vc.colortex.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ji.newstarts.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ge.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bp.panjiajie.cn

Go:   // 手写 map[T]int
来源：http://px.huixinmuqiang.cn

Ruby: arr.tally
来源：http://md.gzmigu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://uv.9csxet.cn

[D21] 判断是否包含某元素
来源：http://bh.521024.cn

Py:   x in arr
来源：http://tl.yuexingan06.cn

PHP:  in_array($x, $arr, true);
来源：http://rm.bookmarksfly.cn

JS:   arr.includes(x)
来源：http://kq.colortex.cn

TS:   arr.includes(x)
来源：http://bn.huixiangedu.cn

Java: list.contains(x)
来源：http://li.szxytkj.cn

Go:   slices.Contains(arr, x)
来源：http://hd.hahajie.cn

Ruby: arr.include?(x)
来源：http://xp.shxzukj.cn

C#:   list.Contains(x)
来源：http://lz.colortex.cn

[D22] 复制数组（避免共享引用）
来源：http://ja.chemitech.net.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qf.szxytkj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gk.shtwfgs.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vv.shtwfgs.cn

TS:   [...arr];
来源：http://aa.colortex.cn

Java: new ArrayList<>(list);
来源：http://ci.521024.cn

Go:   copied := append([]int(nil), arr...)
来源：http://wy.yuntaijiaju.cn

Ruby: arr.dup;  arr.clone
来源：http://zx.newstarts.cn

C#:   new List<int>(list);
来源：http://iq.9csxet.cn

[D23] reduce 累积计算
来源：http://fd.yuexingan06.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jd.9csxet.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pi.huanxung.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ch.yuexingan06.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ki.shtwfgs.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://re.shtwfgs.cn

Go:   // 手写循环
来源：http://sf.shxzukj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://co.nszjky.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://il.huanxung.cn

[D24] 字典 / Map 基本操作
来源：http://ku.haigaiapp.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nk.yuntaijiaju.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cx.szsharing.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dd.jctech888.com.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://he.chemitech.net.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fb.bookmarksfly.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cf.hahajie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://sx.hahajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wy.huixinmuqiang.cn

[D25] Set 集合去重与交并差
来源：http://ej.yuexingan06.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qj.huixinmuqiang.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wk.szxytkj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mp.jctech888.com.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gh.hahajie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://di.huixiangedu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vi.nszjky.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://oy.521024.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wn.yuexingan06.cn

[D26] 数组转字符串
来源：http://ox.panjiajie.cn

Py:   ", ".join(map(str, arr))
来源：http://ce.shxzskj.cn

PHP:  implode(", ", $arr);
来源：http://qx.panjiajie.cn

JS:   arr.join(", ")
来源：http://fv.bjjhwx.cn

TS:   arr.join(", ")
来源：http://ze.jianghongdianzi.cn

Java: String.join(", ", list)
来源：http://ht.hahajie.cn

Go:   strings.Join(strs, ", ")
来源：http://rw.bookmarksfly.cn

Ruby: arr.join(", ")
来源：http://oi.huixiangedu.cn

C#:   string.Join(", ", list)
来源：http://ph.wgjwhj.cn

================================================================================
来源：http://fe.gzmigu.cn

E. 字符串处理
来源：http://ho.yuexingan06.cn

================================================================================
来源：http://fo.jianghongdianzi.cn

[E01] 拼接字符串
来源：http://mo.shxzukj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jm.panjiajie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://be.colortex.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wp.shxzskj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ch.hahajie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dx.muxihuayi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://be.hahajie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://la.nszjky.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gg.hnjuh.cn

[E02] 重复字符串
来源：http://ob.panjiajie.cn

Py:   "ab" * 3
来源：http://qe.521024.cn

PHP:  str_repeat("ab", 3);
来源：http://vk.panjiajie.cn

JS:   "ab".repeat(3)
来源：http://mn.shtwfgs.cn

TS:   "ab".repeat(3)
来源：http://xj.jianghongdianzi.cn

Java: "ab".repeat(3)
来源：http://yw.szsharing.cn

Go:   strings.Repeat("ab", 3)
来源：http://dr.huixiangedu.cn

Ruby: "ab" * 3
来源：http://le.bjjhwx.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hx.hahajie.cn

[E03] 截取子串
来源：http://hu.newstarts.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mw.shxzukj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tv.yuexingan06.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wb.bookmarksfly.cn

TS:   s.slice(1, 4)
来源：http://vo.colortex.cn

Java: s.substring(1, 4)
来源：http://ey.jianghongdianzi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jp.shtwfgs.cn

Ruby: s[1, 3];  s[1..3]
来源：http://qk.shxzukj.cn

C#:   s.Substring(1, 3)
来源：http://ct.nicolike.cn

[E04] 查找子串位置
来源：http://lu.haigaiapp.cn

Py:   s.find("x");  s.index("x")
来源：http://ye.bjjhwx.cn

PHP:  strpos($s, "x");
来源：http://li.chemitech.net.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://li.huanxung.cn

TS:   s.indexOf("x")
来源：http://aq.bookmarksfly.cn

Java: s.indexOf("x")
来源：http://yx.shxzskj.cn

Go:   strings.Index(s, "x")
来源：http://eo.haigaiapp.cn

Ruby: s.index("x")
来源：http://wy.jctech888.com.cn

C#:   s.IndexOf("x")
来源：http://rg.colortex.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://wx.9csxet.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vz.huixinmuqiang.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fd.asd995.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xs.lnxyls.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://fb.szxytkj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yq.haigaiapp.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bh.huixiangedu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lg.nszjky.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://en.asd995.cn

[E06] 替换子串
来源：http://zj.nicolike.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jq.jianghongdianzi.cn

PHP:  str_replace("a", "b", $s);
来源：http://am.huixiangedu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bd.9csxet.cn

TS:   s.replaceAll("a", "b")
来源：http://vd.shtwfgs.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ll.yuntaijiaju.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jk.huixiangedu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xc.muxihuayi.cn

C#:   s.Replace("a", "b")
来源：http://ch.lnxyls.cn

[E07] 按分隔符拆分
来源：http://pm.szsharing.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yo.wgjwhj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bu.shxzskj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://fe.shxzukj.cn

TS:   s.split(",")
来源：http://yx.huixiangedu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://dj.jctech888.com.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lu.nicolike.cn


<!-- 参考信息 -->