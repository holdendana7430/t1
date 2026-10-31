代发 wailian999

[D03] 在指定位置插入元素
来源：http://ns.yuntaijiaju.cn

Py:   arr.insert(0, 0)
来源：http://yv.nszjky.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yc.bjjhwx.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://uh.bjjhwx.cn

TS:   arr.splice(0, 0, 0);
来源：http://vq.shtwfgs.cn

Java: list.add(0, 0);
来源：http://cl.szxytkj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://km.nszjky.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ox.huixiangedu.cn

C#:   list.Insert(0, 0);
来源：http://rl.huanxung.cn

[D04] 删除元素
来源：http://ug.szsharing.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rb.huixiangedu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ab.huixinmuqiang.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sa.bookmarksfly.cn

TS:   arr.splice(0, 1);
来源：http://zv.szsharing.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pm.panjiajie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ad.521024.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gz.shxzukj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://em.nicolike.cn

[D05] 访问与修改元素
来源：http://jj.gzmigu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://th.szxytkj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wi.lnxyls.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.panjiajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://hd.jctech888.com.cn

Java: list.get(0); list.set(0, 9);
来源：http://zz.muxihuayi.cn

Go:   arr[0]; arr[0] = 9
来源：http://xy.bookmarksfly.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ub.panjiajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ol.bjjhwx.cn

[D06] 数组长度
来源：http://hp.jctech888.com.cn

Py:   len(arr)
来源：http://jn.shxzskj.cn

PHP:  count($arr);
来源：http://te.shxzskj.cn

JS:   arr.length
来源：http://ho.nicolike.cn

TS:   arr.length
来源：http://ms.szxytkj.cn

Java: list.size();
来源：http://fc.panjiajie.cn

Go:   len(arr)
来源：http://qg.jctech888.com.cn

Ruby: arr.length; arr.size
来源：http://lr.521024.cn

C#:   list.Count;
来源：http://eo.wgjwhj.cn

[D07] 切片 / 取子数组
来源：http://nh.nicolike.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zd.colortex.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ph.bjjhwx.cn

JS:   arr.slice(1, 4);
来源：http://sg.hahajie.cn

TS:   arr.slice(1, 4);
来源：http://oe.chemitech.net.cn

Java: list.subList(1, 4);
来源：http://jq.asd995.cn

Go:   arr[1:4]
来源：http://iu.shxzukj.cn

Ruby: arr[1, 3]
来源：http://nl.shtwfgs.cn

C#:   list.GetRange(1, 3);
来源：http://wt.gzmigu.cn

[D08] 合并两个数组
来源：http://wu.asd995.cn

Py:   a + b;  a.extend(b)
来源：http://qy.hnjuh.cn

PHP:  array_merge($a, $b);
来源：http://km.shxzukj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://cq.shtwfgs.cn

TS:   [...a, ...b];
来源：http://mz.huixiangedu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gp.newstarts.cn

Go:   append(a, b...)
来源：http://fc.huanxung.cn

Ruby: a + b;  a.concat(b)
来源：http://nf.521024.cn

C#:   a.Concat(b).ToList()
来源：http://hm.521024.cn

[D09] 排序（升序）
来源：http://zk.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://wl.colortex.cn

PHP:  sort($arr);
来源：http://dk.newstarts.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gn.muxihuayi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tb.nicolike.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://uz.panjiajie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tg.nszjky.cn

Ruby: arr.sort
来源：http://tu.nszjky.cn

C#:   list.Sort();
来源：http://fa.bookmarksfly.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://dm.shxzskj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mv.bjjhwx.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ne.gzmigu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wa.hahajie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://le.521024.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dq.jctech888.com.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://iz.panjiajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fk.bjjhwx.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://si.haigaiapp.cn

[D11] 反转数组
来源：http://ac.chemitech.net.cn

Py:   arr[::-1];  arr.reverse()
来源：http://lp.9csxet.cn

PHP:  array_reverse($arr);
来源：http://kr.hnjuh.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lz.colortex.cn

TS:   [...arr].reverse();
来源：http://sq.bjjhwx.cn

Java: Collections.reverse(list);
来源：http://sn.newstarts.cn

Go:   slices.Reverse(arr)
来源：http://yp.yuexingan06.cn

Ruby: arr.reverse
来源：http://nx.nszjky.cn

C#:   list.Reverse();
来源：http://qv.szxytkj.cn

[D12] 查找元素下标
来源：http://kk.hnjuh.cn

Py:   arr.index(x);  x in arr
来源：http://uj.jianghongdianzi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xm.yuexingan06.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hc.hahajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qm.hahajie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ji.9csxet.cn

Go:   slices.Index(arr, x)
来源：http://uk.shtwfgs.cn

Ruby: arr.index(x)
来源：http://ws.newstarts.cn

C#:   list.IndexOf(x);
来源：http://ls.szsharing.cn

[D13] 过滤（保留满足条件的）
来源：http://fn.chemitech.net.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://re.panjiajie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dt.szxytkj.cn

JS:   arr.filter(x => x > 3)
来源：http://tt.haigaiapp.cn

TS:   arr.filter(x => x > 3)
来源：http://jw.panjiajie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jp.yuntaijiaju.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lc.bjjhwx.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ab.haigaiapp.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://yi.hnjuh.cn

[D14] 映射转换（每个元素变形）
来源：http://nv.9csxet.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hi.shxzukj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://up.asd995.cn

JS:   arr.map(x => x * 2)
来源：http://br.bookmarksfly.cn

TS:   arr.map(x => x * 2)
来源：http://xv.gzmigu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://hh.asd995.cn

Go:   // 手写循环
来源：http://tk.shxzukj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://mx.panjiajie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://te.jctech888.com.cn

[D15] 去重
来源：http://aa.colortex.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mj.nicolike.cn

PHP:  array_unique($arr);
来源：http://pk.haigaiapp.cn

JS:   [...new Set(arr)]
来源：http://qi.bookmarksfly.cn

TS:   [...new Set(arr)]
来源：http://rv.asd995.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qh.nicolike.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ce.nicolike.cn

Ruby: arr.uniq
来源：http://nw.szsharing.cn

C#:   list.Distinct().ToList()
来源：http://zm.shxzskj.cn

[D16] 求和与平均值
来源：http://ov.lnxyls.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tn.muxihuayi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://co.muxihuayi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xl.wgjwhj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://eq.hahajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lf.panjiajie.cn

Go:   // 手写循环累加
来源：http://bt.hahajie.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qj.szxytkj.cn

C#:   list.Sum();  list.Average()
来源：http://zl.panjiajie.cn

[D17] 最大值与最小值
来源：http://de.szsharing.cn

Py:   max(arr);  min(arr)
来源：http://gf.nszjky.cn

PHP:  max($arr);  min($arr);
来源：http://pr.gzmigu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dq.colortex.cn

TS:   Math.max(...arr);
来源：http://pr.yuexingan06.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://vb.szsharing.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://iq.yuntaijiaju.cn

Ruby: arr.max;  arr.min
来源：http://bg.hnjuh.cn

C#:   list.Max();  list.Min()
来源：http://hf.bjjhwx.cn

[D18] 扁平化嵌套数组
来源：http://go.jctech888.com.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tp.muxihuayi.cn

PHP:  array_merge(...$nested);
来源：http://bb.nicolike.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ie.huixiangedu.cn

TS:   nested.flat();
来源：http://de.hahajie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mu.huanxung.cn

Go:   // 手写双层循环
来源：http://lm.shxzskj.cn

Ruby: nested.flatten
来源：http://yf.jctech888.com.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://rd.szxytkj.cn

[D19] 按字段分组
来源：http://vg.shxzskj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gy.9csxet.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bd.szxytkj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://sz.jctech888.com.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://cv.szxytkj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fg.bjjhwx.cn

Go:   // 手写 map[string][]T
来源：http://xu.szxytkj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://xu.gzmigu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xp.gzmigu.cn

[D20] 统计每个元素出现次数
来源：http://gi.haigaiapp.cn

Py:   Counter(arr)
来源：http://ni.gzmigu.cn

PHP:  array_count_values($arr);
来源：http://to.asd995.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://an.nszjky.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mn.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vu.yuntaijiaju.cn

Go:   // 手写 map[T]int
来源：http://uo.muxihuayi.cn

Ruby: arr.tally
来源：http://mq.yuntaijiaju.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lg.jctech888.com.cn

[D21] 判断是否包含某元素
来源：http://wy.colortex.cn

Py:   x in arr
来源：http://km.huixiangedu.cn

PHP:  in_array($x, $arr, true);
来源：http://jb.muxihuayi.cn

JS:   arr.includes(x)
来源：http://el.huixiangedu.cn

TS:   arr.includes(x)
来源：http://nd.huanxung.cn

Java: list.contains(x)
来源：http://ur.nszjky.cn

Go:   slices.Contains(arr, x)
来源：http://ui.gzmigu.cn

Ruby: arr.include?(x)
来源：http://bc.szsharing.cn

C#:   list.Contains(x)
来源：http://oe.bjjhwx.cn

[D22] 复制数组（避免共享引用）
来源：http://gq.hnjuh.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bs.yuntaijiaju.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://us.hnjuh.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ty.huixinmuqiang.cn

TS:   [...arr];
来源：http://nf.hahajie.cn

Java: new ArrayList<>(list);
来源：http://ar.haigaiapp.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qw.jctech888.com.cn

Ruby: arr.dup;  arr.clone
来源：http://pg.yuntaijiaju.cn

C#:   new List<int>(list);
来源：http://pa.hnjuh.cn

[D23] reduce 累积计算
来源：http://yo.bookmarksfly.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rh.szsharing.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ef.shxzukj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jd.colortex.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hh.521024.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://hn.colortex.cn

Go:   // 手写循环
来源：http://jw.nicolike.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lv.asd995.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wv.shxzukj.cn

[D24] 字典 / Map 基本操作
来源：http://gk.szxytkj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://co.szsharing.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fu.szxytkj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tr.bookmarksfly.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mr.jianghongdianzi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gk.shxzskj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zs.jianghongdianzi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mt.9csxet.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://is.nszjky.cn

[D25] Set 集合去重与交并差
来源：http://ad.lnxyls.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qg.shtwfgs.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hl.jctech888.com.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://us.bookmarksfly.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rt.szsharing.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://le.hahajie.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cw.hahajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://us.huanxung.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ol.huixinmuqiang.cn

[D26] 数组转字符串
来源：http://ky.huixinmuqiang.cn

Py:   ", ".join(map(str, arr))
来源：http://gr.huixiangedu.cn

PHP:  implode(", ", $arr);
来源：http://ke.yuexingan06.cn

JS:   arr.join(", ")
来源：http://nz.colortex.cn

TS:   arr.join(", ")
来源：http://dn.shtwfgs.cn

Java: String.join(", ", list)
来源：http://fm.jctech888.com.cn

Go:   strings.Join(strs, ", ")
来源：http://ej.shxzskj.cn

Ruby: arr.join(", ")
来源：http://mm.panjiajie.cn

C#:   string.Join(", ", list)
来源：http://qv.nszjky.cn

================================================================================
来源：http://ix.szxytkj.cn

E. 字符串处理
来源：http://eg.bjjhwx.cn

================================================================================
来源：http://ma.szxytkj.cn

[E01] 拼接字符串
来源：http://it.shtwfgs.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://er.lnxyls.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dq.shtwfgs.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nj.asd995.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fh.nicolike.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dt.yuexingan06.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hx.haigaiapp.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ld.huixinmuqiang.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kt.jctech888.com.cn

[E02] 重复字符串
来源：http://fw.newstarts.cn

Py:   "ab" * 3
来源：http://or.lnxyls.cn

PHP:  str_repeat("ab", 3);
来源：http://tt.huixiangedu.cn

JS:   "ab".repeat(3)
来源：http://ru.huanxung.cn

TS:   "ab".repeat(3)
来源：http://nt.newstarts.cn

Java: "ab".repeat(3)
来源：http://lf.521024.cn

Go:   strings.Repeat("ab", 3)
来源：http://vs.newstarts.cn

Ruby: "ab" * 3
来源：http://er.hahajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sb.newstarts.cn

[E03] 截取子串
来源：http://nj.shtwfgs.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://he.yuexingan06.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zu.chemitech.net.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gv.szxytkj.cn

TS:   s.slice(1, 4)
来源：http://hu.szsharing.cn

Java: s.substring(1, 4)
来源：http://el.9csxet.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://aw.shtwfgs.cn

Ruby: s[1, 3];  s[1..3]
来源：http://lj.gzmigu.cn

C#:   s.Substring(1, 3)
来源：http://yj.bookmarksfly.cn

[E04] 查找子串位置
来源：http://ey.panjiajie.cn

Py:   s.find("x");  s.index("x")
来源：http://ei.jctech888.com.cn

PHP:  strpos($s, "x");
来源：http://oe.huixinmuqiang.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://at.asd995.cn

TS:   s.indexOf("x")
来源：http://lz.hahajie.cn

Java: s.indexOf("x")
来源：http://dr.bjjhwx.cn

Go:   strings.Index(s, "x")
来源：http://vr.colortex.cn

Ruby: s.index("x")
来源：http://bt.hnjuh.cn

C#:   s.IndexOf("x")
来源：http://eu.huixiangedu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://dr.hahajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://he.jctech888.com.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qz.lnxyls.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ms.shxzskj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://jp.huanxung.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uj.gzmigu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://if.muxihuayi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fl.shxzukj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nu.bjjhwx.cn

[E06] 替换子串
来源：http://dg.haigaiapp.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bg.asd995.cn

PHP:  str_replace("a", "b", $s);
来源：http://wc.shxzskj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fb.lnxyls.cn

TS:   s.replaceAll("a", "b")
来源：http://nf.hahajie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vu.wgjwhj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://me.asd995.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vy.nszjky.cn

C#:   s.Replace("a", "b")
来源：http://fb.yuntaijiaju.cn

[E07] 按分隔符拆分
来源：http://rk.wgjwhj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zl.shxzskj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jj.wgjwhj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ia.9csxet.cn

TS:   s.split(",")
来源：http://fr.9csxet.cn

Java: s.split(",");  s.split("\\s+")
来源：http://gj.panjiajie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://oy.shxzukj.cn

Ruby: s.split(",");  s.split
来源：http://au.huixinmuqiang.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ix.yuntaijiaju.cn

[E08] 数组按分隔符合并
来源：http://jj.huixiangedu.cn

Py:   ",".join(items)
来源：http://xm.chemitech.net.cn

PHP:  implode(",", $items);
来源：http://bw.jianghongdianzi.cn

JS:   items.join(",")
来源：http://gv.colortex.cn

TS:   items.join(",")
来源：http://hx.hahajie.cn

Java: String.join(",", items)
来源：http://ng.521024.cn

Go:   strings.Join(items, ",")
来源：http://oh.shxzskj.cn

Ruby: items.join(",")
来源：http://qf.nszjky.cn

C#:   string.Join(",", items)
来源：http://qb.huixiangedu.cn

[E09] 去除所有空白字符
来源：http://wd.nicolike.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lw.huixinmuqiang.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ah.521024.cn

JS:   s.replace(/\s+/g, "")
来源：http://dj.huixinmuqiang.cn

TS:   s.replace(/\s+/g, "")
来源：http://iv.521024.cn

Java: s.replaceAll("\\s+", "")
来源：http://ig.521024.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://aa.jctech888.com.cn

Ruby: s.gsub(/\s+/, "")
来源：http://tj.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://au.nszjky.cn


<!-- 参考信息 -->