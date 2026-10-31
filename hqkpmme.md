代发 wailian999

C#:   list.Reverse();
来源：http://tn.jianghongdianzi.cn

[D12] 查找元素下标
来源：http://uy.szxytkj.cn

Py:   arr.index(x);  x in arr
来源：http://qq.shtwfgs.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://oj.huixinmuqiang.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://it.newstarts.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qz.shtwfgs.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gy.521024.cn

Go:   slices.Index(arr, x)
来源：http://vc.chemitech.net.cn

Ruby: arr.index(x)
来源：http://cr.jctech888.com.cn

C#:   list.IndexOf(x);
来源：http://yi.newstarts.cn

[D13] 过滤（保留满足条件的）
来源：http://lf.huixiangedu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vk.bookmarksfly.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fg.yuexingan06.cn

JS:   arr.filter(x => x > 3)
来源：http://ju.jianghongdianzi.cn

TS:   arr.filter(x => x > 3)
来源：http://rg.colortex.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yk.asd995.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kf.jctech888.com.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wo.jctech888.com.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://og.9csxet.cn

[D14] 映射转换（每个元素变形）
来源：http://hn.hahajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://uf.asd995.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pv.shtwfgs.cn

JS:   arr.map(x => x * 2)
来源：http://nv.hahajie.cn

TS:   arr.map(x => x * 2)
来源：http://we.huixinmuqiang.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://un.yuexingan06.cn

Go:   // 手写循环
来源：http://xm.bookmarksfly.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ih.gzmigu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://tc.panjiajie.cn

[D15] 去重
来源：http://dk.521024.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ai.bjjhwx.cn

PHP:  array_unique($arr);
来源：http://hi.panjiajie.cn

JS:   [...new Set(arr)]
来源：http://ka.newstarts.cn

TS:   [...new Set(arr)]
来源：http://kx.nicolike.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nv.asd995.cn

Go:   // 用 map[T]struct{} 手写
来源：http://dy.huixiangedu.cn

Ruby: arr.uniq
来源：http://st.shxzskj.cn

C#:   list.Distinct().ToList()
来源：http://jw.9csxet.cn

[D16] 求和与平均值
来源：http://db.huixiangedu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://us.yuexingan06.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pz.chemitech.net.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vw.gzmigu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mw.newstarts.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://uh.huixiangedu.cn

Go:   // 手写循环累加
来源：http://kj.hnjuh.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qg.bookmarksfly.cn

C#:   list.Sum();  list.Average()
来源：http://mw.shtwfgs.cn

[D17] 最大值与最小值
来源：http://nt.nszjky.cn

Py:   max(arr);  min(arr)
来源：http://of.szsharing.cn

PHP:  max($arr);  min($arr);
来源：http://fu.chemitech.net.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pr.wgjwhj.cn

TS:   Math.max(...arr);
来源：http://lh.521024.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://rc.huanxung.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jz.hahajie.cn

Ruby: arr.max;  arr.min
来源：http://yr.jctech888.com.cn

C#:   list.Max();  list.Min()
来源：http://kx.colortex.cn

[D18] 扁平化嵌套数组
来源：http://rc.jianghongdianzi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://oe.shxzskj.cn

PHP:  array_merge(...$nested);
来源：http://pt.hahajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gx.colortex.cn

TS:   nested.flat();
来源：http://pa.colortex.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wl.shxzskj.cn

Go:   // 手写双层循环
来源：http://pn.shtwfgs.cn

Ruby: nested.flatten
来源：http://vj.jianghongdianzi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://wv.nicolike.cn

[D19] 按字段分组
来源：http://nf.huixiangedu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vm.521024.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ev.shxzukj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://se.huixiangedu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ef.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yc.jctech888.com.cn

Go:   // 手写 map[string][]T
来源：http://su.wgjwhj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://wv.hnjuh.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kt.asd995.cn

[D20] 统计每个元素出现次数
来源：http://db.shxzskj.cn

Py:   Counter(arr)
来源：http://wo.shtwfgs.cn

PHP:  array_count_values($arr);
来源：http://ed.huanxung.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ub.9csxet.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vu.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hb.asd995.cn

Go:   // 手写 map[T]int
来源：http://dq.yuexingan06.cn

Ruby: arr.tally
来源：http://iw.yuexingan06.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mi.huanxung.cn

[D21] 判断是否包含某元素
来源：http://in.szxytkj.cn

Py:   x in arr
来源：http://om.shxzukj.cn

PHP:  in_array($x, $arr, true);
来源：http://oy.muxihuayi.cn

JS:   arr.includes(x)
来源：http://jx.chemitech.net.cn

TS:   arr.includes(x)
来源：http://vi.bjjhwx.cn

Java: list.contains(x)
来源：http://vd.jianghongdianzi.cn

Go:   slices.Contains(arr, x)
来源：http://bt.jctech888.com.cn

Ruby: arr.include?(x)
来源：http://ru.shxzskj.cn

C#:   list.Contains(x)
来源：http://wl.asd995.cn

[D22] 复制数组（避免共享引用）
来源：http://no.shxzukj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://th.yuntaijiaju.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ps.huanxung.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fa.shxzukj.cn

TS:   [...arr];
来源：http://yr.shxzukj.cn

Java: new ArrayList<>(list);
来源：http://lt.nicolike.cn

Go:   copied := append([]int(nil), arr...)
来源：http://zx.shxzukj.cn

Ruby: arr.dup;  arr.clone
来源：http://mb.asd995.cn

C#:   new List<int>(list);
来源：http://ne.shtwfgs.cn

[D23] reduce 累积计算
来源：http://ue.hahajie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ka.muxihuayi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://sw.wgjwhj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vp.huixinmuqiang.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ki.nszjky.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://uo.bookmarksfly.cn

Go:   // 手写循环
来源：http://gf.nicolike.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gs.muxihuayi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ay.asd995.cn

[D24] 字典 / Map 基本操作
来源：http://kk.huixinmuqiang.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ry.hahajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kf.nszjky.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xt.gzmigu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tr.shtwfgs.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uf.521024.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ql.haigaiapp.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ah.jianghongdianzi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://td.521024.cn

[D25] Set 集合去重与交并差
来源：http://vc.huixinmuqiang.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ac.yuntaijiaju.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mu.shtwfgs.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mn.nszjky.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://sa.asd995.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ly.bjjhwx.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://px.haigaiapp.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mh.bjjhwx.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rz.hahajie.cn

[D26] 数组转字符串
来源：http://gv.muxihuayi.cn

Py:   ", ".join(map(str, arr))
来源：http://pf.shxzskj.cn

PHP:  implode(", ", $arr);
来源：http://wi.huixinmuqiang.cn

JS:   arr.join(", ")
来源：http://mu.newstarts.cn

TS:   arr.join(", ")
来源：http://ju.huixiangedu.cn

Java: String.join(", ", list)
来源：http://qt.lnxyls.cn

Go:   strings.Join(strs, ", ")
来源：http://qh.haigaiapp.cn

Ruby: arr.join(", ")
来源：http://er.wgjwhj.cn

C#:   string.Join(", ", list)
来源：http://xm.9csxet.cn

================================================================================
来源：http://zc.shxzskj.cn

E. 字符串处理
来源：http://il.szxytkj.cn

================================================================================
来源：http://tz.szsharing.cn

[E01] 拼接字符串
来源：http://ci.9csxet.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ia.shxzukj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qg.haigaiapp.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gh.521024.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sq.muxihuayi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ka.huixiangedu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ax.asd995.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mz.szsharing.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ae.huanxung.cn

[E02] 重复字符串
来源：http://tr.bookmarksfly.cn

Py:   "ab" * 3
来源：http://kz.521024.cn

PHP:  str_repeat("ab", 3);
来源：http://ob.shxzukj.cn

JS:   "ab".repeat(3)
来源：http://zy.szxytkj.cn

TS:   "ab".repeat(3)
来源：http://ta.hahajie.cn

Java: "ab".repeat(3)
来源：http://kj.yuexingan06.cn

Go:   strings.Repeat("ab", 3)
来源：http://zu.bookmarksfly.cn

Ruby: "ab" * 3
来源：http://bz.huixiangedu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qz.asd995.cn

[E03] 截取子串
来源：http://dx.gzmigu.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cu.panjiajie.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ab.hnjuh.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://en.gzmigu.cn

TS:   s.slice(1, 4)
来源：http://qs.shxzukj.cn

Java: s.substring(1, 4)
来源：http://cn.yuexingan06.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://uz.yuntaijiaju.cn

Ruby: s[1, 3];  s[1..3]
来源：http://fx.shtwfgs.cn

C#:   s.Substring(1, 3)
来源：http://ld.9csxet.cn

[E04] 查找子串位置
来源：http://iy.chemitech.net.cn

Py:   s.find("x");  s.index("x")
来源：http://el.yuntaijiaju.cn

PHP:  strpos($s, "x");
来源：http://bq.nszjky.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qx.haigaiapp.cn

TS:   s.indexOf("x")
来源：http://rz.nszjky.cn

Java: s.indexOf("x")
来源：http://mc.521024.cn

Go:   strings.Index(s, "x")
来源：http://cs.haigaiapp.cn

Ruby: s.index("x")
来源：http://wb.asd995.cn

C#:   s.IndexOf("x")
来源：http://ex.asd995.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://cl.panjiajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xb.haigaiapp.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qj.newstarts.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fx.hnjuh.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ux.huixinmuqiang.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ut.huixiangedu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://co.lnxyls.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ub.muxihuayi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ei.panjiajie.cn

[E06] 替换子串
来源：http://lb.huixiangedu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://eh.bookmarksfly.cn

PHP:  str_replace("a", "b", $s);
来源：http://mv.asd995.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nn.asd995.cn

TS:   s.replaceAll("a", "b")
来源：http://rc.jianghongdianzi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zb.szxytkj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kp.hahajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fg.yuntaijiaju.cn

C#:   s.Replace("a", "b")
来源：http://un.shxzskj.cn

[E07] 按分隔符拆分
来源：http://xs.muxihuayi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yu.colortex.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://as.huixinmuqiang.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://tp.shtwfgs.cn

TS:   s.split(",")
来源：http://hp.shtwfgs.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zt.asd995.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ru.bjjhwx.cn

Ruby: s.split(",");  s.split
来源：http://sj.chemitech.net.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bc.newstarts.cn

[E08] 数组按分隔符合并
来源：http://bk.521024.cn

Py:   ",".join(items)
来源：http://ny.jctech888.com.cn

PHP:  implode(",", $items);
来源：http://nu.muxihuayi.cn

JS:   items.join(",")
来源：http://ay.huixiangedu.cn

TS:   items.join(",")
来源：http://vk.9csxet.cn

Java: String.join(",", items)
来源：http://do.gzmigu.cn

Go:   strings.Join(items, ",")
来源：http://qw.nszjky.cn

Ruby: items.join(",")
来源：http://qr.hnjuh.cn

C#:   string.Join(",", items)
来源：http://vn.shxzukj.cn

[E09] 去除所有空白字符
来源：http://od.bjjhwx.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pi.nszjky.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://am.asd995.cn

JS:   s.replace(/\s+/g, "")
来源：http://wm.szsharing.cn

TS:   s.replace(/\s+/g, "")
来源：http://zt.haigaiapp.cn

Java: s.replaceAll("\\s+", "")
来源：http://dc.hnjuh.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://nf.szsharing.cn

Ruby: s.gsub(/\s+/, "")
来源：http://vf.521024.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qs.lnxyls.cn

[E10] 左侧补零 / 定长填充
来源：http://qb.jianghongdianzi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mb.hnjuh.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gu.shtwfgs.cn

JS:   "7".padStart(3, "0")
来源：http://qo.yuntaijiaju.cn

TS:   "7".padStart(3, "0")
来源：http://nz.shxzskj.cn

Java: String.format("%03d", 7)
来源：http://oi.hahajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://im.yuexingan06.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cr.gzmigu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qg.nszjky.cn

[E11] 反转字符串
来源：http://cu.huixinmuqiang.cn

Py:   s[::-1]
来源：http://xd.yuexingan06.cn

PHP:  strrev($s);
来源：http://kh.huixinmuqiang.cn

JS:   [...s].reverse().join("")
来源：http://ig.9csxet.cn

TS:   [...s].reverse().join("")
来源：http://gs.haigaiapp.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://vo.colortex.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://lm.wgjwhj.cn

Ruby: s.reverse
来源：http://ib.nicolike.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ji.asd995.cn

[E12] 统计某字符出现次数
来源：http://if.shtwfgs.cn

Py:   s.count("a")
来源：http://rp.huixiangedu.cn

PHP:  substr_count($s, "a");
来源：http://bh.panjiajie.cn

JS:   s.split("a").length - 1
来源：http://da.szsharing.cn

TS:   s.split("a").length - 1
来源：http://ye.jianghongdianzi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zz.bookmarksfly.cn

Go:   strings.Count(s, "a")
来源：http://fk.huanxung.cn

Ruby: s.count("a")
来源：http://ef.wgjwhj.cn

C#:   s.Count(c => c == 'a')
来源：http://jj.bjjhwx.cn

[E13] 逐字符遍历
来源：http://xt.panjiajie.cn

Py:   for ch in s: print(ch)
来源：http://sq.shtwfgs.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qc.shtwfgs.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://rw.newstarts.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ov.colortex.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wh.gzmigu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gd.haigaiapp.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://oo.shtwfgs.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ck.szsharing.cn

[E14] URL 编码与 Base64
来源：http://sl.huixiangedu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zv.colortex.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://za.huixiangedu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ns.shxzskj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bh.newstarts.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ft.szsharing.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jd.huixiangedu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uw.hahajie.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wb.nszjky.cn

[E15] HTML 转义 / 反转义
来源：http://ki.hahajie.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://go.huixinmuqiang.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ur.newstarts.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.colortex.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ur.gzmigu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tg.newstarts.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nm.nszjky.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://me.nszjky.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://di.newstarts.cn

[E16] 数字千分位
来源：http://wl.huixinmuqiang.cn

Py:   f"{1234567:,}"
来源：http://no.yuntaijiaju.cn

PHP:  number_format(1234567);
来源：http://zp.muxihuayi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://jk.shxzskj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://hk.huanxung.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://oi.nicolike.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nq.wgjwhj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rw.szxytkj.cn

C#:   1234567.ToString("N0")
来源：http://tb.jianghongdianzi.cn

[E17] 首字母大写
来源：http://wh.shxzskj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xj.huixinmuqiang.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://hh.nicolike.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://st.shtwfgs.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wk.huixinmuqiang.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vz.jctech888.com.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ms.chemitech.net.cn

Ruby: s.capitalize
来源：http://we.bookmarksfly.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ss.nicolike.cn

[E18] 模板占位符替换
来源：http://oj.haigaiapp.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jd.hnjuh.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jd.bookmarksfly.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ke.wgjwhj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://fk.wgjwhj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ja.szsharing.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lp.bookmarksfly.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cm.shxzukj.cn


<!-- 参考信息 -->