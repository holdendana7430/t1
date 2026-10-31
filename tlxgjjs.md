代发 wailian999

C#:   list.Reverse();
来源：http://bq.panjiajie.cn

[D12] 查找元素下标
来源：http://dn.haigaiapp.cn

Py:   arr.index(x);  x in arr
来源：http://vc.yuexingan06.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cz.hahajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nc.szsharing.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fb.nicolike.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vj.nszjky.cn

Go:   slices.Index(arr, x)
来源：http://zc.jctech888.com.cn

Ruby: arr.index(x)
来源：http://sv.hahajie.cn

C#:   list.IndexOf(x);
来源：http://fv.huixiangedu.cn

[D13] 过滤（保留满足条件的）
来源：http://ht.jianghongdianzi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cv.shxzukj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nc.huixinmuqiang.cn

JS:   arr.filter(x => x > 3)
来源：http://ns.shtwfgs.cn

TS:   arr.filter(x => x > 3)
来源：http://nb.hnjuh.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ls.chemitech.net.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://sm.haigaiapp.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qn.nicolike.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://fw.yuntaijiaju.cn

[D14] 映射转换（每个元素变形）
来源：http://hm.haigaiapp.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pg.huixiangedu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ot.521024.cn

JS:   arr.map(x => x * 2)
来源：http://fj.haigaiapp.cn

TS:   arr.map(x => x * 2)
来源：http://wr.panjiajie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://aq.gzmigu.cn

Go:   // 手写循环
来源：http://rs.panjiajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jm.shtwfgs.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ib.hahajie.cn

[D15] 去重
来源：http://uq.colortex.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cd.shxzukj.cn

PHP:  array_unique($arr);
来源：http://kb.9csxet.cn

JS:   [...new Set(arr)]
来源：http://vl.shtwfgs.cn

TS:   [...new Set(arr)]
来源：http://gm.chemitech.net.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uz.jianghongdianzi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wd.gzmigu.cn

Ruby: arr.uniq
来源：http://fd.huanxung.cn

C#:   list.Distinct().ToList()
来源：http://ja.huixiangedu.cn

[D16] 求和与平均值
来源：http://so.9csxet.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ll.nicolike.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rc.hnjuh.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wo.gzmigu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jz.muxihuayi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cr.gzmigu.cn

Go:   // 手写循环累加
来源：http://wf.bjjhwx.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ej.wgjwhj.cn

C#:   list.Sum();  list.Average()
来源：http://ho.huixinmuqiang.cn

[D17] 最大值与最小值
来源：http://bx.yuexingan06.cn

Py:   max(arr);  min(arr)
来源：http://tc.hnjuh.cn

PHP:  max($arr);  min($arr);
来源：http://jt.jctech888.com.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jz.wgjwhj.cn

TS:   Math.max(...arr);
来源：http://ht.shxzukj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://tv.huixiangedu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://oz.asd995.cn

Ruby: arr.max;  arr.min
来源：http://tg.521024.cn

C#:   list.Max();  list.Min()
来源：http://zg.shxzukj.cn

[D18] 扁平化嵌套数组
来源：http://cb.hnjuh.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bb.gzmigu.cn

PHP:  array_merge(...$nested);
来源：http://sy.huanxung.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://de.haigaiapp.cn

TS:   nested.flat();
来源：http://ej.yuntaijiaju.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jr.szsharing.cn

Go:   // 手写双层循环
来源：http://qu.huixinmuqiang.cn

Ruby: nested.flatten
来源：http://qg.shxzskj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://co.huixiangedu.cn

[D19] 按字段分组
来源：http://lk.9csxet.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://if.szsharing.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xc.shtwfgs.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qz.nszjky.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://rz.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vq.szxytkj.cn

Go:   // 手写 map[string][]T
来源：http://ge.yuntaijiaju.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fy.shtwfgs.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://in.hahajie.cn

[D20] 统计每个元素出现次数
来源：http://od.panjiajie.cn

Py:   Counter(arr)
来源：http://bq.9csxet.cn

PHP:  array_count_values($arr);
来源：http://qa.yuntaijiaju.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lj.nicolike.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ms.521024.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://da.9csxet.cn

Go:   // 手写 map[T]int
来源：http://cb.yuexingan06.cn

Ruby: arr.tally
来源：http://lb.asd995.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hr.asd995.cn

[D21] 判断是否包含某元素
来源：http://dy.hnjuh.cn

Py:   x in arr
来源：http://jf.yuexingan06.cn

PHP:  in_array($x, $arr, true);
来源：http://qw.szxytkj.cn

JS:   arr.includes(x)
来源：http://lp.huixinmuqiang.cn

TS:   arr.includes(x)
来源：http://nj.asd995.cn

Java: list.contains(x)
来源：http://ia.huixiangedu.cn

Go:   slices.Contains(arr, x)
来源：http://fw.lnxyls.cn

Ruby: arr.include?(x)
来源：http://kh.yuexingan06.cn

C#:   list.Contains(x)
来源：http://vi.521024.cn

[D22] 复制数组（避免共享引用）
来源：http://xf.huixiangedu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vw.jianghongdianzi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ga.huanxung.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zb.bookmarksfly.cn

TS:   [...arr];
来源：http://ta.bookmarksfly.cn

Java: new ArrayList<>(list);
来源：http://ij.newstarts.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ve.shtwfgs.cn

Ruby: arr.dup;  arr.clone
来源：http://nm.lnxyls.cn

C#:   new List<int>(list);
来源：http://ek.shxzukj.cn

[D23] reduce 累积计算
来源：http://pz.muxihuayi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://og.huixinmuqiang.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xu.huixiangedu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lp.hnjuh.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zj.yuexingan06.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://wn.newstarts.cn

Go:   // 手写循环
来源：http://qe.9csxet.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ag.newstarts.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tv.huixinmuqiang.cn

[D24] 字典 / Map 基本操作
来源：http://oc.hnjuh.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hl.huanxung.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://di.521024.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ai.hahajie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gf.bjjhwx.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ea.gzmigu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tr.hahajie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://eh.bjjhwx.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zf.jctech888.com.cn

[D25] Set 集合去重与交并差
来源：http://yh.bjjhwx.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jz.shxzskj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jp.huixinmuqiang.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jm.lnxyls.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://eu.lnxyls.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fp.colortex.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nx.hnjuh.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uw.chemitech.net.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bg.shxzukj.cn

[D26] 数组转字符串
来源：http://bn.gzmigu.cn

Py:   ", ".join(map(str, arr))
来源：http://uy.szsharing.cn

PHP:  implode(", ", $arr);
来源：http://ir.hnjuh.cn

JS:   arr.join(", ")
来源：http://mw.wgjwhj.cn

TS:   arr.join(", ")
来源：http://rl.nszjky.cn

Java: String.join(", ", list)
来源：http://kh.shxzskj.cn

Go:   strings.Join(strs, ", ")
来源：http://og.hnjuh.cn

Ruby: arr.join(", ")
来源：http://wy.shxzskj.cn

C#:   string.Join(", ", list)
来源：http://qw.huixiangedu.cn

================================================================================
来源：http://lx.jianghongdianzi.cn

E. 字符串处理
来源：http://cn.hahajie.cn

================================================================================
来源：http://ck.hnjuh.cn

[E01] 拼接字符串
来源：http://bz.huixinmuqiang.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tq.huanxung.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://iy.haigaiapp.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zy.jctech888.com.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://eg.lnxyls.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xi.bjjhwx.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sp.bookmarksfly.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ip.shxzskj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://in.muxihuayi.cn

[E02] 重复字符串
来源：http://ga.shtwfgs.cn

Py:   "ab" * 3
来源：http://dg.huixinmuqiang.cn

PHP:  str_repeat("ab", 3);
来源：http://cq.jctech888.com.cn

JS:   "ab".repeat(3)
来源：http://mz.jianghongdianzi.cn

TS:   "ab".repeat(3)
来源：http://hu.wgjwhj.cn

Java: "ab".repeat(3)
来源：http://qs.hnjuh.cn

Go:   strings.Repeat("ab", 3)
来源：http://nn.huixiangedu.cn

Ruby: "ab" * 3
来源：http://td.hnjuh.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nl.chemitech.net.cn

[E03] 截取子串
来源：http://ii.panjiajie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cz.asd995.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ev.bookmarksfly.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fg.shxzskj.cn

TS:   s.slice(1, 4)
来源：http://ao.szxytkj.cn

Java: s.substring(1, 4)
来源：http://jq.chemitech.net.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://or.hnjuh.cn

Ruby: s[1, 3];  s[1..3]
来源：http://wt.panjiajie.cn

C#:   s.Substring(1, 3)
来源：http://gv.haigaiapp.cn

[E04] 查找子串位置
来源：http://lf.wgjwhj.cn

Py:   s.find("x");  s.index("x")
来源：http://rk.szsharing.cn

PHP:  strpos($s, "x");
来源：http://ze.gzmigu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://so.yuntaijiaju.cn

TS:   s.indexOf("x")
来源：http://xb.shxzskj.cn

Java: s.indexOf("x")
来源：http://sr.jctech888.com.cn

Go:   strings.Index(s, "x")
来源：http://se.nszjky.cn

Ruby: s.index("x")
来源：http://ws.521024.cn

C#:   s.IndexOf("x")
来源：http://nw.521024.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://qv.nszjky.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qy.yuexingan06.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ym.huanxung.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xh.panjiajie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://vg.nicolike.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bb.jianghongdianzi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cp.nszjky.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://uc.huixiangedu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ug.huanxung.cn

[E06] 替换子串
来源：http://ri.yuntaijiaju.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://eh.hahajie.cn

PHP:  str_replace("a", "b", $s);
来源：http://rd.shtwfgs.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ur.huixinmuqiang.cn

TS:   s.replaceAll("a", "b")
来源：http://na.lnxyls.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cj.szxytkj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rg.jctech888.com.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ik.jianghongdianzi.cn

C#:   s.Replace("a", "b")
来源：http://sj.bookmarksfly.cn

[E07] 按分隔符拆分
来源：http://vg.szsharing.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://en.huixiangedu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://oi.asd995.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://dd.chemitech.net.cn

TS:   s.split(",")
来源：http://oi.bookmarksfly.cn

Java: s.split(",");  s.split("\\s+")
来源：http://en.nicolike.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fl.huixiangedu.cn

Ruby: s.split(",");  s.split
来源：http://oo.9csxet.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://an.shtwfgs.cn

[E08] 数组按分隔符合并
来源：http://qt.newstarts.cn

Py:   ",".join(items)
来源：http://bm.huixiangedu.cn

PHP:  implode(",", $items);
来源：http://hq.shxzskj.cn

JS:   items.join(",")
来源：http://im.bjjhwx.cn

TS:   items.join(",")
来源：http://nq.hahajie.cn

Java: String.join(",", items)
来源：http://cz.muxihuayi.cn

Go:   strings.Join(items, ",")
来源：http://ql.szsharing.cn

Ruby: items.join(",")
来源：http://qy.yuntaijiaju.cn

C#:   string.Join(",", items)
来源：http://rs.jianghongdianzi.cn

[E09] 去除所有空白字符
来源：http://nm.shxzukj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jc.huanxung.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bk.jctech888.com.cn

JS:   s.replace(/\s+/g, "")
来源：http://pi.521024.cn

TS:   s.replace(/\s+/g, "")
来源：http://mt.yuexingan06.cn

Java: s.replaceAll("\\s+", "")
来源：http://sh.bookmarksfly.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://rw.colortex.cn

Ruby: s.gsub(/\s+/, "")
来源：http://oi.shxzskj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vf.nicolike.cn

[E10] 左侧补零 / 定长填充
来源：http://cu.jctech888.com.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://sf.muxihuayi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wy.9csxet.cn

JS:   "7".padStart(3, "0")
来源：http://sv.nszjky.cn

TS:   "7".padStart(3, "0")
来源：http://gd.shtwfgs.cn

Java: String.format("%03d", 7)
来源：http://bg.hahajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://co.colortex.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yh.lnxyls.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://st.colortex.cn

[E11] 反转字符串
来源：http://qy.yuexingan06.cn

Py:   s[::-1]
来源：http://os.shxzukj.cn

PHP:  strrev($s);
来源：http://pi.nszjky.cn

JS:   [...s].reverse().join("")
来源：http://jn.newstarts.cn

TS:   [...s].reverse().join("")
来源：http://qo.szsharing.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://mj.szsharing.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ga.jctech888.com.cn

Ruby: s.reverse
来源：http://vk.hnjuh.cn

C#:   new string(s.Reverse().ToArray())
来源：http://iy.bjjhwx.cn

[E12] 统计某字符出现次数
来源：http://ug.colortex.cn

Py:   s.count("a")
来源：http://vm.hnjuh.cn

PHP:  substr_count($s, "a");
来源：http://rc.colortex.cn

JS:   s.split("a").length - 1
来源：http://si.chemitech.net.cn

TS:   s.split("a").length - 1
来源：http://tt.chemitech.net.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gj.521024.cn

Go:   strings.Count(s, "a")
来源：http://oz.hahajie.cn

Ruby: s.count("a")
来源：http://da.szxytkj.cn

C#:   s.Count(c => c == 'a')
来源：http://ej.szxytkj.cn

[E13] 逐字符遍历
来源：http://kk.huanxung.cn

Py:   for ch in s: print(ch)
来源：http://nd.lnxyls.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hc.shxzskj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://wj.bookmarksfly.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ay.shtwfgs.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ou.huanxung.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ej.shxzukj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://oa.9csxet.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://sv.yuexingan06.cn

[E14] URL 编码与 Base64
来源：http://sw.gzmigu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xq.yuexingan06.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ek.shxzukj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yn.bjjhwx.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dd.huanxung.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wk.shxzskj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tj.asd995.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zl.newstarts.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://da.yuntaijiaju.cn

[E15] HTML 转义 / 反转义
来源：http://bj.haigaiapp.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://hu.muxihuayi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yq.hnjuh.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vs.asd995.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://vk.521024.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ae.szsharing.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://be.521024.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xv.jctech888.com.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ln.huanxung.cn

[E16] 数字千分位
来源：http://ok.yuntaijiaju.cn

Py:   f"{1234567:,}"
来源：http://ch.panjiajie.cn

PHP:  number_format(1234567);
来源：http://ja.nszjky.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://xz.szsharing.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://bp.shxzskj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ni.yuntaijiaju.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qj.521024.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://uy.bookmarksfly.cn

C#:   1234567.ToString("N0")
来源：http://jn.colortex.cn

[E17] 首字母大写
来源：http://iq.jctech888.com.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wd.lnxyls.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ab.huixinmuqiang.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oy.lnxyls.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qh.jctech888.com.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vx.shxzukj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://do.newstarts.cn

Ruby: s.capitalize
来源：http://fo.bjjhwx.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ck.521024.cn

[E18] 模板占位符替换
来源：http://ms.jianghongdianzi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ba.szsharing.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://um.huixinmuqiang.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ex.chemitech.net.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://id.lnxyls.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kh.chemitech.net.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xm.yuntaijiaju.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tr.muxihuayi.cn


<!-- 参考信息 -->