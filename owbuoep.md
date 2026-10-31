代发 wailian999

C#:   list.Insert(0, 0);
来源：http://qp.wgjwhj.cn

[D04] 删除元素
来源：http://iw.shtwfgs.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yv.nicolike.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ts.colortex.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cd.nicolike.cn

TS:   arr.splice(0, 1);
来源：http://cd.szsharing.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zr.szsharing.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://st.muxihuayi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lm.szsharing.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://to.nszjky.cn

[D05] 访问与修改元素
来源：http://zo.panjiajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rn.huixinmuqiang.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ls.jianghongdianzi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wd.szxytkj.cn

TS:   arr[0]; arr.at(-1);
来源：http://at.bookmarksfly.cn

Java: list.get(0); list.set(0, 9);
来源：http://qv.nszjky.cn

Go:   arr[0]; arr[0] = 9
来源：http://yy.jctech888.com.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ok.gzmigu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ie.bookmarksfly.cn

[D06] 数组长度
来源：http://ic.chemitech.net.cn

Py:   len(arr)
来源：http://pr.hnjuh.cn

PHP:  count($arr);
来源：http://gg.szxytkj.cn

JS:   arr.length
来源：http://rc.huanxung.cn

TS:   arr.length
来源：http://jr.colortex.cn

Java: list.size();
来源：http://mp.shxzukj.cn

Go:   len(arr)
来源：http://zt.yuntaijiaju.cn

Ruby: arr.length; arr.size
来源：http://od.yuexingan06.cn

C#:   list.Count;
来源：http://ex.lnxyls.cn

[D07] 切片 / 取子数组
来源：http://hb.521024.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bv.huanxung.cn

PHP:  array_slice($arr, 1, 3);
来源：http://sz.hahajie.cn

JS:   arr.slice(1, 4);
来源：http://zc.szxytkj.cn

TS:   arr.slice(1, 4);
来源：http://kq.shxzskj.cn

Java: list.subList(1, 4);
来源：http://xl.colortex.cn

Go:   arr[1:4]
来源：http://ul.asd995.cn

Ruby: arr[1, 3]
来源：http://qv.huixinmuqiang.cn

C#:   list.GetRange(1, 3);
来源：http://uj.yuexingan06.cn

[D08] 合并两个数组
来源：http://xu.bjjhwx.cn

Py:   a + b;  a.extend(b)
来源：http://yg.yuntaijiaju.cn

PHP:  array_merge($a, $b);
来源：http://zt.yuntaijiaju.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://qv.chemitech.net.cn

TS:   [...a, ...b];
来源：http://tx.asd995.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://su.yuntaijiaju.cn

Go:   append(a, b...)
来源：http://wx.shtwfgs.cn

Ruby: a + b;  a.concat(b)
来源：http://qv.panjiajie.cn

C#:   a.Concat(b).ToList()
来源：http://ye.huixinmuqiang.cn

[D09] 排序（升序）
来源：http://ow.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://bw.521024.cn

PHP:  sort($arr);
来源：http://gf.panjiajie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yf.huanxung.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ro.chemitech.net.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://gy.huixiangedu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ls.szxytkj.cn

Ruby: arr.sort
来源：http://tv.szxytkj.cn

C#:   list.Sort();
来源：http://op.wgjwhj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://yj.haigaiapp.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wc.shxzukj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aa.szxytkj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lj.yuntaijiaju.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ph.nicolike.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cv.huixiangedu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wz.panjiajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://go.nszjky.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mx.haigaiapp.cn

[D11] 反转数组
来源：http://lm.szsharing.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ex.bjjhwx.cn

PHP:  array_reverse($arr);
来源：http://wb.yuntaijiaju.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xd.hnjuh.cn

TS:   [...arr].reverse();
来源：http://wn.jianghongdianzi.cn

Java: Collections.reverse(list);
来源：http://oc.nicolike.cn

Go:   slices.Reverse(arr)
来源：http://aq.lnxyls.cn

Ruby: arr.reverse
来源：http://av.gzmigu.cn

C#:   list.Reverse();
来源：http://aa.521024.cn

[D12] 查找元素下标
来源：http://vn.gzmigu.cn

Py:   arr.index(x);  x in arr
来源：http://vj.huixiangedu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tj.panjiajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zx.szxytkj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uc.chemitech.net.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://us.jianghongdianzi.cn

Go:   slices.Index(arr, x)
来源：http://zw.asd995.cn

Ruby: arr.index(x)
来源：http://al.newstarts.cn

C#:   list.IndexOf(x);
来源：http://xh.hahajie.cn

[D13] 过滤（保留满足条件的）
来源：http://ue.9csxet.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gh.panjiajie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://el.colortex.cn

JS:   arr.filter(x => x > 3)
来源：http://ro.jctech888.com.cn

TS:   arr.filter(x => x > 3)
来源：http://zo.nszjky.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ug.bookmarksfly.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://sm.newstarts.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xy.szxytkj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qa.bookmarksfly.cn

[D14] 映射转换（每个元素变形）
来源：http://qf.shxzukj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vc.9csxet.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fk.jctech888.com.cn

JS:   arr.map(x => x * 2)
来源：http://zs.hahajie.cn

TS:   arr.map(x => x * 2)
来源：http://nx.bookmarksfly.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://jq.shxzukj.cn

Go:   // 手写循环
来源：http://ho.521024.cn

Ruby: arr.map { |x| x * 2 }
来源：http://dx.hnjuh.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://np.jctech888.com.cn

[D15] 去重
来源：http://of.wgjwhj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ad.nicolike.cn

PHP:  array_unique($arr);
来源：http://fc.yuntaijiaju.cn

JS:   [...new Set(arr)]
来源：http://qi.lnxyls.cn

TS:   [...new Set(arr)]
来源：http://it.bjjhwx.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dr.9csxet.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ac.nicolike.cn

Ruby: arr.uniq
来源：http://ps.colortex.cn

C#:   list.Distinct().ToList()
来源：http://vn.huixiangedu.cn

[D16] 求和与平均值
来源：http://op.huixiangedu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://sg.colortex.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jn.yuexingan06.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fq.9csxet.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pf.9csxet.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zp.9csxet.cn

Go:   // 手写循环累加
来源：http://mh.bookmarksfly.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nm.yuntaijiaju.cn

C#:   list.Sum();  list.Average()
来源：http://kf.hnjuh.cn

[D17] 最大值与最小值
来源：http://tu.huanxung.cn

Py:   max(arr);  min(arr)
来源：http://nk.haigaiapp.cn

PHP:  max($arr);  min($arr);
来源：http://jb.bjjhwx.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fu.jianghongdianzi.cn

TS:   Math.max(...arr);
来源：http://xp.huixinmuqiang.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://pb.shxzukj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fh.haigaiapp.cn

Ruby: arr.max;  arr.min
来源：http://ti.huixinmuqiang.cn

C#:   list.Max();  list.Min()
来源：http://fz.newstarts.cn

[D18] 扁平化嵌套数组
来源：http://tq.huanxung.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kj.jianghongdianzi.cn

PHP:  array_merge(...$nested);
来源：http://rl.wgjwhj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qq.jianghongdianzi.cn

TS:   nested.flat();
来源：http://cl.jianghongdianzi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://os.yuexingan06.cn

Go:   // 手写双层循环
来源：http://cd.nszjky.cn

Ruby: nested.flatten
来源：http://pq.wgjwhj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://wu.bjjhwx.cn

[D19] 按字段分组
来源：http://jk.521024.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://eo.521024.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ma.jianghongdianzi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ah.shtwfgs.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://fr.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yt.jctech888.com.cn

Go:   // 手写 map[string][]T
来源：http://uo.shxzskj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://er.lnxyls.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://eh.colortex.cn

[D20] 统计每个元素出现次数
来源：http://fz.lnxyls.cn

Py:   Counter(arr)
来源：http://yj.shxzukj.cn

PHP:  array_count_values($arr);
来源：http://tu.colortex.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sc.wgjwhj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ui.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gw.yuntaijiaju.cn

Go:   // 手写 map[T]int
来源：http://qg.shxzukj.cn

Ruby: arr.tally
来源：http://tr.gzmigu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://od.colortex.cn

[D21] 判断是否包含某元素
来源：http://xb.gzmigu.cn

Py:   x in arr
来源：http://tg.jianghongdianzi.cn

PHP:  in_array($x, $arr, true);
来源：http://fd.shxzukj.cn

JS:   arr.includes(x)
来源：http://lz.szsharing.cn

TS:   arr.includes(x)
来源：http://ur.bjjhwx.cn

Java: list.contains(x)
来源：http://rl.hnjuh.cn

Go:   slices.Contains(arr, x)
来源：http://qa.521024.cn

Ruby: arr.include?(x)
来源：http://zw.bookmarksfly.cn

C#:   list.Contains(x)
来源：http://iu.muxihuayi.cn

[D22] 复制数组（避免共享引用）
来源：http://ow.huanxung.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ve.newstarts.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://br.jctech888.com.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://px.bookmarksfly.cn

TS:   [...arr];
来源：http://uq.chemitech.net.cn

Java: new ArrayList<>(list);
来源：http://cl.yuexingan06.cn

Go:   copied := append([]int(nil), arr...)
来源：http://oy.asd995.cn

Ruby: arr.dup;  arr.clone
来源：http://st.yuntaijiaju.cn

C#:   new List<int>(list);
来源：http://tz.haigaiapp.cn

[D23] reduce 累积计算
来源：http://vo.chemitech.net.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gz.szsharing.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kh.bookmarksfly.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://he.szxytkj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zp.nszjky.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://yb.bjjhwx.cn

Go:   // 手写循环
来源：http://cb.wgjwhj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vb.huixiangedu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zl.shtwfgs.cn

[D24] 字典 / Map 基本操作
来源：http://vr.muxihuayi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qx.haigaiapp.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ae.haigaiapp.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xx.szsharing.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yt.asd995.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ai.asd995.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ql.hahajie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qk.hnjuh.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://io.newstarts.cn

[D25] Set 集合去重与交并差
来源：http://ju.asd995.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dj.yuntaijiaju.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gx.jianghongdianzi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nn.9csxet.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ly.shtwfgs.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://md.nicolike.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sb.szxytkj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mu.nszjky.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jc.bjjhwx.cn

[D26] 数组转字符串
来源：http://iz.haigaiapp.cn

Py:   ", ".join(map(str, arr))
来源：http://jj.bookmarksfly.cn

PHP:  implode(", ", $arr);
来源：http://ja.haigaiapp.cn

JS:   arr.join(", ")
来源：http://ke.huixinmuqiang.cn

TS:   arr.join(", ")
来源：http://ja.nicolike.cn

Java: String.join(", ", list)
来源：http://zj.chemitech.net.cn

Go:   strings.Join(strs, ", ")
来源：http://wh.bookmarksfly.cn

Ruby: arr.join(", ")
来源：http://qz.wgjwhj.cn

C#:   string.Join(", ", list)
来源：http://uu.lnxyls.cn

================================================================================
来源：http://jj.shxzukj.cn

E. 字符串处理
来源：http://gc.521024.cn

================================================================================
来源：http://vx.hnjuh.cn

[E01] 拼接字符串
来源：http://gb.chemitech.net.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lb.nicolike.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://en.colortex.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ux.huixiangedu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fg.hahajie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sk.wgjwhj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nt.szxytkj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dm.huanxung.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zs.bjjhwx.cn

[E02] 重复字符串
来源：http://ou.bookmarksfly.cn

Py:   "ab" * 3
来源：http://rz.jctech888.com.cn

PHP:  str_repeat("ab", 3);
来源：http://ia.521024.cn

JS:   "ab".repeat(3)
来源：http://la.hahajie.cn

TS:   "ab".repeat(3)
来源：http://nz.yuexingan06.cn

Java: "ab".repeat(3)
来源：http://dw.bjjhwx.cn

Go:   strings.Repeat("ab", 3)
来源：http://ax.shtwfgs.cn

Ruby: "ab" * 3
来源：http://sv.asd995.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tu.nicolike.cn

[E03] 截取子串
来源：http://jf.hnjuh.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xg.huanxung.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ha.shxzskj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://uu.huixinmuqiang.cn

TS:   s.slice(1, 4)
来源：http://jm.asd995.cn

Java: s.substring(1, 4)
来源：http://mb.jianghongdianzi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nj.yuntaijiaju.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ww.jianghongdianzi.cn

C#:   s.Substring(1, 3)
来源：http://bj.szxytkj.cn

[E04] 查找子串位置
来源：http://ab.colortex.cn

Py:   s.find("x");  s.index("x")
来源：http://gn.huixiangedu.cn

PHP:  strpos($s, "x");
来源：http://jj.521024.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wp.muxihuayi.cn

TS:   s.indexOf("x")
来源：http://qc.shxzukj.cn

Java: s.indexOf("x")
来源：http://jh.lnxyls.cn

Go:   strings.Index(s, "x")
来源：http://wr.jctech888.com.cn

Ruby: s.index("x")
来源：http://em.panjiajie.cn

C#:   s.IndexOf("x")
来源：http://nv.521024.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://pw.yuexingan06.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cq.yuexingan06.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kc.jianghongdianzi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xa.shxzukj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://vt.gzmigu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uo.szxytkj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ns.lnxyls.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yq.chemitech.net.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://uq.nicolike.cn

[E06] 替换子串
来源：http://sy.yuntaijiaju.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sc.huanxung.cn

PHP:  str_replace("a", "b", $s);
来源：http://nv.yuntaijiaju.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dk.huanxung.cn

TS:   s.replaceAll("a", "b")
来源：http://vu.nszjky.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ov.lnxyls.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ud.panjiajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bh.haigaiapp.cn

C#:   s.Replace("a", "b")
来源：http://sv.hahajie.cn

[E07] 按分隔符拆分
来源：http://ah.nicolike.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ar.chemitech.net.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pp.chemitech.net.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://dx.bookmarksfly.cn

TS:   s.split(",")
来源：http://bd.colortex.cn

Java: s.split(",");  s.split("\\s+")
来源：http://sk.jianghongdianzi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tc.muxihuayi.cn

Ruby: s.split(",");  s.split
来源：http://ae.chemitech.net.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zz.chemitech.net.cn

[E08] 数组按分隔符合并
来源：http://ux.yuexingan06.cn

Py:   ",".join(items)
来源：http://ge.bjjhwx.cn

PHP:  implode(",", $items);
来源：http://qn.shxzukj.cn

JS:   items.join(",")
来源：http://qm.yuntaijiaju.cn

TS:   items.join(",")
来源：http://zw.chemitech.net.cn

Java: String.join(",", items)
来源：http://gl.szxytkj.cn

Go:   strings.Join(items, ",")
来源：http://ty.yuntaijiaju.cn

Ruby: items.join(",")
来源：http://uv.haigaiapp.cn

C#:   string.Join(",", items)
来源：http://jy.nicolike.cn

[E09] 去除所有空白字符
来源：http://iw.muxihuayi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://iw.lnxyls.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cr.colortex.cn

JS:   s.replace(/\s+/g, "")
来源：http://no.jianghongdianzi.cn

TS:   s.replace(/\s+/g, "")
来源：http://gc.9csxet.cn

Java: s.replaceAll("\\s+", "")
来源：http://ce.hahajie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://bd.lnxyls.cn

Ruby: s.gsub(/\s+/, "")
来源：http://dn.hnjuh.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ud.bjjhwx.cn

[E10] 左侧补零 / 定长填充
来源：http://zv.huixinmuqiang.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://to.bjjhwx.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://na.jianghongdianzi.cn

JS:   "7".padStart(3, "0")
来源：http://cc.bookmarksfly.cn

TS:   "7".padStart(3, "0")
来源：http://uv.huixinmuqiang.cn

Java: String.format("%03d", 7)
来源：http://ds.muxihuayi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://vq.szsharing.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hn.lnxyls.cn


<!-- 参考信息 -->