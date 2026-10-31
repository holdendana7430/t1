代发 wailian999

PHP:  sort($arr);
来源：http://of.jianghongdianzi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://oq.bjjhwx.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://kd.jianghongdianzi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://mh.jianghongdianzi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dd.shxzukj.cn

Ruby: arr.sort
来源：http://fk.shtwfgs.cn

C#:   list.Sort();
来源：http://jf.asd995.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://fw.muxihuayi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nu.hnjuh.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uw.yuexingan06.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ga.hahajie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mh.yuntaijiaju.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wj.nicolike.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ga.lnxyls.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xr.hahajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dt.shxzukj.cn

[D11] 反转数组
来源：http://wu.yuntaijiaju.cn

Py:   arr[::-1];  arr.reverse()
来源：http://lt.huanxung.cn

PHP:  array_reverse($arr);
来源：http://ea.szxytkj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pl.bookmarksfly.cn

TS:   [...arr].reverse();
来源：http://wx.huixiangedu.cn

Java: Collections.reverse(list);
来源：http://lf.jctech888.com.cn

Go:   slices.Reverse(arr)
来源：http://fy.bookmarksfly.cn

Ruby: arr.reverse
来源：http://cc.yuntaijiaju.cn

C#:   list.Reverse();
来源：http://aa.jctech888.com.cn

[D12] 查找元素下标
来源：http://cx.wgjwhj.cn

Py:   arr.index(x);  x in arr
来源：http://za.521024.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vf.9csxet.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oo.gzmigu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tj.wgjwhj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kp.chemitech.net.cn

Go:   slices.Index(arr, x)
来源：http://kp.shxzskj.cn

Ruby: arr.index(x)
来源：http://rc.huixiangedu.cn

C#:   list.IndexOf(x);
来源：http://rm.huixinmuqiang.cn

[D13] 过滤（保留满足条件的）
来源：http://fb.shxzskj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zj.wgjwhj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fq.bjjhwx.cn

JS:   arr.filter(x => x > 3)
来源：http://pv.jctech888.com.cn

TS:   arr.filter(x => x > 3)
来源：http://wg.szsharing.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://be.szsharing.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xz.huixiangedu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wn.yuntaijiaju.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qi.haigaiapp.cn

[D14] 映射转换（每个元素变形）
来源：http://cg.newstarts.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sm.huixiangedu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bw.chemitech.net.cn

JS:   arr.map(x => x * 2)
来源：http://yq.szxytkj.cn

TS:   arr.map(x => x * 2)
来源：http://fa.yuntaijiaju.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://sp.panjiajie.cn

Go:   // 手写循环
来源：http://ks.shxzukj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ye.jctech888.com.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://dq.szsharing.cn

[D15] 去重
来源：http://ip.huixinmuqiang.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xy.yuntaijiaju.cn

PHP:  array_unique($arr);
来源：http://om.yuexingan06.cn

JS:   [...new Set(arr)]
来源：http://fe.shxzskj.cn

TS:   [...new Set(arr)]
来源：http://od.shtwfgs.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fd.haigaiapp.cn

Go:   // 用 map[T]struct{} 手写
来源：http://fn.panjiajie.cn

Ruby: arr.uniq
来源：http://gi.colortex.cn

C#:   list.Distinct().ToList()
来源：http://rz.jctech888.com.cn

[D16] 求和与平均值
来源：http://nr.szxytkj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zs.bookmarksfly.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://on.newstarts.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://os.muxihuayi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rw.nicolike.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://il.newstarts.cn

Go:   // 手写循环累加
来源：http://my.asd995.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://td.lnxyls.cn

C#:   list.Sum();  list.Average()
来源：http://ua.hahajie.cn

[D17] 最大值与最小值
来源：http://op.szsharing.cn

Py:   max(arr);  min(arr)
来源：http://ml.gzmigu.cn

PHP:  max($arr);  min($arr);
来源：http://lk.haigaiapp.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zs.panjiajie.cn

TS:   Math.max(...arr);
来源：http://jo.asd995.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://zn.lnxyls.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ot.gzmigu.cn

Ruby: arr.max;  arr.min
来源：http://je.jianghongdianzi.cn

C#:   list.Max();  list.Min()
来源：http://jj.shxzskj.cn

[D18] 扁平化嵌套数组
来源：http://uq.lnxyls.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ch.lnxyls.cn

PHP:  array_merge(...$nested);
来源：http://ec.bookmarksfly.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gy.521024.cn

TS:   nested.flat();
来源：http://og.hahajie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yr.newstarts.cn

Go:   // 手写双层循环
来源：http://ef.newstarts.cn

Ruby: nested.flatten
来源：http://xq.521024.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://qd.asd995.cn

[D19] 按字段分组
来源：http://tb.yuexingan06.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lh.chemitech.net.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vp.chemitech.net.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ee.huixiangedu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qe.shxzskj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://un.asd995.cn

Go:   // 手写 map[string][]T
来源：http://zp.jctech888.com.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://yc.jctech888.com.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://sx.shtwfgs.cn

[D20] 统计每个元素出现次数
来源：http://am.shxzukj.cn

Py:   Counter(arr)
来源：http://rt.gzmigu.cn

PHP:  array_count_values($arr);
来源：http://go.gzmigu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tl.huanxung.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://la.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ch.9csxet.cn

Go:   // 手写 map[T]int
来源：http://st.jctech888.com.cn

Ruby: arr.tally
来源：http://if.shxzukj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kw.chemitech.net.cn

[D21] 判断是否包含某元素
来源：http://mn.nicolike.cn

Py:   x in arr
来源：http://nm.nszjky.cn

PHP:  in_array($x, $arr, true);
来源：http://mj.shxzskj.cn

JS:   arr.includes(x)
来源：http://ar.shtwfgs.cn

TS:   arr.includes(x)
来源：http://qf.hnjuh.cn

Java: list.contains(x)
来源：http://ap.yuntaijiaju.cn

Go:   slices.Contains(arr, x)
来源：http://iy.szsharing.cn

Ruby: arr.include?(x)
来源：http://vy.nszjky.cn

C#:   list.Contains(x)
来源：http://lb.szxytkj.cn

[D22] 复制数组（避免共享引用）
来源：http://pa.9csxet.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://si.panjiajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://aw.shxzskj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dk.jctech888.com.cn

TS:   [...arr];
来源：http://jt.panjiajie.cn

Java: new ArrayList<>(list);
来源：http://ih.huixinmuqiang.cn

Go:   copied := append([]int(nil), arr...)
来源：http://na.jianghongdianzi.cn

Ruby: arr.dup;  arr.clone
来源：http://um.wgjwhj.cn

C#:   new List<int>(list);
来源：http://jc.bookmarksfly.cn

[D23] reduce 累积计算
来源：http://oh.wgjwhj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dt.szsharing.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hn.bjjhwx.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cb.bjjhwx.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tr.jctech888.com.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ek.newstarts.cn

Go:   // 手写循环
来源：http://eu.yuntaijiaju.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fg.hnjuh.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sr.yuexingan06.cn

[D24] 字典 / Map 基本操作
来源：http://op.muxihuayi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ds.newstarts.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://di.newstarts.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pc.nszjky.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rw.haigaiapp.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nq.nicolike.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://te.bookmarksfly.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zw.9csxet.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wk.bookmarksfly.cn

[D25] Set 集合去重与交并差
来源：http://kg.shtwfgs.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ij.gzmigu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yl.bjjhwx.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qj.yuexingan06.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://eb.colortex.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bu.gzmigu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mc.shxzskj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nu.shxzskj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yw.lnxyls.cn

[D26] 数组转字符串
来源：http://vo.haigaiapp.cn

Py:   ", ".join(map(str, arr))
来源：http://of.huanxung.cn

PHP:  implode(", ", $arr);
来源：http://dt.bjjhwx.cn

JS:   arr.join(", ")
来源：http://cl.bjjhwx.cn

TS:   arr.join(", ")
来源：http://zu.jianghongdianzi.cn

Java: String.join(", ", list)
来源：http://bn.521024.cn

Go:   strings.Join(strs, ", ")
来源：http://en.yuntaijiaju.cn

Ruby: arr.join(", ")
来源：http://tu.521024.cn

C#:   string.Join(", ", list)
来源：http://bz.9csxet.cn

================================================================================
来源：http://qk.yuexingan06.cn

E. 字符串处理
来源：http://hn.nicolike.cn

================================================================================
来源：http://lu.huixiangedu.cn

[E01] 拼接字符串
来源：http://ll.bjjhwx.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vb.huanxung.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cg.9csxet.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jy.asd995.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tl.jctech888.com.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pv.newstarts.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wq.newstarts.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ux.gzmigu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wt.yuexingan06.cn

[E02] 重复字符串
来源：http://bo.haigaiapp.cn

Py:   "ab" * 3
来源：http://tk.gzmigu.cn

PHP:  str_repeat("ab", 3);
来源：http://xh.newstarts.cn

JS:   "ab".repeat(3)
来源：http://xp.shtwfgs.cn

TS:   "ab".repeat(3)
来源：http://le.yuexingan06.cn

Java: "ab".repeat(3)
来源：http://hw.panjiajie.cn

Go:   strings.Repeat("ab", 3)
来源：http://en.gzmigu.cn

Ruby: "ab" * 3
来源：http://je.asd995.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kq.shxzukj.cn

[E03] 截取子串
来源：http://me.jctech888.com.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://af.muxihuayi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://iz.panjiajie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ny.asd995.cn

TS:   s.slice(1, 4)
来源：http://ge.newstarts.cn

Java: s.substring(1, 4)
来源：http://wk.lnxyls.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xk.shxzskj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://jx.muxihuayi.cn

C#:   s.Substring(1, 3)
来源：http://zv.nszjky.cn

[E04] 查找子串位置
来源：http://op.hahajie.cn

Py:   s.find("x");  s.index("x")
来源：http://iy.wgjwhj.cn

PHP:  strpos($s, "x");
来源：http://gk.huixinmuqiang.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sr.nszjky.cn

TS:   s.indexOf("x")
来源：http://dl.nszjky.cn

Java: s.indexOf("x")
来源：http://hd.panjiajie.cn

Go:   strings.Index(s, "x")
来源：http://qc.bjjhwx.cn

Ruby: s.index("x")
来源：http://ph.shxzukj.cn

C#:   s.IndexOf("x")
来源：http://sy.nicolike.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://wj.hnjuh.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bj.bjjhwx.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vr.asd995.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ik.szxytkj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qk.jctech888.com.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qx.newstarts.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dd.muxihuayi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://va.nicolike.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sy.521024.cn

[E06] 替换子串
来源：http://ly.bjjhwx.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gq.bookmarksfly.cn

PHP:  str_replace("a", "b", $s);
来源：http://hw.9csxet.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dc.shxzskj.cn

TS:   s.replaceAll("a", "b")
来源：http://nb.wgjwhj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ft.szxytkj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://el.gzmigu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://oy.colortex.cn

C#:   s.Replace("a", "b")
来源：http://gy.bjjhwx.cn

[E07] 按分隔符拆分
来源：http://xo.9csxet.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tx.gzmigu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nf.huixinmuqiang.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://nw.shtwfgs.cn

TS:   s.split(",")
来源：http://ua.521024.cn

Java: s.split(",");  s.split("\\s+")
来源：http://bn.szxytkj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ot.yuexingan06.cn

Ruby: s.split(",");  s.split
来源：http://nb.yuntaijiaju.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bw.huixinmuqiang.cn

[E08] 数组按分隔符合并
来源：http://aa.shxzukj.cn

Py:   ",".join(items)
来源：http://xt.newstarts.cn

PHP:  implode(",", $items);
来源：http://eh.newstarts.cn

JS:   items.join(",")
来源：http://eo.gzmigu.cn

TS:   items.join(",")
来源：http://qz.shtwfgs.cn

Java: String.join(",", items)
来源：http://ui.newstarts.cn

Go:   strings.Join(items, ",")
来源：http://vy.nicolike.cn

Ruby: items.join(",")
来源：http://hd.nicolike.cn

C#:   string.Join(",", items)
来源：http://et.hnjuh.cn

[E09] 去除所有空白字符
来源：http://jc.colortex.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://sn.521024.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hv.newstarts.cn

JS:   s.replace(/\s+/g, "")
来源：http://dg.bjjhwx.cn

TS:   s.replace(/\s+/g, "")
来源：http://ym.jctech888.com.cn

Java: s.replaceAll("\\s+", "")
来源：http://zs.haigaiapp.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://zn.jctech888.com.cn

Ruby: s.gsub(/\s+/, "")
来源：http://dy.shxzukj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tb.gzmigu.cn

[E10] 左侧补零 / 定长填充
来源：http://xv.szxytkj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pz.bjjhwx.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mn.nicolike.cn

JS:   "7".padStart(3, "0")
来源：http://zm.shxzukj.cn

TS:   "7".padStart(3, "0")
来源：http://sf.huixiangedu.cn

Java: String.format("%03d", 7)
来源：http://sc.bjjhwx.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ea.wgjwhj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sc.shxzukj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rg.jctech888.com.cn

[E11] 反转字符串
来源：http://wu.jctech888.com.cn

Py:   s[::-1]
来源：http://ww.nicolike.cn

PHP:  strrev($s);
来源：http://pm.jianghongdianzi.cn

JS:   [...s].reverse().join("")
来源：http://yy.szsharing.cn

TS:   [...s].reverse().join("")
来源：http://cq.bjjhwx.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://sd.lnxyls.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://xt.huanxung.cn

Ruby: s.reverse
来源：http://uy.9csxet.cn

C#:   new string(s.Reverse().ToArray())
来源：http://oo.hahajie.cn

[E12] 统计某字符出现次数
来源：http://cl.lnxyls.cn

Py:   s.count("a")
来源：http://ak.bookmarksfly.cn

PHP:  substr_count($s, "a");
来源：http://qi.bjjhwx.cn

JS:   s.split("a").length - 1
来源：http://zy.shxzukj.cn

TS:   s.split("a").length - 1
来源：http://hc.bookmarksfly.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ab.newstarts.cn

Go:   strings.Count(s, "a")
来源：http://kv.jianghongdianzi.cn

Ruby: s.count("a")
来源：http://wg.jianghongdianzi.cn

C#:   s.Count(c => c == 'a')
来源：http://di.haigaiapp.cn

[E13] 逐字符遍历
来源：http://fq.yuntaijiaju.cn

Py:   for ch in s: print(ch)
来源：http://os.nicolike.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tz.haigaiapp.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://pm.nszjky.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://rc.bjjhwx.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vb.huanxung.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ih.bookmarksfly.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ru.nicolike.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wx.nszjky.cn

[E14] URL 编码与 Base64
来源：http://ew.bjjhwx.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nd.bjjhwx.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://lu.shtwfgs.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wl.bjjhwx.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gv.asd995.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lr.colortex.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://op.lnxyls.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bh.chemitech.net.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tz.nicolike.cn

[E15] HTML 转义 / 反转义
来源：http://fe.521024.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://if.9csxet.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uv.muxihuayi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lx.haigaiapp.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://sp.hnjuh.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dg.nszjky.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bn.haigaiapp.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gc.hahajie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ca.szsharing.cn

[E16] 数字千分位
来源：http://oy.nicolike.cn

Py:   f"{1234567:,}"
来源：http://zl.nszjky.cn


<!-- 参考信息 -->