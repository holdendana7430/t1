代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qy.chemitech.net.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://op.haigaiapp.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zp.bookmarksfly.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kq.shtwfgs.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zm.bookmarksfly.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://oi.hahajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yz.huixinmuqiang.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://le.yuexingan06.cn

[D11] 反转数组
来源：http://yt.jianghongdianzi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://hc.huixiangedu.cn

PHP:  array_reverse($arr);
来源：http://jr.panjiajie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cz.szxytkj.cn

TS:   [...arr].reverse();
来源：http://yj.shxzskj.cn

Java: Collections.reverse(list);
来源：http://jx.jctech888.com.cn

Go:   slices.Reverse(arr)
来源：http://zj.lnxyls.cn

Ruby: arr.reverse
来源：http://mu.lnxyls.cn

C#:   list.Reverse();
来源：http://tv.hahajie.cn

[D12] 查找元素下标
来源：http://qw.muxihuayi.cn

Py:   arr.index(x);  x in arr
来源：http://wm.muxihuayi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qb.panjiajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hi.nicolike.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tx.muxihuayi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yb.szsharing.cn

Go:   slices.Index(arr, x)
来源：http://ti.szxytkj.cn

Ruby: arr.index(x)
来源：http://cs.szsharing.cn

C#:   list.IndexOf(x);
来源：http://zo.jctech888.com.cn

[D13] 过滤（保留满足条件的）
来源：http://xa.521024.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pw.shxzskj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mt.gzmigu.cn

JS:   arr.filter(x => x > 3)
来源：http://pk.hnjuh.cn

TS:   arr.filter(x => x > 3)
来源：http://yh.yuexingan06.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tw.521024.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://py.shxzskj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ot.shtwfgs.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://gs.yuntaijiaju.cn

[D14] 映射转换（每个元素变形）
来源：http://tm.nszjky.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://or.huanxung.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yg.521024.cn

JS:   arr.map(x => x * 2)
来源：http://jy.szsharing.cn

TS:   arr.map(x => x * 2)
来源：http://qh.wgjwhj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://iv.chemitech.net.cn

Go:   // 手写循环
来源：http://fs.nicolike.cn

Ruby: arr.map { |x| x * 2 }
来源：http://iv.nszjky.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ss.muxihuayi.cn

[D15] 去重
来源：http://px.nicolike.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://au.hnjuh.cn

PHP:  array_unique($arr);
来源：http://ff.nszjky.cn

JS:   [...new Set(arr)]
来源：http://gv.nicolike.cn

TS:   [...new Set(arr)]
来源：http://zp.521024.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kb.bjjhwx.cn

Go:   // 用 map[T]struct{} 手写
来源：http://fc.shxzukj.cn

Ruby: arr.uniq
来源：http://bt.gzmigu.cn

C#:   list.Distinct().ToList()
来源：http://gs.hahajie.cn

[D16] 求和与平均值
来源：http://gr.panjiajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://au.nszjky.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://us.colortex.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bz.shxzskj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rb.panjiajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bs.szsharing.cn

Go:   // 手写循环累加
来源：http://cp.haigaiapp.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bh.huixinmuqiang.cn

C#:   list.Sum();  list.Average()
来源：http://nr.bjjhwx.cn

[D17] 最大值与最小值
来源：http://al.newstarts.cn

Py:   max(arr);  min(arr)
来源：http://lx.gzmigu.cn

PHP:  max($arr);  min($arr);
来源：http://vy.asd995.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nr.haigaiapp.cn

TS:   Math.max(...arr);
来源：http://hl.lnxyls.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://oh.muxihuayi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://na.panjiajie.cn

Ruby: arr.max;  arr.min
来源：http://hv.colortex.cn

C#:   list.Max();  list.Min()
来源：http://mk.chemitech.net.cn

[D18] 扁平化嵌套数组
来源：http://lk.gzmigu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zm.hnjuh.cn

PHP:  array_merge(...$nested);
来源：http://pw.hnjuh.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mq.nicolike.cn

TS:   nested.flat();
来源：http://rh.szxytkj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bx.chemitech.net.cn

Go:   // 手写双层循环
来源：http://pu.haigaiapp.cn

Ruby: nested.flatten
来源：http://ri.colortex.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://tl.hnjuh.cn

[D19] 按字段分组
来源：http://ul.gzmigu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ue.9csxet.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bw.huixinmuqiang.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ae.hnjuh.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://dj.gzmigu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xi.shtwfgs.cn

Go:   // 手写 map[string][]T
来源：http://ge.shxzukj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ye.9csxet.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://if.lnxyls.cn

[D20] 统计每个元素出现次数
来源：http://sd.yuexingan06.cn

Py:   Counter(arr)
来源：http://de.jctech888.com.cn

PHP:  array_count_values($arr);
来源：http://yo.nicolike.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://is.haigaiapp.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yl.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ie.nszjky.cn

Go:   // 手写 map[T]int
来源：http://ra.521024.cn

Ruby: arr.tally
来源：http://ul.hahajie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ub.chemitech.net.cn

[D21] 判断是否包含某元素
来源：http://gd.asd995.cn

Py:   x in arr
来源：http://xg.jctech888.com.cn

PHP:  in_array($x, $arr, true);
来源：http://yx.9csxet.cn

JS:   arr.includes(x)
来源：http://fe.lnxyls.cn

TS:   arr.includes(x)
来源：http://nn.gzmigu.cn

Java: list.contains(x)
来源：http://lo.nicolike.cn

Go:   slices.Contains(arr, x)
来源：http://ev.nicolike.cn

Ruby: arr.include?(x)
来源：http://nm.jianghongdianzi.cn

C#:   list.Contains(x)
来源：http://ex.asd995.cn

[D22] 复制数组（避免共享引用）
来源：http://bm.huixiangedu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zh.huixiangedu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fs.yuntaijiaju.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://az.jianghongdianzi.cn

TS:   [...arr];
来源：http://bo.gzmigu.cn

Java: new ArrayList<>(list);
来源：http://dg.shxzukj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://di.wgjwhj.cn

Ruby: arr.dup;  arr.clone
来源：http://tl.521024.cn

C#:   new List<int>(list);
来源：http://yt.colortex.cn

[D23] reduce 累积计算
来源：http://aw.gzmigu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ip.huixinmuqiang.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zx.gzmigu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rx.huixiangedu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tu.muxihuayi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://wf.hnjuh.cn

Go:   // 手写循环
来源：http://zp.shxzukj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hg.szxytkj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cu.szxytkj.cn

[D24] 字典 / Map 基本操作
来源：http://gp.521024.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://th.lnxyls.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tf.jctech888.com.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://es.bjjhwx.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cu.nicolike.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lb.shxzskj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://eu.muxihuayi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nv.huixinmuqiang.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zg.shxzukj.cn

[D25] Set 集合去重与交并差
来源：http://lm.wgjwhj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://un.jianghongdianzi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tv.huanxung.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://op.szxytkj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cj.yuntaijiaju.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ln.yuntaijiaju.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dm.bookmarksfly.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qv.bookmarksfly.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://oo.gzmigu.cn

[D26] 数组转字符串
来源：http://ku.hnjuh.cn

Py:   ", ".join(map(str, arr))
来源：http://jf.shxzukj.cn

PHP:  implode(", ", $arr);
来源：http://an.asd995.cn

JS:   arr.join(", ")
来源：http://vn.asd995.cn

TS:   arr.join(", ")
来源：http://hv.asd995.cn

Java: String.join(", ", list)
来源：http://dz.jianghongdianzi.cn

Go:   strings.Join(strs, ", ")
来源：http://im.shtwfgs.cn

Ruby: arr.join(", ")
来源：http://pc.lnxyls.cn

C#:   string.Join(", ", list)
来源：http://ai.yuntaijiaju.cn

================================================================================
来源：http://oi.yuntaijiaju.cn

E. 字符串处理
来源：http://bx.muxihuayi.cn

================================================================================
来源：http://tt.hnjuh.cn

[E01] 拼接字符串
来源：http://te.hahajie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ag.hahajie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lk.hahajie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hw.hahajie.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dl.newstarts.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://og.gzmigu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fk.haigaiapp.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xt.colortex.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jk.shxzskj.cn

[E02] 重复字符串
来源：http://nf.wgjwhj.cn

Py:   "ab" * 3
来源：http://zn.huixiangedu.cn

PHP:  str_repeat("ab", 3);
来源：http://ne.chemitech.net.cn

JS:   "ab".repeat(3)
来源：http://fa.nszjky.cn

TS:   "ab".repeat(3)
来源：http://ty.hnjuh.cn

Java: "ab".repeat(3)
来源：http://ma.huanxung.cn

Go:   strings.Repeat("ab", 3)
来源：http://uq.panjiajie.cn

Ruby: "ab" * 3
来源：http://wb.huixinmuqiang.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rw.shtwfgs.cn

[E03] 截取子串
来源：http://gg.colortex.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://iv.haigaiapp.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ya.hahajie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yd.newstarts.cn

TS:   s.slice(1, 4)
来源：http://fo.haigaiapp.cn

Java: s.substring(1, 4)
来源：http://ph.huixiangedu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cp.bookmarksfly.cn

Ruby: s[1, 3];  s[1..3]
来源：http://hw.yuntaijiaju.cn

C#:   s.Substring(1, 3)
来源：http://wn.szxytkj.cn

[E04] 查找子串位置
来源：http://mk.9csxet.cn

Py:   s.find("x");  s.index("x")
来源：http://iz.jianghongdianzi.cn

PHP:  strpos($s, "x");
来源：http://rq.huanxung.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://od.newstarts.cn

TS:   s.indexOf("x")
来源：http://sn.bjjhwx.cn

Java: s.indexOf("x")
来源：http://ol.nicolike.cn

Go:   strings.Index(s, "x")
来源：http://uo.chemitech.net.cn

Ruby: s.index("x")
来源：http://zr.asd995.cn

C#:   s.IndexOf("x")
来源：http://ix.jctech888.com.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://sk.huixiangedu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ex.nszjky.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://er.panjiajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bu.jianghongdianzi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://vb.shtwfgs.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fc.huanxung.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tk.9csxet.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qf.jctech888.com.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ah.wgjwhj.cn

[E06] 替换子串
来源：http://iz.huixiangedu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hf.muxihuayi.cn

PHP:  str_replace("a", "b", $s);
来源：http://nf.wgjwhj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tv.panjiajie.cn

TS:   s.replaceAll("a", "b")
来源：http://sk.panjiajie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kr.chemitech.net.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://uw.muxihuayi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fd.yuexingan06.cn

C#:   s.Replace("a", "b")
来源：http://nq.shxzskj.cn

[E07] 按分隔符拆分
来源：http://ri.521024.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ar.szxytkj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ba.bookmarksfly.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://nj.gzmigu.cn

TS:   s.split(",")
来源：http://rl.szxytkj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xq.lnxyls.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://sb.shxzukj.cn

Ruby: s.split(",");  s.split
来源：http://em.huixinmuqiang.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dk.shxzukj.cn

[E08] 数组按分隔符合并
来源：http://wu.huixinmuqiang.cn

Py:   ",".join(items)
来源：http://pj.szsharing.cn

PHP:  implode(",", $items);
来源：http://fn.panjiajie.cn

JS:   items.join(",")
来源：http://xc.colortex.cn

TS:   items.join(",")
来源：http://kr.haigaiapp.cn

Java: String.join(",", items)
来源：http://bm.gzmigu.cn

Go:   strings.Join(items, ",")
来源：http://ym.yuntaijiaju.cn

Ruby: items.join(",")
来源：http://ga.haigaiapp.cn

C#:   string.Join(",", items)
来源：http://or.szsharing.cn

[E09] 去除所有空白字符
来源：http://uw.yuntaijiaju.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kt.colortex.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zf.szxytkj.cn

JS:   s.replace(/\s+/g, "")
来源：http://lb.muxihuayi.cn

TS:   s.replace(/\s+/g, "")
来源：http://gb.huixiangedu.cn

Java: s.replaceAll("\\s+", "")
来源：http://of.yuntaijiaju.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qn.newstarts.cn

Ruby: s.gsub(/\s+/, "")
来源：http://wb.nszjky.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qw.nszjky.cn

[E10] 左侧补零 / 定长填充
来源：http://re.asd995.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://np.szsharing.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ik.szxytkj.cn

JS:   "7".padStart(3, "0")
来源：http://bf.9csxet.cn

TS:   "7".padStart(3, "0")
来源：http://nj.9csxet.cn

Java: String.format("%03d", 7)
来源：http://jd.nszjky.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xr.newstarts.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ox.huixinmuqiang.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lj.gzmigu.cn

[E11] 反转字符串
来源：http://lv.9csxet.cn

Py:   s[::-1]
来源：http://mm.huixinmuqiang.cn

PHP:  strrev($s);
来源：http://zx.chemitech.net.cn

JS:   [...s].reverse().join("")
来源：http://ep.colortex.cn

TS:   [...s].reverse().join("")
来源：http://ep.shtwfgs.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ju.szxytkj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://tb.huixinmuqiang.cn

Ruby: s.reverse
来源：http://vx.huanxung.cn

C#:   new string(s.Reverse().ToArray())
来源：http://hz.bookmarksfly.cn

[E12] 统计某字符出现次数
来源：http://sm.huanxung.cn

Py:   s.count("a")
来源：http://ve.nicolike.cn

PHP:  substr_count($s, "a");
来源：http://gz.newstarts.cn

JS:   s.split("a").length - 1
来源：http://ko.521024.cn

TS:   s.split("a").length - 1
来源：http://wi.jctech888.com.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wm.bookmarksfly.cn

Go:   strings.Count(s, "a")
来源：http://sw.newstarts.cn

Ruby: s.count("a")
来源：http://ih.huixinmuqiang.cn

C#:   s.Count(c => c == 'a')
来源：http://ud.chemitech.net.cn

[E13] 逐字符遍历
来源：http://un.shxzskj.cn

Py:   for ch in s: print(ch)
来源：http://wc.bookmarksfly.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vj.bookmarksfly.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://cq.asd995.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://oj.huixinmuqiang.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xe.yuexingan06.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://oo.lnxyls.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ni.yuexingan06.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zb.shtwfgs.cn

[E14] URL 编码与 Base64
来源：http://fi.jianghongdianzi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xn.hnjuh.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ti.wgjwhj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ng.haigaiapp.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qv.bjjhwx.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ot.lnxyls.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://na.haigaiapp.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yo.9csxet.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zi.haigaiapp.cn

[E15] HTML 转义 / 反转义
来源：http://gy.gzmigu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://pm.wgjwhj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sb.jctech888.com.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xx.shxzskj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ly.haigaiapp.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qo.panjiajie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://at.asd995.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rk.lnxyls.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mx.jctech888.com.cn

[E16] 数字千分位
来源：http://ug.nszjky.cn

Py:   f"{1234567:,}"
来源：http://dw.shxzskj.cn

PHP:  number_format(1234567);
来源：http://xe.lnxyls.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://zn.muxihuayi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://to.shxzskj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ly.szxytkj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pp.muxihuayi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://on.yuntaijiaju.cn

C#:   1234567.ToString("N0")
来源：http://pg.lnxyls.cn

[E17] 首字母大写
来源：http://ff.huanxung.cn


<!-- 参考信息 -->