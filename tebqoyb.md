代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://is.szsharing.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xx.shtwfgs.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xj.bookmarksfly.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dl.newstarts.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://sc.bjjhwx.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lx.hahajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ot.hahajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wb.panjiajie.cn

[D11] 反转数组
来源：http://ky.colortex.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ft.hnjuh.cn

PHP:  array_reverse($arr);
来源：http://ch.asd995.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zr.521024.cn

TS:   [...arr].reverse();
来源：http://xf.yuntaijiaju.cn

Java: Collections.reverse(list);
来源：http://ap.521024.cn

Go:   slices.Reverse(arr)
来源：http://pu.wgjwhj.cn

Ruby: arr.reverse
来源：http://sv.panjiajie.cn

C#:   list.Reverse();
来源：http://di.chemitech.net.cn

[D12] 查找元素下标
来源：http://cd.gzmigu.cn

Py:   arr.index(x);  x in arr
来源：http://bd.colortex.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jx.shxzukj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fl.yuntaijiaju.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xz.hnjuh.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xt.newstarts.cn

Go:   slices.Index(arr, x)
来源：http://gv.huixiangedu.cn

Ruby: arr.index(x)
来源：http://hy.chemitech.net.cn

C#:   list.IndexOf(x);
来源：http://bm.szxytkj.cn

[D13] 过滤（保留满足条件的）
来源：http://hs.haigaiapp.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ho.szsharing.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fp.shxzukj.cn

JS:   arr.filter(x => x > 3)
来源：http://mj.shtwfgs.cn

TS:   arr.filter(x => x > 3)
来源：http://bl.yuntaijiaju.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bs.asd995.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qn.muxihuayi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://cy.szsharing.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vp.szxytkj.cn

[D14] 映射转换（每个元素变形）
来源：http://gy.szxytkj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nk.yuexingan06.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sq.chemitech.net.cn

JS:   arr.map(x => x * 2)
来源：http://ox.szsharing.cn

TS:   arr.map(x => x * 2)
来源：http://ka.nicolike.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://pd.jctech888.com.cn

Go:   // 手写循环
来源：http://dr.bookmarksfly.cn

Ruby: arr.map { |x| x * 2 }
来源：http://bs.shxzukj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://bd.shxzskj.cn

[D15] 去重
来源：http://kj.huanxung.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cp.panjiajie.cn

PHP:  array_unique($arr);
来源：http://jl.yuexingan06.cn

JS:   [...new Set(arr)]
来源：http://lx.huanxung.cn

TS:   [...new Set(arr)]
来源：http://hk.shtwfgs.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mm.hnjuh.cn

Go:   // 用 map[T]struct{} 手写
来源：http://nd.lnxyls.cn

Ruby: arr.uniq
来源：http://ma.szsharing.cn

C#:   list.Distinct().ToList()
来源：http://hv.muxihuayi.cn

[D16] 求和与平均值
来源：http://dc.huixiangedu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mh.newstarts.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bc.yuntaijiaju.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zk.hahajie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gf.jianghongdianzi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://af.wgjwhj.cn

Go:   // 手写循环累加
来源：http://em.gzmigu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fn.asd995.cn

C#:   list.Sum();  list.Average()
来源：http://jy.huixinmuqiang.cn

[D17] 最大值与最小值
来源：http://ju.yuntaijiaju.cn

Py:   max(arr);  min(arr)
来源：http://cl.bookmarksfly.cn

PHP:  max($arr);  min($arr);
来源：http://nq.szxytkj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ak.szsharing.cn

TS:   Math.max(...arr);
来源：http://lf.shtwfgs.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://uc.panjiajie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bb.shxzskj.cn

Ruby: arr.max;  arr.min
来源：http://sc.wgjwhj.cn

C#:   list.Max();  list.Min()
来源：http://eb.shtwfgs.cn

[D18] 扁平化嵌套数组
来源：http://kb.shxzukj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sn.panjiajie.cn

PHP:  array_merge(...$nested);
来源：http://el.nicolike.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://av.jctech888.com.cn

TS:   nested.flat();
来源：http://lq.huixinmuqiang.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tn.shtwfgs.cn

Go:   // 手写双层循环
来源：http://oc.hahajie.cn

Ruby: nested.flatten
来源：http://kn.haigaiapp.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://aw.nszjky.cn

[D19] 按字段分组
来源：http://gj.panjiajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kc.asd995.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nd.521024.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rl.newstarts.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://wo.nicolike.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yt.bookmarksfly.cn

Go:   // 手写 map[string][]T
来源：http://yv.newstarts.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rx.gzmigu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ia.asd995.cn

[D20] 统计每个元素出现次数
来源：http://du.hnjuh.cn

Py:   Counter(arr)
来源：http://iu.lnxyls.cn

PHP:  array_count_values($arr);
来源：http://ou.colortex.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tw.huixinmuqiang.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nd.gzmigu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cb.asd995.cn

Go:   // 手写 map[T]int
来源：http://tz.yuexingan06.cn

Ruby: arr.tally
来源：http://wp.521024.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ua.bjjhwx.cn

[D21] 判断是否包含某元素
来源：http://wt.muxihuayi.cn

Py:   x in arr
来源：http://en.yuntaijiaju.cn

PHP:  in_array($x, $arr, true);
来源：http://cz.asd995.cn

JS:   arr.includes(x)
来源：http://fp.gzmigu.cn

TS:   arr.includes(x)
来源：http://ae.hnjuh.cn

Java: list.contains(x)
来源：http://pz.asd995.cn

Go:   slices.Contains(arr, x)
来源：http://jt.jctech888.com.cn

Ruby: arr.include?(x)
来源：http://uj.asd995.cn

C#:   list.Contains(x)
来源：http://gq.9csxet.cn

[D22] 复制数组（避免共享引用）
来源：http://vw.huixiangedu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dd.huixiangedu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gx.shxzukj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nh.wgjwhj.cn

TS:   [...arr];
来源：http://kg.wgjwhj.cn

Java: new ArrayList<>(list);
来源：http://fp.shtwfgs.cn

Go:   copied := append([]int(nil), arr...)
来源：http://zx.9csxet.cn

Ruby: arr.dup;  arr.clone
来源：http://dh.yuntaijiaju.cn

C#:   new List<int>(list);
来源：http://re.yuexingan06.cn

[D23] reduce 累积计算
来源：http://lh.shxzskj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cw.huanxung.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ol.yuntaijiaju.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yh.huanxung.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ra.haigaiapp.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://so.colortex.cn

Go:   // 手写循环
来源：http://iy.huixiangedu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vy.9csxet.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cx.yuntaijiaju.cn

[D24] 字典 / Map 基本操作
来源：http://pc.gzmigu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vi.asd995.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kt.hnjuh.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qy.panjiajie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://iy.yuexingan06.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ut.shxzukj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://be.szxytkj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://re.hahajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vi.chemitech.net.cn

[D25] Set 集合去重与交并差
来源：http://vc.nszjky.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rw.huanxung.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://oh.bookmarksfly.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lu.lnxyls.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qz.panjiajie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vr.yuntaijiaju.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://oo.asd995.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lw.shtwfgs.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://aj.shtwfgs.cn

[D26] 数组转字符串
来源：http://xv.huixinmuqiang.cn

Py:   ", ".join(map(str, arr))
来源：http://tc.shxzskj.cn

PHP:  implode(", ", $arr);
来源：http://nl.shxzskj.cn

JS:   arr.join(", ")
来源：http://li.nicolike.cn

TS:   arr.join(", ")
来源：http://ag.lnxyls.cn

Java: String.join(", ", list)
来源：http://ci.yuntaijiaju.cn

Go:   strings.Join(strs, ", ")
来源：http://tk.nszjky.cn

Ruby: arr.join(", ")
来源：http://wt.nszjky.cn

C#:   string.Join(", ", list)
来源：http://cd.colortex.cn

================================================================================
来源：http://dr.9csxet.cn

E. 字符串处理
来源：http://ik.bjjhwx.cn

================================================================================
来源：http://aj.yuexingan06.cn

[E01] 拼接字符串
来源：http://zr.muxihuayi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://io.huixinmuqiang.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kb.lnxyls.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kz.panjiajie.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://iq.nszjky.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hf.yuexingan06.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lc.szxytkj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ss.asd995.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://if.gzmigu.cn

[E02] 重复字符串
来源：http://pi.yuexingan06.cn

Py:   "ab" * 3
来源：http://gl.panjiajie.cn

PHP:  str_repeat("ab", 3);
来源：http://om.muxihuayi.cn

JS:   "ab".repeat(3)
来源：http://mp.bjjhwx.cn

TS:   "ab".repeat(3)
来源：http://ec.haigaiapp.cn

Java: "ab".repeat(3)
来源：http://qa.jctech888.com.cn

Go:   strings.Repeat("ab", 3)
来源：http://is.colortex.cn

Ruby: "ab" * 3
来源：http://sg.szxytkj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ae.huanxung.cn

[E03] 截取子串
来源：http://fx.muxihuayi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mr.hnjuh.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ae.huixinmuqiang.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ar.huixiangedu.cn

TS:   s.slice(1, 4)
来源：http://cn.hnjuh.cn

Java: s.substring(1, 4)
来源：http://hd.szsharing.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pn.newstarts.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ex.jianghongdianzi.cn

C#:   s.Substring(1, 3)
来源：http://tv.hnjuh.cn

[E04] 查找子串位置
来源：http://no.shxzukj.cn

Py:   s.find("x");  s.index("x")
来源：http://wu.szsharing.cn

PHP:  strpos($s, "x");
来源：http://qj.szsharing.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sk.huixiangedu.cn

TS:   s.indexOf("x")
来源：http://rk.huanxung.cn

Java: s.indexOf("x")
来源：http://fc.shtwfgs.cn

Go:   strings.Index(s, "x")
来源：http://di.wgjwhj.cn

Ruby: s.index("x")
来源：http://ub.huixiangedu.cn

C#:   s.IndexOf("x")
来源：http://tx.9csxet.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://au.szsharing.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jm.521024.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://es.nszjky.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wd.gzmigu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xi.szxytkj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ts.nszjky.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://io.muxihuayi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ou.newstarts.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hf.gzmigu.cn

[E06] 替换子串
来源：http://wd.hnjuh.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ir.shxzukj.cn

PHP:  str_replace("a", "b", $s);
来源：http://je.muxihuayi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hk.haigaiapp.cn

TS:   s.replaceAll("a", "b")
来源：http://ck.szsharing.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wp.szxytkj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hs.yuntaijiaju.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ni.nicolike.cn

C#:   s.Replace("a", "b")
来源：http://zm.yuexingan06.cn

[E07] 按分隔符拆分
来源：http://ub.yuexingan06.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ov.shxzskj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xf.hnjuh.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ay.shxzukj.cn

TS:   s.split(",")
来源：http://jb.bjjhwx.cn

Java: s.split(",");  s.split("\\s+")
来源：http://lf.chemitech.net.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kt.bookmarksfly.cn

Ruby: s.split(",");  s.split
来源：http://hz.huixiangedu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://eo.muxihuayi.cn

[E08] 数组按分隔符合并
来源：http://by.szxytkj.cn

Py:   ",".join(items)
来源：http://gy.muxihuayi.cn

PHP:  implode(",", $items);
来源：http://hp.newstarts.cn

JS:   items.join(",")
来源：http://fb.yuntaijiaju.cn

TS:   items.join(",")
来源：http://aw.szxytkj.cn

Java: String.join(",", items)
来源：http://os.colortex.cn

Go:   strings.Join(items, ",")
来源：http://ix.panjiajie.cn

Ruby: items.join(",")
来源：http://zb.huanxung.cn

C#:   string.Join(",", items)
来源：http://se.yuexingan06.cn

[E09] 去除所有空白字符
来源：http://mb.huanxung.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ht.shtwfgs.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ce.jctech888.com.cn

JS:   s.replace(/\s+/g, "")
来源：http://cm.colortex.cn

TS:   s.replace(/\s+/g, "")
来源：http://cs.lnxyls.cn

Java: s.replaceAll("\\s+", "")
来源：http://zo.haigaiapp.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://we.lnxyls.cn

Ruby: s.gsub(/\s+/, "")
来源：http://du.hahajie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://co.muxihuayi.cn

[E10] 左侧补零 / 定长填充
来源：http://my.nicolike.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pm.jctech888.com.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://il.9csxet.cn

JS:   "7".padStart(3, "0")
来源：http://eu.huanxung.cn

TS:   "7".padStart(3, "0")
来源：http://ab.gzmigu.cn

Java: String.format("%03d", 7)
来源：http://hl.hahajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://rf.nszjky.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://iz.521024.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wy.asd995.cn

[E11] 反转字符串
来源：http://ne.haigaiapp.cn

Py:   s[::-1]
来源：http://me.panjiajie.cn

PHP:  strrev($s);
来源：http://wo.yuntaijiaju.cn

JS:   [...s].reverse().join("")
来源：http://ms.newstarts.cn

TS:   [...s].reverse().join("")
来源：http://sz.shxzukj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://te.huixinmuqiang.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://gl.colortex.cn

Ruby: s.reverse
来源：http://so.yuntaijiaju.cn

C#:   new string(s.Reverse().ToArray())
来源：http://xh.yuntaijiaju.cn

[E12] 统计某字符出现次数
来源：http://xx.yuexingan06.cn

Py:   s.count("a")
来源：http://ap.shxzukj.cn

PHP:  substr_count($s, "a");
来源：http://ef.chemitech.net.cn

JS:   s.split("a").length - 1
来源：http://jf.wgjwhj.cn

TS:   s.split("a").length - 1
来源：http://dp.9csxet.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qw.colortex.cn

Go:   strings.Count(s, "a")
来源：http://uv.chemitech.net.cn

Ruby: s.count("a")
来源：http://vd.yuexingan06.cn

C#:   s.Count(c => c == 'a')
来源：http://wd.lnxyls.cn

[E13] 逐字符遍历
来源：http://wl.muxihuayi.cn

Py:   for ch in s: print(ch)
来源：http://au.9csxet.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yp.muxihuayi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://lx.nszjky.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ke.shtwfgs.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kh.hahajie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tf.shtwfgs.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://xy.chemitech.net.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ea.yuntaijiaju.cn

[E14] URL 编码与 Base64
来源：http://ve.521024.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qk.shtwfgs.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://oh.huixinmuqiang.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ag.wgjwhj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fc.shxzskj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dc.huixiangedu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jn.huixiangedu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ub.bookmarksfly.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sc.bjjhwx.cn

[E15] HTML 转义 / 反转义
来源：http://dh.szxytkj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xi.chemitech.net.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ht.bookmarksfly.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rv.nszjky.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://bd.newstarts.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://oh.nszjky.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dw.521024.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://na.nszjky.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lj.panjiajie.cn

[E16] 数字千分位
来源：http://iq.lnxyls.cn

Py:   f"{1234567:,}"
来源：http://bp.lnxyls.cn

PHP:  number_format(1234567);
来源：http://ip.huixiangedu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://zb.jianghongdianzi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://bc.huixinmuqiang.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ls.szsharing.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bc.jctech888.com.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ta.szxytkj.cn

C#:   1234567.ToString("N0")
来源：http://uh.haigaiapp.cn

[E17] 首字母大写
来源：http://eh.yuexingan06.cn


<!-- 参考信息 -->