代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fr.9csxet.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://du.szxytkj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xz.jianghongdianzi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fl.huanxung.cn

[D11] 反转数组
来源：http://pg.asd995.cn

Py:   arr[::-1];  arr.reverse()
来源：http://gg.asd995.cn

PHP:  array_reverse($arr);
来源：http://za.jctech888.com.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qc.hnjuh.cn

TS:   [...arr].reverse();
来源：http://ls.newstarts.cn

Java: Collections.reverse(list);
来源：http://yq.muxihuayi.cn

Go:   slices.Reverse(arr)
来源：http://xb.asd995.cn

Ruby: arr.reverse
来源：http://pn.haigaiapp.cn

C#:   list.Reverse();
来源：http://fu.jctech888.com.cn

[D12] 查找元素下标
来源：http://dp.panjiajie.cn

Py:   arr.index(x);  x in arr
来源：http://ha.521024.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mv.shxzukj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bg.yuntaijiaju.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fo.shxzskj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nv.wgjwhj.cn

Go:   slices.Index(arr, x)
来源：http://rb.huanxung.cn

Ruby: arr.index(x)
来源：http://ym.chemitech.net.cn

C#:   list.IndexOf(x);
来源：http://wg.yuntaijiaju.cn

[D13] 过滤（保留满足条件的）
来源：http://ye.haigaiapp.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hw.yuexingan06.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://an.newstarts.cn

JS:   arr.filter(x => x > 3)
来源：http://sa.szxytkj.cn

TS:   arr.filter(x => x > 3)
来源：http://hp.lnxyls.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fm.hnjuh.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mv.shxzskj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://oe.shxzukj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://bp.chemitech.net.cn

[D14] 映射转换（每个元素变形）
来源：http://tp.huixiangedu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nj.panjiajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cq.yuntaijiaju.cn

JS:   arr.map(x => x * 2)
来源：http://yy.lnxyls.cn

TS:   arr.map(x => x * 2)
来源：http://xv.nicolike.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://vi.szsharing.cn

Go:   // 手写循环
来源：http://wg.521024.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vj.szxytkj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://md.bookmarksfly.cn

[D15] 去重
来源：http://ay.jianghongdianzi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gr.gzmigu.cn

PHP:  array_unique($arr);
来源：http://jt.yuntaijiaju.cn

JS:   [...new Set(arr)]
来源：http://vm.jianghongdianzi.cn

TS:   [...new Set(arr)]
来源：http://yf.szxytkj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ga.jctech888.com.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xz.asd995.cn

Ruby: arr.uniq
来源：http://uy.nszjky.cn

C#:   list.Distinct().ToList()
来源：http://ik.jctech888.com.cn

[D16] 求和与平均值
来源：http://dj.panjiajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wd.huixiangedu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cr.huixinmuqiang.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://oq.panjiajie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rb.9csxet.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sj.huixinmuqiang.cn

Go:   // 手写循环累加
来源：http://ww.nszjky.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wg.huanxung.cn

C#:   list.Sum();  list.Average()
来源：http://fc.nszjky.cn

[D17] 最大值与最小值
来源：http://gv.asd995.cn

Py:   max(arr);  min(arr)
来源：http://qd.colortex.cn

PHP:  max($arr);  min($arr);
来源：http://pe.jctech888.com.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ox.chemitech.net.cn

TS:   Math.max(...arr);
来源：http://xv.nszjky.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jb.huixiangedu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fi.shxzukj.cn

Ruby: arr.max;  arr.min
来源：http://ql.muxihuayi.cn

C#:   list.Max();  list.Min()
来源：http://of.haigaiapp.cn

[D18] 扁平化嵌套数组
来源：http://sw.gzmigu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ba.yuntaijiaju.cn

PHP:  array_merge(...$nested);
来源：http://iv.haigaiapp.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://je.lnxyls.cn

TS:   nested.flat();
来源：http://ts.nicolike.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fm.shxzukj.cn

Go:   // 手写双层循环
来源：http://fd.nszjky.cn

Ruby: nested.flatten
来源：http://ed.hahajie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://bi.szsharing.cn

[D19] 按字段分组
来源：http://pv.shxzukj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://es.bookmarksfly.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vu.bookmarksfly.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kr.521024.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xm.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fv.nicolike.cn

Go:   // 手写 map[string][]T
来源：http://ss.hahajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://nq.shtwfgs.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pm.nszjky.cn

[D20] 统计每个元素出现次数
来源：http://cl.szsharing.cn

Py:   Counter(arr)
来源：http://di.jctech888.com.cn

PHP:  array_count_values($arr);
来源：http://ig.huixiangedu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ws.hahajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tk.asd995.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://iy.huixiangedu.cn

Go:   // 手写 map[T]int
来源：http://ea.gzmigu.cn

Ruby: arr.tally
来源：http://uo.hahajie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bc.yuexingan06.cn

[D21] 判断是否包含某元素
来源：http://xt.muxihuayi.cn

Py:   x in arr
来源：http://bh.szxytkj.cn

PHP:  in_array($x, $arr, true);
来源：http://ye.panjiajie.cn

JS:   arr.includes(x)
来源：http://tl.jianghongdianzi.cn

TS:   arr.includes(x)
来源：http://mo.gzmigu.cn

Java: list.contains(x)
来源：http://fg.colortex.cn

Go:   slices.Contains(arr, x)
来源：http://hf.muxihuayi.cn

Ruby: arr.include?(x)
来源：http://ac.panjiajie.cn

C#:   list.Contains(x)
来源：http://nk.hnjuh.cn

[D22] 复制数组（避免共享引用）
来源：http://mp.shtwfgs.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wi.yuntaijiaju.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ut.hnjuh.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hb.wgjwhj.cn

TS:   [...arr];
来源：http://qn.hnjuh.cn

Java: new ArrayList<>(list);
来源：http://wj.nszjky.cn

Go:   copied := append([]int(nil), arr...)
来源：http://db.haigaiapp.cn

Ruby: arr.dup;  arr.clone
来源：http://vf.newstarts.cn

C#:   new List<int>(list);
来源：http://pz.nicolike.cn

[D23] reduce 累积计算
来源：http://oo.colortex.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mb.colortex.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cu.jctech888.com.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://or.hahajie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xr.szxytkj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xz.szsharing.cn

Go:   // 手写循环
来源：http://mu.yuexingan06.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nn.newstarts.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wi.yuntaijiaju.cn

[D24] 字典 / Map 基本操作
来源：http://mn.nicolike.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zn.panjiajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gs.huanxung.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tj.wgjwhj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hd.jianghongdianzi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mq.hahajie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fp.asd995.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ky.shxzukj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ih.szxytkj.cn

[D25] Set 集合去重与交并差
来源：http://es.521024.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ls.colortex.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://km.szsharing.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lj.jianghongdianzi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ft.hnjuh.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rg.jianghongdianzi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ne.9csxet.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gq.hnjuh.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://go.huanxung.cn

[D26] 数组转字符串
来源：http://cd.wgjwhj.cn

Py:   ", ".join(map(str, arr))
来源：http://in.bjjhwx.cn

PHP:  implode(", ", $arr);
来源：http://ee.hnjuh.cn

JS:   arr.join(", ")
来源：http://ln.jianghongdianzi.cn

TS:   arr.join(", ")
来源：http://kf.hnjuh.cn

Java: String.join(", ", list)
来源：http://ks.colortex.cn

Go:   strings.Join(strs, ", ")
来源：http://us.huixinmuqiang.cn

Ruby: arr.join(", ")
来源：http://fi.shxzukj.cn

C#:   string.Join(", ", list)
来源：http://od.szsharing.cn

================================================================================
来源：http://po.shxzskj.cn

E. 字符串处理
来源：http://xy.chemitech.net.cn

================================================================================
来源：http://mh.muxihuayi.cn

[E01] 拼接字符串
来源：http://jh.nszjky.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xg.huanxung.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ag.haigaiapp.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://eu.wgjwhj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://td.colortex.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fb.yuexingan06.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hb.jianghongdianzi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pr.wgjwhj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yl.nszjky.cn

[E02] 重复字符串
来源：http://wf.huixinmuqiang.cn

Py:   "ab" * 3
来源：http://ag.shxzukj.cn

PHP:  str_repeat("ab", 3);
来源：http://lm.huixiangedu.cn

JS:   "ab".repeat(3)
来源：http://kd.shtwfgs.cn

TS:   "ab".repeat(3)
来源：http://dd.jianghongdianzi.cn

Java: "ab".repeat(3)
来源：http://rq.yuexingan06.cn

Go:   strings.Repeat("ab", 3)
来源：http://dm.jianghongdianzi.cn

Ruby: "ab" * 3
来源：http://yz.hnjuh.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uh.szxytkj.cn

[E03] 截取子串
来源：http://gc.yuntaijiaju.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ke.shxzskj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ki.wgjwhj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pb.shtwfgs.cn

TS:   s.slice(1, 4)
来源：http://ve.bookmarksfly.cn

Java: s.substring(1, 4)
来源：http://xq.szsharing.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ho.huanxung.cn

Ruby: s[1, 3];  s[1..3]
来源：http://hf.newstarts.cn

C#:   s.Substring(1, 3)
来源：http://po.huixinmuqiang.cn

[E04] 查找子串位置
来源：http://fs.panjiajie.cn

Py:   s.find("x");  s.index("x")
来源：http://bm.lnxyls.cn

PHP:  strpos($s, "x");
来源：http://gx.lnxyls.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vs.muxihuayi.cn

TS:   s.indexOf("x")
来源：http://df.haigaiapp.cn

Java: s.indexOf("x")
来源：http://uh.lnxyls.cn

Go:   strings.Index(s, "x")
来源：http://le.9csxet.cn

Ruby: s.index("x")
来源：http://oo.yuexingan06.cn

C#:   s.IndexOf("x")
来源：http://fd.wgjwhj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://pz.asd995.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://yd.9csxet.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ti.jianghongdianzi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uc.hnjuh.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xc.nicolike.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ko.asd995.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gy.bookmarksfly.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tn.szxytkj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://je.shxzskj.cn

[E06] 替换子串
来源：http://vq.jctech888.com.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ef.jctech888.com.cn

PHP:  str_replace("a", "b", $s);
来源：http://yi.shxzukj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kb.haigaiapp.cn

TS:   s.replaceAll("a", "b")
来源：http://qd.muxihuayi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ae.huixiangedu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gz.jianghongdianzi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mh.chemitech.net.cn

C#:   s.Replace("a", "b")
来源：http://hp.hahajie.cn

[E07] 按分隔符拆分
来源：http://sb.newstarts.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://om.huanxung.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ar.nicolike.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://qq.haigaiapp.cn

TS:   s.split(",")
来源：http://ou.hnjuh.cn

Java: s.split(",");  s.split("\\s+")
来源：http://tt.jctech888.com.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ko.nicolike.cn

Ruby: s.split(",");  s.split
来源：http://pi.wgjwhj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dv.shxzukj.cn

[E08] 数组按分隔符合并
来源：http://py.wgjwhj.cn

Py:   ",".join(items)
来源：http://zg.gzmigu.cn

PHP:  implode(",", $items);
来源：http://lp.yuexingan06.cn

JS:   items.join(",")
来源：http://ft.yuntaijiaju.cn

TS:   items.join(",")
来源：http://xm.gzmigu.cn

Java: String.join(",", items)
来源：http://sx.szxytkj.cn

Go:   strings.Join(items, ",")
来源：http://ud.bjjhwx.cn

Ruby: items.join(",")
来源：http://px.9csxet.cn

C#:   string.Join(",", items)
来源：http://ep.yuntaijiaju.cn

[E09] 去除所有空白字符
来源：http://mh.521024.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pa.yuexingan06.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://eg.szxytkj.cn

JS:   s.replace(/\s+/g, "")
来源：http://oh.huanxung.cn

TS:   s.replace(/\s+/g, "")
来源：http://qr.jianghongdianzi.cn

Java: s.replaceAll("\\s+", "")
来源：http://hn.newstarts.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://sw.bjjhwx.cn

Ruby: s.gsub(/\s+/, "")
来源：http://cm.muxihuayi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zo.wgjwhj.cn

[E10] 左侧补零 / 定长填充
来源：http://vh.huixiangedu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fr.lnxyls.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://yk.muxihuayi.cn

JS:   "7".padStart(3, "0")
来源：http://tb.yuexingan06.cn

TS:   "7".padStart(3, "0")
来源：http://sb.huixiangedu.cn

Java: String.format("%03d", 7)
来源：http://hb.asd995.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ys.9csxet.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wj.shxzskj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ab.nicolike.cn

[E11] 反转字符串
来源：http://uc.wgjwhj.cn

Py:   s[::-1]
来源：http://au.szsharing.cn

PHP:  strrev($s);
来源：http://ta.wgjwhj.cn

JS:   [...s].reverse().join("")
来源：http://av.chemitech.net.cn

TS:   [...s].reverse().join("")
来源：http://et.muxihuayi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ax.chemitech.net.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ja.bookmarksfly.cn

Ruby: s.reverse
来源：http://lj.shxzukj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vz.hahajie.cn

[E12] 统计某字符出现次数
来源：http://yg.bookmarksfly.cn

Py:   s.count("a")
来源：http://da.bjjhwx.cn

PHP:  substr_count($s, "a");
来源：http://cp.jianghongdianzi.cn

JS:   s.split("a").length - 1
来源：http://hf.nicolike.cn

TS:   s.split("a").length - 1
来源：http://ca.newstarts.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nr.shtwfgs.cn

Go:   strings.Count(s, "a")
来源：http://zf.huanxung.cn

Ruby: s.count("a")
来源：http://gd.bjjhwx.cn

C#:   s.Count(c => c == 'a')
来源：http://cc.hahajie.cn

[E13] 逐字符遍历
来源：http://ps.yuntaijiaju.cn

Py:   for ch in s: print(ch)
来源：http://jj.bookmarksfly.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kq.huixinmuqiang.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://nb.nszjky.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wj.shxzskj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pt.muxihuayi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ex.newstarts.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://be.hahajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nl.colortex.cn

[E14] URL 编码与 Base64
来源：http://li.chemitech.net.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tz.huixinmuqiang.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ga.panjiajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tj.yuntaijiaju.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://di.shxzukj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://am.chemitech.net.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://uy.wgjwhj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vm.bookmarksfly.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nm.huixinmuqiang.cn

[E15] HTML 转义 / 反转义
来源：http://nx.jianghongdianzi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://vy.huixiangedu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vt.chemitech.net.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qh.chemitech.net.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wy.shxzukj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vj.shxzukj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sw.nszjky.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ru.huixiangedu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tf.huixinmuqiang.cn

[E16] 数字千分位
来源：http://nv.muxihuayi.cn

Py:   f"{1234567:,}"
来源：http://ik.jctech888.com.cn

PHP:  number_format(1234567);
来源：http://la.hahajie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://eb.panjiajie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://cn.bookmarksfly.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rs.haigaiapp.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nq.haigaiapp.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://sj.521024.cn

C#:   1234567.ToString("N0")
来源：http://qx.huixiangedu.cn

[E17] 首字母大写
来源：http://zh.chemitech.net.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zk.shtwfgs.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://yq.nszjky.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://im.colortex.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zw.szsharing.cn


<!-- 参考信息 -->