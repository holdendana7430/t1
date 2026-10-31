代发 wailian999

[D11] 反转数组
来源：http://dg.shxzskj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://cy.panjiajie.cn

PHP:  array_reverse($arr);
来源：http://fa.wgjwhj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zc.bookmarksfly.cn

TS:   [...arr].reverse();
来源：http://ja.huixiangedu.cn

Java: Collections.reverse(list);
来源：http://gv.yuexingan06.cn

Go:   slices.Reverse(arr)
来源：http://sd.huanxung.cn

Ruby: arr.reverse
来源：http://kl.colortex.cn

C#:   list.Reverse();
来源：http://gk.muxihuayi.cn

[D12] 查找元素下标
来源：http://va.9csxet.cn

Py:   arr.index(x);  x in arr
来源：http://xh.huixiangedu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ls.haigaiapp.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lt.huanxung.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wb.szxytkj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cx.shxzskj.cn

Go:   slices.Index(arr, x)
来源：http://sr.shtwfgs.cn

Ruby: arr.index(x)
来源：http://zd.bjjhwx.cn

C#:   list.IndexOf(x);
来源：http://vi.szxytkj.cn

[D13] 过滤（保留满足条件的）
来源：http://sw.szsharing.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gh.nszjky.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wc.hahajie.cn

JS:   arr.filter(x => x > 3)
来源：http://xo.huixinmuqiang.cn

TS:   arr.filter(x => x > 3)
来源：http://ix.hahajie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ip.asd995.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yt.nicolike.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fa.nszjky.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://wf.gzmigu.cn

[D14] 映射转换（每个元素变形）
来源：http://ix.521024.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sj.shxzskj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fu.wgjwhj.cn

JS:   arr.map(x => x * 2)
来源：http://it.shtwfgs.cn

TS:   arr.map(x => x * 2)
来源：http://hm.521024.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ed.yuexingan06.cn

Go:   // 手写循环
来源：http://ax.muxihuayi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qr.bjjhwx.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://gq.panjiajie.cn

[D15] 去重
来源：http://kk.haigaiapp.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ta.hnjuh.cn

PHP:  array_unique($arr);
来源：http://dt.nszjky.cn

JS:   [...new Set(arr)]
来源：http://bt.huixiangedu.cn

TS:   [...new Set(arr)]
来源：http://uu.hnjuh.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://eg.huixinmuqiang.cn

Go:   // 用 map[T]struct{} 手写
来源：http://kc.521024.cn

Ruby: arr.uniq
来源：http://rg.colortex.cn

C#:   list.Distinct().ToList()
来源：http://fc.jianghongdianzi.cn

[D16] 求和与平均值
来源：http://gs.nszjky.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kq.shxzukj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qz.szsharing.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ed.hnjuh.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nk.bjjhwx.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vm.asd995.cn

Go:   // 手写循环累加
来源：http://xn.szxytkj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dr.bjjhwx.cn

C#:   list.Sum();  list.Average()
来源：http://ia.bjjhwx.cn

[D17] 最大值与最小值
来源：http://au.yuntaijiaju.cn

Py:   max(arr);  min(arr)
来源：http://up.hnjuh.cn

PHP:  max($arr);  min($arr);
来源：http://ui.shxzukj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yd.yuntaijiaju.cn

TS:   Math.max(...arr);
来源：http://dh.bookmarksfly.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://fi.szxytkj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lf.newstarts.cn

Ruby: arr.max;  arr.min
来源：http://ud.huanxung.cn

C#:   list.Max();  list.Min()
来源：http://bv.gzmigu.cn

[D18] 扁平化嵌套数组
来源：http://jp.haigaiapp.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ek.panjiajie.cn

PHP:  array_merge(...$nested);
来源：http://ng.yuexingan06.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lp.haigaiapp.cn

TS:   nested.flat();
来源：http://sv.huanxung.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ih.yuntaijiaju.cn

Go:   // 手写双层循环
来源：http://db.shxzukj.cn

Ruby: nested.flatten
来源：http://tk.jianghongdianzi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://td.9csxet.cn

[D19] 按字段分组
来源：http://mu.yuexingan06.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nb.huanxung.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hw.yuntaijiaju.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zj.huixiangedu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://fy.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ct.521024.cn

Go:   // 手写 map[string][]T
来源：http://zk.huixinmuqiang.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://wa.panjiajie.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nk.panjiajie.cn

[D20] 统计每个元素出现次数
来源：http://cc.huixinmuqiang.cn

Py:   Counter(arr)
来源：http://br.szxytkj.cn

PHP:  array_count_values($arr);
来源：http://rx.szsharing.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hb.shxzukj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kq.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fb.asd995.cn

Go:   // 手写 map[T]int
来源：http://ok.muxihuayi.cn

Ruby: arr.tally
来源：http://dz.hnjuh.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tz.asd995.cn

[D21] 判断是否包含某元素
来源：http://ps.hahajie.cn

Py:   x in arr
来源：http://cy.asd995.cn

PHP:  in_array($x, $arr, true);
来源：http://hn.newstarts.cn

JS:   arr.includes(x)
来源：http://by.panjiajie.cn

TS:   arr.includes(x)
来源：http://ch.bookmarksfly.cn

Java: list.contains(x)
来源：http://ef.nszjky.cn

Go:   slices.Contains(arr, x)
来源：http://rw.yuntaijiaju.cn

Ruby: arr.include?(x)
来源：http://gz.shxzskj.cn

C#:   list.Contains(x)
来源：http://wc.szxytkj.cn

[D22] 复制数组（避免共享引用）
来源：http://gq.shxzskj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://sm.asd995.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zu.szsharing.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://sg.huanxung.cn

TS:   [...arr];
来源：http://kb.nicolike.cn

Java: new ArrayList<>(list);
来源：http://wn.szsharing.cn

Go:   copied := append([]int(nil), arr...)
来源：http://sv.nicolike.cn

Ruby: arr.dup;  arr.clone
来源：http://cz.hnjuh.cn

C#:   new List<int>(list);
来源：http://pf.nicolike.cn

[D23] reduce 累积计算
来源：http://oy.shxzskj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xt.hahajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xw.jctech888.com.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tc.newstarts.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sr.lnxyls.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://um.bookmarksfly.cn

Go:   // 手写循环
来源：http://fh.wgjwhj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hs.haigaiapp.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ft.haigaiapp.cn

[D24] 字典 / Map 基本操作
来源：http://qo.huanxung.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qw.yuexingan06.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ya.muxihuayi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hs.nszjky.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wq.521024.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qd.yuexingan06.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://av.haigaiapp.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://sn.yuntaijiaju.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://sh.asd995.cn

[D25] Set 集合去重与交并差
来源：http://az.newstarts.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wt.jianghongdianzi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ax.szsharing.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ro.panjiajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mb.panjiajie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xb.szsharing.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gp.shxzukj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qn.muxihuayi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bn.521024.cn

[D26] 数组转字符串
来源：http://zb.szsharing.cn

Py:   ", ".join(map(str, arr))
来源：http://ew.hahajie.cn

PHP:  implode(", ", $arr);
来源：http://jk.asd995.cn

JS:   arr.join(", ")
来源：http://jl.lnxyls.cn

TS:   arr.join(", ")
来源：http://cz.nszjky.cn

Java: String.join(", ", list)
来源：http://cl.muxihuayi.cn

Go:   strings.Join(strs, ", ")
来源：http://ro.szxytkj.cn

Ruby: arr.join(", ")
来源：http://tm.huixinmuqiang.cn

C#:   string.Join(", ", list)
来源：http://po.szxytkj.cn

================================================================================
来源：http://pi.huanxung.cn

E. 字符串处理
来源：http://xx.chemitech.net.cn

================================================================================
来源：http://ma.9csxet.cn

[E01] 拼接字符串
来源：http://zw.shtwfgs.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sw.gzmigu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ak.huanxung.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bn.shxzukj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://po.huanxung.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qj.nicolike.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ld.yuexingan06.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bu.bjjhwx.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ko.hahajie.cn

[E02] 重复字符串
来源：http://ux.jianghongdianzi.cn

Py:   "ab" * 3
来源：http://ch.huanxung.cn

PHP:  str_repeat("ab", 3);
来源：http://ub.shxzskj.cn

JS:   "ab".repeat(3)
来源：http://co.lnxyls.cn

TS:   "ab".repeat(3)
来源：http://ah.9csxet.cn

Java: "ab".repeat(3)
来源：http://ea.shxzskj.cn

Go:   strings.Repeat("ab", 3)
来源：http://ai.huixinmuqiang.cn

Ruby: "ab" * 3
来源：http://ua.wgjwhj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mt.wgjwhj.cn

[E03] 截取子串
来源：http://zs.shtwfgs.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vc.muxihuayi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://md.521024.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jf.szxytkj.cn

TS:   s.slice(1, 4)
来源：http://fn.shxzskj.cn

Java: s.substring(1, 4)
来源：http://hn.jctech888.com.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xw.muxihuayi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://bq.muxihuayi.cn

C#:   s.Substring(1, 3)
来源：http://wy.lnxyls.cn

[E04] 查找子串位置
来源：http://jh.shtwfgs.cn

Py:   s.find("x");  s.index("x")
来源：http://zg.9csxet.cn

PHP:  strpos($s, "x");
来源：http://gr.yuexingan06.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ch.huanxung.cn

TS:   s.indexOf("x")
来源：http://et.yuexingan06.cn

Java: s.indexOf("x")
来源：http://ii.jctech888.com.cn

Go:   strings.Index(s, "x")
来源：http://av.hahajie.cn

Ruby: s.index("x")
来源：http://vv.szxytkj.cn

C#:   s.IndexOf("x")
来源：http://sd.newstarts.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ac.jianghongdianzi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ra.huanxung.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ds.asd995.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uv.9csxet.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ef.hnjuh.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://im.yuntaijiaju.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tf.hahajie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://au.bjjhwx.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wi.colortex.cn

[E06] 替换子串
来源：http://bb.colortex.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://of.shxzukj.cn

PHP:  str_replace("a", "b", $s);
来源：http://xh.huixinmuqiang.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ch.chemitech.net.cn

TS:   s.replaceAll("a", "b")
来源：http://od.newstarts.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zm.521024.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mt.hahajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lj.asd995.cn

C#:   s.Replace("a", "b")
来源：http://hb.asd995.cn

[E07] 按分隔符拆分
来源：http://lu.bjjhwx.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nt.wgjwhj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://oj.colortex.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://qr.colortex.cn

TS:   s.split(",")
来源：http://im.9csxet.cn

Java: s.split(",");  s.split("\\s+")
来源：http://cn.hahajie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ij.huixiangedu.cn

Ruby: s.split(",");  s.split
来源：http://xx.wgjwhj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ff.haigaiapp.cn

[E08] 数组按分隔符合并
来源：http://rl.nicolike.cn

Py:   ",".join(items)
来源：http://qw.jctech888.com.cn

PHP:  implode(",", $items);
来源：http://ij.jianghongdianzi.cn

JS:   items.join(",")
来源：http://tu.wgjwhj.cn

TS:   items.join(",")
来源：http://dm.shxzskj.cn

Java: String.join(",", items)
来源：http://ss.bookmarksfly.cn

Go:   strings.Join(items, ",")
来源：http://ah.bjjhwx.cn

Ruby: items.join(",")
来源：http://sr.bookmarksfly.cn

C#:   string.Join(",", items)
来源：http://tq.chemitech.net.cn

[E09] 去除所有空白字符
来源：http://zs.yuexingan06.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qy.panjiajie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fs.szsharing.cn

JS:   s.replace(/\s+/g, "")
来源：http://vv.gzmigu.cn

TS:   s.replace(/\s+/g, "")
来源：http://lk.szxytkj.cn

Java: s.replaceAll("\\s+", "")
来源：http://fz.gzmigu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ga.yuexingan06.cn

Ruby: s.gsub(/\s+/, "")
来源：http://yp.lnxyls.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kx.asd995.cn

[E10] 左侧补零 / 定长填充
来源：http://ka.hnjuh.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fu.huixinmuqiang.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fl.gzmigu.cn

JS:   "7".padStart(3, "0")
来源：http://cw.colortex.cn

TS:   "7".padStart(3, "0")
来源：http://tt.nicolike.cn

Java: String.format("%03d", 7)
来源：http://rf.newstarts.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ui.wgjwhj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qz.chemitech.net.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bp.nicolike.cn

[E11] 反转字符串
来源：http://jd.gzmigu.cn

Py:   s[::-1]
来源：http://dx.gzmigu.cn

PHP:  strrev($s);
来源：http://ft.huixiangedu.cn

JS:   [...s].reverse().join("")
来源：http://do.bookmarksfly.cn

TS:   [...s].reverse().join("")
来源：http://di.gzmigu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://lc.colortex.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://md.hahajie.cn

Ruby: s.reverse
来源：http://qt.shxzskj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ep.nszjky.cn

[E12] 统计某字符出现次数
来源：http://ie.szxytkj.cn

Py:   s.count("a")
来源：http://kb.haigaiapp.cn

PHP:  substr_count($s, "a");
来源：http://mj.jctech888.com.cn

JS:   s.split("a").length - 1
来源：http://et.muxihuayi.cn

TS:   s.split("a").length - 1
来源：http://xb.huanxung.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lj.bookmarksfly.cn

Go:   strings.Count(s, "a")
来源：http://bo.nicolike.cn

Ruby: s.count("a")
来源：http://hl.szsharing.cn

C#:   s.Count(c => c == 'a')
来源：http://vn.szxytkj.cn

[E13] 逐字符遍历
来源：http://wo.szsharing.cn

Py:   for ch in s: print(ch)
来源：http://pf.hnjuh.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ef.nszjky.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://kg.haigaiapp.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://nq.jctech888.com.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sz.haigaiapp.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vz.colortex.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://oq.hahajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://uw.521024.cn

[E14] URL 编码与 Base64
来源：http://nv.gzmigu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qb.colortex.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://xw.wgjwhj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yi.huixiangedu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ts.asd995.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ld.521024.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vb.nszjky.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ua.shxzskj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ts.shxzukj.cn

[E15] HTML 转义 / 反转义
来源：http://da.9csxet.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://zx.shxzskj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://us.huixiangedu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://oq.9csxet.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://vd.szxytkj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wn.hnjuh.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bu.bookmarksfly.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ve.haigaiapp.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://eo.gzmigu.cn

[E16] 数字千分位
来源：http://du.bjjhwx.cn

Py:   f"{1234567:,}"
来源：http://vk.chemitech.net.cn

PHP:  number_format(1234567);
来源：http://qn.hnjuh.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://eq.nszjky.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ge.nszjky.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dk.lnxyls.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pc.shtwfgs.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://iv.521024.cn

C#:   1234567.ToString("N0")
来源：http://gy.nszjky.cn

[E17] 首字母大写
来源：http://wt.shtwfgs.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://un.nszjky.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://qj.colortex.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ax.521024.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tu.newstarts.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://oo.shxzskj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mb.newstarts.cn

Ruby: s.capitalize
来源：http://uh.nicolike.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zq.colortex.cn


<!-- 参考信息 -->