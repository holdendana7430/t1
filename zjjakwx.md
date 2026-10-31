代发 wailian999

C#:   list.Reverse();
来源：http://dr.jctech888.com.cn

[D12] 查找元素下标
来源：http://md.jianghongdianzi.cn

Py:   arr.index(x);  x in arr
来源：http://ui.hnjuh.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://om.shxzukj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tg.lnxyls.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lx.haigaiapp.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wx.shxzukj.cn

Go:   slices.Index(arr, x)
来源：http://nh.521024.cn

Ruby: arr.index(x)
来源：http://ja.haigaiapp.cn

C#:   list.IndexOf(x);
来源：http://ko.521024.cn

[D13] 过滤（保留满足条件的）
来源：http://lj.bjjhwx.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qd.yuexingan06.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jm.9csxet.cn

JS:   arr.filter(x => x > 3)
来源：http://cg.yuntaijiaju.cn

TS:   arr.filter(x => x > 3)
来源：http://ve.huixinmuqiang.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vj.gzmigu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wb.nszjky.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ck.gzmigu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ls.9csxet.cn

[D14] 映射转换（每个元素变形）
来源：http://bn.9csxet.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pp.haigaiapp.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ci.jianghongdianzi.cn

JS:   arr.map(x => x * 2)
来源：http://wx.nicolike.cn

TS:   arr.map(x => x * 2)
来源：http://ur.szsharing.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://so.szxytkj.cn

Go:   // 手写循环
来源：http://zk.szsharing.cn

Ruby: arr.map { |x| x * 2 }
来源：http://oc.hnjuh.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://dx.yuexingan06.cn

[D15] 去重
来源：http://wf.hnjuh.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kp.521024.cn

PHP:  array_unique($arr);
来源：http://do.szsharing.cn

JS:   [...new Set(arr)]
来源：http://me.jctech888.com.cn

TS:   [...new Set(arr)]
来源：http://uq.nszjky.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ou.hahajie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://fq.huixinmuqiang.cn

Ruby: arr.uniq
来源：http://ui.nicolike.cn

C#:   list.Distinct().ToList()
来源：http://ja.shtwfgs.cn

[D16] 求和与平均值
来源：http://ho.huanxung.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ix.szxytkj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://el.nszjky.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yt.huixinmuqiang.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ad.yuntaijiaju.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dt.szsharing.cn

Go:   // 手写循环累加
来源：http://vy.newstarts.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pt.muxihuayi.cn

C#:   list.Sum();  list.Average()
来源：http://up.shxzukj.cn

[D17] 最大值与最小值
来源：http://qh.haigaiapp.cn

Py:   max(arr);  min(arr)
来源：http://jg.muxihuayi.cn

PHP:  max($arr);  min($arr);
来源：http://mi.bjjhwx.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ap.521024.cn

TS:   Math.max(...arr);
来源：http://tg.shtwfgs.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://lt.szxytkj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://by.shtwfgs.cn

Ruby: arr.max;  arr.min
来源：http://cv.asd995.cn

C#:   list.Max();  list.Min()
来源：http://np.huixiangedu.cn

[D18] 扁平化嵌套数组
来源：http://fx.huixinmuqiang.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://th.yuexingan06.cn

PHP:  array_merge(...$nested);
来源：http://ha.lnxyls.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xf.huixiangedu.cn

TS:   nested.flat();
来源：http://ig.gzmigu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cu.bookmarksfly.cn

Go:   // 手写双层循环
来源：http://ji.bookmarksfly.cn

Ruby: nested.flatten
来源：http://br.asd995.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ov.bookmarksfly.cn

[D19] 按字段分组
来源：http://is.hahajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://va.9csxet.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ae.haigaiapp.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zm.szsharing.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://oy.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://in.panjiajie.cn

Go:   // 手写 map[string][]T
来源：http://kk.panjiajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://xj.szsharing.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gu.9csxet.cn

[D20] 统计每个元素出现次数
来源：http://gl.muxihuayi.cn

Py:   Counter(arr)
来源：http://wp.szsharing.cn

PHP:  array_count_values($arr);
来源：http://ld.jctech888.com.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gn.521024.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kq.gzmigu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wu.huixinmuqiang.cn

Go:   // 手写 map[T]int
来源：http://or.hnjuh.cn

Ruby: arr.tally
来源：http://cq.9csxet.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zy.asd995.cn

[D21] 判断是否包含某元素
来源：http://vu.asd995.cn

Py:   x in arr
来源：http://jx.9csxet.cn

PHP:  in_array($x, $arr, true);
来源：http://hn.jctech888.com.cn

JS:   arr.includes(x)
来源：http://os.jctech888.com.cn

TS:   arr.includes(x)
来源：http://tj.lnxyls.cn

Java: list.contains(x)
来源：http://dv.521024.cn

Go:   slices.Contains(arr, x)
来源：http://vp.szsharing.cn

Ruby: arr.include?(x)
来源：http://lr.shxzskj.cn

C#:   list.Contains(x)
来源：http://cx.huixiangedu.cn

[D22] 复制数组（避免共享引用）
来源：http://ag.gzmigu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ge.shtwfgs.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vj.521024.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kp.szxytkj.cn

TS:   [...arr];
来源：http://sp.shxzukj.cn

Java: new ArrayList<>(list);
来源：http://zi.wgjwhj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cl.szxytkj.cn

Ruby: arr.dup;  arr.clone
来源：http://df.haigaiapp.cn

C#:   new List<int>(list);
来源：http://wn.gzmigu.cn

[D23] reduce 累积计算
来源：http://oa.szsharing.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sk.szxytkj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kc.lnxyls.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://on.yuntaijiaju.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lk.asd995.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://hv.newstarts.cn

Go:   // 手写循环
来源：http://ws.huanxung.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ix.huanxung.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ds.shxzukj.cn

[D24] 字典 / Map 基本操作
来源：http://eh.gzmigu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pm.nszjky.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vs.jianghongdianzi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bz.hnjuh.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zh.haigaiapp.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uu.panjiajie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zl.shxzukj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dc.shtwfgs.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lh.haigaiapp.cn

[D25] Set 集合去重与交并差
来源：http://lq.bjjhwx.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ek.chemitech.net.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jy.gzmigu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tj.muxihuayi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jc.gzmigu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pg.chemitech.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vi.jctech888.com.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vg.gzmigu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vy.bookmarksfly.cn

[D26] 数组转字符串
来源：http://wc.9csxet.cn

Py:   ", ".join(map(str, arr))
来源：http://da.gzmigu.cn

PHP:  implode(", ", $arr);
来源：http://qn.asd995.cn

JS:   arr.join(", ")
来源：http://rn.yuntaijiaju.cn

TS:   arr.join(", ")
来源：http://yd.muxihuayi.cn

Java: String.join(", ", list)
来源：http://ck.hnjuh.cn

Go:   strings.Join(strs, ", ")
来源：http://pb.newstarts.cn

Ruby: arr.join(", ")
来源：http://pi.jianghongdianzi.cn

C#:   string.Join(", ", list)
来源：http://qq.muxihuayi.cn

================================================================================
来源：http://gx.asd995.cn

E. 字符串处理
来源：http://il.shxzukj.cn

================================================================================
来源：http://nr.jctech888.com.cn

[E01] 拼接字符串
来源：http://gw.jctech888.com.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wm.muxihuayi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tb.huixinmuqiang.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tk.nszjky.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://px.szsharing.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pm.bookmarksfly.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ou.lnxyls.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yu.yuntaijiaju.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ei.hahajie.cn

[E02] 重复字符串
来源：http://hz.shxzukj.cn

Py:   "ab" * 3
来源：http://ru.szxytkj.cn

PHP:  str_repeat("ab", 3);
来源：http://ww.yuexingan06.cn

JS:   "ab".repeat(3)
来源：http://cx.szxytkj.cn

TS:   "ab".repeat(3)
来源：http://uq.jctech888.com.cn

Java: "ab".repeat(3)
来源：http://am.521024.cn

Go:   strings.Repeat("ab", 3)
来源：http://kq.lnxyls.cn

Ruby: "ab" * 3
来源：http://bw.newstarts.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ex.shxzukj.cn

[E03] 截取子串
来源：http://mu.lnxyls.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tf.bookmarksfly.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jg.haigaiapp.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vl.hahajie.cn

TS:   s.slice(1, 4)
来源：http://sw.newstarts.cn

Java: s.substring(1, 4)
来源：http://ta.gzmigu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://os.shtwfgs.cn

Ruby: s[1, 3];  s[1..3]
来源：http://tu.521024.cn

C#:   s.Substring(1, 3)
来源：http://uu.shxzukj.cn

[E04] 查找子串位置
来源：http://ld.panjiajie.cn

Py:   s.find("x");  s.index("x")
来源：http://ef.521024.cn

PHP:  strpos($s, "x");
来源：http://ns.nszjky.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://um.huanxung.cn

TS:   s.indexOf("x")
来源：http://ce.panjiajie.cn

Java: s.indexOf("x")
来源：http://xb.yuexingan06.cn

Go:   strings.Index(s, "x")
来源：http://pe.asd995.cn

Ruby: s.index("x")
来源：http://mw.muxihuayi.cn

C#:   s.IndexOf("x")
来源：http://bv.hahajie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://jj.9csxet.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wq.wgjwhj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://gq.hahajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xy.lnxyls.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://wk.newstarts.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hv.jctech888.com.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pr.521024.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vw.shxzukj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zs.bjjhwx.cn

[E06] 替换子串
来源：http://yi.hahajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jr.jctech888.com.cn

PHP:  str_replace("a", "b", $s);
来源：http://ah.bjjhwx.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qd.huixinmuqiang.cn

TS:   s.replaceAll("a", "b")
来源：http://uk.hahajie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bz.panjiajie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tk.chemitech.net.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mw.jctech888.com.cn

C#:   s.Replace("a", "b")
来源：http://vp.huixiangedu.cn

[E07] 按分隔符拆分
来源：http://ra.bookmarksfly.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://uq.huixinmuqiang.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ab.muxihuayi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://rr.wgjwhj.cn

TS:   s.split(",")
来源：http://cw.asd995.cn

Java: s.split(",");  s.split("\\s+")
来源：http://sg.nicolike.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://os.shtwfgs.cn

Ruby: s.split(",");  s.split
来源：http://yb.haigaiapp.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zz.nszjky.cn

[E08] 数组按分隔符合并
来源：http://vb.asd995.cn

Py:   ",".join(items)
来源：http://kb.lnxyls.cn

PHP:  implode(",", $items);
来源：http://jw.shxzskj.cn

JS:   items.join(",")
来源：http://gi.shxzskj.cn

TS:   items.join(",")
来源：http://ga.szxytkj.cn

Java: String.join(",", items)
来源：http://nd.panjiajie.cn

Go:   strings.Join(items, ",")
来源：http://qx.haigaiapp.cn

Ruby: items.join(",")
来源：http://vu.gzmigu.cn

C#:   string.Join(",", items)
来源：http://ho.newstarts.cn

[E09] 去除所有空白字符
来源：http://dy.panjiajie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ev.jianghongdianzi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qv.huixiangedu.cn

JS:   s.replace(/\s+/g, "")
来源：http://ck.muxihuayi.cn

TS:   s.replace(/\s+/g, "")
来源：http://oc.szxytkj.cn

Java: s.replaceAll("\\s+", "")
来源：http://cr.szsharing.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://vb.shtwfgs.cn

Ruby: s.gsub(/\s+/, "")
来源：http://vr.yuexingan06.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nj.huixiangedu.cn

[E10] 左侧补零 / 定长填充
来源：http://rz.nszjky.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://br.gzmigu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pt.huixiangedu.cn

JS:   "7".padStart(3, "0")
来源：http://cq.nicolike.cn

TS:   "7".padStart(3, "0")
来源：http://xy.colortex.cn

Java: String.format("%03d", 7)
来源：http://ud.szsharing.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://kq.szxytkj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fd.bjjhwx.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xy.huixinmuqiang.cn

[E11] 反转字符串
来源：http://zs.lnxyls.cn

Py:   s[::-1]
来源：http://na.9csxet.cn

PHP:  strrev($s);
来源：http://ke.shxzskj.cn

JS:   [...s].reverse().join("")
来源：http://ds.shxzukj.cn

TS:   [...s].reverse().join("")
来源：http://wj.shxzukj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://cy.huanxung.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zb.newstarts.cn

Ruby: s.reverse
来源：http://xs.chemitech.net.cn

C#:   new string(s.Reverse().ToArray())
来源：http://iw.haigaiapp.cn

[E12] 统计某字符出现次数
来源：http://df.yuexingan06.cn

Py:   s.count("a")
来源：http://gs.newstarts.cn

PHP:  substr_count($s, "a");
来源：http://tb.huixinmuqiang.cn

JS:   s.split("a").length - 1
来源：http://bb.nszjky.cn

TS:   s.split("a").length - 1
来源：http://yj.bookmarksfly.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qg.nicolike.cn

Go:   strings.Count(s, "a")
来源：http://qv.shxzukj.cn

Ruby: s.count("a")
来源：http://xc.hnjuh.cn

C#:   s.Count(c => c == 'a')
来源：http://zz.gzmigu.cn

[E13] 逐字符遍历
来源：http://jy.shxzukj.cn

Py:   for ch in s: print(ch)
来源：http://pu.colortex.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bv.jctech888.com.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://wx.chemitech.net.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://my.panjiajie.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ff.szsharing.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kg.bjjhwx.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://jq.jctech888.com.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zj.asd995.cn

[E14] URL 编码与 Base64
来源：http://vy.yuntaijiaju.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dk.szsharing.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://wh.colortex.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://eo.nicolike.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rg.shxzukj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://es.shxzskj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vf.huixinmuqiang.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://aq.asd995.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kn.huanxung.cn

[E15] HTML 转义 / 反转义
来源：http://rh.gzmigu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://fk.gzmigu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sf.nszjky.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sf.jctech888.com.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://my.nicolike.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://nv.shxzskj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://oz.bookmarksfly.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wa.szxytkj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://up.bjjhwx.cn

[E16] 数字千分位
来源：http://sy.jctech888.com.cn

Py:   f"{1234567:,}"
来源：http://qi.bookmarksfly.cn

PHP:  number_format(1234567);
来源：http://rk.shtwfgs.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://da.wgjwhj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ck.muxihuayi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fe.huixinmuqiang.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://em.chemitech.net.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mb.huixiangedu.cn

C#:   1234567.ToString("N0")
来源：http://zg.wgjwhj.cn

[E17] 首字母大写
来源：http://on.chemitech.net.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ly.nszjky.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://bc.lnxyls.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://or.szsharing.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://de.shxzukj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qg.asd995.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mh.shxzskj.cn

Ruby: s.capitalize
来源：http://os.jianghongdianzi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nb.huixinmuqiang.cn

[E18] 模板占位符替换
来源：http://rv.haigaiapp.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://te.521024.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ft.newstarts.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://hj.jianghongdianzi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://lu.colortex.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ly.wgjwhj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://uq.huixiangedu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rm.9csxet.cn


<!-- 参考信息 -->