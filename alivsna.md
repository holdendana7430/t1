代发 wailian999

TS:   arr.slice(1, 4);
来源：http://ig.shtwfgs.cn

Java: list.subList(1, 4);
来源：http://nr.bookmarksfly.cn

Go:   arr[1:4]
来源：http://rb.asd995.cn

Ruby: arr[1, 3]
来源：http://fz.bookmarksfly.cn

C#:   list.GetRange(1, 3);
来源：http://hm.gzmigu.cn

[D08] 合并两个数组
来源：http://ua.chemitech.net.cn

Py:   a + b;  a.extend(b)
来源：http://re.shxzskj.cn

PHP:  array_merge($a, $b);
来源：http://fu.shxzskj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://dt.shxzskj.cn

TS:   [...a, ...b];
来源：http://ir.newstarts.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://id.szsharing.cn

Go:   append(a, b...)
来源：http://qf.colortex.cn

Ruby: a + b;  a.concat(b)
来源：http://fz.521024.cn

C#:   a.Concat(b).ToList()
来源：http://oq.nicolike.cn

[D09] 排序（升序）
来源：http://le.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://hb.huanxung.cn

PHP:  sort($arr);
来源：http://zy.nicolike.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vs.jianghongdianzi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://bv.nicolike.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://kh.shtwfgs.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tl.jctech888.com.cn

Ruby: arr.sort
来源：http://jt.bjjhwx.cn

C#:   list.Sort();
来源：http://lv.szsharing.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ts.huixinmuqiang.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hk.asd995.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pt.bjjhwx.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gd.newstarts.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ix.huanxung.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ao.nszjky.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tp.huixinmuqiang.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://as.9csxet.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lr.huixinmuqiang.cn

[D11] 反转数组
来源：http://wy.colortex.cn

Py:   arr[::-1];  arr.reverse()
来源：http://cb.hahajie.cn

PHP:  array_reverse($arr);
来源：http://zd.bookmarksfly.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ix.newstarts.cn

TS:   [...arr].reverse();
来源：http://sn.hahajie.cn

Java: Collections.reverse(list);
来源：http://vp.shtwfgs.cn

Go:   slices.Reverse(arr)
来源：http://ja.bookmarksfly.cn

Ruby: arr.reverse
来源：http://zt.nicolike.cn

C#:   list.Reverse();
来源：http://gl.lnxyls.cn

[D12] 查找元素下标
来源：http://xf.panjiajie.cn

Py:   arr.index(x);  x in arr
来源：http://os.nszjky.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lk.chemitech.net.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://an.hahajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pe.shxzskj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cu.hnjuh.cn

Go:   slices.Index(arr, x)
来源：http://lp.bookmarksfly.cn

Ruby: arr.index(x)
来源：http://yb.nszjky.cn

C#:   list.IndexOf(x);
来源：http://vr.521024.cn

[D13] 过滤（保留满足条件的）
来源：http://go.nicolike.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gt.jianghongdianzi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ym.shxzskj.cn

JS:   arr.filter(x => x > 3)
来源：http://nb.shtwfgs.cn

TS:   arr.filter(x => x > 3)
来源：http://um.bookmarksfly.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rv.shxzskj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://oi.huanxung.cn

Ruby: arr.select { |x| x > 3 }
来源：http://kn.bookmarksfly.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://wp.shxzukj.cn

[D14] 映射转换（每个元素变形）
来源：http://kr.shtwfgs.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://in.521024.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sy.newstarts.cn

JS:   arr.map(x => x * 2)
来源：http://qn.wgjwhj.cn

TS:   arr.map(x => x * 2)
来源：http://jw.hahajie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ev.muxihuayi.cn

Go:   // 手写循环
来源：http://xp.huanxung.cn

Ruby: arr.map { |x| x * 2 }
来源：http://re.colortex.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://vz.newstarts.cn

[D15] 去重
来源：http://bw.wgjwhj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ip.shxzskj.cn

PHP:  array_unique($arr);
来源：http://jk.9csxet.cn

JS:   [...new Set(arr)]
来源：http://xu.bjjhwx.cn

TS:   [...new Set(arr)]
来源：http://wf.shxzukj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://li.hahajie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://pg.huixiangedu.cn

Ruby: arr.uniq
来源：http://ns.hnjuh.cn

C#:   list.Distinct().ToList()
来源：http://my.lnxyls.cn

[D16] 求和与平均值
来源：http://bg.bjjhwx.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://va.muxihuayi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mv.panjiajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://eu.szsharing.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cw.gzmigu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ej.colortex.cn

Go:   // 手写循环累加
来源：http://iq.huixinmuqiang.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cw.nicolike.cn

C#:   list.Sum();  list.Average()
来源：http://dh.huixinmuqiang.cn

[D17] 最大值与最小值
来源：http://vl.panjiajie.cn

Py:   max(arr);  min(arr)
来源：http://fp.9csxet.cn

PHP:  max($arr);  min($arr);
来源：http://qc.gzmigu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uc.jctech888.com.cn

TS:   Math.max(...arr);
来源：http://nk.hahajie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://tz.bjjhwx.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gy.hahajie.cn

Ruby: arr.max;  arr.min
来源：http://zw.lnxyls.cn

C#:   list.Max();  list.Min()
来源：http://uf.szxytkj.cn

[D18] 扁平化嵌套数组
来源：http://th.szsharing.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ws.huixinmuqiang.cn

PHP:  array_merge(...$nested);
来源：http://vg.lnxyls.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jo.panjiajie.cn

TS:   nested.flat();
来源：http://fj.asd995.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qq.shtwfgs.cn

Go:   // 手写双层循环
来源：http://ay.panjiajie.cn

Ruby: nested.flatten
来源：http://gq.haigaiapp.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ik.shxzukj.cn

[D19] 按字段分组
来源：http://ut.jctech888.com.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://et.szsharing.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ug.nicolike.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cb.bjjhwx.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ro.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://to.nszjky.cn

Go:   // 手写 map[string][]T
来源：http://ld.jianghongdianzi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ms.panjiajie.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ks.huanxung.cn

[D20] 统计每个元素出现次数
来源：http://uk.hahajie.cn

Py:   Counter(arr)
来源：http://zk.asd995.cn

PHP:  array_count_values($arr);
来源：http://zm.szxytkj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mw.haigaiapp.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jn.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://sc.panjiajie.cn

Go:   // 手写 map[T]int
来源：http://gx.shxzukj.cn

Ruby: arr.tally
来源：http://kg.yuexingan06.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nu.9csxet.cn

[D21] 判断是否包含某元素
来源：http://si.asd995.cn

Py:   x in arr
来源：http://kk.wgjwhj.cn

PHP:  in_array($x, $arr, true);
来源：http://xf.lnxyls.cn

JS:   arr.includes(x)
来源：http://or.521024.cn

TS:   arr.includes(x)
来源：http://jj.hnjuh.cn

Java: list.contains(x)
来源：http://pm.shxzukj.cn

Go:   slices.Contains(arr, x)
来源：http://ts.bookmarksfly.cn

Ruby: arr.include?(x)
来源：http://ru.muxihuayi.cn

C#:   list.Contains(x)
来源：http://kh.521024.cn

[D22] 复制数组（避免共享引用）
来源：http://su.hahajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://et.yuntaijiaju.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ej.bjjhwx.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://li.bookmarksfly.cn

TS:   [...arr];
来源：http://ri.jctech888.com.cn

Java: new ArrayList<>(list);
来源：http://jn.nicolike.cn

Go:   copied := append([]int(nil), arr...)
来源：http://td.jctech888.com.cn

Ruby: arr.dup;  arr.clone
来源：http://he.nicolike.cn

C#:   new List<int>(list);
来源：http://zf.shxzukj.cn

[D23] reduce 累积计算
来源：http://ua.wgjwhj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tj.chemitech.net.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lp.9csxet.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ob.wgjwhj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wd.nicolike.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://il.wgjwhj.cn

Go:   // 手写循环
来源：http://ut.yuexingan06.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dy.gzmigu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vb.nszjky.cn

[D24] 字典 / Map 基本操作
来源：http://ej.shxzukj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ia.huanxung.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dj.szsharing.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wd.521024.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dq.nicolike.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lz.huixiangedu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bs.521024.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qv.hahajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wt.szxytkj.cn

[D25] Set 集合去重与交并差
来源：http://yg.panjiajie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hf.jianghongdianzi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jb.muxihuayi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://iy.chemitech.net.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vj.yuexingan06.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zu.shxzskj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mc.szxytkj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zn.bjjhwx.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://il.nszjky.cn

[D26] 数组转字符串
来源：http://ge.521024.cn

Py:   ", ".join(map(str, arr))
来源：http://de.huanxung.cn

PHP:  implode(", ", $arr);
来源：http://ki.panjiajie.cn

JS:   arr.join(", ")
来源：http://ne.szsharing.cn

TS:   arr.join(", ")
来源：http://fi.asd995.cn

Java: String.join(", ", list)
来源：http://vi.shxzskj.cn

Go:   strings.Join(strs, ", ")
来源：http://fl.szxytkj.cn

Ruby: arr.join(", ")
来源：http://om.colortex.cn

C#:   string.Join(", ", list)
来源：http://hr.yuntaijiaju.cn

================================================================================
来源：http://yi.chemitech.net.cn

E. 字符串处理
来源：http://mw.hahajie.cn

================================================================================
来源：http://yf.521024.cn

[E01] 拼接字符串
来源：http://om.shtwfgs.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zf.asd995.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lw.newstarts.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rh.asd995.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wz.asd995.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nb.wgjwhj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://po.huanxung.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tm.huanxung.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xx.huanxung.cn

[E02] 重复字符串
来源：http://cp.shxzukj.cn

Py:   "ab" * 3
来源：http://mb.szsharing.cn

PHP:  str_repeat("ab", 3);
来源：http://mg.szsharing.cn

JS:   "ab".repeat(3)
来源：http://pb.szsharing.cn

TS:   "ab".repeat(3)
来源：http://aw.wgjwhj.cn

Java: "ab".repeat(3)
来源：http://jk.gzmigu.cn

Go:   strings.Repeat("ab", 3)
来源：http://xu.9csxet.cn

Ruby: "ab" * 3
来源：http://ls.newstarts.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yr.jianghongdianzi.cn

[E03] 截取子串
来源：http://nz.panjiajie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://be.shtwfgs.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fr.bookmarksfly.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hu.521024.cn

TS:   s.slice(1, 4)
来源：http://qp.wgjwhj.cn

Java: s.substring(1, 4)
来源：http://xq.bjjhwx.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hw.bookmarksfly.cn

Ruby: s[1, 3];  s[1..3]
来源：http://wl.hahajie.cn

C#:   s.Substring(1, 3)
来源：http://bw.huixiangedu.cn

[E04] 查找子串位置
来源：http://cp.lnxyls.cn

Py:   s.find("x");  s.index("x")
来源：http://xq.newstarts.cn

PHP:  strpos($s, "x");
来源：http://jk.hnjuh.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wg.szxytkj.cn

TS:   s.indexOf("x")
来源：http://mq.chemitech.net.cn

Java: s.indexOf("x")
来源：http://dl.jianghongdianzi.cn

Go:   strings.Index(s, "x")
来源：http://vd.bookmarksfly.cn

Ruby: s.index("x")
来源：http://gf.gzmigu.cn

C#:   s.IndexOf("x")
来源：http://us.colortex.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://yt.nszjky.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://sn.shxzukj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://aw.hnjuh.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dx.huixiangedu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://cd.nicolike.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://eu.huixiangedu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zv.chemitech.net.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gt.haigaiapp.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kp.hnjuh.cn

[E06] 替换子串
来源：http://uc.gzmigu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nk.bjjhwx.cn

PHP:  str_replace("a", "b", $s);
来源：http://iu.shtwfgs.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pq.szxytkj.cn

TS:   s.replaceAll("a", "b")
来源：http://il.huixiangedu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gk.yuexingan06.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://em.shxzskj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dp.panjiajie.cn

C#:   s.Replace("a", "b")
来源：http://la.szxytkj.cn

[E07] 按分隔符拆分
来源：http://pj.521024.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://br.jctech888.com.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ok.shxzskj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ed.nszjky.cn

TS:   s.split(",")
来源：http://kc.nszjky.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zy.bookmarksfly.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://uq.521024.cn

Ruby: s.split(",");  s.split
来源：http://uz.szxytkj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ig.panjiajie.cn

[E08] 数组按分隔符合并
来源：http://kj.haigaiapp.cn

Py:   ",".join(items)
来源：http://on.nicolike.cn

PHP:  implode(",", $items);
来源：http://eo.jctech888.com.cn

JS:   items.join(",")
来源：http://im.chemitech.net.cn

TS:   items.join(",")
来源：http://zl.wgjwhj.cn

Java: String.join(",", items)
来源：http://ag.haigaiapp.cn

Go:   strings.Join(items, ",")
来源：http://al.bookmarksfly.cn

Ruby: items.join(",")
来源：http://cl.yuntaijiaju.cn

C#:   string.Join(",", items)
来源：http://ir.shxzskj.cn

[E09] 去除所有空白字符
来源：http://qw.huanxung.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cu.nszjky.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lu.huanxung.cn

JS:   s.replace(/\s+/g, "")
来源：http://it.wgjwhj.cn

TS:   s.replace(/\s+/g, "")
来源：http://op.newstarts.cn

Java: s.replaceAll("\\s+", "")
来源：http://gm.shxzskj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ml.nicolike.cn

Ruby: s.gsub(/\s+/, "")
来源：http://dp.huixiangedu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nl.bookmarksfly.cn

[E10] 左侧补零 / 定长填充
来源：http://th.hnjuh.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ui.chemitech.net.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bg.colortex.cn

JS:   "7".padStart(3, "0")
来源：http://qs.shxzukj.cn

TS:   "7".padStart(3, "0")
来源：http://is.shxzukj.cn

Java: String.format("%03d", 7)
来源：http://ji.shxzukj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ud.hnjuh.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zk.szsharing.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://oj.bookmarksfly.cn

[E11] 反转字符串
来源：http://vp.yuntaijiaju.cn

Py:   s[::-1]
来源：http://sw.panjiajie.cn

PHP:  strrev($s);
来源：http://aw.jctech888.com.cn

JS:   [...s].reverse().join("")
来源：http://ew.colortex.cn

TS:   [...s].reverse().join("")
来源：http://qm.panjiajie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zd.colortex.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://gc.bookmarksfly.cn

Ruby: s.reverse
来源：http://hs.hnjuh.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ys.huixiangedu.cn

[E12] 统计某字符出现次数
来源：http://dg.panjiajie.cn

Py:   s.count("a")
来源：http://bf.colortex.cn

PHP:  substr_count($s, "a");
来源：http://fg.szxytkj.cn

JS:   s.split("a").length - 1
来源：http://qs.yuntaijiaju.cn

TS:   s.split("a").length - 1
来源：http://ab.shtwfgs.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gu.huanxung.cn

Go:   strings.Count(s, "a")
来源：http://nr.szxytkj.cn

Ruby: s.count("a")
来源：http://ps.wgjwhj.cn

C#:   s.Count(c => c == 'a')
来源：http://ab.shtwfgs.cn

[E13] 逐字符遍历
来源：http://dl.muxihuayi.cn

Py:   for ch in s: print(ch)
来源：http://ns.gzmigu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ii.hnjuh.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://bi.muxihuayi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bn.bookmarksfly.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ne.521024.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wb.lnxyls.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://id.lnxyls.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yz.shxzukj.cn

[E14] URL 编码与 Base64
来源：http://wi.chemitech.net.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yq.yuntaijiaju.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ln.bjjhwx.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xe.hnjuh.cn


<!-- 参考信息 -->