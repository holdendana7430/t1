代发 wailian999

TS:   [...arr].reverse();
来源：http://ff.shtwfgs.cn

Java: Collections.reverse(list);
来源：http://pj.wgjwhj.cn

Go:   slices.Reverse(arr)
来源：http://em.bookmarksfly.cn

Ruby: arr.reverse
来源：http://ii.shxzskj.cn

C#:   list.Reverse();
来源：http://xu.bjjhwx.cn

[D12] 查找元素下标
来源：http://wb.nicolike.cn

Py:   arr.index(x);  x in arr
来源：http://kb.huixinmuqiang.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ys.haigaiapp.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rj.huanxung.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ub.haigaiapp.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wd.muxihuayi.cn

Go:   slices.Index(arr, x)
来源：http://cl.hahajie.cn

Ruby: arr.index(x)
来源：http://pc.yuntaijiaju.cn

C#:   list.IndexOf(x);
来源：http://zm.nicolike.cn

[D13] 过滤（保留满足条件的）
来源：http://kc.wgjwhj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nd.colortex.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://iv.szsharing.cn

JS:   arr.filter(x => x > 3)
来源：http://vu.bjjhwx.cn

TS:   arr.filter(x => x > 3)
来源：http://kf.panjiajie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://kf.nicolike.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xt.jctech888.com.cn

Ruby: arr.select { |x| x > 3 }
来源：http://sm.szxytkj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://dz.wgjwhj.cn

[D14] 映射转换（每个元素变形）
来源：http://ku.yuexingan06.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wg.hnjuh.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jo.jianghongdianzi.cn

JS:   arr.map(x => x * 2)
来源：http://pf.hahajie.cn

TS:   arr.map(x => x * 2)
来源：http://gm.haigaiapp.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://yi.bjjhwx.cn

Go:   // 手写循环
来源：http://si.9csxet.cn

Ruby: arr.map { |x| x * 2 }
来源：http://gp.bookmarksfly.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://cg.muxihuayi.cn

[D15] 去重
来源：http://zq.yuexingan06.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cc.wgjwhj.cn

PHP:  array_unique($arr);
来源：http://is.szxytkj.cn

JS:   [...new Set(arr)]
来源：http://ul.bookmarksfly.cn

TS:   [...new Set(arr)]
来源：http://zn.yuntaijiaju.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xd.huixiangedu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zb.shxzskj.cn

Ruby: arr.uniq
来源：http://sc.yuntaijiaju.cn

C#:   list.Distinct().ToList()
来源：http://hk.jctech888.com.cn

[D16] 求和与平均值
来源：http://nb.wgjwhj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nh.jianghongdianzi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://es.shxzukj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hd.9csxet.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ta.shtwfgs.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cw.haigaiapp.cn

Go:   // 手写循环累加
来源：http://ig.shxzskj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rq.asd995.cn

C#:   list.Sum();  list.Average()
来源：http://li.9csxet.cn

[D17] 最大值与最小值
来源：http://od.chemitech.net.cn

Py:   max(arr);  min(arr)
来源：http://qm.shtwfgs.cn

PHP:  max($arr);  min($arr);
来源：http://iy.wgjwhj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://th.yuexingan06.cn

TS:   Math.max(...arr);
来源：http://sf.gzmigu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://hi.colortex.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fb.gzmigu.cn

Ruby: arr.max;  arr.min
来源：http://aa.jianghongdianzi.cn

C#:   list.Max();  list.Min()
来源：http://tl.yuexingan06.cn

[D18] 扁平化嵌套数组
来源：http://ig.hahajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mp.shxzukj.cn

PHP:  array_merge(...$nested);
来源：http://wm.nszjky.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ui.wgjwhj.cn

TS:   nested.flat();
来源：http://dh.9csxet.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rp.shxzukj.cn

Go:   // 手写双层循环
来源：http://tn.hnjuh.cn

Ruby: nested.flatten
来源：http://zz.szxytkj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hc.521024.cn

[D19] 按字段分组
来源：http://sv.panjiajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pe.huixinmuqiang.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jj.szxytkj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xg.nicolike.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://rk.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wh.panjiajie.cn

Go:   // 手写 map[string][]T
来源：http://eo.shxzskj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fd.nicolike.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vv.muxihuayi.cn

[D20] 统计每个元素出现次数
来源：http://hj.lnxyls.cn

Py:   Counter(arr)
来源：http://uw.huanxung.cn

PHP:  array_count_values($arr);
来源：http://js.yuntaijiaju.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xv.521024.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bt.shxzskj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://oa.huanxung.cn

Go:   // 手写 map[T]int
来源：http://hi.panjiajie.cn

Ruby: arr.tally
来源：http://zj.asd995.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cf.yuexingan06.cn

[D21] 判断是否包含某元素
来源：http://nj.nszjky.cn

Py:   x in arr
来源：http://rh.521024.cn

PHP:  in_array($x, $arr, true);
来源：http://ej.hahajie.cn

JS:   arr.includes(x)
来源：http://ru.shxzukj.cn

TS:   arr.includes(x)
来源：http://dx.bookmarksfly.cn

Java: list.contains(x)
来源：http://vw.yuexingan06.cn

Go:   slices.Contains(arr, x)
来源：http://nj.yuntaijiaju.cn

Ruby: arr.include?(x)
来源：http://zc.nszjky.cn

C#:   list.Contains(x)
来源：http://ah.hnjuh.cn

[D22] 复制数组（避免共享引用）
来源：http://eo.bjjhwx.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pz.521024.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ky.huanxung.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xl.panjiajie.cn

TS:   [...arr];
来源：http://yr.hnjuh.cn

Java: new ArrayList<>(list);
来源：http://af.9csxet.cn

Go:   copied := append([]int(nil), arr...)
来源：http://mm.wgjwhj.cn

Ruby: arr.dup;  arr.clone
来源：http://hd.521024.cn

C#:   new List<int>(list);
来源：http://qr.colortex.cn

[D23] reduce 累积计算
来源：http://pb.521024.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mg.lnxyls.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uy.asd995.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pf.jctech888.com.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ak.wgjwhj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qp.jianghongdianzi.cn

Go:   // 手写循环
来源：http://px.muxihuayi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bo.521024.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ur.bookmarksfly.cn

[D24] 字典 / Map 基本操作
来源：http://sh.chemitech.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pn.huixiangedu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gs.panjiajie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xv.szsharing.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hn.gzmigu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jx.szsharing.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hp.521024.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kr.nszjky.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ab.yuntaijiaju.cn

[D25] Set 集合去重与交并差
来源：http://jh.lnxyls.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rx.shtwfgs.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dh.szxytkj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qv.hahajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nn.haigaiapp.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fs.bjjhwx.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jk.yuntaijiaju.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ut.nicolike.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ji.gzmigu.cn

[D26] 数组转字符串
来源：http://dd.huixinmuqiang.cn

Py:   ", ".join(map(str, arr))
来源：http://eg.muxihuayi.cn

PHP:  implode(", ", $arr);
来源：http://ht.huixinmuqiang.cn

JS:   arr.join(", ")
来源：http://zq.jctech888.com.cn

TS:   arr.join(", ")
来源：http://pt.jctech888.com.cn

Java: String.join(", ", list)
来源：http://to.lnxyls.cn

Go:   strings.Join(strs, ", ")
来源：http://df.hnjuh.cn

Ruby: arr.join(", ")
来源：http://sf.newstarts.cn

C#:   string.Join(", ", list)
来源：http://ie.jctech888.com.cn

================================================================================
来源：http://fg.panjiajie.cn

E. 字符串处理
来源：http://ph.newstarts.cn

================================================================================
来源：http://ae.asd995.cn

[E01] 拼接字符串
来源：http://ky.colortex.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pg.huanxung.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wu.yuexingan06.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lh.haigaiapp.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vu.yuntaijiaju.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cf.jianghongdianzi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kx.asd995.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ok.newstarts.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lw.szsharing.cn

[E02] 重复字符串
来源：http://fp.nszjky.cn

Py:   "ab" * 3
来源：http://rs.szxytkj.cn

PHP:  str_repeat("ab", 3);
来源：http://oq.muxihuayi.cn

JS:   "ab".repeat(3)
来源：http://jv.9csxet.cn

TS:   "ab".repeat(3)
来源：http://bg.hnjuh.cn

Java: "ab".repeat(3)
来源：http://iz.huanxung.cn

Go:   strings.Repeat("ab", 3)
来源：http://zs.lnxyls.cn

Ruby: "ab" * 3
来源：http://pz.shxzskj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://oa.newstarts.cn

[E03] 截取子串
来源：http://zp.huixinmuqiang.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nd.shtwfgs.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://sc.9csxet.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://iy.lnxyls.cn

TS:   s.slice(1, 4)
来源：http://as.jctech888.com.cn

Java: s.substring(1, 4)
来源：http://ei.asd995.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rg.muxihuayi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://gx.shxzukj.cn

C#:   s.Substring(1, 3)
来源：http://iw.yuntaijiaju.cn

[E04] 查找子串位置
来源：http://tu.huixiangedu.cn

Py:   s.find("x");  s.index("x")
来源：http://an.521024.cn

PHP:  strpos($s, "x");
来源：http://jr.huanxung.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kb.shxzukj.cn

TS:   s.indexOf("x")
来源：http://dm.huixinmuqiang.cn

Java: s.indexOf("x")
来源：http://fj.hahajie.cn

Go:   strings.Index(s, "x")
来源：http://sv.newstarts.cn

Ruby: s.index("x")
来源：http://hb.lnxyls.cn

C#:   s.IndexOf("x")
来源：http://rj.nszjky.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://bg.gzmigu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ll.nicolike.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nm.hahajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pg.lnxyls.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://vk.nicolike.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hj.huixiangedu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tz.yuntaijiaju.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://an.wgjwhj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ng.jctech888.com.cn

[E06] 替换子串
来源：http://wl.huixinmuqiang.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kx.szsharing.cn

PHP:  str_replace("a", "b", $s);
来源：http://ra.muxihuayi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nd.9csxet.cn

TS:   s.replaceAll("a", "b")
来源：http://te.colortex.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bt.hahajie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fk.521024.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ae.muxihuayi.cn

C#:   s.Replace("a", "b")
来源：http://ga.lnxyls.cn

[E07] 按分隔符拆分
来源：http://aq.shxzskj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ak.bjjhwx.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lx.lnxyls.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://lb.asd995.cn

TS:   s.split(",")
来源：http://nu.huixinmuqiang.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zy.shtwfgs.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://us.panjiajie.cn

Ruby: s.split(",");  s.split
来源：http://js.gzmigu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kv.shtwfgs.cn

[E08] 数组按分隔符合并
来源：http://wj.bookmarksfly.cn

Py:   ",".join(items)
来源：http://lu.hnjuh.cn

PHP:  implode(",", $items);
来源：http://sp.muxihuayi.cn

JS:   items.join(",")
来源：http://re.bookmarksfly.cn

TS:   items.join(",")
来源：http://tv.wgjwhj.cn

Java: String.join(",", items)
来源：http://rc.szxytkj.cn

Go:   strings.Join(items, ",")
来源：http://to.hnjuh.cn

Ruby: items.join(",")
来源：http://au.hnjuh.cn

C#:   string.Join(",", items)
来源：http://xb.szsharing.cn

[E09] 去除所有空白字符
来源：http://ug.huanxung.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://yb.szxytkj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gr.9csxet.cn

JS:   s.replace(/\s+/g, "")
来源：http://aj.bjjhwx.cn

TS:   s.replace(/\s+/g, "")
来源：http://dd.shxzukj.cn

Java: s.replaceAll("\\s+", "")
来源：http://zk.bookmarksfly.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://hl.colortex.cn

Ruby: s.gsub(/\s+/, "")
来源：http://wy.wgjwhj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://at.yuexingan06.cn

[E10] 左侧补零 / 定长填充
来源：http://dz.bookmarksfly.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nq.haigaiapp.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fm.colortex.cn

JS:   "7".padStart(3, "0")
来源：http://yb.bjjhwx.cn

TS:   "7".padStart(3, "0")
来源：http://rw.asd995.cn

Java: String.format("%03d", 7)
来源：http://nw.lnxyls.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ns.muxihuayi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mf.muxihuayi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mf.huixiangedu.cn

[E11] 反转字符串
来源：http://ca.muxihuayi.cn

Py:   s[::-1]
来源：http://vg.gzmigu.cn

PHP:  strrev($s);
来源：http://jf.lnxyls.cn

JS:   [...s].reverse().join("")
来源：http://jm.yuntaijiaju.cn

TS:   [...s].reverse().join("")
来源：http://mx.shxzskj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://gi.9csxet.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://fj.chemitech.net.cn

Ruby: s.reverse
来源：http://je.nicolike.cn

C#:   new string(s.Reverse().ToArray())
来源：http://dq.yuntaijiaju.cn

[E12] 统计某字符出现次数
来源：http://wo.colortex.cn

Py:   s.count("a")
来源：http://zu.muxihuayi.cn

PHP:  substr_count($s, "a");
来源：http://ed.chemitech.net.cn

JS:   s.split("a").length - 1
来源：http://aw.chemitech.net.cn

TS:   s.split("a").length - 1
来源：http://ws.huixiangedu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nc.gzmigu.cn

Go:   strings.Count(s, "a")
来源：http://ig.asd995.cn

Ruby: s.count("a")
来源：http://lx.huixiangedu.cn

C#:   s.Count(c => c == 'a')
来源：http://sy.asd995.cn

[E13] 逐字符遍历
来源：http://nu.hnjuh.cn

Py:   for ch in s: print(ch)
来源：http://xk.jctech888.com.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sa.shxzukj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ry.panjiajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://tb.jctech888.com.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zb.bjjhwx.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://py.muxihuayi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://nl.newstarts.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qc.shxzukj.cn

[E14] URL 编码与 Base64
来源：http://el.jctech888.com.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hi.lnxyls.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://nn.hahajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bi.asd995.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kc.haigaiapp.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cl.shxzukj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://es.shtwfgs.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ef.szsharing.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ww.gzmigu.cn

[E15] HTML 转义 / 反转义
来源：http://oj.chemitech.net.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://dc.jianghongdianzi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rg.huixinmuqiang.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fl.9csxet.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://zu.9csxet.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://og.shxzukj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://da.wgjwhj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nl.nszjky.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tx.bookmarksfly.cn

[E16] 数字千分位
来源：http://cz.9csxet.cn

Py:   f"{1234567:,}"
来源：http://cr.shtwfgs.cn

PHP:  number_format(1234567);
来源：http://py.huixinmuqiang.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://kt.yuexingan06.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://fv.szsharing.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qj.jctech888.com.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fd.jctech888.com.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dk.huanxung.cn

C#:   1234567.ToString("N0")
来源：http://zc.colortex.cn

[E17] 首字母大写
来源：http://dw.bookmarksfly.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ud.huanxung.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://cp.9csxet.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fb.hnjuh.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://td.shxzukj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cw.521024.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tq.haigaiapp.cn

Ruby: s.capitalize
来源：http://nu.muxihuayi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://sa.lnxyls.cn

[E18] 模板占位符替换
来源：http://pd.521024.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ry.bjjhwx.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pq.asd995.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ub.bjjhwx.cn


<!-- 参考信息 -->