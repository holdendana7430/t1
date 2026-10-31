代发 wailian999

Java: list.size();
来源：http://rh.521024.cn

Go:   len(arr)
来源：http://gq.521024.cn

Ruby: arr.length; arr.size
来源：http://yq.lnxyls.cn

C#:   list.Count;
来源：http://di.jctech888.com.cn

[D07] 切片 / 取子数组
来源：http://sh.jctech888.com.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lf.shxzukj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://to.bjjhwx.cn

JS:   arr.slice(1, 4);
来源：http://eu.bookmarksfly.cn

TS:   arr.slice(1, 4);
来源：http://yf.muxihuayi.cn

Java: list.subList(1, 4);
来源：http://vq.huixinmuqiang.cn

Go:   arr[1:4]
来源：http://ul.lnxyls.cn

Ruby: arr[1, 3]
来源：http://vj.nicolike.cn

C#:   list.GetRange(1, 3);
来源：http://ej.huixinmuqiang.cn

[D08] 合并两个数组
来源：http://pg.nicolike.cn

Py:   a + b;  a.extend(b)
来源：http://xj.lnxyls.cn

PHP:  array_merge($a, $b);
来源：http://kk.panjiajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://dc.huixiangedu.cn

TS:   [...a, ...b];
来源：http://df.jctech888.com.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kt.wgjwhj.cn

Go:   append(a, b...)
来源：http://jr.jianghongdianzi.cn

Ruby: a + b;  a.concat(b)
来源：http://nq.9csxet.cn

C#:   a.Concat(b).ToList()
来源：http://hl.huixiangedu.cn

[D09] 排序（升序）
来源：http://ik.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://be.shxzukj.cn

PHP:  sort($arr);
来源：http://oh.chemitech.net.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ax.jctech888.com.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://op.nszjky.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ag.haigaiapp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wr.chemitech.net.cn

Ruby: arr.sort
来源：http://pz.9csxet.cn

C#:   list.Sort();
来源：http://xr.szsharing.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mw.jianghongdianzi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qq.panjiajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ea.newstarts.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dk.shxzukj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://np.huixiangedu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fw.jianghongdianzi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xm.shxzskj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qj.chemitech.net.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://td.gzmigu.cn

[D11] 反转数组
来源：http://vc.huanxung.cn

Py:   arr[::-1];  arr.reverse()
来源：http://rn.panjiajie.cn

PHP:  array_reverse($arr);
来源：http://pe.szxytkj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kr.hnjuh.cn

TS:   [...arr].reverse();
来源：http://wh.nicolike.cn

Java: Collections.reverse(list);
来源：http://kn.newstarts.cn

Go:   slices.Reverse(arr)
来源：http://ls.chemitech.net.cn

Ruby: arr.reverse
来源：http://zl.shxzskj.cn

C#:   list.Reverse();
来源：http://fx.panjiajie.cn

[D12] 查找元素下标
来源：http://vs.wgjwhj.cn

Py:   arr.index(x);  x in arr
来源：http://dw.bjjhwx.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wd.521024.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uv.huixinmuqiang.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mk.hnjuh.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mf.jctech888.com.cn

Go:   slices.Index(arr, x)
来源：http://pd.yuexingan06.cn

Ruby: arr.index(x)
来源：http://zi.gzmigu.cn

C#:   list.IndexOf(x);
来源：http://iz.shxzskj.cn

[D13] 过滤（保留满足条件的）
来源：http://lw.haigaiapp.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xy.yuexingan06.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rx.yuntaijiaju.cn

JS:   arr.filter(x => x > 3)
来源：http://eh.panjiajie.cn

TS:   arr.filter(x => x > 3)
来源：http://en.lnxyls.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yy.muxihuayi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xv.lnxyls.cn

Ruby: arr.select { |x| x > 3 }
来源：http://zw.521024.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qn.wgjwhj.cn

[D14] 映射转换（每个元素变形）
来源：http://ia.gzmigu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qc.9csxet.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qj.hnjuh.cn

JS:   arr.map(x => x * 2)
来源：http://by.nicolike.cn

TS:   arr.map(x => x * 2)
来源：http://xg.asd995.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://uv.jctech888.com.cn

Go:   // 手写循环
来源：http://sz.szxytkj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hw.shxzukj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ay.asd995.cn

[D15] 去重
来源：http://ji.huanxung.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ul.haigaiapp.cn

PHP:  array_unique($arr);
来源：http://pe.wgjwhj.cn

JS:   [...new Set(arr)]
来源：http://pv.szxytkj.cn

TS:   [...new Set(arr)]
来源：http://qh.shtwfgs.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lx.wgjwhj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xw.muxihuayi.cn

Ruby: arr.uniq
来源：http://by.newstarts.cn

C#:   list.Distinct().ToList()
来源：http://vi.huixiangedu.cn

[D16] 求和与平均值
来源：http://sf.9csxet.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gn.huanxung.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cy.huixinmuqiang.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dp.asd995.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jm.huixinmuqiang.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ua.bjjhwx.cn

Go:   // 手写循环累加
来源：http://ub.9csxet.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://iz.jctech888.com.cn

C#:   list.Sum();  list.Average()
来源：http://pp.huanxung.cn

[D17] 最大值与最小值
来源：http://tl.huanxung.cn

Py:   max(arr);  min(arr)
来源：http://yr.gzmigu.cn

PHP:  max($arr);  min($arr);
来源：http://tl.shxzukj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ym.nszjky.cn

TS:   Math.max(...arr);
来源：http://sl.bookmarksfly.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://dd.wgjwhj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mu.bookmarksfly.cn

Ruby: arr.max;  arr.min
来源：http://cw.shxzskj.cn

C#:   list.Max();  list.Min()
来源：http://tk.shxzskj.cn

[D18] 扁平化嵌套数组
来源：http://on.panjiajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jf.jctech888.com.cn

PHP:  array_merge(...$nested);
来源：http://wh.bookmarksfly.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lb.asd995.cn

TS:   nested.flat();
来源：http://rx.nicolike.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ja.szxytkj.cn

Go:   // 手写双层循环
来源：http://md.colortex.cn

Ruby: nested.flatten
来源：http://jr.huixiangedu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://jz.shxzukj.cn

[D19] 按字段分组
来源：http://ag.lnxyls.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://up.nszjky.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lm.bookmarksfly.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fo.bjjhwx.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ni.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qf.bjjhwx.cn

Go:   // 手写 map[string][]T
来源：http://ps.wgjwhj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ec.9csxet.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cr.hnjuh.cn

[D20] 统计每个元素出现次数
来源：http://ot.szxytkj.cn

Py:   Counter(arr)
来源：http://kq.nicolike.cn

PHP:  array_count_values($arr);
来源：http://kl.shxzukj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ul.nszjky.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hm.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://im.jianghongdianzi.cn

Go:   // 手写 map[T]int
来源：http://kn.bookmarksfly.cn

Ruby: arr.tally
来源：http://ly.bjjhwx.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ty.chemitech.net.cn

[D21] 判断是否包含某元素
来源：http://un.shxzskj.cn

Py:   x in arr
来源：http://aa.yuexingan06.cn

PHP:  in_array($x, $arr, true);
来源：http://zs.szsharing.cn

JS:   arr.includes(x)
来源：http://pn.shxzskj.cn

TS:   arr.includes(x)
来源：http://uz.hnjuh.cn

Java: list.contains(x)
来源：http://qm.nszjky.cn

Go:   slices.Contains(arr, x)
来源：http://qc.521024.cn

Ruby: arr.include?(x)
来源：http://wd.nicolike.cn

C#:   list.Contains(x)
来源：http://ro.nicolike.cn

[D22] 复制数组（避免共享引用）
来源：http://lg.jctech888.com.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qy.huixinmuqiang.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xk.bjjhwx.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cf.szsharing.cn

TS:   [...arr];
来源：http://rk.nicolike.cn

Java: new ArrayList<>(list);
来源：http://oj.wgjwhj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://hu.newstarts.cn

Ruby: arr.dup;  arr.clone
来源：http://pu.shtwfgs.cn

C#:   new List<int>(list);
来源：http://th.nszjky.cn

[D23] reduce 累积计算
来源：http://yq.nicolike.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://in.shtwfgs.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gr.nszjky.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cx.haigaiapp.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lj.jctech888.com.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://or.shxzskj.cn

Go:   // 手写循环
来源：http://lj.gzmigu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ci.nicolike.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xx.nszjky.cn

[D24] 字典 / Map 基本操作
来源：http://pz.huixiangedu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ip.hnjuh.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://at.lnxyls.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fa.huixiangedu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ep.hnjuh.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vw.asd995.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vu.huanxung.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://va.huixinmuqiang.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ae.bookmarksfly.cn

[D25] Set 集合去重与交并差
来源：http://ax.jianghongdianzi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jr.lnxyls.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://db.gzmigu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wv.yuntaijiaju.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tb.huixinmuqiang.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gh.jianghongdianzi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mh.huanxung.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gg.lnxyls.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ge.wgjwhj.cn

[D26] 数组转字符串
来源：http://it.huanxung.cn

Py:   ", ".join(map(str, arr))
来源：http://on.yuntaijiaju.cn

PHP:  implode(", ", $arr);
来源：http://cf.shxzskj.cn

JS:   arr.join(", ")
来源：http://tu.muxihuayi.cn

TS:   arr.join(", ")
来源：http://py.chemitech.net.cn

Java: String.join(", ", list)
来源：http://ur.colortex.cn

Go:   strings.Join(strs, ", ")
来源：http://xi.bjjhwx.cn

Ruby: arr.join(", ")
来源：http://gh.panjiajie.cn

C#:   string.Join(", ", list)
来源：http://fy.newstarts.cn

================================================================================
来源：http://go.chemitech.net.cn

E. 字符串处理
来源：http://cg.bjjhwx.cn

================================================================================
来源：http://jz.521024.cn

[E01] 拼接字符串
来源：http://st.nicolike.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bx.jctech888.com.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tz.shxzukj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ui.jctech888.com.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kz.huanxung.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ah.szxytkj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lz.jianghongdianzi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ty.huixinmuqiang.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dp.bjjhwx.cn

[E02] 重复字符串
来源：http://ns.bjjhwx.cn

Py:   "ab" * 3
来源：http://be.huixinmuqiang.cn

PHP:  str_repeat("ab", 3);
来源：http://ys.huanxung.cn

JS:   "ab".repeat(3)
来源：http://dt.colortex.cn

TS:   "ab".repeat(3)
来源：http://ri.shxzskj.cn

Java: "ab".repeat(3)
来源：http://yr.nicolike.cn

Go:   strings.Repeat("ab", 3)
来源：http://bf.yuntaijiaju.cn

Ruby: "ab" * 3
来源：http://jx.shtwfgs.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wx.colortex.cn

[E03] 截取子串
来源：http://zw.9csxet.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ms.gzmigu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jl.huixinmuqiang.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ji.szsharing.cn

TS:   s.slice(1, 4)
来源：http://kz.shtwfgs.cn

Java: s.substring(1, 4)
来源：http://kx.muxihuayi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cv.jianghongdianzi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zq.asd995.cn

C#:   s.Substring(1, 3)
来源：http://wo.yuexingan06.cn

[E04] 查找子串位置
来源：http://rg.muxihuayi.cn

Py:   s.find("x");  s.index("x")
来源：http://ne.panjiajie.cn

PHP:  strpos($s, "x");
来源：http://ew.newstarts.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://aa.nicolike.cn

TS:   s.indexOf("x")
来源：http://jj.bookmarksfly.cn

Java: s.indexOf("x")
来源：http://fz.szsharing.cn

Go:   strings.Index(s, "x")
来源：http://nc.9csxet.cn

Ruby: s.index("x")
来源：http://mq.szxytkj.cn

C#:   s.IndexOf("x")
来源：http://iy.hahajie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ws.gzmigu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qx.shxzukj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ib.nicolike.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lv.shxzukj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://wu.nszjky.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mz.newstarts.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hc.bjjhwx.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kg.haigaiapp.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yl.nicolike.cn

[E06] 替换子串
来源：http://tg.lnxyls.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vq.yuexingan06.cn

PHP:  str_replace("a", "b", $s);
来源：http://ey.chemitech.net.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eo.newstarts.cn

TS:   s.replaceAll("a", "b")
来源：http://iy.nszjky.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wu.jctech888.com.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bg.huixinmuqiang.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://om.panjiajie.cn

C#:   s.Replace("a", "b")
来源：http://db.9csxet.cn

[E07] 按分隔符拆分
来源：http://cd.jctech888.com.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tt.hahajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yu.muxihuayi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ne.bookmarksfly.cn

TS:   s.split(",")
来源：http://bw.chemitech.net.cn

Java: s.split(",");  s.split("\\s+")
来源：http://tg.hahajie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lb.yuntaijiaju.cn

Ruby: s.split(",");  s.split
来源：http://bn.haigaiapp.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://eb.panjiajie.cn

[E08] 数组按分隔符合并
来源：http://zd.yuntaijiaju.cn

Py:   ",".join(items)
来源：http://pw.yuntaijiaju.cn

PHP:  implode(",", $items);
来源：http://jd.bjjhwx.cn

JS:   items.join(",")
来源：http://dw.yuexingan06.cn

TS:   items.join(",")
来源：http://rg.shxzukj.cn

Java: String.join(",", items)
来源：http://ci.nicolike.cn

Go:   strings.Join(items, ",")
来源：http://li.nszjky.cn

Ruby: items.join(",")
来源：http://ks.shxzukj.cn

C#:   string.Join(",", items)
来源：http://fn.huixinmuqiang.cn

[E09] 去除所有空白字符
来源：http://vo.chemitech.net.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kr.shtwfgs.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://sf.colortex.cn

JS:   s.replace(/\s+/g, "")
来源：http://sg.lnxyls.cn

TS:   s.replace(/\s+/g, "")
来源：http://gs.panjiajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://ch.szxytkj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://cb.jctech888.com.cn

Ruby: s.gsub(/\s+/, "")
来源：http://vi.hahajie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gz.panjiajie.cn

[E10] 左侧补零 / 定长填充
来源：http://hc.szxytkj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ot.wgjwhj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dk.bjjhwx.cn

JS:   "7".padStart(3, "0")
来源：http://te.haigaiapp.cn

TS:   "7".padStart(3, "0")
来源：http://vz.huanxung.cn

Java: String.format("%03d", 7)
来源：http://fv.521024.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://sg.haigaiapp.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zg.szxytkj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://um.lnxyls.cn

[E11] 反转字符串
来源：http://iv.gzmigu.cn

Py:   s[::-1]
来源：http://zj.gzmigu.cn

PHP:  strrev($s);
来源：http://jq.asd995.cn

JS:   [...s].reverse().join("")
来源：http://ug.chemitech.net.cn

TS:   [...s].reverse().join("")
来源：http://hi.hnjuh.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://cr.521024.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://dw.9csxet.cn

Ruby: s.reverse
来源：http://pp.huanxung.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ht.shxzukj.cn

[E12] 统计某字符出现次数
来源：http://ld.shxzskj.cn

Py:   s.count("a")
来源：http://ge.asd995.cn

PHP:  substr_count($s, "a");
来源：http://tt.bjjhwx.cn

JS:   s.split("a").length - 1
来源：http://wd.huixinmuqiang.cn

TS:   s.split("a").length - 1
来源：http://of.nszjky.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bh.bookmarksfly.cn

Go:   strings.Count(s, "a")
来源：http://wg.hnjuh.cn

Ruby: s.count("a")
来源：http://iu.szxytkj.cn

C#:   s.Count(c => c == 'a')
来源：http://en.jctech888.com.cn

[E13] 逐字符遍历
来源：http://ny.shxzukj.cn

Py:   for ch in s: print(ch)
来源：http://mp.wgjwhj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cb.newstarts.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://cr.muxihuayi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://dw.chemitech.net.cn


<!-- 参考信息 -->