代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kj.9csxet.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bk.jctech888.com.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lo.huixinmuqiang.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yo.huixinmuqiang.cn

[D11] 反转数组
来源：http://qp.shxzukj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://uw.shxzskj.cn

PHP:  array_reverse($arr);
来源：http://gz.panjiajie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://va.shxzskj.cn

TS:   [...arr].reverse();
来源：http://qq.yuexingan06.cn

Java: Collections.reverse(list);
来源：http://kc.shxzskj.cn

Go:   slices.Reverse(arr)
来源：http://dj.wgjwhj.cn

Ruby: arr.reverse
来源：http://di.shxzskj.cn

C#:   list.Reverse();
来源：http://lt.colortex.cn

[D12] 查找元素下标
来源：http://lx.newstarts.cn

Py:   arr.index(x);  x in arr
来源：http://qc.lnxyls.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://eq.panjiajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dw.shxzskj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ky.colortex.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://go.muxihuayi.cn

Go:   slices.Index(arr, x)
来源：http://cx.chemitech.net.cn

Ruby: arr.index(x)
来源：http://yi.lnxyls.cn

C#:   list.IndexOf(x);
来源：http://kd.szxytkj.cn

[D13] 过滤（保留满足条件的）
来源：http://vz.chemitech.net.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lq.szsharing.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://az.521024.cn

JS:   arr.filter(x => x > 3)
来源：http://bj.szxytkj.cn

TS:   arr.filter(x => x > 3)
来源：http://wf.hahajie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zk.shxzskj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wz.521024.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ls.huixinmuqiang.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://yc.colortex.cn

[D14] 映射转换（每个元素变形）
来源：http://go.jctech888.com.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://af.nicolike.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pb.nicolike.cn

JS:   arr.map(x => x * 2)
来源：http://ec.shtwfgs.cn

TS:   arr.map(x => x * 2)
来源：http://og.hnjuh.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://bg.huixinmuqiang.cn

Go:   // 手写循环
来源：http://xk.bookmarksfly.cn

Ruby: arr.map { |x| x * 2 }
来源：http://mg.colortex.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ry.newstarts.cn

[D15] 去重
来源：http://cx.bookmarksfly.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://er.asd995.cn

PHP:  array_unique($arr);
来源：http://es.yuntaijiaju.cn

JS:   [...new Set(arr)]
来源：http://xp.nszjky.cn

TS:   [...new Set(arr)]
来源：http://ni.521024.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bo.huixinmuqiang.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ju.huixiangedu.cn

Ruby: arr.uniq
来源：http://jt.huixiangedu.cn

C#:   list.Distinct().ToList()
来源：http://vo.nszjky.cn

[D16] 求和与平均值
来源：http://cw.huixiangedu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vo.huanxung.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wo.huanxung.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qs.shxzukj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://aq.huixiangedu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://im.huixinmuqiang.cn

Go:   // 手写循环累加
来源：http://qe.521024.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mg.hnjuh.cn

C#:   list.Sum();  list.Average()
来源：http://tw.hnjuh.cn

[D17] 最大值与最小值
来源：http://ru.huanxung.cn

Py:   max(arr);  min(arr)
来源：http://zn.nicolike.cn

PHP:  max($arr);  min($arr);
来源：http://by.gzmigu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lx.huixinmuqiang.cn

TS:   Math.max(...arr);
来源：http://bh.colortex.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mk.shxzukj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mv.yuexingan06.cn

Ruby: arr.max;  arr.min
来源：http://hj.yuntaijiaju.cn

C#:   list.Max();  list.Min()
来源：http://to.shtwfgs.cn

[D18] 扁平化嵌套数组
来源：http://vl.hahajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ht.bookmarksfly.cn

PHP:  array_merge(...$nested);
来源：http://wh.chemitech.net.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qy.asd995.cn

TS:   nested.flat();
来源：http://fs.hnjuh.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hx.521024.cn

Go:   // 手写双层循环
来源：http://xq.hahajie.cn

Ruby: nested.flatten
来源：http://dh.shxzskj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ck.newstarts.cn

[D19] 按字段分组
来源：http://ia.hnjuh.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ij.newstarts.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ag.newstarts.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cj.jctech888.com.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://pf.yuntaijiaju.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://to.huixinmuqiang.cn

Go:   // 手写 map[string][]T
来源：http://ru.asd995.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://wq.bjjhwx.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nc.asd995.cn

[D20] 统计每个元素出现次数
来源：http://mf.huixinmuqiang.cn

Py:   Counter(arr)
来源：http://kv.jianghongdianzi.cn

PHP:  array_count_values($arr);
来源：http://qn.hahajie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fs.shxzskj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jn.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tl.huixiangedu.cn

Go:   // 手写 map[T]int
来源：http://yn.9csxet.cn

Ruby: arr.tally
来源：http://qs.colortex.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mb.yuexingan06.cn

[D21] 判断是否包含某元素
来源：http://cc.bookmarksfly.cn

Py:   x in arr
来源：http://ao.szsharing.cn

PHP:  in_array($x, $arr, true);
来源：http://na.szsharing.cn

JS:   arr.includes(x)
来源：http://ff.szxytkj.cn

TS:   arr.includes(x)
来源：http://fv.bjjhwx.cn

Java: list.contains(x)
来源：http://qt.newstarts.cn

Go:   slices.Contains(arr, x)
来源：http://gt.yuntaijiaju.cn

Ruby: arr.include?(x)
来源：http://zy.colortex.cn

C#:   list.Contains(x)
来源：http://mx.shtwfgs.cn

[D22] 复制数组（避免共享引用）
来源：http://re.9csxet.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bu.huanxung.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cm.newstarts.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vr.lnxyls.cn

TS:   [...arr];
来源：http://nl.shtwfgs.cn

Java: new ArrayList<>(list);
来源：http://iy.lnxyls.cn

Go:   copied := append([]int(nil), arr...)
来源：http://vb.lnxyls.cn

Ruby: arr.dup;  arr.clone
来源：http://wl.muxihuayi.cn

C#:   new List<int>(list);
来源：http://zk.shtwfgs.cn

[D23] reduce 累积计算
来源：http://pv.gzmigu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ij.panjiajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kj.asd995.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gw.muxihuayi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fk.jctech888.com.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://gg.huixinmuqiang.cn

Go:   // 手写循环
来源：http://nz.chemitech.net.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fr.huanxung.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dr.asd995.cn

[D24] 字典 / Map 基本操作
来源：http://kq.yuntaijiaju.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://de.yuntaijiaju.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ma.newstarts.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ai.panjiajie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fn.hnjuh.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xe.yuexingan06.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ny.muxihuayi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mk.huixinmuqiang.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kz.wgjwhj.cn

[D25] Set 集合去重与交并差
来源：http://ev.szxytkj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://up.jianghongdianzi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tk.nszjky.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ba.9csxet.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mv.yuexingan06.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wh.huixinmuqiang.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kc.wgjwhj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vj.bookmarksfly.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xw.shxzskj.cn

[D26] 数组转字符串
来源：http://ah.nszjky.cn

Py:   ", ".join(map(str, arr))
来源：http://uw.hnjuh.cn

PHP:  implode(", ", $arr);
来源：http://hu.hnjuh.cn

JS:   arr.join(", ")
来源：http://fm.panjiajie.cn

TS:   arr.join(", ")
来源：http://hx.colortex.cn

Java: String.join(", ", list)
来源：http://sx.chemitech.net.cn

Go:   strings.Join(strs, ", ")
来源：http://zb.asd995.cn

Ruby: arr.join(", ")
来源：http://eq.asd995.cn

C#:   string.Join(", ", list)
来源：http://td.huixinmuqiang.cn

================================================================================
来源：http://kg.lnxyls.cn

E. 字符串处理
来源：http://kd.panjiajie.cn

================================================================================
来源：http://ue.newstarts.cn

[E01] 拼接字符串
来源：http://nk.hnjuh.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fi.jctech888.com.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pc.wgjwhj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bq.asd995.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jv.nicolike.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fl.shxzukj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gm.521024.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ri.muxihuayi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://po.szsharing.cn

[E02] 重复字符串
来源：http://cw.panjiajie.cn

Py:   "ab" * 3
来源：http://wv.nicolike.cn

PHP:  str_repeat("ab", 3);
来源：http://jx.huanxung.cn

JS:   "ab".repeat(3)
来源：http://os.chemitech.net.cn

TS:   "ab".repeat(3)
来源：http://sg.colortex.cn

Java: "ab".repeat(3)
来源：http://cz.newstarts.cn

Go:   strings.Repeat("ab", 3)
来源：http://xu.shtwfgs.cn

Ruby: "ab" * 3
来源：http://si.jianghongdianzi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fw.shxzskj.cn

[E03] 截取子串
来源：http://qo.wgjwhj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yi.colortex.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tm.bjjhwx.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ny.gzmigu.cn

TS:   s.slice(1, 4)
来源：http://ce.muxihuayi.cn

Java: s.substring(1, 4)
来源：http://fy.newstarts.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hj.bjjhwx.cn

Ruby: s[1, 3];  s[1..3]
来源：http://iq.szsharing.cn

C#:   s.Substring(1, 3)
来源：http://ul.asd995.cn

[E04] 查找子串位置
来源：http://nv.hahajie.cn

Py:   s.find("x");  s.index("x")
来源：http://yk.shtwfgs.cn

PHP:  strpos($s, "x");
来源：http://mv.bookmarksfly.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bj.colortex.cn

TS:   s.indexOf("x")
来源：http://sj.lnxyls.cn

Java: s.indexOf("x")
来源：http://hp.haigaiapp.cn

Go:   strings.Index(s, "x")
来源：http://jm.szsharing.cn

Ruby: s.index("x")
来源：http://ag.9csxet.cn

C#:   s.IndexOf("x")
来源：http://lw.chemitech.net.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://qd.hahajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://es.gzmigu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jv.chemitech.net.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zv.shxzukj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zi.newstarts.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sa.chemitech.net.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pv.muxihuayi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://iv.yuntaijiaju.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bi.panjiajie.cn

[E06] 替换子串
来源：http://pw.yuexingan06.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pg.yuexingan06.cn

PHP:  str_replace("a", "b", $s);
来源：http://zx.jianghongdianzi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pr.haigaiapp.cn

TS:   s.replaceAll("a", "b")
来源：http://rj.haigaiapp.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gl.asd995.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zm.huixinmuqiang.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ps.szsharing.cn

C#:   s.Replace("a", "b")
来源：http://iu.asd995.cn

[E07] 按分隔符拆分
来源：http://ld.yuntaijiaju.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bn.521024.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zx.shtwfgs.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://mn.jctech888.com.cn

TS:   s.split(",")
来源：http://mq.shtwfgs.cn

Java: s.split(",");  s.split("\\s+")
来源：http://pj.asd995.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gr.521024.cn

Ruby: s.split(",");  s.split
来源：http://ij.jianghongdianzi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://uf.newstarts.cn

[E08] 数组按分隔符合并
来源：http://qr.haigaiapp.cn

Py:   ",".join(items)
来源：http://eb.521024.cn

PHP:  implode(",", $items);
来源：http://pg.gzmigu.cn

JS:   items.join(",")
来源：http://qh.colortex.cn

TS:   items.join(",")
来源：http://az.nicolike.cn

Java: String.join(",", items)
来源：http://do.yuexingan06.cn

Go:   strings.Join(items, ",")
来源：http://jw.asd995.cn

Ruby: items.join(",")
来源：http://ed.yuntaijiaju.cn

C#:   string.Join(",", items)
来源：http://wr.yuntaijiaju.cn

[E09] 去除所有空白字符
来源：http://tl.hahajie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mc.lnxyls.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mi.huixinmuqiang.cn

JS:   s.replace(/\s+/g, "")
来源：http://ov.hahajie.cn

TS:   s.replace(/\s+/g, "")
来源：http://yq.hahajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://zt.nicolike.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://me.huanxung.cn

Ruby: s.gsub(/\s+/, "")
来源：http://jw.gzmigu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ol.szsharing.cn

[E10] 左侧补零 / 定长填充
来源：http://qr.colortex.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xx.shxzskj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dq.nszjky.cn

JS:   "7".padStart(3, "0")
来源：http://bw.shxzukj.cn

TS:   "7".padStart(3, "0")
来源：http://qi.haigaiapp.cn

Java: String.format("%03d", 7)
来源：http://pz.szxytkj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://rk.huanxung.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ay.wgjwhj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://no.huixiangedu.cn

[E11] 反转字符串
来源：http://aq.colortex.cn

Py:   s[::-1]
来源：http://lu.shxzskj.cn

PHP:  strrev($s);
来源：http://lk.shtwfgs.cn

JS:   [...s].reverse().join("")
来源：http://he.wgjwhj.cn

TS:   [...s].reverse().join("")
来源：http://mm.jianghongdianzi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://on.nszjky.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://lc.shxzukj.cn

Ruby: s.reverse
来源：http://kk.521024.cn

C#:   new string(s.Reverse().ToArray())
来源：http://lq.chemitech.net.cn

[E12] 统计某字符出现次数
来源：http://lf.huixiangedu.cn

Py:   s.count("a")
来源：http://yt.lnxyls.cn

PHP:  substr_count($s, "a");
来源：http://rm.huanxung.cn

JS:   s.split("a").length - 1
来源：http://ae.lnxyls.cn

TS:   s.split("a").length - 1
来源：http://ax.lnxyls.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://sa.shtwfgs.cn

Go:   strings.Count(s, "a")
来源：http://vv.521024.cn

Ruby: s.count("a")
来源：http://vl.jianghongdianzi.cn

C#:   s.Count(c => c == 'a')
来源：http://hq.wgjwhj.cn

[E13] 逐字符遍历
来源：http://km.szsharing.cn

Py:   for ch in s: print(ch)
来源：http://wd.huixinmuqiang.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fz.muxihuayi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ka.huixiangedu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ih.lnxyls.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ut.lnxyls.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ak.szsharing.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://qh.hahajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fu.huanxung.cn

[E14] URL 编码与 Base64
来源：http://av.nicolike.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yz.bjjhwx.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bj.nszjky.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vi.nszjky.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sw.521024.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://sk.bjjhwx.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bw.9csxet.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://en.szxytkj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ms.szsharing.cn

[E15] HTML 转义 / 反转义
来源：http://bs.szsharing.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://dj.shtwfgs.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ow.shxzskj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rs.shxzukj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://rx.yuntaijiaju.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tv.yuntaijiaju.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dn.haigaiapp.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://an.nszjky.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qm.asd995.cn

[E16] 数字千分位
来源：http://dx.bjjhwx.cn

Py:   f"{1234567:,}"
来源：http://yf.huixinmuqiang.cn

PHP:  number_format(1234567);
来源：http://nf.bookmarksfly.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ht.huanxung.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ow.lnxyls.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bh.bookmarksfly.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yo.haigaiapp.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vh.yuexingan06.cn

C#:   1234567.ToString("N0")
来源：http://zr.asd995.cn

[E17] 首字母大写
来源：http://yp.muxihuayi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ru.jianghongdianzi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ab.newstarts.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ou.shxzukj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wf.huixinmuqiang.cn


<!-- 参考信息 -->