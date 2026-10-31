代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lk.yuexingan06.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mn.szsharing.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://vt.newstarts.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qf.huanxung.cn

Go:   arr := []int{1, 2, 3}
来源：http://ob.shxzskj.cn

Ruby: arr = [1, 2, 3]
来源：http://uc.gzmigu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ef.szsharing.cn

[D02] 追加元素到末尾
来源：http://ux.gzmigu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ab.gzmigu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zw.nicolike.cn

JS:   arr.push(4);
来源：http://re.bookmarksfly.cn

TS:   arr.push(4);
来源：http://rs.gzmigu.cn

Java: list.add(4);
来源：http://sf.hnjuh.cn

Go:   arr = append(arr, 4)
来源：http://ya.jctech888.com.cn

Ruby: arr << 4; arr.push(5)
来源：http://pl.newstarts.cn

C#:   list.Add(4);
来源：http://qh.nszjky.cn

[D03] 在指定位置插入元素
来源：http://vv.szsharing.cn

Py:   arr.insert(0, 0)
来源：http://tx.huanxung.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xh.jianghongdianzi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dw.yuexingan06.cn

TS:   arr.splice(0, 0, 0);
来源：http://yr.yuexingan06.cn

Java: list.add(0, 0);
来源：http://dq.haigaiapp.cn

Go:   arr = append([]int{0}, arr...)
来源：http://eq.nszjky.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ia.hahajie.cn

C#:   list.Insert(0, 0);
来源：http://ot.muxihuayi.cn

[D04] 删除元素
来源：http://xm.hahajie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://oj.bookmarksfly.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yp.bjjhwx.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ik.nszjky.cn

TS:   arr.splice(0, 1);
来源：http://kg.9csxet.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://me.asd995.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ue.jianghongdianzi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ab.nszjky.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sa.hahajie.cn

[D05] 访问与修改元素
来源：http://on.9csxet.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lz.asd995.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xu.hahajie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fk.asd995.cn

TS:   arr[0]; arr.at(-1);
来源：http://df.huanxung.cn

Java: list.get(0); list.set(0, 9);
来源：http://xl.huixiangedu.cn

Go:   arr[0]; arr[0] = 9
来源：http://fz.szsharing.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pf.muxihuayi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nu.jctech888.com.cn

[D06] 数组长度
来源：http://gx.szxytkj.cn

Py:   len(arr)
来源：http://er.gzmigu.cn

PHP:  count($arr);
来源：http://lk.szsharing.cn

JS:   arr.length
来源：http://cs.shtwfgs.cn

TS:   arr.length
来源：http://ki.nszjky.cn

Java: list.size();
来源：http://vx.shxzskj.cn

Go:   len(arr)
来源：http://xd.nicolike.cn

Ruby: arr.length; arr.size
来源：http://mk.jianghongdianzi.cn

C#:   list.Count;
来源：http://vg.bookmarksfly.cn

[D07] 切片 / 取子数组
来源：http://uy.hnjuh.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qa.panjiajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://em.shxzskj.cn

JS:   arr.slice(1, 4);
来源：http://kw.huixinmuqiang.cn

TS:   arr.slice(1, 4);
来源：http://qd.yuexingan06.cn

Java: list.subList(1, 4);
来源：http://lc.haigaiapp.cn

Go:   arr[1:4]
来源：http://ud.yuntaijiaju.cn

Ruby: arr[1, 3]
来源：http://ce.szxytkj.cn

C#:   list.GetRange(1, 3);
来源：http://ge.colortex.cn

[D08] 合并两个数组
来源：http://hq.yuexingan06.cn

Py:   a + b;  a.extend(b)
来源：http://el.bjjhwx.cn

PHP:  array_merge($a, $b);
来源：http://yz.asd995.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://hm.wgjwhj.cn

TS:   [...a, ...b];
来源：http://na.hnjuh.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://me.shxzukj.cn

Go:   append(a, b...)
来源：http://zd.chemitech.net.cn

Ruby: a + b;  a.concat(b)
来源：http://ax.chemitech.net.cn

C#:   a.Concat(b).ToList()
来源：http://pl.wgjwhj.cn

[D09] 排序（升序）
来源：http://rl.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://cv.nicolike.cn

PHP:  sort($arr);
来源：http://mr.shtwfgs.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://op.bookmarksfly.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://sx.yuntaijiaju.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://tg.jctech888.com.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ai.521024.cn

Ruby: arr.sort
来源：http://ky.shxzskj.cn

C#:   list.Sort();
来源：http://ea.hnjuh.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://fm.asd995.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ri.panjiajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ke.bjjhwx.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gv.jianghongdianzi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ej.jianghongdianzi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mr.jctech888.com.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gv.bookmarksfly.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fe.asd995.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fi.asd995.cn

[D11] 反转数组
来源：http://du.yuntaijiaju.cn

Py:   arr[::-1];  arr.reverse()
来源：http://cq.shxzskj.cn

PHP:  array_reverse($arr);
来源：http://bs.shtwfgs.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nz.shtwfgs.cn

TS:   [...arr].reverse();
来源：http://cc.wgjwhj.cn

Java: Collections.reverse(list);
来源：http://jh.yuexingan06.cn

Go:   slices.Reverse(arr)
来源：http://kh.gzmigu.cn

Ruby: arr.reverse
来源：http://ek.yuntaijiaju.cn

C#:   list.Reverse();
来源：http://bj.asd995.cn

[D12] 查找元素下标
来源：http://bz.szsharing.cn

Py:   arr.index(x);  x in arr
来源：http://fp.shtwfgs.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qn.gzmigu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mz.shtwfgs.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xw.wgjwhj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://so.szxytkj.cn

Go:   slices.Index(arr, x)
来源：http://al.panjiajie.cn

Ruby: arr.index(x)
来源：http://ka.lnxyls.cn

C#:   list.IndexOf(x);
来源：http://mc.nicolike.cn

[D13] 过滤（保留满足条件的）
来源：http://df.yuntaijiaju.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nt.panjiajie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xw.shxzukj.cn

JS:   arr.filter(x => x > 3)
来源：http://sw.colortex.cn

TS:   arr.filter(x => x > 3)
来源：http://fw.wgjwhj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://el.nszjky.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hv.jctech888.com.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hz.yuntaijiaju.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ad.huixinmuqiang.cn

[D14] 映射转换（每个元素变形）
来源：http://ah.hahajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pg.szsharing.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pm.shxzskj.cn

JS:   arr.map(x => x * 2)
来源：http://zm.nszjky.cn

TS:   arr.map(x => x * 2)
来源：http://td.hnjuh.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://zq.haigaiapp.cn

Go:   // 手写循环
来源：http://vp.lnxyls.cn

Ruby: arr.map { |x| x * 2 }
来源：http://nj.haigaiapp.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://jr.bjjhwx.cn

[D15] 去重
来源：http://wj.shtwfgs.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://aq.panjiajie.cn

PHP:  array_unique($arr);
来源：http://dj.newstarts.cn

JS:   [...new Set(arr)]
来源：http://yp.bjjhwx.cn

TS:   [...new Set(arr)]
来源：http://sm.lnxyls.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://iu.yuntaijiaju.cn

Go:   // 用 map[T]struct{} 手写
来源：http://kh.hnjuh.cn

Ruby: arr.uniq
来源：http://gn.hnjuh.cn

C#:   list.Distinct().ToList()
来源：http://uu.bookmarksfly.cn

[D16] 求和与平均值
来源：http://qr.huixinmuqiang.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bb.lnxyls.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vt.muxihuayi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nk.shxzskj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pq.521024.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://md.shxzukj.cn

Go:   // 手写循环累加
来源：http://ao.gzmigu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://od.huanxung.cn

C#:   list.Sum();  list.Average()
来源：http://oh.nicolike.cn

[D17] 最大值与最小值
来源：http://hm.9csxet.cn

Py:   max(arr);  min(arr)
来源：http://vt.nicolike.cn

PHP:  max($arr);  min($arr);
来源：http://xy.haigaiapp.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gj.newstarts.cn

TS:   Math.max(...arr);
来源：http://dx.gzmigu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://fj.panjiajie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qw.hnjuh.cn

Ruby: arr.max;  arr.min
来源：http://iv.bookmarksfly.cn

C#:   list.Max();  list.Min()
来源：http://ln.chemitech.net.cn

[D18] 扁平化嵌套数组
来源：http://le.hnjuh.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vq.hahajie.cn

PHP:  array_merge(...$nested);
来源：http://yl.nszjky.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ho.panjiajie.cn

TS:   nested.flat();
来源：http://ma.hnjuh.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kc.colortex.cn

Go:   // 手写双层循环
来源：http://nq.jctech888.com.cn

Ruby: nested.flatten
来源：http://nt.huanxung.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ge.shxzukj.cn

[D19] 按字段分组
来源：http://hh.shxzskj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yq.huixinmuqiang.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zl.szsharing.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lw.nszjky.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xy.muxihuayi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pf.shtwfgs.cn

Go:   // 手写 map[string][]T
来源：http://yd.9csxet.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rz.panjiajie.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://za.yuntaijiaju.cn

[D20] 统计每个元素出现次数
来源：http://mm.szxytkj.cn

Py:   Counter(arr)
来源：http://fj.muxihuayi.cn

PHP:  array_count_values($arr);
来源：http://ov.huixiangedu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pi.hnjuh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://up.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hy.asd995.cn

Go:   // 手写 map[T]int
来源：http://eb.chemitech.net.cn

Ruby: arr.tally
来源：http://oo.asd995.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ex.haigaiapp.cn

[D21] 判断是否包含某元素
来源：http://of.colortex.cn

Py:   x in arr
来源：http://os.shxzukj.cn

PHP:  in_array($x, $arr, true);
来源：http://cs.gzmigu.cn

JS:   arr.includes(x)
来源：http://in.szxytkj.cn

TS:   arr.includes(x)
来源：http://sy.shxzskj.cn

Java: list.contains(x)
来源：http://ic.bookmarksfly.cn

Go:   slices.Contains(arr, x)
来源：http://ku.shxzukj.cn

Ruby: arr.include?(x)
来源：http://kp.bookmarksfly.cn

C#:   list.Contains(x)
来源：http://pl.huixiangedu.cn

[D22] 复制数组（避免共享引用）
来源：http://ce.nicolike.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://es.asd995.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gv.nszjky.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://en.shxzskj.cn

TS:   [...arr];
来源：http://zq.wgjwhj.cn

Java: new ArrayList<>(list);
来源：http://zr.bjjhwx.cn

Go:   copied := append([]int(nil), arr...)
来源：http://rn.huixinmuqiang.cn

Ruby: arr.dup;  arr.clone
来源：http://px.gzmigu.cn

C#:   new List<int>(list);
来源：http://ys.szxytkj.cn

[D23] reduce 累积计算
来源：http://go.gzmigu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sk.bookmarksfly.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://on.hnjuh.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://de.gzmigu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qf.hnjuh.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qq.shxzukj.cn

Go:   // 手写循环
来源：http://wh.jianghongdianzi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kr.jctech888.com.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qx.shtwfgs.cn

[D24] 字典 / Map 基本操作
来源：http://gb.yuexingan06.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://sa.huanxung.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sh.muxihuayi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xp.521024.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ik.gzmigu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xm.shxzukj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kf.colortex.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pq.yuexingan06.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ft.colortex.cn

[D25] Set 集合去重与交并差
来源：http://yu.asd995.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vk.haigaiapp.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ys.9csxet.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vg.wgjwhj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cu.yuexingan06.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://eq.szsharing.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qn.lnxyls.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yd.521024.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://em.huanxung.cn

[D26] 数组转字符串
来源：http://yg.yuexingan06.cn

Py:   ", ".join(map(str, arr))
来源：http://gj.shxzskj.cn

PHP:  implode(", ", $arr);
来源：http://xl.9csxet.cn

JS:   arr.join(", ")
来源：http://de.szxytkj.cn

TS:   arr.join(", ")
来源：http://ai.wgjwhj.cn

Java: String.join(", ", list)
来源：http://zu.shxzskj.cn

Go:   strings.Join(strs, ", ")
来源：http://ae.szsharing.cn

Ruby: arr.join(", ")
来源：http://nf.panjiajie.cn

C#:   string.Join(", ", list)
来源：http://ou.huixiangedu.cn

================================================================================
来源：http://oo.haigaiapp.cn

E. 字符串处理
来源：http://ca.521024.cn

================================================================================
来源：http://wm.huixiangedu.cn

[E01] 拼接字符串
来源：http://gq.nicolike.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ix.huixinmuqiang.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tx.gzmigu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ea.wgjwhj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jr.szsharing.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ks.szsharing.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fx.newstarts.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dn.nszjky.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qn.jctech888.com.cn

[E02] 重复字符串
来源：http://yb.jctech888.com.cn

Py:   "ab" * 3
来源：http://ut.muxihuayi.cn

PHP:  str_repeat("ab", 3);
来源：http://gr.jianghongdianzi.cn

JS:   "ab".repeat(3)
来源：http://dc.szxytkj.cn

TS:   "ab".repeat(3)
来源：http://nl.haigaiapp.cn

Java: "ab".repeat(3)
来源：http://di.bjjhwx.cn

Go:   strings.Repeat("ab", 3)
来源：http://uo.newstarts.cn

Ruby: "ab" * 3
来源：http://yp.hahajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kj.bjjhwx.cn

[E03] 截取子串
来源：http://vm.asd995.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cf.szsharing.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bo.muxihuayi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ho.gzmigu.cn

TS:   s.slice(1, 4)
来源：http://rv.wgjwhj.cn

Java: s.substring(1, 4)
来源：http://zt.chemitech.net.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hu.lnxyls.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zx.szsharing.cn

C#:   s.Substring(1, 3)
来源：http://ft.newstarts.cn

[E04] 查找子串位置
来源：http://jw.szsharing.cn

Py:   s.find("x");  s.index("x")
来源：http://bq.shxzukj.cn

PHP:  strpos($s, "x");
来源：http://fr.huixiangedu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gv.asd995.cn

TS:   s.indexOf("x")
来源：http://vq.shtwfgs.cn

Java: s.indexOf("x")
来源：http://gh.bjjhwx.cn

Go:   strings.Index(s, "x")
来源：http://bd.hahajie.cn

Ruby: s.index("x")
来源：http://ji.chemitech.net.cn

C#:   s.IndexOf("x")
来源：http://ui.9csxet.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://th.huanxung.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gv.521024.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://se.jianghongdianzi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yz.huixiangedu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://to.yuntaijiaju.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://am.nszjky.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ki.hahajie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tn.gzmigu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ih.bookmarksfly.cn

[E06] 替换子串
来源：http://xo.yuexingan06.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://oc.shxzukj.cn

PHP:  str_replace("a", "b", $s);
来源：http://yq.nicolike.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ee.nszjky.cn

TS:   s.replaceAll("a", "b")
来源：http://ec.huanxung.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gn.haigaiapp.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fw.yuntaijiaju.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cr.chemitech.net.cn

C#:   s.Replace("a", "b")
来源：http://nv.shxzskj.cn

[E07] 按分隔符拆分
来源：http://yi.szsharing.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://by.9csxet.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kr.hahajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://gb.521024.cn

TS:   s.split(",")
来源：http://ze.hnjuh.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ss.colortex.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ra.wgjwhj.cn

Ruby: s.split(",");  s.split
来源：http://jm.wgjwhj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qk.haigaiapp.cn

[E08] 数组按分隔符合并
来源：http://dx.jianghongdianzi.cn

Py:   ",".join(items)
来源：http://ag.szsharing.cn


<!-- 参考信息 -->