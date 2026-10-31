代发 wailian999

C#:   list.Insert(0, 0);
来源：http://tu.newstarts.cn

[D04] 删除元素
来源：http://wx.521024.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://oq.521024.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vd.jctech888.com.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xi.yuexingan06.cn

TS:   arr.splice(0, 1);
来源：http://tc.521024.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fg.szsharing.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rt.521024.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fa.gzmigu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kh.9csxet.cn

[D05] 访问与修改元素
来源：http://rz.nicolike.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://og.nicolike.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sd.muxihuayi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fx.wgjwhj.cn

TS:   arr[0]; arr.at(-1);
来源：http://ue.szsharing.cn

Java: list.get(0); list.set(0, 9);
来源：http://mm.szxytkj.cn

Go:   arr[0]; arr[0] = 9
来源：http://bl.huanxung.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dv.yuntaijiaju.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ji.huixinmuqiang.cn

[D06] 数组长度
来源：http://aj.yuexingan06.cn

Py:   len(arr)
来源：http://gf.bjjhwx.cn

PHP:  count($arr);
来源：http://tu.nicolike.cn

JS:   arr.length
来源：http://sb.nszjky.cn

TS:   arr.length
来源：http://pq.bjjhwx.cn

Java: list.size();
来源：http://ez.jianghongdianzi.cn

Go:   len(arr)
来源：http://df.panjiajie.cn

Ruby: arr.length; arr.size
来源：http://ps.yuexingan06.cn

C#:   list.Count;
来源：http://sr.lnxyls.cn

[D07] 切片 / 取子数组
来源：http://de.huixinmuqiang.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fm.szxytkj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://xh.hnjuh.cn

JS:   arr.slice(1, 4);
来源：http://cx.jianghongdianzi.cn

TS:   arr.slice(1, 4);
来源：http://fa.huixinmuqiang.cn

Java: list.subList(1, 4);
来源：http://mq.muxihuayi.cn

Go:   arr[1:4]
来源：http://rh.jianghongdianzi.cn

Ruby: arr[1, 3]
来源：http://pr.haigaiapp.cn

C#:   list.GetRange(1, 3);
来源：http://to.huixiangedu.cn

[D08] 合并两个数组
来源：http://kw.szxytkj.cn

Py:   a + b;  a.extend(b)
来源：http://cs.9csxet.cn

PHP:  array_merge($a, $b);
来源：http://yb.szsharing.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://zj.huixiangedu.cn

TS:   [...a, ...b];
来源：http://oc.panjiajie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ty.huixiangedu.cn

Go:   append(a, b...)
来源：http://dp.shxzukj.cn

Ruby: a + b;  a.concat(b)
来源：http://xn.panjiajie.cn

C#:   a.Concat(b).ToList()
来源：http://fq.haigaiapp.cn

[D09] 排序（升序）
来源：http://uz.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://xg.muxihuayi.cn

PHP:  sort($arr);
来源：http://sp.muxihuayi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://eq.jianghongdianzi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xk.shtwfgs.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://kq.huanxung.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bk.jianghongdianzi.cn

Ruby: arr.sort
来源：http://wu.shxzskj.cn

C#:   list.Sort();
来源：http://iw.shxzskj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://um.huanxung.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kn.muxihuayi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jn.colortex.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jg.yuntaijiaju.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pw.haigaiapp.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://db.asd995.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yz.asd995.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bj.shtwfgs.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yp.asd995.cn

[D11] 反转数组
来源：http://ds.jctech888.com.cn

Py:   arr[::-1];  arr.reverse()
来源：http://pz.asd995.cn

PHP:  array_reverse($arr);
来源：http://mn.bjjhwx.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hk.shtwfgs.cn

TS:   [...arr].reverse();
来源：http://lb.colortex.cn

Java: Collections.reverse(list);
来源：http://av.shxzskj.cn

Go:   slices.Reverse(arr)
来源：http://bp.jctech888.com.cn

Ruby: arr.reverse
来源：http://zb.jctech888.com.cn

C#:   list.Reverse();
来源：http://vt.bookmarksfly.cn

[D12] 查找元素下标
来源：http://so.shxzukj.cn

Py:   arr.index(x);  x in arr
来源：http://lq.huanxung.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dx.huixinmuqiang.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rd.gzmigu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dq.huanxung.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mg.asd995.cn

Go:   slices.Index(arr, x)
来源：http://ue.jianghongdianzi.cn

Ruby: arr.index(x)
来源：http://bd.szxytkj.cn

C#:   list.IndexOf(x);
来源：http://hp.hahajie.cn

[D13] 过滤（保留满足条件的）
来源：http://ln.yuexingan06.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yg.gzmigu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://uk.shxzskj.cn

JS:   arr.filter(x => x > 3)
来源：http://kz.jctech888.com.cn

TS:   arr.filter(x => x > 3)
来源：http://oc.huixiangedu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zn.szxytkj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://sb.lnxyls.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ei.shxzukj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://jy.wgjwhj.cn

[D14] 映射转换（每个元素变形）
来源：http://ye.lnxyls.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kg.haigaiapp.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ed.muxihuayi.cn

JS:   arr.map(x => x * 2)
来源：http://qu.colortex.cn

TS:   arr.map(x => x * 2)
来源：http://pt.colortex.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://az.jianghongdianzi.cn

Go:   // 手写循环
来源：http://mb.jianghongdianzi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://zv.muxihuayi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://on.panjiajie.cn

[D15] 去重
来源：http://hc.lnxyls.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://js.huixinmuqiang.cn

PHP:  array_unique($arr);
来源：http://nj.colortex.cn

JS:   [...new Set(arr)]
来源：http://bz.nicolike.cn

TS:   [...new Set(arr)]
来源：http://ih.yuexingan06.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://us.shxzskj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://uo.haigaiapp.cn

Ruby: arr.uniq
来源：http://th.wgjwhj.cn

C#:   list.Distinct().ToList()
来源：http://hh.szxytkj.cn

[D16] 求和与平均值
来源：http://sq.huixinmuqiang.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vo.gzmigu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kv.bjjhwx.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jm.hahajie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sh.huixiangedu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ca.jctech888.com.cn

Go:   // 手写循环累加
来源：http://xb.huanxung.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rn.hahajie.cn

C#:   list.Sum();  list.Average()
来源：http://ho.9csxet.cn

[D17] 最大值与最小值
来源：http://dx.bookmarksfly.cn

Py:   max(arr);  min(arr)
来源：http://vo.shxzukj.cn

PHP:  max($arr);  min($arr);
来源：http://mh.nicolike.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kn.szxytkj.cn

TS:   Math.max(...arr);
来源：http://fr.yuntaijiaju.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://cq.chemitech.net.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dg.lnxyls.cn

Ruby: arr.max;  arr.min
来源：http://vx.szxytkj.cn

C#:   list.Max();  list.Min()
来源：http://kb.huixinmuqiang.cn

[D18] 扁平化嵌套数组
来源：http://bs.chemitech.net.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vu.jctech888.com.cn

PHP:  array_merge(...$nested);
来源：http://wr.yuexingan06.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ee.yuntaijiaju.cn

TS:   nested.flat();
来源：http://ax.newstarts.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rc.shtwfgs.cn

Go:   // 手写双层循环
来源：http://sv.chemitech.net.cn

Ruby: nested.flatten
来源：http://bw.shtwfgs.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://mv.asd995.cn

[D19] 按字段分组
来源：http://kv.shxzskj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ew.hahajie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yq.521024.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://os.panjiajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://hh.huixinmuqiang.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qn.yuexingan06.cn

Go:   // 手写 map[string][]T
来源：http://mg.9csxet.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://yx.huanxung.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tu.lnxyls.cn

[D20] 统计每个元素出现次数
来源：http://cc.bjjhwx.cn

Py:   Counter(arr)
来源：http://jb.chemitech.net.cn

PHP:  array_count_values($arr);
来源：http://qx.nszjky.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pf.jianghongdianzi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ou.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pd.huixinmuqiang.cn

Go:   // 手写 map[T]int
来源：http://fp.haigaiapp.cn

Ruby: arr.tally
来源：http://wa.bjjhwx.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dk.haigaiapp.cn

[D21] 判断是否包含某元素
来源：http://cs.jctech888.com.cn

Py:   x in arr
来源：http://wh.colortex.cn

PHP:  in_array($x, $arr, true);
来源：http://gx.panjiajie.cn

JS:   arr.includes(x)
来源：http://hl.haigaiapp.cn

TS:   arr.includes(x)
来源：http://zg.lnxyls.cn

Java: list.contains(x)
来源：http://un.huixinmuqiang.cn

Go:   slices.Contains(arr, x)
来源：http://ga.nszjky.cn

Ruby: arr.include?(x)
来源：http://rf.huixinmuqiang.cn

C#:   list.Contains(x)
来源：http://gy.hnjuh.cn

[D22] 复制数组（避免共享引用）
来源：http://ik.huixinmuqiang.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://td.lnxyls.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gw.huanxung.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ur.chemitech.net.cn

TS:   [...arr];
来源：http://od.chemitech.net.cn

Java: new ArrayList<>(list);
来源：http://po.huanxung.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xu.gzmigu.cn

Ruby: arr.dup;  arr.clone
来源：http://qm.haigaiapp.cn

C#:   new List<int>(list);
来源：http://lv.shxzskj.cn

[D23] reduce 累积计算
来源：http://sj.colortex.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pg.chemitech.net.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cy.shtwfgs.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hj.nszjky.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yx.yuntaijiaju.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://zk.jianghongdianzi.cn

Go:   // 手写循环
来源：http://uf.lnxyls.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xr.521024.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dx.szxytkj.cn

[D24] 字典 / Map 基本操作
来源：http://lr.yuntaijiaju.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hi.haigaiapp.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gp.muxihuayi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kw.huixinmuqiang.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mx.colortex.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ub.hnjuh.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bf.nicolike.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wz.jctech888.com.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lm.yuexingan06.cn

[D25] Set 集合去重与交并差
来源：http://wd.yuexingan06.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xh.shxzskj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hn.jctech888.com.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mh.bookmarksfly.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://eb.hnjuh.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qq.huixiangedu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sr.521024.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dz.huixiangedu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://be.hnjuh.cn

[D26] 数组转字符串
来源：http://tv.szsharing.cn

Py:   ", ".join(map(str, arr))
来源：http://tc.muxihuayi.cn

PHP:  implode(", ", $arr);
来源：http://yf.shtwfgs.cn

JS:   arr.join(", ")
来源：http://fg.bookmarksfly.cn

TS:   arr.join(", ")
来源：http://ea.newstarts.cn

Java: String.join(", ", list)
来源：http://fw.muxihuayi.cn

Go:   strings.Join(strs, ", ")
来源：http://om.bookmarksfly.cn

Ruby: arr.join(", ")
来源：http://tz.hnjuh.cn

C#:   string.Join(", ", list)
来源：http://wg.nszjky.cn

================================================================================
来源：http://yx.huanxung.cn

E. 字符串处理
来源：http://jv.huixiangedu.cn

================================================================================
来源：http://gt.shtwfgs.cn

[E01] 拼接字符串
来源：http://wc.hahajie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://oc.shxzukj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ek.bjjhwx.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://sd.huanxung.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://no.szsharing.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wl.muxihuayi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://om.szsharing.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kg.shxzukj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jw.panjiajie.cn

[E02] 重复字符串
来源：http://za.haigaiapp.cn

Py:   "ab" * 3
来源：http://co.nicolike.cn

PHP:  str_repeat("ab", 3);
来源：http://rb.szsharing.cn

JS:   "ab".repeat(3)
来源：http://zy.huanxung.cn

TS:   "ab".repeat(3)
来源：http://wm.szsharing.cn

Java: "ab".repeat(3)
来源：http://pt.haigaiapp.cn

Go:   strings.Repeat("ab", 3)
来源：http://eb.huixinmuqiang.cn

Ruby: "ab" * 3
来源：http://ix.shtwfgs.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ow.yuntaijiaju.cn

[E03] 截取子串
来源：http://fe.szxytkj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ep.chemitech.net.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bw.nicolike.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ns.shxzskj.cn

TS:   s.slice(1, 4)
来源：http://yx.panjiajie.cn

Java: s.substring(1, 4)
来源：http://ru.shxzukj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gk.huixinmuqiang.cn

Ruby: s[1, 3];  s[1..3]
来源：http://dx.yuexingan06.cn

C#:   s.Substring(1, 3)
来源：http://qk.chemitech.net.cn

[E04] 查找子串位置
来源：http://gd.gzmigu.cn

Py:   s.find("x");  s.index("x")
来源：http://bd.szsharing.cn

PHP:  strpos($s, "x");
来源：http://pa.jctech888.com.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://iq.szxytkj.cn

TS:   s.indexOf("x")
来源：http://wr.panjiajie.cn

Java: s.indexOf("x")
来源：http://im.nicolike.cn

Go:   strings.Index(s, "x")
来源：http://zx.jianghongdianzi.cn

Ruby: s.index("x")
来源：http://jj.yuexingan06.cn

C#:   s.IndexOf("x")
来源：http://io.jctech888.com.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gn.shxzskj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mk.yuntaijiaju.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zq.huanxung.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://eo.nicolike.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hr.9csxet.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nu.shxzukj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fh.bjjhwx.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tt.haigaiapp.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://il.shxzukj.cn

[E06] 替换子串
来源：http://rq.asd995.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hy.asd995.cn

PHP:  str_replace("a", "b", $s);
来源：http://ja.nicolike.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kl.wgjwhj.cn

TS:   s.replaceAll("a", "b")
来源：http://pp.nszjky.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dv.jianghongdianzi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hi.huixinmuqiang.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bm.hnjuh.cn

C#:   s.Replace("a", "b")
来源：http://hj.bookmarksfly.cn

[E07] 按分隔符拆分
来源：http://fx.jctech888.com.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ud.huixinmuqiang.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gl.shxzukj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://py.shxzskj.cn

TS:   s.split(",")
来源：http://fp.muxihuayi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://pq.hnjuh.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://it.yuntaijiaju.cn

Ruby: s.split(",");  s.split
来源：http://yx.hnjuh.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fj.yuexingan06.cn

[E08] 数组按分隔符合并
来源：http://hr.huanxung.cn

Py:   ",".join(items)
来源：http://wv.shtwfgs.cn

PHP:  implode(",", $items);
来源：http://jw.521024.cn

JS:   items.join(",")
来源：http://bo.bookmarksfly.cn

TS:   items.join(",")
来源：http://cu.nicolike.cn

Java: String.join(",", items)
来源：http://pm.jctech888.com.cn

Go:   strings.Join(items, ",")
来源：http://ag.jctech888.com.cn

Ruby: items.join(",")
来源：http://pt.bookmarksfly.cn

C#:   string.Join(",", items)
来源：http://zu.lnxyls.cn

[E09] 去除所有空白字符
来源：http://cg.huixiangedu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zh.yuexingan06.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://iu.gzmigu.cn

JS:   s.replace(/\s+/g, "")
来源：http://xs.bookmarksfly.cn

TS:   s.replace(/\s+/g, "")
来源：http://he.hahajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://ml.hnjuh.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://pp.huixinmuqiang.cn

Ruby: s.gsub(/\s+/, "")
来源：http://nc.shxzskj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://oz.hnjuh.cn

[E10] 左侧补零 / 定长填充
来源：http://lf.nszjky.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://js.jianghongdianzi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xf.nicolike.cn

JS:   "7".padStart(3, "0")
来源：http://ny.huanxung.cn

TS:   "7".padStart(3, "0")
来源：http://yp.muxihuayi.cn

Java: String.format("%03d", 7)
来源：http://gr.hnjuh.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://so.shxzukj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://aa.newstarts.cn


<!-- 参考信息 -->