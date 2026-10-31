代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hc.haigaiapp.cn

TS:   arr.splice(0, 1);
来源：http://vg.nicolike.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ym.hnjuh.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lv.jctech888.com.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ib.haigaiapp.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bd.huixinmuqiang.cn

[D05] 访问与修改元素
来源：http://dn.shtwfgs.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bc.hnjuh.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://iy.shtwfgs.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xn.szsharing.cn

TS:   arr[0]; arr.at(-1);
来源：http://ti.jctech888.com.cn

Java: list.get(0); list.set(0, 9);
来源：http://xm.jianghongdianzi.cn

Go:   arr[0]; arr[0] = 9
来源：http://nh.chemitech.net.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pd.haigaiapp.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lk.9csxet.cn

[D06] 数组长度
来源：http://gg.huixinmuqiang.cn

Py:   len(arr)
来源：http://gc.bjjhwx.cn

PHP:  count($arr);
来源：http://ny.nicolike.cn

JS:   arr.length
来源：http://bs.bookmarksfly.cn

TS:   arr.length
来源：http://kw.shtwfgs.cn

Java: list.size();
来源：http://or.newstarts.cn

Go:   len(arr)
来源：http://oh.jctech888.com.cn

Ruby: arr.length; arr.size
来源：http://uo.huixiangedu.cn

C#:   list.Count;
来源：http://ll.jianghongdianzi.cn

[D07] 切片 / 取子数组
来源：http://bk.shtwfgs.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qr.colortex.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yh.szxytkj.cn

JS:   arr.slice(1, 4);
来源：http://ie.jctech888.com.cn

TS:   arr.slice(1, 4);
来源：http://zi.gzmigu.cn

Java: list.subList(1, 4);
来源：http://cs.muxihuayi.cn

Go:   arr[1:4]
来源：http://yf.gzmigu.cn

Ruby: arr[1, 3]
来源：http://oa.szxytkj.cn

C#:   list.GetRange(1, 3);
来源：http://cn.huanxung.cn

[D08] 合并两个数组
来源：http://xx.hnjuh.cn

Py:   a + b;  a.extend(b)
来源：http://jb.huanxung.cn

PHP:  array_merge($a, $b);
来源：http://fe.huanxung.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://nb.gzmigu.cn

TS:   [...a, ...b];
来源：http://av.colortex.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pz.9csxet.cn

Go:   append(a, b...)
来源：http://mw.muxihuayi.cn

Ruby: a + b;  a.concat(b)
来源：http://wd.jianghongdianzi.cn

C#:   a.Concat(b).ToList()
来源：http://dn.shxzukj.cn

[D09] 排序（升序）
来源：http://uz.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://xn.szsharing.cn

PHP:  sort($arr);
来源：http://vj.szxytkj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gj.shtwfgs.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ui.panjiajie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ok.shtwfgs.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ic.huixiangedu.cn

Ruby: arr.sort
来源：http://yq.hahajie.cn

C#:   list.Sort();
来源：http://bh.asd995.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://hm.huixiangedu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dp.szsharing.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rp.huixiangedu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sz.yuntaijiaju.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cu.szxytkj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qk.jctech888.com.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gl.hahajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ms.bookmarksfly.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wn.chemitech.net.cn

[D11] 反转数组
来源：http://mq.haigaiapp.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ju.asd995.cn

PHP:  array_reverse($arr);
来源：http://dw.bookmarksfly.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nd.9csxet.cn

TS:   [...arr].reverse();
来源：http://op.9csxet.cn

Java: Collections.reverse(list);
来源：http://yo.lnxyls.cn

Go:   slices.Reverse(arr)
来源：http://nq.jianghongdianzi.cn

Ruby: arr.reverse
来源：http://lu.nicolike.cn

C#:   list.Reverse();
来源：http://hr.bjjhwx.cn

[D12] 查找元素下标
来源：http://vi.hnjuh.cn

Py:   arr.index(x);  x in arr
来源：http://ua.szxytkj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ui.panjiajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dc.colortex.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oj.huixinmuqiang.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zd.9csxet.cn

Go:   slices.Index(arr, x)
来源：http://kb.jctech888.com.cn

Ruby: arr.index(x)
来源：http://cs.muxihuayi.cn

C#:   list.IndexOf(x);
来源：http://ke.huixiangedu.cn

[D13] 过滤（保留满足条件的）
来源：http://ne.nicolike.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://le.panjiajie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://br.hnjuh.cn

JS:   arr.filter(x => x > 3)
来源：http://vu.szxytkj.cn

TS:   arr.filter(x => x > 3)
来源：http://xi.bjjhwx.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xl.huanxung.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://uz.bookmarksfly.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fp.wgjwhj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://sx.chemitech.net.cn

[D14] 映射转换（每个元素变形）
来源：http://ti.shxzskj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://oa.newstarts.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fo.panjiajie.cn

JS:   arr.map(x => x * 2)
来源：http://qu.jctech888.com.cn

TS:   arr.map(x => x * 2)
来源：http://rs.yuexingan06.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://cc.nszjky.cn

Go:   // 手写循环
来源：http://ze.shxzskj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://bg.jianghongdianzi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://vu.521024.cn

[D15] 去重
来源：http://cg.wgjwhj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rf.hnjuh.cn

PHP:  array_unique($arr);
来源：http://en.muxihuayi.cn

JS:   [...new Set(arr)]
来源：http://xr.jianghongdianzi.cn

TS:   [...new Set(arr)]
来源：http://ru.hnjuh.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ee.bookmarksfly.cn

Go:   // 用 map[T]struct{} 手写
来源：http://db.muxihuayi.cn

Ruby: arr.uniq
来源：http://uz.jctech888.com.cn

C#:   list.Distinct().ToList()
来源：http://yv.hahajie.cn

[D16] 求和与平均值
来源：http://ri.newstarts.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ze.chemitech.net.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ps.huanxung.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://py.wgjwhj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tq.yuexingan06.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zl.szsharing.cn

Go:   // 手写循环累加
来源：http://xc.nicolike.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ak.newstarts.cn

C#:   list.Sum();  list.Average()
来源：http://pf.jianghongdianzi.cn

[D17] 最大值与最小值
来源：http://ei.chemitech.net.cn

Py:   max(arr);  min(arr)
来源：http://mb.haigaiapp.cn

PHP:  max($arr);  min($arr);
来源：http://pf.shxzukj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pb.gzmigu.cn

TS:   Math.max(...arr);
来源：http://gf.colortex.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ku.huixinmuqiang.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://sk.nicolike.cn

Ruby: arr.max;  arr.min
来源：http://ys.hahajie.cn

C#:   list.Max();  list.Min()
来源：http://bi.shxzukj.cn

[D18] 扁平化嵌套数组
来源：http://ca.hnjuh.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hw.shtwfgs.cn

PHP:  array_merge(...$nested);
来源：http://xk.huixinmuqiang.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://aw.wgjwhj.cn

TS:   nested.flat();
来源：http://qf.huixinmuqiang.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bd.panjiajie.cn

Go:   // 手写双层循环
来源：http://ml.521024.cn

Ruby: nested.flatten
来源：http://hl.gzmigu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xu.shxzskj.cn

[D19] 按字段分组
来源：http://mv.chemitech.net.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xk.bjjhwx.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hd.hnjuh.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nw.lnxyls.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ve.muxihuayi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yx.521024.cn

Go:   // 手写 map[string][]T
来源：http://qi.nszjky.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://gl.asd995.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pq.huixinmuqiang.cn

[D20] 统计每个元素出现次数
来源：http://hm.9csxet.cn

Py:   Counter(arr)
来源：http://xc.gzmigu.cn

PHP:  array_count_values($arr);
来源：http://sh.colortex.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nj.shtwfgs.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tu.lnxyls.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ax.nicolike.cn

Go:   // 手写 map[T]int
来源：http://wb.lnxyls.cn

Ruby: arr.tally
来源：http://mv.haigaiapp.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://eb.yuntaijiaju.cn

[D21] 判断是否包含某元素
来源：http://sd.shxzskj.cn

Py:   x in arr
来源：http://hv.szxytkj.cn

PHP:  in_array($x, $arr, true);
来源：http://qb.jctech888.com.cn

JS:   arr.includes(x)
来源：http://uz.colortex.cn

TS:   arr.includes(x)
来源：http://xt.yuntaijiaju.cn

Java: list.contains(x)
来源：http://hz.lnxyls.cn

Go:   slices.Contains(arr, x)
来源：http://vx.newstarts.cn

Ruby: arr.include?(x)
来源：http://fa.nicolike.cn

C#:   list.Contains(x)
来源：http://jx.9csxet.cn

[D22] 复制数组（避免共享引用）
来源：http://nn.bookmarksfly.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ge.wgjwhj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kl.szsharing.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cp.bjjhwx.cn

TS:   [...arr];
来源：http://wg.yuntaijiaju.cn

Java: new ArrayList<>(list);
来源：http://gt.jctech888.com.cn

Go:   copied := append([]int(nil), arr...)
来源：http://on.yuntaijiaju.cn

Ruby: arr.dup;  arr.clone
来源：http://xu.shxzskj.cn

C#:   new List<int>(list);
来源：http://eh.hnjuh.cn

[D23] reduce 累积计算
来源：http://dl.szxytkj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sc.yuntaijiaju.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://am.shxzskj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://la.hahajie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ct.szsharing.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://dl.shtwfgs.cn

Go:   // 手写循环
来源：http://sr.lnxyls.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://if.yuntaijiaju.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://te.shxzukj.cn

[D24] 字典 / Map 基本操作
来源：http://rw.newstarts.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pa.hahajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://iv.jctech888.com.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vw.521024.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://al.nszjky.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dq.wgjwhj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jn.yuntaijiaju.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wc.yuntaijiaju.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://id.haigaiapp.cn

[D25] Set 集合去重与交并差
来源：http://dl.nicolike.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lr.szsharing.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wv.shxzukj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qh.nszjky.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ke.jianghongdianzi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pq.jianghongdianzi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hg.521024.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vu.yuntaijiaju.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lc.szsharing.cn

[D26] 数组转字符串
来源：http://en.newstarts.cn

Py:   ", ".join(map(str, arr))
来源：http://zx.9csxet.cn

PHP:  implode(", ", $arr);
来源：http://eo.muxihuayi.cn

JS:   arr.join(", ")
来源：http://eq.szxytkj.cn

TS:   arr.join(", ")
来源：http://gj.9csxet.cn

Java: String.join(", ", list)
来源：http://rd.bjjhwx.cn

Go:   strings.Join(strs, ", ")
来源：http://pp.huixiangedu.cn

Ruby: arr.join(", ")
来源：http://zn.nicolike.cn

C#:   string.Join(", ", list)
来源：http://ff.szxytkj.cn

================================================================================
来源：http://mn.huixiangedu.cn

E. 字符串处理
来源：http://wg.hnjuh.cn

================================================================================
来源：http://lf.hnjuh.cn

[E01] 拼接字符串
来源：http://uk.huixinmuqiang.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dw.wgjwhj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yk.jctech888.com.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fs.szsharing.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vw.wgjwhj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hx.521024.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mj.haigaiapp.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lb.bookmarksfly.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mt.jianghongdianzi.cn

[E02] 重复字符串
来源：http://lt.9csxet.cn

Py:   "ab" * 3
来源：http://bq.jctech888.com.cn

PHP:  str_repeat("ab", 3);
来源：http://oz.jctech888.com.cn

JS:   "ab".repeat(3)
来源：http://sc.nicolike.cn

TS:   "ab".repeat(3)
来源：http://fh.huanxung.cn

Java: "ab".repeat(3)
来源：http://jg.haigaiapp.cn

Go:   strings.Repeat("ab", 3)
来源：http://bi.bjjhwx.cn

Ruby: "ab" * 3
来源：http://ko.nszjky.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ih.wgjwhj.cn

[E03] 截取子串
来源：http://pm.bookmarksfly.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://de.szsharing.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bb.wgjwhj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zf.yuntaijiaju.cn

TS:   s.slice(1, 4)
来源：http://am.gzmigu.cn

Java: s.substring(1, 4)
来源：http://ph.521024.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xg.gzmigu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://js.huixinmuqiang.cn

C#:   s.Substring(1, 3)
来源：http://fd.9csxet.cn

[E04] 查找子串位置
来源：http://yh.shtwfgs.cn

Py:   s.find("x");  s.index("x")
来源：http://hs.szxytkj.cn

PHP:  strpos($s, "x");
来源：http://ij.muxihuayi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cx.shxzskj.cn

TS:   s.indexOf("x")
来源：http://bz.szxytkj.cn

Java: s.indexOf("x")
来源：http://yt.bookmarksfly.cn

Go:   strings.Index(s, "x")
来源：http://nk.muxihuayi.cn

Ruby: s.index("x")
来源：http://ms.yuexingan06.cn

C#:   s.IndexOf("x")
来源：http://ae.asd995.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://wu.yuexingan06.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jb.szsharing.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rr.shtwfgs.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oi.wgjwhj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ev.jianghongdianzi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qp.shtwfgs.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tx.shtwfgs.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ue.yuntaijiaju.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cz.shtwfgs.cn

[E06] 替换子串
来源：http://rm.haigaiapp.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://eh.shxzskj.cn

PHP:  str_replace("a", "b", $s);
来源：http://rv.huixiangedu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cf.huanxung.cn

TS:   s.replaceAll("a", "b")
来源：http://cf.shtwfgs.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vi.521024.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fc.bjjhwx.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lb.haigaiapp.cn

C#:   s.Replace("a", "b")
来源：http://fe.huixinmuqiang.cn

[E07] 按分隔符拆分
来源：http://aj.haigaiapp.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tt.gzmigu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://do.newstarts.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ys.wgjwhj.cn

TS:   s.split(",")
来源：http://au.yuntaijiaju.cn

Java: s.split(",");  s.split("\\s+")
来源：http://tc.yuexingan06.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lz.shxzukj.cn

Ruby: s.split(",");  s.split
来源：http://sq.521024.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cz.lnxyls.cn

[E08] 数组按分隔符合并
来源：http://mu.shtwfgs.cn

Py:   ",".join(items)
来源：http://zm.hnjuh.cn

PHP:  implode(",", $items);
来源：http://ac.shxzskj.cn

JS:   items.join(",")
来源：http://lv.hahajie.cn

TS:   items.join(",")
来源：http://ew.huixiangedu.cn

Java: String.join(",", items)
来源：http://ca.jianghongdianzi.cn

Go:   strings.Join(items, ",")
来源：http://ir.hnjuh.cn

Ruby: items.join(",")
来源：http://zm.asd995.cn

C#:   string.Join(",", items)
来源：http://fb.haigaiapp.cn

[E09] 去除所有空白字符
来源：http://fz.hahajie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tq.nicolike.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wv.yuexingan06.cn

JS:   s.replace(/\s+/g, "")
来源：http://nc.huanxung.cn

TS:   s.replace(/\s+/g, "")
来源：http://sj.521024.cn

Java: s.replaceAll("\\s+", "")
来源：http://bp.9csxet.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ty.szxytkj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://am.szxytkj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ev.huixiangedu.cn

[E10] 左侧补零 / 定长填充
来源：http://zq.haigaiapp.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ey.asd995.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ze.newstarts.cn

JS:   "7".padStart(3, "0")
来源：http://gb.huixiangedu.cn

TS:   "7".padStart(3, "0")
来源：http://cl.wgjwhj.cn

Java: String.format("%03d", 7)
来源：http://dl.9csxet.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://dz.nicolike.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vo.wgjwhj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ed.huixinmuqiang.cn

[E11] 反转字符串
来源：http://fm.szsharing.cn

Py:   s[::-1]
来源：http://vw.newstarts.cn

PHP:  strrev($s);
来源：http://ia.wgjwhj.cn


<!-- 参考信息 -->