代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://cd.szxytkj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ap.lnxyls.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pv.newstarts.cn

[D06] 数组长度
来源：http://db.szxytkj.cn

Py:   len(arr)
来源：http://zp.9csxet.cn

PHP:  count($arr);
来源：http://cy.szxytkj.cn

JS:   arr.length
来源：http://st.bookmarksfly.cn

TS:   arr.length
来源：http://gk.gzmigu.cn

Java: list.size();
来源：http://kx.jctech888.com.cn

Go:   len(arr)
来源：http://yy.jctech888.com.cn

Ruby: arr.length; arr.size
来源：http://aw.huixinmuqiang.cn

C#:   list.Count;
来源：http://cu.hnjuh.cn

[D07] 切片 / 取子数组
来源：http://vo.huixinmuqiang.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bo.huixinmuqiang.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ea.wgjwhj.cn

JS:   arr.slice(1, 4);
来源：http://mk.yuntaijiaju.cn

TS:   arr.slice(1, 4);
来源：http://ox.szsharing.cn

Java: list.subList(1, 4);
来源：http://li.nicolike.cn

Go:   arr[1:4]
来源：http://xm.huixinmuqiang.cn

Ruby: arr[1, 3]
来源：http://fg.szxytkj.cn

C#:   list.GetRange(1, 3);
来源：http://cp.yuexingan06.cn

[D08] 合并两个数组
来源：http://iw.newstarts.cn

Py:   a + b;  a.extend(b)
来源：http://lo.bookmarksfly.cn

PHP:  array_merge($a, $b);
来源：http://zw.yuexingan06.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://jn.shtwfgs.cn

TS:   [...a, ...b];
来源：http://qn.huixinmuqiang.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ea.newstarts.cn

Go:   append(a, b...)
来源：http://bj.huixiangedu.cn

Ruby: a + b;  a.concat(b)
来源：http://ct.haigaiapp.cn

C#:   a.Concat(b).ToList()
来源：http://fs.lnxyls.cn

[D09] 排序（升序）
来源：http://zi.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://aw.9csxet.cn

PHP:  sort($arr);
来源：http://on.nszjky.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vn.gzmigu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://vs.szxytkj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ei.huixiangedu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zc.huanxung.cn

Ruby: arr.sort
来源：http://oh.nszjky.cn

C#:   list.Sort();
来源：http://rr.huanxung.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://dl.newstarts.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nx.szxytkj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ym.nszjky.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mc.shxzukj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mu.bjjhwx.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://uk.bjjhwx.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://if.jctech888.com.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hy.yuexingan06.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vy.huixinmuqiang.cn

[D11] 反转数组
来源：http://by.shxzskj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ji.nicolike.cn

PHP:  array_reverse($arr);
来源：http://uf.huixiangedu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://su.asd995.cn

TS:   [...arr].reverse();
来源：http://rx.chemitech.net.cn

Java: Collections.reverse(list);
来源：http://ho.bookmarksfly.cn

Go:   slices.Reverse(arr)
来源：http://lg.chemitech.net.cn

Ruby: arr.reverse
来源：http://fb.huixiangedu.cn

C#:   list.Reverse();
来源：http://od.szxytkj.cn

[D12] 查找元素下标
来源：http://ma.szxytkj.cn

Py:   arr.index(x);  x in arr
来源：http://ef.bookmarksfly.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mm.szsharing.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rv.colortex.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vg.szxytkj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ix.jianghongdianzi.cn

Go:   slices.Index(arr, x)
来源：http://ar.bjjhwx.cn

Ruby: arr.index(x)
来源：http://xz.bjjhwx.cn

C#:   list.IndexOf(x);
来源：http://ko.panjiajie.cn

[D13] 过滤（保留满足条件的）
来源：http://hz.bjjhwx.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mn.yuexingan06.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://oq.9csxet.cn

JS:   arr.filter(x => x > 3)
来源：http://rz.shxzukj.cn

TS:   arr.filter(x => x > 3)
来源：http://yj.hnjuh.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://io.nszjky.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nj.gzmigu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://nl.shxzskj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ud.newstarts.cn

[D14] 映射转换（每个元素变形）
来源：http://tx.szxytkj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ts.hahajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mb.shtwfgs.cn

JS:   arr.map(x => x * 2)
来源：http://pz.huanxung.cn

TS:   arr.map(x => x * 2)
来源：http://oo.colortex.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://xs.jctech888.com.cn

Go:   // 手写循环
来源：http://vt.yuexingan06.cn

Ruby: arr.map { |x| x * 2 }
来源：http://sa.asd995.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://dg.muxihuayi.cn

[D15] 去重
来源：http://rq.shtwfgs.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qg.panjiajie.cn

PHP:  array_unique($arr);
来源：http://aw.yuexingan06.cn

JS:   [...new Set(arr)]
来源：http://sc.hnjuh.cn

TS:   [...new Set(arr)]
来源：http://ns.nicolike.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vd.huixiangedu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vm.yuexingan06.cn

Ruby: arr.uniq
来源：http://aw.hahajie.cn

C#:   list.Distinct().ToList()
来源：http://oh.shxzskj.cn

[D16] 求和与平均值
来源：http://od.bjjhwx.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yc.chemitech.net.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cy.haigaiapp.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://iz.nszjky.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://un.asd995.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qb.bjjhwx.cn

Go:   // 手写循环累加
来源：http://bp.asd995.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wz.nicolike.cn

C#:   list.Sum();  list.Average()
来源：http://cl.lnxyls.cn

[D17] 最大值与最小值
来源：http://pj.newstarts.cn

Py:   max(arr);  min(arr)
来源：http://dc.bjjhwx.cn

PHP:  max($arr);  min($arr);
来源：http://vw.nszjky.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cm.muxihuayi.cn

TS:   Math.max(...arr);
来源：http://ih.chemitech.net.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://tt.haigaiapp.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nu.muxihuayi.cn

Ruby: arr.max;  arr.min
来源：http://zu.gzmigu.cn

C#:   list.Max();  list.Min()
来源：http://rh.jianghongdianzi.cn

[D18] 扁平化嵌套数组
来源：http://xs.jianghongdianzi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://uz.jianghongdianzi.cn

PHP:  array_merge(...$nested);
来源：http://pa.gzmigu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zk.newstarts.cn

TS:   nested.flat();
来源：http://uq.shxzskj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://el.newstarts.cn

Go:   // 手写双层循环
来源：http://wv.hnjuh.cn

Ruby: nested.flatten
来源：http://ul.nicolike.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://nx.gzmigu.cn

[D19] 按字段分组
来源：http://rh.yuexingan06.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dg.muxihuayi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gn.521024.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ll.huixiangedu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://yq.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://er.haigaiapp.cn

Go:   // 手写 map[string][]T
来源：http://ma.szxytkj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ar.huixinmuqiang.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hh.jctech888.com.cn

[D20] 统计每个元素出现次数
来源：http://tq.gzmigu.cn

Py:   Counter(arr)
来源：http://ie.wgjwhj.cn

PHP:  array_count_values($arr);
来源：http://df.szxytkj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uu.bookmarksfly.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dw.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://al.nszjky.cn

Go:   // 手写 map[T]int
来源：http://kk.hahajie.cn

Ruby: arr.tally
来源：http://kz.lnxyls.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gd.huanxung.cn

[D21] 判断是否包含某元素
来源：http://sa.colortex.cn

Py:   x in arr
来源：http://bi.shxzukj.cn

PHP:  in_array($x, $arr, true);
来源：http://ad.shxzskj.cn

JS:   arr.includes(x)
来源：http://dp.panjiajie.cn

TS:   arr.includes(x)
来源：http://il.jianghongdianzi.cn

Java: list.contains(x)
来源：http://zh.9csxet.cn

Go:   slices.Contains(arr, x)
来源：http://hh.yuntaijiaju.cn

Ruby: arr.include?(x)
来源：http://kv.panjiajie.cn

C#:   list.Contains(x)
来源：http://nx.bookmarksfly.cn

[D22] 复制数组（避免共享引用）
来源：http://lg.shxzskj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vh.asd995.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vj.muxihuayi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lv.shxzukj.cn

TS:   [...arr];
来源：http://fb.colortex.cn

Java: new ArrayList<>(list);
来源：http://fn.jctech888.com.cn

Go:   copied := append([]int(nil), arr...)
来源：http://rq.gzmigu.cn

Ruby: arr.dup;  arr.clone
来源：http://vp.panjiajie.cn

C#:   new List<int>(list);
来源：http://sb.shxzskj.cn

[D23] reduce 累积计算
来源：http://mg.hnjuh.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xr.9csxet.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xe.bjjhwx.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://aa.nicolike.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qw.nszjky.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xo.521024.cn

Go:   // 手写循环
来源：http://ve.nicolike.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mj.shxzskj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pz.shxzskj.cn

[D24] 字典 / Map 基本操作
来源：http://oq.shtwfgs.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ee.colortex.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://aw.bookmarksfly.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ue.szsharing.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://od.9csxet.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uy.521024.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tc.nszjky.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wp.shxzskj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kt.szxytkj.cn

[D25] Set 集合去重与交并差
来源：http://zj.huixinmuqiang.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zz.huixinmuqiang.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cc.asd995.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://eo.9csxet.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bn.hahajie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://eo.bookmarksfly.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ab.hnjuh.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jq.chemitech.net.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xo.panjiajie.cn

[D26] 数组转字符串
来源：http://cc.hahajie.cn

Py:   ", ".join(map(str, arr))
来源：http://yp.lnxyls.cn

PHP:  implode(", ", $arr);
来源：http://ri.szxytkj.cn

JS:   arr.join(", ")
来源：http://oj.newstarts.cn

TS:   arr.join(", ")
来源：http://id.haigaiapp.cn

Java: String.join(", ", list)
来源：http://oi.colortex.cn

Go:   strings.Join(strs, ", ")
来源：http://cx.shxzukj.cn

Ruby: arr.join(", ")
来源：http://ec.wgjwhj.cn

C#:   string.Join(", ", list)
来源：http://vz.nszjky.cn

================================================================================
来源：http://os.shxzukj.cn

E. 字符串处理
来源：http://ua.haigaiapp.cn

================================================================================
来源：http://hr.9csxet.cn

[E01] 拼接字符串
来源：http://ha.lnxyls.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tm.szsharing.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ik.colortex.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zi.szxytkj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pz.hnjuh.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ar.newstarts.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zw.colortex.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ou.huanxung.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kj.lnxyls.cn

[E02] 重复字符串
来源：http://jb.huixiangedu.cn

Py:   "ab" * 3
来源：http://vi.shxzukj.cn

PHP:  str_repeat("ab", 3);
来源：http://sx.chemitech.net.cn

JS:   "ab".repeat(3)
来源：http://jd.asd995.cn

TS:   "ab".repeat(3)
来源：http://xn.szxytkj.cn

Java: "ab".repeat(3)
来源：http://vi.gzmigu.cn

Go:   strings.Repeat("ab", 3)
来源：http://yf.shtwfgs.cn

Ruby: "ab" * 3
来源：http://rw.521024.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ma.szxytkj.cn

[E03] 截取子串
来源：http://tj.colortex.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://se.shtwfgs.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://to.asd995.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ns.nicolike.cn

TS:   s.slice(1, 4)
来源：http://dm.panjiajie.cn

Java: s.substring(1, 4)
来源：http://vr.yuexingan06.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ig.jctech888.com.cn

Ruby: s[1, 3];  s[1..3]
来源：http://li.wgjwhj.cn

C#:   s.Substring(1, 3)
来源：http://sq.bjjhwx.cn

[E04] 查找子串位置
来源：http://ob.nszjky.cn

Py:   s.find("x");  s.index("x")
来源：http://im.shxzskj.cn

PHP:  strpos($s, "x");
来源：http://wc.jctech888.com.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kw.bjjhwx.cn

TS:   s.indexOf("x")
来源：http://nw.shxzukj.cn

Java: s.indexOf("x")
来源：http://pl.jianghongdianzi.cn

Go:   strings.Index(s, "x")
来源：http://jn.huixinmuqiang.cn

Ruby: s.index("x")
来源：http://zy.jctech888.com.cn

C#:   s.IndexOf("x")
来源：http://bm.yuexingan06.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://sc.shtwfgs.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xd.shtwfgs.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jy.szxytkj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ug.haigaiapp.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://bw.9csxet.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pt.hnjuh.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://eo.yuntaijiaju.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vo.szxytkj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yb.shxzukj.cn

[E06] 替换子串
来源：http://xr.lnxyls.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pr.asd995.cn

PHP:  str_replace("a", "b", $s);
来源：http://qw.wgjwhj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://te.jctech888.com.cn

TS:   s.replaceAll("a", "b")
来源：http://ib.521024.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tt.szxytkj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nk.lnxyls.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ga.521024.cn

C#:   s.Replace("a", "b")
来源：http://wl.jctech888.com.cn

[E07] 按分隔符拆分
来源：http://yq.jianghongdianzi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jc.huixiangedu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ek.gzmigu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://fk.szsharing.cn

TS:   s.split(",")
来源：http://uc.szxytkj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://tf.521024.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kz.huanxung.cn

Ruby: s.split(",");  s.split
来源：http://qn.nicolike.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ua.asd995.cn

[E08] 数组按分隔符合并
来源：http://py.bjjhwx.cn

Py:   ",".join(items)
来源：http://eo.hnjuh.cn

PHP:  implode(",", $items);
来源：http://os.hnjuh.cn

JS:   items.join(",")
来源：http://rh.bjjhwx.cn

TS:   items.join(",")
来源：http://ir.colortex.cn

Java: String.join(",", items)
来源：http://qk.wgjwhj.cn

Go:   strings.Join(items, ",")
来源：http://xh.jianghongdianzi.cn

Ruby: items.join(",")
来源：http://sd.yuexingan06.cn

C#:   string.Join(",", items)
来源：http://mk.haigaiapp.cn

[E09] 去除所有空白字符
来源：http://xf.gzmigu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ob.jianghongdianzi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gy.bjjhwx.cn

JS:   s.replace(/\s+/g, "")
来源：http://ic.szxytkj.cn

TS:   s.replace(/\s+/g, "")
来源：http://ez.bjjhwx.cn

Java: s.replaceAll("\\s+", "")
来源：http://gy.szsharing.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://nq.shtwfgs.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ok.huanxung.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ld.colortex.cn

[E10] 左侧补零 / 定长填充
来源：http://ho.huanxung.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nl.newstarts.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lc.chemitech.net.cn

JS:   "7".padStart(3, "0")
来源：http://gi.huixiangedu.cn

TS:   "7".padStart(3, "0")
来源：http://gn.nicolike.cn

Java: String.format("%03d", 7)
来源：http://zt.asd995.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://iz.gzmigu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ic.jianghongdianzi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cw.szxytkj.cn

[E11] 反转字符串
来源：http://kd.szxytkj.cn

Py:   s[::-1]
来源：http://ir.shxzskj.cn

PHP:  strrev($s);
来源：http://om.shtwfgs.cn

JS:   [...s].reverse().join("")
来源：http://zf.jctech888.com.cn

TS:   [...s].reverse().join("")
来源：http://ey.haigaiapp.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ks.wgjwhj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://xk.panjiajie.cn

Ruby: s.reverse
来源：http://dd.wgjwhj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://dt.wgjwhj.cn

[E12] 统计某字符出现次数
来源：http://so.hnjuh.cn

Py:   s.count("a")
来源：http://gt.haigaiapp.cn

PHP:  substr_count($s, "a");
来源：http://bz.newstarts.cn

JS:   s.split("a").length - 1
来源：http://po.lnxyls.cn

TS:   s.split("a").length - 1
来源：http://wy.haigaiapp.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lv.nszjky.cn


<!-- 参考信息 -->