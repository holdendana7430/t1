代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pf.jctech888.com.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fw.gzmigu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kr.yuexingan06.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gl.haigaiapp.cn

[D11] 反转数组
来源：http://tr.bjjhwx.cn

Py:   arr[::-1];  arr.reverse()
来源：http://mc.shxzskj.cn

PHP:  array_reverse($arr);
来源：http://en.szxytkj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qn.szxytkj.cn

TS:   [...arr].reverse();
来源：http://qz.szsharing.cn

Java: Collections.reverse(list);
来源：http://fp.huixiangedu.cn

Go:   slices.Reverse(arr)
来源：http://gh.hahajie.cn

Ruby: arr.reverse
来源：http://mo.haigaiapp.cn

C#:   list.Reverse();
来源：http://yc.haigaiapp.cn

[D12] 查找元素下标
来源：http://iz.yuexingan06.cn

Py:   arr.index(x);  x in arr
来源：http://no.yuntaijiaju.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gb.yuexingan06.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jy.nszjky.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kc.bjjhwx.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vc.gzmigu.cn

Go:   slices.Index(arr, x)
来源：http://hr.bookmarksfly.cn

Ruby: arr.index(x)
来源：http://xx.9csxet.cn

C#:   list.IndexOf(x);
来源：http://wh.521024.cn

[D13] 过滤（保留满足条件的）
来源：http://er.huixiangedu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wl.bjjhwx.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gh.haigaiapp.cn

JS:   arr.filter(x => x > 3)
来源：http://fv.panjiajie.cn

TS:   arr.filter(x => x > 3)
来源：http://mv.nszjky.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zt.shxzskj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://td.huixiangedu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ow.shxzukj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://gm.chemitech.net.cn

[D14] 映射转换（每个元素变形）
来源：http://wm.chemitech.net.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://um.yuexingan06.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yc.haigaiapp.cn

JS:   arr.map(x => x * 2)
来源：http://bn.shxzskj.cn

TS:   arr.map(x => x * 2)
来源：http://rp.newstarts.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://cg.hnjuh.cn

Go:   // 手写循环
来源：http://ft.521024.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qp.hahajie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://rm.lnxyls.cn

[D15] 去重
来源：http://ho.jctech888.com.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gw.hahajie.cn

PHP:  array_unique($arr);
来源：http://ik.jianghongdianzi.cn

JS:   [...new Set(arr)]
来源：http://hv.jctech888.com.cn

TS:   [...new Set(arr)]
来源：http://rq.bookmarksfly.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jr.szsharing.cn

Go:   // 用 map[T]struct{} 手写
来源：http://qb.lnxyls.cn

Ruby: arr.uniq
来源：http://hv.huanxung.cn

C#:   list.Distinct().ToList()
来源：http://py.bjjhwx.cn

[D16] 求和与平均值
来源：http://jh.szxytkj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pc.gzmigu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://di.szsharing.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qb.panjiajie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jx.wgjwhj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pr.yuntaijiaju.cn

Go:   // 手写循环累加
来源：http://we.jianghongdianzi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rb.hahajie.cn

C#:   list.Sum();  list.Average()
来源：http://ih.yuntaijiaju.cn

[D17] 最大值与最小值
来源：http://it.hnjuh.cn

Py:   max(arr);  min(arr)
来源：http://sc.haigaiapp.cn

PHP:  max($arr);  min($arr);
来源：http://li.bookmarksfly.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gi.shxzskj.cn

TS:   Math.max(...arr);
来源：http://uu.haigaiapp.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://hd.yuntaijiaju.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://uq.bookmarksfly.cn

Ruby: arr.max;  arr.min
来源：http://rd.gzmigu.cn

C#:   list.Max();  list.Min()
来源：http://ot.chemitech.net.cn

[D18] 扁平化嵌套数组
来源：http://gz.lnxyls.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bu.huixinmuqiang.cn

PHP:  array_merge(...$nested);
来源：http://xo.shxzukj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ld.chemitech.net.cn

TS:   nested.flat();
来源：http://rg.lnxyls.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qb.lnxyls.cn

Go:   // 手写双层循环
来源：http://tm.szxytkj.cn

Ruby: nested.flatten
来源：http://vy.shtwfgs.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://oo.nszjky.cn

[D19] 按字段分组
来源：http://gr.jianghongdianzi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wj.szsharing.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://br.yuntaijiaju.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yu.szsharing.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://fo.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tq.szsharing.cn

Go:   // 手写 map[string][]T
来源：http://eb.shxzskj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://qo.9csxet.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bw.hnjuh.cn

[D20] 统计每个元素出现次数
来源：http://zq.newstarts.cn

Py:   Counter(arr)
来源：http://ln.shtwfgs.cn

PHP:  array_count_values($arr);
来源：http://rk.jianghongdianzi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ov.shtwfgs.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xl.szsharing.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ez.colortex.cn

Go:   // 手写 map[T]int
来源：http://oi.jianghongdianzi.cn

Ruby: arr.tally
来源：http://fv.gzmigu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zf.hahajie.cn

[D21] 判断是否包含某元素
来源：http://cp.shtwfgs.cn

Py:   x in arr
来源：http://pd.gzmigu.cn

PHP:  in_array($x, $arr, true);
来源：http://cz.hahajie.cn

JS:   arr.includes(x)
来源：http://qz.panjiajie.cn

TS:   arr.includes(x)
来源：http://jx.lnxyls.cn

Java: list.contains(x)
来源：http://rq.shxzukj.cn

Go:   slices.Contains(arr, x)
来源：http://hc.lnxyls.cn

Ruby: arr.include?(x)
来源：http://dg.asd995.cn

C#:   list.Contains(x)
来源：http://ip.panjiajie.cn

[D22] 复制数组（避免共享引用）
来源：http://ci.hahajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wp.asd995.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fy.lnxyls.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nd.asd995.cn

TS:   [...arr];
来源：http://gn.gzmigu.cn

Java: new ArrayList<>(list);
来源：http://zm.shxzukj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qw.chemitech.net.cn

Ruby: arr.dup;  arr.clone
来源：http://li.gzmigu.cn

C#:   new List<int>(list);
来源：http://ae.nszjky.cn

[D23] reduce 累积计算
来源：http://jb.lnxyls.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dn.jctech888.com.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kg.chemitech.net.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kx.colortex.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gv.shxzukj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://zi.gzmigu.cn

Go:   // 手写循环
来源：http://zq.haigaiapp.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bx.bjjhwx.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ko.szxytkj.cn

[D24] 字典 / Map 基本操作
来源：http://dg.colortex.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uk.lnxyls.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bk.huixiangedu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bx.szsharing.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bw.gzmigu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qm.huanxung.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bb.yuntaijiaju.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://yw.jctech888.com.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://du.9csxet.cn

[D25] Set 集合去重与交并差
来源：http://pe.nszjky.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dd.haigaiapp.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://je.panjiajie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ta.hahajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://od.9csxet.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kd.shxzskj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xx.shtwfgs.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sg.colortex.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yx.nicolike.cn

[D26] 数组转字符串
来源：http://up.szxytkj.cn

Py:   ", ".join(map(str, arr))
来源：http://ca.gzmigu.cn

PHP:  implode(", ", $arr);
来源：http://wr.panjiajie.cn

JS:   arr.join(", ")
来源：http://ob.yuexingan06.cn

TS:   arr.join(", ")
来源：http://gv.bjjhwx.cn

Java: String.join(", ", list)
来源：http://jt.szsharing.cn

Go:   strings.Join(strs, ", ")
来源：http://rz.szxytkj.cn

Ruby: arr.join(", ")
来源：http://xx.9csxet.cn

C#:   string.Join(", ", list)
来源：http://lp.panjiajie.cn

================================================================================
来源：http://ic.wgjwhj.cn

E. 字符串处理
来源：http://fj.bookmarksfly.cn

================================================================================
来源：http://bv.colortex.cn

[E01] 拼接字符串
来源：http://nb.yuexingan06.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hu.9csxet.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kk.huixinmuqiang.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vb.lnxyls.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://iy.haigaiapp.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dq.shtwfgs.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ug.yuntaijiaju.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mn.shxzukj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qx.shxzskj.cn

[E02] 重复字符串
来源：http://vd.szxytkj.cn

Py:   "ab" * 3
来源：http://jp.huixiangedu.cn

PHP:  str_repeat("ab", 3);
来源：http://ta.hahajie.cn

JS:   "ab".repeat(3)
来源：http://id.huanxung.cn

TS:   "ab".repeat(3)
来源：http://fd.asd995.cn

Java: "ab".repeat(3)
来源：http://dn.lnxyls.cn

Go:   strings.Repeat("ab", 3)
来源：http://la.shtwfgs.cn

Ruby: "ab" * 3
来源：http://ya.nszjky.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jl.asd995.cn

[E03] 截取子串
来源：http://xm.asd995.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zk.521024.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ta.yuntaijiaju.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://it.chemitech.net.cn

TS:   s.slice(1, 4)
来源：http://wn.hahajie.cn

Java: s.substring(1, 4)
来源：http://nj.haigaiapp.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wo.jianghongdianzi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://wr.szsharing.cn

C#:   s.Substring(1, 3)
来源：http://zb.jianghongdianzi.cn

[E04] 查找子串位置
来源：http://uc.chemitech.net.cn

Py:   s.find("x");  s.index("x")
来源：http://zm.panjiajie.cn

PHP:  strpos($s, "x");
来源：http://gj.hnjuh.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yy.gzmigu.cn

TS:   s.indexOf("x")
来源：http://rn.szxytkj.cn

Java: s.indexOf("x")
来源：http://gf.yuexingan06.cn

Go:   strings.Index(s, "x")
来源：http://ff.huanxung.cn

Ruby: s.index("x")
来源：http://qu.colortex.cn

C#:   s.IndexOf("x")
来源：http://qc.shtwfgs.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://we.gzmigu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://sk.asd995.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rx.szxytkj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vh.shxzukj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zc.chemitech.net.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fp.wgjwhj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qf.muxihuayi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ck.panjiajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cs.bookmarksfly.cn

[E06] 替换子串
来源：http://mo.bookmarksfly.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://uk.szsharing.cn

PHP:  str_replace("a", "b", $s);
来源：http://on.szsharing.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iq.huanxung.cn

TS:   s.replaceAll("a", "b")
来源：http://dw.nszjky.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pb.gzmigu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jr.gzmigu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lz.9csxet.cn

C#:   s.Replace("a", "b")
来源：http://oz.nicolike.cn

[E07] 按分隔符拆分
来源：http://fs.yuntaijiaju.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gv.gzmigu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ho.bookmarksfly.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://rm.shtwfgs.cn

TS:   s.split(",")
来源：http://dh.huixiangedu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://fe.muxihuayi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ct.asd995.cn

Ruby: s.split(",");  s.split
来源：http://tk.bjjhwx.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vb.huixiangedu.cn

[E08] 数组按分隔符合并
来源：http://cs.haigaiapp.cn

Py:   ",".join(items)
来源：http://ao.colortex.cn

PHP:  implode(",", $items);
来源：http://th.newstarts.cn

JS:   items.join(",")
来源：http://jp.szxytkj.cn

TS:   items.join(",")
来源：http://yy.hahajie.cn

Java: String.join(",", items)
来源：http://iw.9csxet.cn

Go:   strings.Join(items, ",")
来源：http://xj.muxihuayi.cn

Ruby: items.join(",")
来源：http://gm.szxytkj.cn

C#:   string.Join(",", items)
来源：http://to.jctech888.com.cn

[E09] 去除所有空白字符
来源：http://fa.hahajie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hb.chemitech.net.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xz.szxytkj.cn

JS:   s.replace(/\s+/g, "")
来源：http://gx.9csxet.cn

TS:   s.replace(/\s+/g, "")
来源：http://tm.chemitech.net.cn

Java: s.replaceAll("\\s+", "")
来源：http://kh.nicolike.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://io.nicolike.cn

Ruby: s.gsub(/\s+/, "")
来源：http://zp.chemitech.net.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://iy.huixinmuqiang.cn

[E10] 左侧补零 / 定长填充
来源：http://ks.newstarts.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jg.huanxung.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qj.wgjwhj.cn

JS:   "7".padStart(3, "0")
来源：http://ar.gzmigu.cn

TS:   "7".padStart(3, "0")
来源：http://te.huixiangedu.cn

Java: String.format("%03d", 7)
来源：http://mr.yuexingan06.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://gq.szxytkj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://og.wgjwhj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ns.wgjwhj.cn

[E11] 反转字符串
来源：http://qx.jctech888.com.cn

Py:   s[::-1]
来源：http://qs.huixiangedu.cn

PHP:  strrev($s);
来源：http://jb.nszjky.cn

JS:   [...s].reverse().join("")
来源：http://wt.wgjwhj.cn

TS:   [...s].reverse().join("")
来源：http://dd.bjjhwx.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wq.9csxet.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://up.bjjhwx.cn

Ruby: s.reverse
来源：http://wd.chemitech.net.cn

C#:   new string(s.Reverse().ToArray())
来源：http://om.newstarts.cn

[E12] 统计某字符出现次数
来源：http://ui.huixiangedu.cn

Py:   s.count("a")
来源：http://he.colortex.cn

PHP:  substr_count($s, "a");
来源：http://ca.nicolike.cn

JS:   s.split("a").length - 1
来源：http://cf.chemitech.net.cn

TS:   s.split("a").length - 1
来源：http://um.huanxung.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qo.chemitech.net.cn

Go:   strings.Count(s, "a")
来源：http://hy.lnxyls.cn

Ruby: s.count("a")
来源：http://oy.bjjhwx.cn

C#:   s.Count(c => c == 'a')
来源：http://ya.hahajie.cn

[E13] 逐字符遍历
来源：http://nf.lnxyls.cn

Py:   for ch in s: print(ch)
来源：http://sa.shtwfgs.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://oi.shtwfgs.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://kw.jctech888.com.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bh.szxytkj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vi.muxihuayi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ds.521024.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ow.szxytkj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yw.asd995.cn

[E14] URL 编码与 Base64
来源：http://fz.szsharing.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://up.shtwfgs.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://am.nicolike.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ut.huixiangedu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nk.521024.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wx.huixinmuqiang.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qp.hnjuh.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qr.colortex.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ir.bookmarksfly.cn

[E15] HTML 转义 / 反转义
来源：http://cj.hahajie.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://cv.hahajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hn.yuexingan06.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rq.hahajie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://bs.521024.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ge.huixinmuqiang.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wp.jianghongdianzi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cx.shxzukj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zr.hahajie.cn

[E16] 数字千分位
来源：http://zq.9csxet.cn

Py:   f"{1234567:,}"
来源：http://qy.jctech888.com.cn

PHP:  number_format(1234567);
来源：http://wh.newstarts.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ey.chemitech.net.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://mi.nicolike.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mu.lnxyls.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mt.shxzukj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dy.haigaiapp.cn

C#:   1234567.ToString("N0")
来源：http://xs.chemitech.net.cn

[E17] 首字母大写
来源：http://iq.asd995.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pi.nicolike.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://py.panjiajie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dm.bookmarksfly.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fu.huixinmuqiang.cn


<!-- 参考信息 -->