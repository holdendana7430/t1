代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://ru.nicolike.cn

[D08] 合并两个数组
来源：http://jv.bookmarksfly.cn

Py:   a + b;  a.extend(b)
来源：http://xr.muxihuayi.cn

PHP:  array_merge($a, $b);
来源：http://nz.szxytkj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://mk.yuntaijiaju.cn

TS:   [...a, ...b];
来源：http://ab.muxihuayi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tp.lnxyls.cn

Go:   append(a, b...)
来源：http://wz.haigaiapp.cn

Ruby: a + b;  a.concat(b)
来源：http://ga.muxihuayi.cn

C#:   a.Concat(b).ToList()
来源：http://yj.jianghongdianzi.cn

[D09] 排序（升序）
来源：http://gx.jctech888.com.cn

Py:   sorted(arr);  arr.sort()
来源：http://ul.muxihuayi.cn

PHP:  sort($arr);
来源：http://ko.huixiangedu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://eq.bookmarksfly.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://yh.panjiajie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vj.9csxet.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://et.nszjky.cn

Ruby: arr.sort
来源：http://xz.nszjky.cn

C#:   list.Sort();
来源：http://kd.nicolike.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qp.asd995.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jp.hahajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mb.jctech888.com.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jg.shxzukj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bn.shxzskj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nn.huixiangedu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hm.wgjwhj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fs.nicolike.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jn.hnjuh.cn

[D11] 反转数组
来源：http://ki.bjjhwx.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xo.nszjky.cn

PHP:  array_reverse($arr);
来源：http://wp.hnjuh.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://le.9csxet.cn

TS:   [...arr].reverse();
来源：http://ra.szsharing.cn

Java: Collections.reverse(list);
来源：http://so.huanxung.cn

Go:   slices.Reverse(arr)
来源：http://ta.colortex.cn

Ruby: arr.reverse
来源：http://gz.szsharing.cn

C#:   list.Reverse();
来源：http://wy.gzmigu.cn

[D12] 查找元素下标
来源：http://hf.shxzukj.cn

Py:   arr.index(x);  x in arr
来源：http://fk.shxzskj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ld.yuntaijiaju.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qt.nszjky.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yy.yuexingan06.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ti.9csxet.cn

Go:   slices.Index(arr, x)
来源：http://gx.huixinmuqiang.cn

Ruby: arr.index(x)
来源：http://of.bookmarksfly.cn

C#:   list.IndexOf(x);
来源：http://tz.huanxung.cn

[D13] 过滤（保留满足条件的）
来源：http://wl.hnjuh.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lh.huixiangedu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://la.chemitech.net.cn

JS:   arr.filter(x => x > 3)
来源：http://az.9csxet.cn

TS:   arr.filter(x => x > 3)
来源：http://ab.colortex.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bx.9csxet.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ki.huanxung.cn

Ruby: arr.select { |x| x > 3 }
来源：http://sa.asd995.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vp.asd995.cn

[D14] 映射转换（每个元素变形）
来源：http://sr.wgjwhj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sk.wgjwhj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wf.gzmigu.cn

JS:   arr.map(x => x * 2)
来源：http://dv.yuexingan06.cn

TS:   arr.map(x => x * 2)
来源：http://ox.hnjuh.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://hl.yuntaijiaju.cn

Go:   // 手写循环
来源：http://kl.gzmigu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://du.bjjhwx.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zm.haigaiapp.cn

[D15] 去重
来源：http://gi.shxzukj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ct.yuexingan06.cn

PHP:  array_unique($arr);
来源：http://uj.shxzskj.cn

JS:   [...new Set(arr)]
来源：http://bw.shxzskj.cn

TS:   [...new Set(arr)]
来源：http://ma.huanxung.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://na.muxihuayi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wr.asd995.cn

Ruby: arr.uniq
来源：http://zc.haigaiapp.cn

C#:   list.Distinct().ToList()
来源：http://kq.panjiajie.cn

[D16] 求和与平均值
来源：http://rx.panjiajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ev.jianghongdianzi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kk.huixiangedu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rx.bookmarksfly.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xl.yuntaijiaju.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tt.gzmigu.cn

Go:   // 手写循环累加
来源：http://pm.huixinmuqiang.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bx.huixiangedu.cn

C#:   list.Sum();  list.Average()
来源：http://qt.colortex.cn

[D17] 最大值与最小值
来源：http://tq.szxytkj.cn

Py:   max(arr);  min(arr)
来源：http://qq.panjiajie.cn

PHP:  max($arr);  min($arr);
来源：http://ky.yuexingan06.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mn.szsharing.cn

TS:   Math.max(...arr);
来源：http://fd.shxzskj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ik.huixiangedu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wa.shxzukj.cn

Ruby: arr.max;  arr.min
来源：http://jd.yuntaijiaju.cn

C#:   list.Max();  list.Min()
来源：http://lf.lnxyls.cn

[D18] 扁平化嵌套数组
来源：http://vz.521024.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://aq.hahajie.cn

PHP:  array_merge(...$nested);
来源：http://vw.shxzukj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ln.jctech888.com.cn

TS:   nested.flat();
来源：http://ji.yuntaijiaju.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ia.wgjwhj.cn

Go:   // 手写双层循环
来源：http://td.shtwfgs.cn

Ruby: nested.flatten
来源：http://cc.muxihuayi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xy.hahajie.cn

[D19] 按字段分组
来源：http://ix.asd995.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://iu.shtwfgs.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ky.haigaiapp.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kd.nszjky.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://cn.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wi.nicolike.cn

Go:   // 手写 map[string][]T
来源：http://pm.szsharing.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://vx.hnjuh.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fg.panjiajie.cn

[D20] 统计每个元素出现次数
来源：http://oc.jianghongdianzi.cn

Py:   Counter(arr)
来源：http://bd.huanxung.cn

PHP:  array_count_values($arr);
来源：http://vd.colortex.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ah.hahajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://on.newstarts.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pm.wgjwhj.cn

Go:   // 手写 map[T]int
来源：http://jv.jianghongdianzi.cn

Ruby: arr.tally
来源：http://ub.szxytkj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ng.lnxyls.cn

[D21] 判断是否包含某元素
来源：http://at.nszjky.cn

Py:   x in arr
来源：http://qh.huixiangedu.cn

PHP:  in_array($x, $arr, true);
来源：http://rj.9csxet.cn

JS:   arr.includes(x)
来源：http://af.shtwfgs.cn

TS:   arr.includes(x)
来源：http://fh.huanxung.cn

Java: list.contains(x)
来源：http://tp.huanxung.cn

Go:   slices.Contains(arr, x)
来源：http://tb.9csxet.cn

Ruby: arr.include?(x)
来源：http://ln.newstarts.cn

C#:   list.Contains(x)
来源：http://ze.szxytkj.cn

[D22] 复制数组（避免共享引用）
来源：http://fl.haigaiapp.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hx.jianghongdianzi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://uu.szxytkj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://oq.9csxet.cn

TS:   [...arr];
来源：http://xj.yuntaijiaju.cn

Java: new ArrayList<>(list);
来源：http://wn.521024.cn

Go:   copied := append([]int(nil), arr...)
来源：http://tn.szxytkj.cn

Ruby: arr.dup;  arr.clone
来源：http://hl.521024.cn

C#:   new List<int>(list);
来源：http://pl.nszjky.cn

[D23] reduce 累积计算
来源：http://bs.gzmigu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fl.newstarts.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dy.huixinmuqiang.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bf.panjiajie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ao.asd995.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xc.huanxung.cn

Go:   // 手写循环
来源：http://rh.shxzukj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ac.nszjky.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vw.hahajie.cn

[D24] 字典 / Map 基本操作
来源：http://jd.huixiangedu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qr.shtwfgs.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fm.shxzukj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://uq.asd995.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ob.jianghongdianzi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ds.szsharing.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jf.yuexingan06.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rz.panjiajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vy.nicolike.cn

[D25] Set 集合去重与交并差
来源：http://la.huixiangedu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://eu.huanxung.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yj.jctech888.com.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mz.bjjhwx.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gb.huanxung.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ou.hnjuh.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cq.muxihuayi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ne.yuntaijiaju.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xx.shtwfgs.cn

[D26] 数组转字符串
来源：http://kc.yuntaijiaju.cn

Py:   ", ".join(map(str, arr))
来源：http://rh.szxytkj.cn

PHP:  implode(", ", $arr);
来源：http://oq.asd995.cn

JS:   arr.join(", ")
来源：http://nf.colortex.cn

TS:   arr.join(", ")
来源：http://he.szxytkj.cn

Java: String.join(", ", list)
来源：http://vi.muxihuayi.cn

Go:   strings.Join(strs, ", ")
来源：http://ab.yuntaijiaju.cn

Ruby: arr.join(", ")
来源：http://oi.bjjhwx.cn

C#:   string.Join(", ", list)
来源：http://om.muxihuayi.cn

================================================================================
来源：http://ke.shxzskj.cn

E. 字符串处理
来源：http://th.jctech888.com.cn

================================================================================
来源：http://vh.colortex.cn

[E01] 拼接字符串
来源：http://ei.muxihuayi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cg.shxzskj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ml.521024.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dj.huixiangedu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ss.chemitech.net.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mm.hnjuh.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wv.huixiangedu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hv.9csxet.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jf.9csxet.cn

[E02] 重复字符串
来源：http://fx.nszjky.cn

Py:   "ab" * 3
来源：http://is.muxihuayi.cn

PHP:  str_repeat("ab", 3);
来源：http://rf.jianghongdianzi.cn

JS:   "ab".repeat(3)
来源：http://ad.huixinmuqiang.cn

TS:   "ab".repeat(3)
来源：http://sm.shxzskj.cn

Java: "ab".repeat(3)
来源：http://jf.szsharing.cn

Go:   strings.Repeat("ab", 3)
来源：http://hj.521024.cn

Ruby: "ab" * 3
来源：http://ei.huanxung.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mm.szsharing.cn

[E03] 截取子串
来源：http://te.shxzskj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tw.colortex.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hp.nicolike.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://am.jianghongdianzi.cn

TS:   s.slice(1, 4)
来源：http://ok.wgjwhj.cn

Java: s.substring(1, 4)
来源：http://xs.yuexingan06.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gu.huixinmuqiang.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ww.shtwfgs.cn

C#:   s.Substring(1, 3)
来源：http://qz.nszjky.cn

[E04] 查找子串位置
来源：http://lg.nicolike.cn

Py:   s.find("x");  s.index("x")
来源：http://zi.bjjhwx.cn

PHP:  strpos($s, "x");
来源：http://wm.panjiajie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fc.szxytkj.cn

TS:   s.indexOf("x")
来源：http://ao.huixinmuqiang.cn

Java: s.indexOf("x")
来源：http://ym.bjjhwx.cn

Go:   strings.Index(s, "x")
来源：http://hr.yuexingan06.cn

Ruby: s.index("x")
来源：http://nv.shxzskj.cn

C#:   s.IndexOf("x")
来源：http://sc.hnjuh.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gk.newstarts.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fz.wgjwhj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ax.szsharing.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ms.jianghongdianzi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://nq.bookmarksfly.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tg.bookmarksfly.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ei.huixinmuqiang.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pk.lnxyls.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jd.jianghongdianzi.cn

[E06] 替换子串
来源：http://fr.521024.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://eo.gzmigu.cn

PHP:  str_replace("a", "b", $s);
来源：http://tk.shxzukj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://we.huixinmuqiang.cn

TS:   s.replaceAll("a", "b")
来源：http://gg.bookmarksfly.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hb.gzmigu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tb.shtwfgs.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qd.huixiangedu.cn

C#:   s.Replace("a", "b")
来源：http://xd.jianghongdianzi.cn

[E07] 按分隔符拆分
来源：http://rd.9csxet.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://am.jctech888.com.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nt.haigaiapp.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://eu.nszjky.cn

TS:   s.split(",")
来源：http://fi.shxzskj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ic.gzmigu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://la.huixinmuqiang.cn

Ruby: s.split(",");  s.split
来源：http://mb.asd995.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wq.yuntaijiaju.cn

[E08] 数组按分隔符合并
来源：http://qp.panjiajie.cn

Py:   ",".join(items)
来源：http://xk.shxzskj.cn

PHP:  implode(",", $items);
来源：http://xi.bookmarksfly.cn

JS:   items.join(",")
来源：http://hp.muxihuayi.cn

TS:   items.join(",")
来源：http://em.newstarts.cn

Java: String.join(",", items)
来源：http://ij.wgjwhj.cn

Go:   strings.Join(items, ",")
来源：http://ue.haigaiapp.cn

Ruby: items.join(",")
来源：http://re.huixinmuqiang.cn

C#:   string.Join(",", items)
来源：http://zz.jctech888.com.cn

[E09] 去除所有空白字符
来源：http://au.haigaiapp.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ep.newstarts.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://sr.nicolike.cn

JS:   s.replace(/\s+/g, "")
来源：http://wl.hahajie.cn

TS:   s.replace(/\s+/g, "")
来源：http://ua.nszjky.cn

Java: s.replaceAll("\\s+", "")
来源：http://iw.nszjky.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ma.szsharing.cn

Ruby: s.gsub(/\s+/, "")
来源：http://du.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wz.shxzskj.cn

[E10] 左侧补零 / 定长填充
来源：http://ph.shxzskj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zc.huixiangedu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jf.panjiajie.cn

JS:   "7".padStart(3, "0")
来源：http://eq.szsharing.cn

TS:   "7".padStart(3, "0")
来源：http://kq.haigaiapp.cn

Java: String.format("%03d", 7)
来源：http://ha.newstarts.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://pq.asd995.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ei.shxzskj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zd.jianghongdianzi.cn

[E11] 反转字符串
来源：http://qr.muxihuayi.cn

Py:   s[::-1]
来源：http://zw.9csxet.cn

PHP:  strrev($s);
来源：http://dw.jctech888.com.cn

JS:   [...s].reverse().join("")
来源：http://rt.szxytkj.cn

TS:   [...s].reverse().join("")
来源：http://ru.bjjhwx.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://it.9csxet.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zr.wgjwhj.cn

Ruby: s.reverse
来源：http://zs.9csxet.cn

C#:   new string(s.Reverse().ToArray())
来源：http://fo.huixinmuqiang.cn

[E12] 统计某字符出现次数
来源：http://ru.asd995.cn

Py:   s.count("a")
来源：http://yo.yuexingan06.cn

PHP:  substr_count($s, "a");
来源：http://tm.nszjky.cn

JS:   s.split("a").length - 1
来源：http://rz.chemitech.net.cn

TS:   s.split("a").length - 1
来源：http://rx.jctech888.com.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nv.asd995.cn

Go:   strings.Count(s, "a")
来源：http://fw.huixinmuqiang.cn

Ruby: s.count("a")
来源：http://fh.huanxung.cn

C#:   s.Count(c => c == 'a')
来源：http://da.yuntaijiaju.cn

[E13] 逐字符遍历
来源：http://bo.shxzskj.cn

Py:   for ch in s: print(ch)
来源：http://ld.jianghongdianzi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xg.shxzukj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://tx.bookmarksfly.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bc.muxihuayi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://aj.bookmarksfly.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ox.panjiajie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://uj.jianghongdianzi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wn.asd995.cn

[E14] URL 编码与 Base64
来源：http://dt.haigaiapp.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mg.chemitech.net.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://da.hnjuh.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bo.jianghongdianzi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gj.yuntaijiaju.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nt.jctech888.com.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nt.huanxung.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://am.9csxet.cn


<!-- 参考信息 -->