代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://zd.szsharing.cn

C#:   a.Concat(b).ToList()
来源：http://js.yuntaijiaju.cn

[D09] 排序（升序）
来源：http://qc.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://xj.panjiajie.cn

PHP:  sort($arr);
来源：http://hw.bookmarksfly.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tx.szsharing.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://om.colortex.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://li.nszjky.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zm.newstarts.cn

Ruby: arr.sort
来源：http://jn.hnjuh.cn

C#:   list.Sort();
来源：http://kl.haigaiapp.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ps.asd995.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lb.panjiajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lg.szsharing.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dd.521024.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://np.hnjuh.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hj.521024.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mc.jianghongdianzi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kz.hahajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wd.colortex.cn

[D11] 反转数组
来源：http://yi.shxzukj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://jq.jianghongdianzi.cn

PHP:  array_reverse($arr);
来源：http://dv.haigaiapp.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nw.bjjhwx.cn

TS:   [...arr].reverse();
来源：http://zp.szxytkj.cn

Java: Collections.reverse(list);
来源：http://rr.lnxyls.cn

Go:   slices.Reverse(arr)
来源：http://dl.hnjuh.cn

Ruby: arr.reverse
来源：http://eh.521024.cn

C#:   list.Reverse();
来源：http://fd.yuntaijiaju.cn

[D12] 查找元素下标
来源：http://xy.nszjky.cn

Py:   arr.index(x);  x in arr
来源：http://rk.shtwfgs.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vq.newstarts.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rk.hahajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ok.521024.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gd.bjjhwx.cn

Go:   slices.Index(arr, x)
来源：http://qm.szsharing.cn

Ruby: arr.index(x)
来源：http://ez.shxzukj.cn

C#:   list.IndexOf(x);
来源：http://ia.szsharing.cn

[D13] 过滤（保留满足条件的）
来源：http://oq.muxihuayi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mb.szsharing.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ki.yuntaijiaju.cn

JS:   arr.filter(x => x > 3)
来源：http://pi.shxzskj.cn

TS:   arr.filter(x => x > 3)
来源：http://en.nszjky.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ke.wgjwhj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dg.muxihuayi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://pa.yuntaijiaju.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qg.szxytkj.cn

[D14] 映射转换（每个元素变形）
来源：http://mc.jctech888.com.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nx.muxihuayi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dc.521024.cn

JS:   arr.map(x => x * 2)
来源：http://ta.jctech888.com.cn

TS:   arr.map(x => x * 2)
来源：http://mz.hnjuh.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://jg.muxihuayi.cn

Go:   // 手写循环
来源：http://lt.huixiangedu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://xr.9csxet.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://wj.szsharing.cn

[D15] 去重
来源：http://bt.chemitech.net.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pz.haigaiapp.cn

PHP:  array_unique($arr);
来源：http://wi.nicolike.cn

JS:   [...new Set(arr)]
来源：http://ko.shtwfgs.cn

TS:   [...new Set(arr)]
来源：http://rw.9csxet.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ga.shxzukj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://gg.yuntaijiaju.cn

Ruby: arr.uniq
来源：http://en.panjiajie.cn

C#:   list.Distinct().ToList()
来源：http://bx.panjiajie.cn

[D16] 求和与平均值
来源：http://qr.jctech888.com.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wi.shxzukj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://td.szsharing.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://iu.huixinmuqiang.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://iv.9csxet.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wd.haigaiapp.cn

Go:   // 手写循环累加
来源：http://rc.yuexingan06.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ds.huanxung.cn

C#:   list.Sum();  list.Average()
来源：http://yv.bjjhwx.cn

[D17] 最大值与最小值
来源：http://dy.yuntaijiaju.cn

Py:   max(arr);  min(arr)
来源：http://ir.nicolike.cn

PHP:  max($arr);  min($arr);
来源：http://ko.huixinmuqiang.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ie.521024.cn

TS:   Math.max(...arr);
来源：http://jm.asd995.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://dj.wgjwhj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tm.gzmigu.cn

Ruby: arr.max;  arr.min
来源：http://ho.colortex.cn

C#:   list.Max();  list.Min()
来源：http://fp.yuntaijiaju.cn

[D18] 扁平化嵌套数组
来源：http://yn.huixiangedu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hl.lnxyls.cn

PHP:  array_merge(...$nested);
来源：http://ky.lnxyls.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xi.huixiangedu.cn

TS:   nested.flat();
来源：http://go.9csxet.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ww.haigaiapp.cn

Go:   // 手写双层循环
来源：http://so.bjjhwx.cn

Ruby: nested.flatten
来源：http://or.nszjky.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ys.haigaiapp.cn

[D19] 按字段分组
来源：http://bc.shxzskj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lr.jctech888.com.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zn.521024.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yq.9csxet.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://uf.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ob.gzmigu.cn

Go:   // 手写 map[string][]T
来源：http://in.yuexingan06.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fz.shtwfgs.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dp.shxzukj.cn

[D20] 统计每个元素出现次数
来源：http://hy.bookmarksfly.cn

Py:   Counter(arr)
来源：http://xy.gzmigu.cn

PHP:  array_count_values($arr);
来源：http://oh.shtwfgs.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yl.yuexingan06.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rg.wgjwhj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ll.lnxyls.cn

Go:   // 手写 map[T]int
来源：http://yr.shxzukj.cn

Ruby: arr.tally
来源：http://wp.szsharing.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wx.jianghongdianzi.cn

[D21] 判断是否包含某元素
来源：http://wm.wgjwhj.cn

Py:   x in arr
来源：http://gg.muxihuayi.cn

PHP:  in_array($x, $arr, true);
来源：http://jz.wgjwhj.cn

JS:   arr.includes(x)
来源：http://zz.asd995.cn

TS:   arr.includes(x)
来源：http://fg.yuntaijiaju.cn

Java: list.contains(x)
来源：http://uh.shxzukj.cn

Go:   slices.Contains(arr, x)
来源：http://sg.yuntaijiaju.cn

Ruby: arr.include?(x)
来源：http://xi.nicolike.cn

C#:   list.Contains(x)
来源：http://wx.nszjky.cn

[D22] 复制数组（避免共享引用）
来源：http://ax.jianghongdianzi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xl.szsharing.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vf.huixinmuqiang.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yk.huanxung.cn

TS:   [...arr];
来源：http://fv.shxzukj.cn

Java: new ArrayList<>(list);
来源：http://lc.huixinmuqiang.cn

Go:   copied := append([]int(nil), arr...)
来源：http://zi.huixinmuqiang.cn

Ruby: arr.dup;  arr.clone
来源：http://bu.huixiangedu.cn

C#:   new List<int>(list);
来源：http://pt.wgjwhj.cn

[D23] reduce 累积计算
来源：http://zm.bjjhwx.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ak.nszjky.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wc.asd995.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xv.gzmigu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tf.jianghongdianzi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qj.shtwfgs.cn

Go:   // 手写循环
来源：http://lu.jctech888.com.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tz.shxzskj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://me.bookmarksfly.cn

[D24] 字典 / Map 基本操作
来源：http://fl.jctech888.com.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://az.panjiajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://so.shxzukj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://eo.szxytkj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zn.shtwfgs.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wr.bjjhwx.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zw.newstarts.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bo.yuntaijiaju.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xh.lnxyls.cn

[D25] Set 集合去重与交并差
来源：http://fv.shtwfgs.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pf.hahajie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ty.huanxung.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fw.wgjwhj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bz.huixinmuqiang.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fg.panjiajie.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ls.lnxyls.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ob.szxytkj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fn.nicolike.cn

[D26] 数组转字符串
来源：http://ii.yuexingan06.cn

Py:   ", ".join(map(str, arr))
来源：http://iw.lnxyls.cn

PHP:  implode(", ", $arr);
来源：http://zy.gzmigu.cn

JS:   arr.join(", ")
来源：http://eb.nicolike.cn

TS:   arr.join(", ")
来源：http://ql.haigaiapp.cn

Java: String.join(", ", list)
来源：http://cr.shtwfgs.cn

Go:   strings.Join(strs, ", ")
来源：http://nn.panjiajie.cn

Ruby: arr.join(", ")
来源：http://il.huanxung.cn

C#:   string.Join(", ", list)
来源：http://ss.muxihuayi.cn

================================================================================
来源：http://or.huixinmuqiang.cn

E. 字符串处理
来源：http://lq.shtwfgs.cn

================================================================================
来源：http://zu.huanxung.cn

[E01] 拼接字符串
来源：http://de.asd995.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jr.bookmarksfly.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sz.panjiajie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zl.bjjhwx.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://az.lnxyls.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hx.chemitech.net.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bp.muxihuayi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://om.jctech888.com.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hh.szxytkj.cn

[E02] 重复字符串
来源：http://af.huixinmuqiang.cn

Py:   "ab" * 3
来源：http://mu.panjiajie.cn

PHP:  str_repeat("ab", 3);
来源：http://ok.9csxet.cn

JS:   "ab".repeat(3)
来源：http://mn.521024.cn

TS:   "ab".repeat(3)
来源：http://tp.haigaiapp.cn

Java: "ab".repeat(3)
来源：http://sm.shxzukj.cn

Go:   strings.Repeat("ab", 3)
来源：http://nr.yuexingan06.cn

Ruby: "ab" * 3
来源：http://xz.huixiangedu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fk.panjiajie.cn

[E03] 截取子串
来源：http://vx.colortex.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ht.nicolike.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ob.gzmigu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dy.huixinmuqiang.cn

TS:   s.slice(1, 4)
来源：http://cp.yuexingan06.cn

Java: s.substring(1, 4)
来源：http://wa.jianghongdianzi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://am.jianghongdianzi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://az.huanxung.cn

C#:   s.Substring(1, 3)
来源：http://ox.szxytkj.cn

[E04] 查找子串位置
来源：http://uq.shtwfgs.cn

Py:   s.find("x");  s.index("x")
来源：http://wl.panjiajie.cn

PHP:  strpos($s, "x");
来源：http://cn.wgjwhj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gn.szxytkj.cn

TS:   s.indexOf("x")
来源：http://it.wgjwhj.cn

Java: s.indexOf("x")
来源：http://wa.panjiajie.cn

Go:   strings.Index(s, "x")
来源：http://up.wgjwhj.cn

Ruby: s.index("x")
来源：http://jr.bookmarksfly.cn

C#:   s.IndexOf("x")
来源：http://qc.jianghongdianzi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://vu.huixiangedu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uq.huanxung.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hp.huixiangedu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nq.huanxung.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://sw.9csxet.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://co.asd995.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vt.chemitech.net.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gl.lnxyls.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://at.hahajie.cn

[E06] 替换子串
来源：http://bm.lnxyls.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://og.9csxet.cn

PHP:  str_replace("a", "b", $s);
来源：http://ts.huixiangedu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://co.huixinmuqiang.cn

TS:   s.replaceAll("a", "b")
来源：http://zw.haigaiapp.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bu.wgjwhj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ky.szxytkj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bq.hahajie.cn

C#:   s.Replace("a", "b")
来源：http://ac.lnxyls.cn

[E07] 按分隔符拆分
来源：http://qi.szsharing.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ya.jctech888.com.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vj.muxihuayi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://hq.panjiajie.cn

TS:   s.split(",")
来源：http://vh.yuntaijiaju.cn

Java: s.split(",");  s.split("\\s+")
来源：http://sk.wgjwhj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ho.asd995.cn

Ruby: s.split(",");  s.split
来源：http://ou.shtwfgs.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lw.hnjuh.cn

[E08] 数组按分隔符合并
来源：http://js.haigaiapp.cn

Py:   ",".join(items)
来源：http://wk.yuexingan06.cn

PHP:  implode(",", $items);
来源：http://nc.9csxet.cn

JS:   items.join(",")
来源：http://iv.nicolike.cn

TS:   items.join(",")
来源：http://pz.muxihuayi.cn

Java: String.join(",", items)
来源：http://jd.szxytkj.cn

Go:   strings.Join(items, ",")
来源：http://fb.jctech888.com.cn

Ruby: items.join(",")
来源：http://ra.nszjky.cn

C#:   string.Join(",", items)
来源：http://dv.chemitech.net.cn

[E09] 去除所有空白字符
来源：http://qt.521024.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qm.wgjwhj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ij.newstarts.cn

JS:   s.replace(/\s+/g, "")
来源：http://gz.hahajie.cn

TS:   s.replace(/\s+/g, "")
来源：http://ln.521024.cn

Java: s.replaceAll("\\s+", "")
来源：http://xz.9csxet.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://wx.wgjwhj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://im.asd995.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pg.muxihuayi.cn

[E10] 左侧补零 / 定长填充
来源：http://la.asd995.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://au.yuexingan06.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xh.hnjuh.cn

JS:   "7".padStart(3, "0")
来源：http://xn.szxytkj.cn

TS:   "7".padStart(3, "0")
来源：http://mm.shxzskj.cn

Java: String.format("%03d", 7)
来源：http://da.9csxet.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://bb.hnjuh.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hf.szsharing.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ve.lnxyls.cn

[E11] 反转字符串
来源：http://je.huixinmuqiang.cn

Py:   s[::-1]
来源：http://fl.gzmigu.cn

PHP:  strrev($s);
来源：http://wc.bjjhwx.cn

JS:   [...s].reverse().join("")
来源：http://iw.hnjuh.cn

TS:   [...s].reverse().join("")
来源：http://al.panjiajie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ap.bjjhwx.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://wc.huixinmuqiang.cn

Ruby: s.reverse
来源：http://zm.colortex.cn

C#:   new string(s.Reverse().ToArray())
来源：http://sm.haigaiapp.cn

[E12] 统计某字符出现次数
来源：http://vy.huanxung.cn

Py:   s.count("a")
来源：http://aa.szxytkj.cn

PHP:  substr_count($s, "a");
来源：http://hw.huanxung.cn

JS:   s.split("a").length - 1
来源：http://fn.jctech888.com.cn

TS:   s.split("a").length - 1
来源：http://wb.asd995.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ui.9csxet.cn

Go:   strings.Count(s, "a")
来源：http://mz.jianghongdianzi.cn

Ruby: s.count("a")
来源：http://kc.szxytkj.cn

C#:   s.Count(c => c == 'a')
来源：http://pq.wgjwhj.cn

[E13] 逐字符遍历
来源：http://ma.huanxung.cn

Py:   for ch in s: print(ch)
来源：http://zi.colortex.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zc.szxytkj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://zg.shtwfgs.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qo.hnjuh.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ik.szxytkj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lb.jianghongdianzi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://lx.szsharing.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://di.chemitech.net.cn

[E14] URL 编码与 Base64
来源：http://wj.huixiangedu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://of.huixiangedu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://nk.huanxung.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://or.hnjuh.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://iv.huanxung.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rm.jianghongdianzi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lg.wgjwhj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xv.hnjuh.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xp.newstarts.cn

[E15] HTML 转义 / 反转义
来源：http://lx.huanxung.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://qj.shxzukj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://aq.lnxyls.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xm.hnjuh.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ht.panjiajie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://iw.bookmarksfly.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://et.huixiangedu.cn


<!-- 参考信息 -->