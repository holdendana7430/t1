代发 wailian999

[D03] 在指定位置插入元素
来源：http://td.bjjhwx.cn

Py:   arr.insert(0, 0)
来源：http://yt.jctech888.com.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kq.asd995.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://di.9csxet.cn

TS:   arr.splice(0, 0, 0);
来源：http://ui.hnjuh.cn

Java: list.add(0, 0);
来源：http://gz.bjjhwx.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ji.9csxet.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dg.shtwfgs.cn

C#:   list.Insert(0, 0);
来源：http://kr.szsharing.cn

[D04] 删除元素
来源：http://ng.shxzukj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jj.panjiajie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zg.jianghongdianzi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kn.chemitech.net.cn

TS:   arr.splice(0, 1);
来源：http://tl.hnjuh.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jx.521024.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hj.hahajie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dm.asd995.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://st.9csxet.cn

[D05] 访问与修改元素
来源：http://db.chemitech.net.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wr.nszjky.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cv.wgjwhj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ny.hnjuh.cn

TS:   arr[0]; arr.at(-1);
来源：http://pt.asd995.cn

Java: list.get(0); list.set(0, 9);
来源：http://ov.shxzskj.cn

Go:   arr[0]; arr[0] = 9
来源：http://ti.521024.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gr.huixiangedu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ko.newstarts.cn

[D06] 数组长度
来源：http://ny.jctech888.com.cn

Py:   len(arr)
来源：http://kh.colortex.cn

PHP:  count($arr);
来源：http://yh.muxihuayi.cn

JS:   arr.length
来源：http://so.haigaiapp.cn

TS:   arr.length
来源：http://gk.9csxet.cn

Java: list.size();
来源：http://cx.shtwfgs.cn

Go:   len(arr)
来源：http://yp.lnxyls.cn

Ruby: arr.length; arr.size
来源：http://ws.huanxung.cn

C#:   list.Count;
来源：http://gy.hnjuh.cn

[D07] 切片 / 取子数组
来源：http://vd.haigaiapp.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qd.hnjuh.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ns.asd995.cn

JS:   arr.slice(1, 4);
来源：http://rg.nicolike.cn

TS:   arr.slice(1, 4);
来源：http://tc.hnjuh.cn

Java: list.subList(1, 4);
来源：http://bj.muxihuayi.cn

Go:   arr[1:4]
来源：http://bu.panjiajie.cn

Ruby: arr[1, 3]
来源：http://rb.wgjwhj.cn

C#:   list.GetRange(1, 3);
来源：http://pd.nicolike.cn

[D08] 合并两个数组
来源：http://kp.huixinmuqiang.cn

Py:   a + b;  a.extend(b)
来源：http://fd.asd995.cn

PHP:  array_merge($a, $b);
来源：http://gw.nszjky.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://fw.szsharing.cn

TS:   [...a, ...b];
来源：http://ns.521024.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sd.jctech888.com.cn

Go:   append(a, b...)
来源：http://rw.jctech888.com.cn

Ruby: a + b;  a.concat(b)
来源：http://re.nicolike.cn

C#:   a.Concat(b).ToList()
来源：http://td.newstarts.cn

[D09] 排序（升序）
来源：http://dd.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://oq.huixiangedu.cn

PHP:  sort($arr);
来源：http://ga.colortex.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ri.bjjhwx.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://pe.jianghongdianzi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://pz.gzmigu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zz.lnxyls.cn

Ruby: arr.sort
来源：http://zx.chemitech.net.cn

C#:   list.Sort();
来源：http://ks.huixinmuqiang.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://pq.haigaiapp.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xj.shxzskj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qe.shtwfgs.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://by.gzmigu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xy.huanxung.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://df.nszjky.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tb.huixinmuqiang.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://iw.szsharing.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nf.asd995.cn

[D11] 反转数组
来源：http://ly.newstarts.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xc.bjjhwx.cn

PHP:  array_reverse($arr);
来源：http://cl.nicolike.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://li.huixinmuqiang.cn

TS:   [...arr].reverse();
来源：http://cd.huixiangedu.cn

Java: Collections.reverse(list);
来源：http://ks.9csxet.cn

Go:   slices.Reverse(arr)
来源：http://ju.huanxung.cn

Ruby: arr.reverse
来源：http://la.jctech888.com.cn

C#:   list.Reverse();
来源：http://ai.szsharing.cn

[D12] 查找元素下标
来源：http://tq.huanxung.cn

Py:   arr.index(x);  x in arr
来源：http://va.haigaiapp.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://da.jctech888.com.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tn.hnjuh.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ay.huixinmuqiang.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://of.yuntaijiaju.cn

Go:   slices.Index(arr, x)
来源：http://xc.nszjky.cn

Ruby: arr.index(x)
来源：http://cl.panjiajie.cn

C#:   list.IndexOf(x);
来源：http://qz.szsharing.cn

[D13] 过滤（保留满足条件的）
来源：http://yw.szxytkj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nc.colortex.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mv.9csxet.cn

JS:   arr.filter(x => x > 3)
来源：http://ut.yuntaijiaju.cn

TS:   arr.filter(x => x > 3)
来源：http://uv.shtwfgs.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rf.panjiajie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://el.panjiajie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://nj.shxzskj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ru.jctech888.com.cn

[D14] 映射转换（每个元素变形）
来源：http://nz.yuexingan06.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ud.shxzskj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xf.hahajie.cn

JS:   arr.map(x => x * 2)
来源：http://kz.newstarts.cn

TS:   arr.map(x => x * 2)
来源：http://tl.lnxyls.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ts.nszjky.cn

Go:   // 手写循环
来源：http://tg.huixinmuqiang.cn

Ruby: arr.map { |x| x * 2 }
来源：http://tq.yuexingan06.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://wm.9csxet.cn

[D15] 去重
来源：http://dv.szsharing.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ep.wgjwhj.cn

PHP:  array_unique($arr);
来源：http://en.bjjhwx.cn

JS:   [...new Set(arr)]
来源：http://wa.bookmarksfly.cn

TS:   [...new Set(arr)]
来源：http://zt.shxzskj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hb.szsharing.cn

Go:   // 用 map[T]struct{} 手写
来源：http://qi.panjiajie.cn

Ruby: arr.uniq
来源：http://cz.chemitech.net.cn

C#:   list.Distinct().ToList()
来源：http://qf.shtwfgs.cn

[D16] 求和与平均值
来源：http://sj.nicolike.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fd.gzmigu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://df.hnjuh.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ik.muxihuayi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xj.hahajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nh.bookmarksfly.cn

Go:   // 手写循环累加
来源：http://db.chemitech.net.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://up.asd995.cn

C#:   list.Sum();  list.Average()
来源：http://ts.lnxyls.cn

[D17] 最大值与最小值
来源：http://gj.huanxung.cn

Py:   max(arr);  min(arr)
来源：http://lk.colortex.cn

PHP:  max($arr);  min($arr);
来源：http://ek.haigaiapp.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mw.hnjuh.cn

TS:   Math.max(...arr);
来源：http://ao.shtwfgs.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ak.9csxet.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ed.bookmarksfly.cn

Ruby: arr.max;  arr.min
来源：http://rw.szxytkj.cn

C#:   list.Max();  list.Min()
来源：http://ya.hnjuh.cn

[D18] 扁平化嵌套数组
来源：http://hq.huixinmuqiang.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zx.asd995.cn

PHP:  array_merge(...$nested);
来源：http://oy.gzmigu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nq.bookmarksfly.cn

TS:   nested.flat();
来源：http://po.hahajie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fr.szxytkj.cn

Go:   // 手写双层循环
来源：http://dg.szxytkj.cn

Ruby: nested.flatten
来源：http://cc.huanxung.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://mz.huanxung.cn

[D19] 按字段分组
来源：http://ui.shxzukj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ng.chemitech.net.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hb.nszjky.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qy.nszjky.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://fg.yuntaijiaju.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qx.hnjuh.cn

Go:   // 手写 map[string][]T
来源：http://bp.shxzskj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://kt.huixiangedu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ta.haigaiapp.cn

[D20] 统计每个元素出现次数
来源：http://fy.huixiangedu.cn

Py:   Counter(arr)
来源：http://cl.szxytkj.cn

PHP:  array_count_values($arr);
来源：http://dv.lnxyls.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://et.521024.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oi.huixinmuqiang.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://np.hnjuh.cn

Go:   // 手写 map[T]int
来源：http://ah.shtwfgs.cn

Ruby: arr.tally
来源：http://te.bjjhwx.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ns.shxzskj.cn

[D21] 判断是否包含某元素
来源：http://wv.newstarts.cn

Py:   x in arr
来源：http://np.bookmarksfly.cn

PHP:  in_array($x, $arr, true);
来源：http://jb.colortex.cn

JS:   arr.includes(x)
来源：http://su.chemitech.net.cn

TS:   arr.includes(x)
来源：http://ll.hnjuh.cn

Java: list.contains(x)
来源：http://ag.521024.cn

Go:   slices.Contains(arr, x)
来源：http://or.hnjuh.cn

Ruby: arr.include?(x)
来源：http://el.wgjwhj.cn

C#:   list.Contains(x)
来源：http://us.shtwfgs.cn

[D22] 复制数组（避免共享引用）
来源：http://zc.szsharing.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xp.jctech888.com.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cp.hahajie.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cx.muxihuayi.cn

TS:   [...arr];
来源：http://ai.huixiangedu.cn

Java: new ArrayList<>(list);
来源：http://lh.521024.cn

Go:   copied := append([]int(nil), arr...)
来源：http://he.shtwfgs.cn

Ruby: arr.dup;  arr.clone
来源：http://ld.huixiangedu.cn

C#:   new List<int>(list);
来源：http://rp.chemitech.net.cn

[D23] reduce 累积计算
来源：http://iv.jianghongdianzi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jv.bookmarksfly.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wz.lnxyls.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ve.hnjuh.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lx.szxytkj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qb.newstarts.cn

Go:   // 手写循环
来源：http://xf.haigaiapp.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fd.shxzukj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://se.chemitech.net.cn

[D24] 字典 / Map 基本操作
来源：http://bd.panjiajie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://he.newstarts.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://os.nszjky.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zv.nszjky.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xq.huanxung.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://sc.bookmarksfly.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://km.chemitech.net.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ev.colortex.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://en.huixinmuqiang.cn

[D25] Set 集合去重与交并差
来源：http://yc.szsharing.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ng.bjjhwx.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tx.nszjky.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://px.yuntaijiaju.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qa.huanxung.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dm.jctech888.com.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zx.nicolike.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wh.szxytkj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mu.gzmigu.cn

[D26] 数组转字符串
来源：http://ee.521024.cn

Py:   ", ".join(map(str, arr))
来源：http://vx.lnxyls.cn

PHP:  implode(", ", $arr);
来源：http://ws.hnjuh.cn

JS:   arr.join(", ")
来源：http://et.szxytkj.cn

TS:   arr.join(", ")
来源：http://zq.colortex.cn

Java: String.join(", ", list)
来源：http://xv.panjiajie.cn

Go:   strings.Join(strs, ", ")
来源：http://yr.huixinmuqiang.cn

Ruby: arr.join(", ")
来源：http://qg.huixiangedu.cn

C#:   string.Join(", ", list)
来源：http://jx.chemitech.net.cn

================================================================================
来源：http://pc.huanxung.cn

E. 字符串处理
来源：http://ku.newstarts.cn

================================================================================
来源：http://sh.shxzukj.cn

[E01] 拼接字符串
来源：http://hz.huixiangedu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ou.gzmigu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hr.haigaiapp.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tw.jctech888.com.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qu.nicolike.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tl.nszjky.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://so.bjjhwx.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dd.chemitech.net.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pq.colortex.cn

[E02] 重复字符串
来源：http://fe.yuexingan06.cn

Py:   "ab" * 3
来源：http://sg.szxytkj.cn

PHP:  str_repeat("ab", 3);
来源：http://la.huixinmuqiang.cn

JS:   "ab".repeat(3)
来源：http://vx.huixinmuqiang.cn

TS:   "ab".repeat(3)
来源：http://ji.yuntaijiaju.cn

Java: "ab".repeat(3)
来源：http://ml.szxytkj.cn

Go:   strings.Repeat("ab", 3)
来源：http://oc.szsharing.cn

Ruby: "ab" * 3
来源：http://mw.asd995.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jb.yuexingan06.cn

[E03] 截取子串
来源：http://sw.asd995.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mr.lnxyls.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cs.chemitech.net.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jx.gzmigu.cn

TS:   s.slice(1, 4)
来源：http://js.bookmarksfly.cn

Java: s.substring(1, 4)
来源：http://sh.colortex.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://my.muxihuayi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://pu.szxytkj.cn

C#:   s.Substring(1, 3)
来源：http://kq.yuexingan06.cn

[E04] 查找子串位置
来源：http://en.hahajie.cn

Py:   s.find("x");  s.index("x")
来源：http://pf.colortex.cn

PHP:  strpos($s, "x");
来源：http://ai.newstarts.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vv.huixiangedu.cn

TS:   s.indexOf("x")
来源：http://gv.hahajie.cn

Java: s.indexOf("x")
来源：http://qk.521024.cn

Go:   strings.Index(s, "x")
来源：http://vh.shxzskj.cn

Ruby: s.index("x")
来源：http://gk.yuexingan06.cn

C#:   s.IndexOf("x")
来源：http://ss.huixinmuqiang.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://my.shxzukj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kb.panjiajie.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tp.jianghongdianzi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xy.shtwfgs.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://fs.szsharing.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ib.newstarts.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ss.shxzskj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nw.bookmarksfly.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ku.jctech888.com.cn

[E06] 替换子串
来源：http://qu.jctech888.com.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sw.chemitech.net.cn

PHP:  str_replace("a", "b", $s);
来源：http://uj.hnjuh.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ne.huanxung.cn

TS:   s.replaceAll("a", "b")
来源：http://mh.9csxet.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ap.hnjuh.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://md.newstarts.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rg.shxzskj.cn

C#:   s.Replace("a", "b")
来源：http://ds.9csxet.cn

[E07] 按分隔符拆分
来源：http://hn.huixiangedu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sm.wgjwhj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nw.shtwfgs.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://gf.9csxet.cn

TS:   s.split(",")
来源：http://kt.nszjky.cn

Java: s.split(",");  s.split("\\s+")
来源：http://pp.asd995.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qf.yuntaijiaju.cn

Ruby: s.split(",");  s.split
来源：http://ih.bjjhwx.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ob.hahajie.cn

[E08] 数组按分隔符合并
来源：http://jt.colortex.cn

Py:   ",".join(items)
来源：http://rh.yuexingan06.cn

PHP:  implode(",", $items);
来源：http://xm.szxytkj.cn

JS:   items.join(",")
来源：http://ee.asd995.cn

TS:   items.join(",")
来源：http://xa.521024.cn

Java: String.join(",", items)
来源：http://hp.nszjky.cn

Go:   strings.Join(items, ",")
来源：http://kz.jianghongdianzi.cn

Ruby: items.join(",")
来源：http://vj.bookmarksfly.cn

C#:   string.Join(",", items)
来源：http://lr.colortex.cn

[E09] 去除所有空白字符
来源：http://la.hahajie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mt.jctech888.com.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://op.bookmarksfly.cn

JS:   s.replace(/\s+/g, "")
来源：http://vg.yuntaijiaju.cn

TS:   s.replace(/\s+/g, "")
来源：http://zd.huixinmuqiang.cn

Java: s.replaceAll("\\s+", "")
来源：http://pz.jianghongdianzi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qm.szsharing.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qe.nszjky.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://md.bjjhwx.cn


<!-- 参考信息 -->