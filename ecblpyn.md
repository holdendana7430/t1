代发 wailian999

PHP:  sort($arr);
来源：http://hd.bookmarksfly.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jy.shtwfgs.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://yz.jianghongdianzi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://dp.nicolike.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mp.jianghongdianzi.cn

Ruby: arr.sort
来源：http://jx.bookmarksfly.cn

C#:   list.Sort();
来源：http://ff.shxzskj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://xo.huixiangedu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qs.newstarts.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yc.newstarts.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gr.asd995.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ie.bookmarksfly.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://aw.huanxung.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cr.wgjwhj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://oc.yuexingan06.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pu.hnjuh.cn

[D11] 反转数组
来源：http://jt.shxzukj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ws.nicolike.cn

PHP:  array_reverse($arr);
来源：http://mi.asd995.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tj.szxytkj.cn

TS:   [...arr].reverse();
来源：http://fg.huanxung.cn

Java: Collections.reverse(list);
来源：http://gi.haigaiapp.cn

Go:   slices.Reverse(arr)
来源：http://ee.jctech888.com.cn

Ruby: arr.reverse
来源：http://kb.jctech888.com.cn

C#:   list.Reverse();
来源：http://rc.newstarts.cn

[D12] 查找元素下标
来源：http://ob.521024.cn

Py:   arr.index(x);  x in arr
来源：http://dg.shtwfgs.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ad.panjiajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gp.chemitech.net.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iu.wgjwhj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bw.hahajie.cn

Go:   slices.Index(arr, x)
来源：http://oe.shxzskj.cn

Ruby: arr.index(x)
来源：http://yc.nszjky.cn

C#:   list.IndexOf(x);
来源：http://lk.panjiajie.cn

[D13] 过滤（保留满足条件的）
来源：http://lk.shxzukj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vq.haigaiapp.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://co.shtwfgs.cn

JS:   arr.filter(x => x > 3)
来源：http://ov.yuexingan06.cn

TS:   arr.filter(x => x > 3)
来源：http://bo.huixinmuqiang.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ed.huanxung.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xo.jctech888.com.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xh.shxzskj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://no.hahajie.cn

[D14] 映射转换（每个元素变形）
来源：http://dh.9csxet.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://us.shtwfgs.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lb.gzmigu.cn

JS:   arr.map(x => x * 2)
来源：http://li.hnjuh.cn

TS:   arr.map(x => x * 2)
来源：http://cx.huixiangedu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ap.521024.cn

Go:   // 手写循环
来源：http://ev.bjjhwx.cn

Ruby: arr.map { |x| x * 2 }
来源：http://gc.shxzskj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ih.bookmarksfly.cn

[D15] 去重
来源：http://ye.panjiajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qv.muxihuayi.cn

PHP:  array_unique($arr);
来源：http://ba.nicolike.cn

JS:   [...new Set(arr)]
来源：http://pg.shxzskj.cn

TS:   [...new Set(arr)]
来源：http://je.shxzukj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ex.szxytkj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://qc.jianghongdianzi.cn

Ruby: arr.uniq
来源：http://fd.jctech888.com.cn

C#:   list.Distinct().ToList()
来源：http://jt.yuntaijiaju.cn

[D16] 求和与平均值
来源：http://jy.nicolike.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qd.nszjky.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://li.nicolike.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rp.hahajie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xy.szxytkj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kd.nicolike.cn

Go:   // 手写循环累加
来源：http://pl.szxytkj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cj.szsharing.cn

C#:   list.Sum();  list.Average()
来源：http://ek.yuntaijiaju.cn

[D17] 最大值与最小值
来源：http://rx.huanxung.cn

Py:   max(arr);  min(arr)
来源：http://op.bjjhwx.cn

PHP:  max($arr);  min($arr);
来源：http://mz.bjjhwx.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mh.chemitech.net.cn

TS:   Math.max(...arr);
来源：http://qk.colortex.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://tk.szxytkj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pn.nszjky.cn

Ruby: arr.max;  arr.min
来源：http://ch.hahajie.cn

C#:   list.Max();  list.Min()
来源：http://eu.haigaiapp.cn

[D18] 扁平化嵌套数组
来源：http://ha.huanxung.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jj.asd995.cn

PHP:  array_merge(...$nested);
来源：http://wt.muxihuayi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xj.bjjhwx.cn

TS:   nested.flat();
来源：http://cw.huixiangedu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://er.shxzukj.cn

Go:   // 手写双层循环
来源：http://ko.jctech888.com.cn

Ruby: nested.flatten
来源：http://gn.521024.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://gz.yuntaijiaju.cn

[D19] 按字段分组
来源：http://yj.hnjuh.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tv.jctech888.com.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nq.hnjuh.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wi.shxzskj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ju.szsharing.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://av.panjiajie.cn

Go:   // 手写 map[string][]T
来源：http://rg.bookmarksfly.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://hf.newstarts.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wi.shxzukj.cn

[D20] 统计每个元素出现次数
来源：http://kh.nicolike.cn

Py:   Counter(arr)
来源：http://ip.shxzskj.cn

PHP:  array_count_values($arr);
来源：http://zf.shtwfgs.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://md.shtwfgs.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zj.521024.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fl.huanxung.cn

Go:   // 手写 map[T]int
来源：http://uk.haigaiapp.cn

Ruby: arr.tally
来源：http://up.nszjky.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://io.newstarts.cn

[D21] 判断是否包含某元素
来源：http://jl.huanxung.cn

Py:   x in arr
来源：http://gq.huanxung.cn

PHP:  in_array($x, $arr, true);
来源：http://fx.hnjuh.cn

JS:   arr.includes(x)
来源：http://yw.wgjwhj.cn

TS:   arr.includes(x)
来源：http://xx.asd995.cn

Java: list.contains(x)
来源：http://cj.hahajie.cn

Go:   slices.Contains(arr, x)
来源：http://hc.lnxyls.cn

Ruby: arr.include?(x)
来源：http://yt.gzmigu.cn

C#:   list.Contains(x)
来源：http://wi.bjjhwx.cn

[D22] 复制数组（避免共享引用）
来源：http://eu.shxzskj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gb.newstarts.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qm.shxzukj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ws.bjjhwx.cn

TS:   [...arr];
来源：http://ef.huanxung.cn

Java: new ArrayList<>(list);
来源：http://xn.huanxung.cn

Go:   copied := append([]int(nil), arr...)
来源：http://vv.newstarts.cn

Ruby: arr.dup;  arr.clone
来源：http://yd.521024.cn

C#:   new List<int>(list);
来源：http://wd.szxytkj.cn

[D23] reduce 累积计算
来源：http://gq.chemitech.net.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://du.lnxyls.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ze.bookmarksfly.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bg.newstarts.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rj.shxzukj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://jg.asd995.cn

Go:   // 手写循环
来源：http://po.bookmarksfly.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://do.huanxung.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bs.hahajie.cn

[D24] 字典 / Map 基本操作
来源：http://ux.wgjwhj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://oj.huixinmuqiang.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tl.lnxyls.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hi.9csxet.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ce.hnjuh.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yl.huixiangedu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xq.nicolike.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ef.yuexingan06.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ax.haigaiapp.cn

[D25] Set 集合去重与交并差
来源：http://th.yuexingan06.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fu.shxzukj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ea.yuntaijiaju.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fa.shtwfgs.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nl.huixiangedu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ih.huixiangedu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ac.9csxet.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://is.colortex.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://td.gzmigu.cn

[D26] 数组转字符串
来源：http://cz.chemitech.net.cn

Py:   ", ".join(map(str, arr))
来源：http://gh.521024.cn

PHP:  implode(", ", $arr);
来源：http://lo.huixiangedu.cn

JS:   arr.join(", ")
来源：http://fq.szxytkj.cn

TS:   arr.join(", ")
来源：http://cd.muxihuayi.cn

Java: String.join(", ", list)
来源：http://sh.szxytkj.cn

Go:   strings.Join(strs, ", ")
来源：http://jk.nicolike.cn

Ruby: arr.join(", ")
来源：http://ei.nicolike.cn

C#:   string.Join(", ", list)
来源：http://gx.lnxyls.cn

================================================================================
来源：http://bl.muxihuayi.cn

E. 字符串处理
来源：http://sn.chemitech.net.cn

================================================================================
来源：http://gn.jianghongdianzi.cn

[E01] 拼接字符串
来源：http://fc.lnxyls.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fy.colortex.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nq.shxzskj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://on.9csxet.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cs.haigaiapp.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hj.huixiangedu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://va.hnjuh.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yy.yuntaijiaju.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sd.hnjuh.cn

[E02] 重复字符串
来源：http://vs.bookmarksfly.cn

Py:   "ab" * 3
来源：http://mn.huixinmuqiang.cn

PHP:  str_repeat("ab", 3);
来源：http://gf.huixiangedu.cn

JS:   "ab".repeat(3)
来源：http://ft.hnjuh.cn

TS:   "ab".repeat(3)
来源：http://uc.szsharing.cn

Java: "ab".repeat(3)
来源：http://hw.shtwfgs.cn

Go:   strings.Repeat("ab", 3)
来源：http://gx.huixiangedu.cn

Ruby: "ab" * 3
来源：http://lc.jianghongdianzi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ds.yuexingan06.cn

[E03] 截取子串
来源：http://jv.bookmarksfly.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ug.gzmigu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wf.521024.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://os.yuexingan06.cn

TS:   s.slice(1, 4)
来源：http://zf.521024.cn

Java: s.substring(1, 4)
来源：http://ki.shxzukj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://od.chemitech.net.cn

Ruby: s[1, 3];  s[1..3]
来源：http://pg.muxihuayi.cn

C#:   s.Substring(1, 3)
来源：http://fw.hnjuh.cn

[E04] 查找子串位置
来源：http://cc.gzmigu.cn

Py:   s.find("x");  s.index("x")
来源：http://yn.huixinmuqiang.cn

PHP:  strpos($s, "x");
来源：http://yu.9csxet.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nq.jctech888.com.cn

TS:   s.indexOf("x")
来源：http://qv.huanxung.cn

Java: s.indexOf("x")
来源：http://xk.shxzskj.cn

Go:   strings.Index(s, "x")
来源：http://np.chemitech.net.cn

Ruby: s.index("x")
来源：http://ke.wgjwhj.cn

C#:   s.IndexOf("x")
来源：http://sh.gzmigu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://st.shxzskj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ix.gzmigu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vu.521024.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ui.hnjuh.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://vp.panjiajie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yf.wgjwhj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cb.hahajie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nn.colortex.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fk.szxytkj.cn

[E06] 替换子串
来源：http://rk.yuntaijiaju.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bs.gzmigu.cn

PHP:  str_replace("a", "b", $s);
来源：http://ov.bookmarksfly.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ks.huanxung.cn

TS:   s.replaceAll("a", "b")
来源：http://ly.newstarts.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yy.bjjhwx.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nm.shtwfgs.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://af.shxzskj.cn

C#:   s.Replace("a", "b")
来源：http://dl.szxytkj.cn

[E07] 按分隔符拆分
来源：http://kq.bjjhwx.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qm.hahajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zv.huanxung.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ww.huanxung.cn

TS:   s.split(",")
来源：http://nz.shxzskj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://aw.wgjwhj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bw.szxytkj.cn

Ruby: s.split(",");  s.split
来源：http://wj.shxzskj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rt.shtwfgs.cn

[E08] 数组按分隔符合并
来源：http://vw.9csxet.cn

Py:   ",".join(items)
来源：http://zy.jianghongdianzi.cn

PHP:  implode(",", $items);
来源：http://wg.huanxung.cn

JS:   items.join(",")
来源：http://tl.szxytkj.cn

TS:   items.join(",")
来源：http://kf.shxzukj.cn

Java: String.join(",", items)
来源：http://uf.lnxyls.cn

Go:   strings.Join(items, ",")
来源：http://hf.shxzskj.cn

Ruby: items.join(",")
来源：http://vo.jianghongdianzi.cn

C#:   string.Join(",", items)
来源：http://sw.shxzukj.cn

[E09] 去除所有空白字符
来源：http://qg.huixiangedu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fo.huixiangedu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kf.wgjwhj.cn

JS:   s.replace(/\s+/g, "")
来源：http://zr.huixiangedu.cn

TS:   s.replace(/\s+/g, "")
来源：http://wu.panjiajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://vw.szsharing.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://iq.shxzukj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://hh.muxihuayi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ne.9csxet.cn

[E10] 左侧补零 / 定长填充
来源：http://kn.hnjuh.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bf.bjjhwx.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nb.huanxung.cn

JS:   "7".padStart(3, "0")
来源：http://wc.nicolike.cn

TS:   "7".padStart(3, "0")
来源：http://uo.jctech888.com.cn

Java: String.format("%03d", 7)
来源：http://fq.chemitech.net.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://vv.newstarts.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sa.szsharing.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hk.szsharing.cn

[E11] 反转字符串
来源：http://zs.shxzukj.cn

Py:   s[::-1]
来源：http://tx.huixiangedu.cn

PHP:  strrev($s);
来源：http://to.521024.cn

JS:   [...s].reverse().join("")
来源：http://jv.bookmarksfly.cn

TS:   [...s].reverse().join("")
来源：http://wa.lnxyls.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://xp.jianghongdianzi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://li.haigaiapp.cn

Ruby: s.reverse
来源：http://hg.hnjuh.cn

C#:   new string(s.Reverse().ToArray())
来源：http://fr.shtwfgs.cn

[E12] 统计某字符出现次数
来源：http://ce.jianghongdianzi.cn

Py:   s.count("a")
来源：http://dk.haigaiapp.cn

PHP:  substr_count($s, "a");
来源：http://hi.shtwfgs.cn

JS:   s.split("a").length - 1
来源：http://mq.jianghongdianzi.cn

TS:   s.split("a").length - 1
来源：http://vy.shxzukj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ow.shxzskj.cn

Go:   strings.Count(s, "a")
来源：http://et.hahajie.cn

Ruby: s.count("a")
来源：http://gd.chemitech.net.cn

C#:   s.Count(c => c == 'a')
来源：http://qi.hnjuh.cn

[E13] 逐字符遍历
来源：http://nc.nszjky.cn

Py:   for ch in s: print(ch)
来源：http://hp.lnxyls.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://je.huixinmuqiang.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://va.huanxung.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://us.jianghongdianzi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dx.huanxung.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zw.shtwfgs.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://dk.huixiangedu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bp.huixinmuqiang.cn

[E14] URL 编码与 Base64
来源：http://mx.521024.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://td.521024.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://or.chemitech.net.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gb.521024.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jx.gzmigu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mr.nszjky.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gm.panjiajie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pe.yuexingan06.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hw.shtwfgs.cn

[E15] HTML 转义 / 反转义
来源：http://rd.jctech888.com.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://mz.shxzukj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cx.bjjhwx.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://on.chemitech.net.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://un.wgjwhj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bn.panjiajie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://oo.lnxyls.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vh.asd995.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ih.yuexingan06.cn

[E16] 数字千分位
来源：http://fk.yuntaijiaju.cn

Py:   f"{1234567:,}"
来源：http://fj.hahajie.cn


<!-- 参考信息 -->