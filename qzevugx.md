代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rg.huixiangedu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dc.huixiangedu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wu.asd995.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bv.yuntaijiaju.cn

[D11] 反转数组
来源：http://pd.gzmigu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://yh.huixinmuqiang.cn

PHP:  array_reverse($arr);
来源：http://lu.szxytkj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://at.yuexingan06.cn

TS:   [...arr].reverse();
来源：http://vf.chemitech.net.cn

Java: Collections.reverse(list);
来源：http://ob.lnxyls.cn

Go:   slices.Reverse(arr)
来源：http://ro.hnjuh.cn

Ruby: arr.reverse
来源：http://jq.lnxyls.cn

C#:   list.Reverse();
来源：http://gm.shtwfgs.cn

[D12] 查找元素下标
来源：http://li.yuexingan06.cn

Py:   arr.index(x);  x in arr
来源：http://ly.bjjhwx.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://to.shxzskj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oc.muxihuayi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ro.panjiajie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ce.huixiangedu.cn

Go:   slices.Index(arr, x)
来源：http://an.muxihuayi.cn

Ruby: arr.index(x)
来源：http://xn.bookmarksfly.cn

C#:   list.IndexOf(x);
来源：http://ie.yuntaijiaju.cn

[D13] 过滤（保留满足条件的）
来源：http://tg.yuntaijiaju.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wj.jianghongdianzi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://uz.chemitech.net.cn

JS:   arr.filter(x => x > 3)
来源：http://no.newstarts.cn

TS:   arr.filter(x => x > 3)
来源：http://qg.nicolike.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://sn.nicolike.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ub.shtwfgs.cn

Ruby: arr.select { |x| x > 3 }
来源：http://jt.jctech888.com.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://rw.jctech888.com.cn

[D14] 映射转换（每个元素变形）
来源：http://ue.szsharing.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fh.szsharing.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cg.shtwfgs.cn

JS:   arr.map(x => x * 2)
来源：http://xi.hnjuh.cn

TS:   arr.map(x => x * 2)
来源：http://vr.shxzskj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ss.wgjwhj.cn

Go:   // 手写循环
来源：http://uq.gzmigu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jh.muxihuayi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://me.muxihuayi.cn

[D15] 去重
来源：http://mf.huixinmuqiang.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jo.shxzskj.cn

PHP:  array_unique($arr);
来源：http://om.bookmarksfly.cn

JS:   [...new Set(arr)]
来源：http://xt.shxzskj.cn

TS:   [...new Set(arr)]
来源：http://da.lnxyls.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hf.asd995.cn

Go:   // 用 map[T]struct{} 手写
来源：http://dk.szxytkj.cn

Ruby: arr.uniq
来源：http://or.wgjwhj.cn

C#:   list.Distinct().ToList()
来源：http://yu.huanxung.cn

[D16] 求和与平均值
来源：http://pt.hnjuh.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qr.nszjky.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bn.szxytkj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pg.nicolike.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wn.bjjhwx.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://it.521024.cn

Go:   // 手写循环累加
来源：http://rg.bjjhwx.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ui.colortex.cn

C#:   list.Sum();  list.Average()
来源：http://tv.szsharing.cn

[D17] 最大值与最小值
来源：http://yn.haigaiapp.cn

Py:   max(arr);  min(arr)
来源：http://ah.shtwfgs.cn

PHP:  max($arr);  min($arr);
来源：http://xk.hnjuh.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vd.nicolike.cn

TS:   Math.max(...arr);
来源：http://fb.lnxyls.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://nl.gzmigu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hb.lnxyls.cn

Ruby: arr.max;  arr.min
来源：http://io.huanxung.cn

C#:   list.Max();  list.Min()
来源：http://yu.nszjky.cn

[D18] 扁平化嵌套数组
来源：http://sl.chemitech.net.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xr.shxzukj.cn

PHP:  array_merge(...$nested);
来源：http://oi.szsharing.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ab.szsharing.cn

TS:   nested.flat();
来源：http://ot.nszjky.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hs.bookmarksfly.cn

Go:   // 手写双层循环
来源：http://uy.shxzukj.cn

Ruby: nested.flatten
来源：http://hi.colortex.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ix.yuntaijiaju.cn

[D19] 按字段分组
来源：http://pa.huixinmuqiang.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bp.szsharing.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://us.521024.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vq.hahajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://gu.shtwfgs.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://my.asd995.cn

Go:   // 手写 map[string][]T
来源：http://us.lnxyls.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://wj.chemitech.net.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ay.hahajie.cn

[D20] 统计每个元素出现次数
来源：http://rf.haigaiapp.cn

Py:   Counter(arr)
来源：http://qm.szxytkj.cn

PHP:  array_count_values($arr);
来源：http://cm.lnxyls.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ig.nicolike.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bb.shxzskj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tm.lnxyls.cn

Go:   // 手写 map[T]int
来源：http://ez.asd995.cn

Ruby: arr.tally
来源：http://ih.panjiajie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jt.gzmigu.cn

[D21] 判断是否包含某元素
来源：http://gf.hahajie.cn

Py:   x in arr
来源：http://qi.newstarts.cn

PHP:  in_array($x, $arr, true);
来源：http://oy.jctech888.com.cn

JS:   arr.includes(x)
来源：http://ty.nszjky.cn

TS:   arr.includes(x)
来源：http://ei.szsharing.cn

Java: list.contains(x)
来源：http://mk.nicolike.cn

Go:   slices.Contains(arr, x)
来源：http://kl.nicolike.cn

Ruby: arr.include?(x)
来源：http://qw.asd995.cn

C#:   list.Contains(x)
来源：http://rq.shtwfgs.cn

[D22] 复制数组（避免共享引用）
来源：http://uk.lnxyls.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fe.lnxyls.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ug.9csxet.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zw.521024.cn

TS:   [...arr];
来源：http://kd.newstarts.cn

Java: new ArrayList<>(list);
来源：http://br.bookmarksfly.cn

Go:   copied := append([]int(nil), arr...)
来源：http://op.jianghongdianzi.cn

Ruby: arr.dup;  arr.clone
来源：http://vo.newstarts.cn

C#:   new List<int>(list);
来源：http://cn.yuntaijiaju.cn

[D23] reduce 累积计算
来源：http://fq.szsharing.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://aa.wgjwhj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pm.nicolike.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ta.asd995.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xn.szxytkj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://hm.szxytkj.cn

Go:   // 手写循环
来源：http://aq.chemitech.net.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yh.szxytkj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://aq.bookmarksfly.cn

[D24] 字典 / Map 基本操作
来源：http://kx.521024.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://op.szsharing.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jd.hahajie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://is.wgjwhj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://re.bookmarksfly.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zc.bjjhwx.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sg.hnjuh.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ja.bookmarksfly.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tu.panjiajie.cn

[D25] Set 集合去重与交并差
来源：http://el.jctech888.com.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zv.bjjhwx.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sv.nszjky.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lu.muxihuayi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rd.bjjhwx.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lw.lnxyls.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wz.colortex.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://je.muxihuayi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://li.huixiangedu.cn

[D26] 数组转字符串
来源：http://pe.hnjuh.cn

Py:   ", ".join(map(str, arr))
来源：http://hi.jctech888.com.cn

PHP:  implode(", ", $arr);
来源：http://jj.haigaiapp.cn

JS:   arr.join(", ")
来源：http://xd.yuntaijiaju.cn

TS:   arr.join(", ")
来源：http://nu.wgjwhj.cn

Java: String.join(", ", list)
来源：http://hv.panjiajie.cn

Go:   strings.Join(strs, ", ")
来源：http://rg.yuntaijiaju.cn

Ruby: arr.join(", ")
来源：http://hn.huixiangedu.cn

C#:   string.Join(", ", list)
来源：http://zo.huixiangedu.cn

================================================================================
来源：http://at.yuntaijiaju.cn

E. 字符串处理
来源：http://rv.asd995.cn

================================================================================
来源：http://wd.shxzskj.cn

[E01] 拼接字符串
来源：http://so.gzmigu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bl.bookmarksfly.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dc.colortex.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xo.yuexingan06.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ji.jctech888.com.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xr.yuntaijiaju.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cf.panjiajie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vp.huixinmuqiang.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ra.panjiajie.cn

[E02] 重复字符串
来源：http://ob.hahajie.cn

Py:   "ab" * 3
来源：http://sv.jctech888.com.cn

PHP:  str_repeat("ab", 3);
来源：http://kp.lnxyls.cn

JS:   "ab".repeat(3)
来源：http://jd.shtwfgs.cn

TS:   "ab".repeat(3)
来源：http://oa.huixinmuqiang.cn

Java: "ab".repeat(3)
来源：http://lr.shxzukj.cn

Go:   strings.Repeat("ab", 3)
来源：http://rl.lnxyls.cn

Ruby: "ab" * 3
来源：http://kf.asd995.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ta.hahajie.cn

[E03] 截取子串
来源：http://ns.panjiajie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://om.hnjuh.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nu.huanxung.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bv.jianghongdianzi.cn

TS:   s.slice(1, 4)
来源：http://hv.wgjwhj.cn

Java: s.substring(1, 4)
来源：http://me.huixiangedu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vd.haigaiapp.cn

Ruby: s[1, 3];  s[1..3]
来源：http://uc.chemitech.net.cn

C#:   s.Substring(1, 3)
来源：http://yz.hahajie.cn

[E04] 查找子串位置
来源：http://ap.shxzskj.cn

Py:   s.find("x");  s.index("x")
来源：http://qz.newstarts.cn

PHP:  strpos($s, "x");
来源：http://tc.huixiangedu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://to.bookmarksfly.cn

TS:   s.indexOf("x")
来源：http://gr.colortex.cn

Java: s.indexOf("x")
来源：http://bb.shxzskj.cn

Go:   strings.Index(s, "x")
来源：http://jw.szxytkj.cn

Ruby: s.index("x")
来源：http://ab.szsharing.cn

C#:   s.IndexOf("x")
来源：http://yn.szxytkj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gy.9csxet.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ac.9csxet.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qz.jctech888.com.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rk.muxihuayi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://cy.bookmarksfly.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ww.yuntaijiaju.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pt.bookmarksfly.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fp.shxzskj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fd.hahajie.cn

[E06] 替换子串
来源：http://cn.bookmarksfly.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hw.colortex.cn

PHP:  str_replace("a", "b", $s);
来源：http://kn.jctech888.com.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yk.bjjhwx.cn

TS:   s.replaceAll("a", "b")
来源：http://hz.panjiajie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cg.hnjuh.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://uu.nszjky.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fb.newstarts.cn

C#:   s.Replace("a", "b")
来源：http://ia.gzmigu.cn

[E07] 按分隔符拆分
来源：http://gj.huixinmuqiang.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://be.hnjuh.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tp.chemitech.net.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://hd.asd995.cn

TS:   s.split(",")
来源：http://gw.muxihuayi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://pi.newstarts.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gl.yuexingan06.cn

Ruby: s.split(",");  s.split
来源：http://lr.9csxet.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xd.jctech888.com.cn

[E08] 数组按分隔符合并
来源：http://vs.yuntaijiaju.cn

Py:   ",".join(items)
来源：http://wb.521024.cn

PHP:  implode(",", $items);
来源：http://ks.chemitech.net.cn

JS:   items.join(",")
来源：http://tw.newstarts.cn

TS:   items.join(",")
来源：http://bw.9csxet.cn

Java: String.join(",", items)
来源：http://ur.colortex.cn

Go:   strings.Join(items, ",")
来源：http://qx.muxihuayi.cn

Ruby: items.join(",")
来源：http://hx.colortex.cn

C#:   string.Join(",", items)
来源：http://kt.jctech888.com.cn

[E09] 去除所有空白字符
来源：http://xl.hahajie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://co.szsharing.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://so.szsharing.cn

JS:   s.replace(/\s+/g, "")
来源：http://wn.521024.cn

TS:   s.replace(/\s+/g, "")
来源：http://qs.szsharing.cn

Java: s.replaceAll("\\s+", "")
来源：http://hk.shtwfgs.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://fu.shxzukj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://oh.yuexingan06.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pq.muxihuayi.cn

[E10] 左侧补零 / 定长填充
来源：http://jb.bookmarksfly.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mm.asd995.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jq.shxzskj.cn

JS:   "7".padStart(3, "0")
来源：http://ul.yuntaijiaju.cn

TS:   "7".padStart(3, "0")
来源：http://fm.jctech888.com.cn

Java: String.format("%03d", 7)
来源：http://uf.yuntaijiaju.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://yr.asd995.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pn.asd995.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hw.newstarts.cn

[E11] 反转字符串
来源：http://gw.bjjhwx.cn

Py:   s[::-1]
来源：http://xn.colortex.cn

PHP:  strrev($s);
来源：http://ep.wgjwhj.cn

JS:   [...s].reverse().join("")
来源：http://qd.huanxung.cn

TS:   [...s].reverse().join("")
来源：http://da.shtwfgs.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://cp.nicolike.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://lk.muxihuayi.cn

Ruby: s.reverse
来源：http://td.yuntaijiaju.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qn.jctech888.com.cn

[E12] 统计某字符出现次数
来源：http://vv.huanxung.cn

Py:   s.count("a")
来源：http://tm.521024.cn

PHP:  substr_count($s, "a");
来源：http://ue.shxzskj.cn

JS:   s.split("a").length - 1
来源：http://rt.huanxung.cn

TS:   s.split("a").length - 1
来源：http://dd.wgjwhj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zk.panjiajie.cn

Go:   strings.Count(s, "a")
来源：http://gi.nicolike.cn

Ruby: s.count("a")
来源：http://wv.huixinmuqiang.cn

C#:   s.Count(c => c == 'a')
来源：http://wt.9csxet.cn

[E13] 逐字符遍历
来源：http://of.muxihuayi.cn

Py:   for ch in s: print(ch)
来源：http://gm.newstarts.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pg.panjiajie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://jn.szsharing.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://fw.521024.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gm.hahajie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rm.bookmarksfly.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://cf.nicolike.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nc.chemitech.net.cn

[E14] URL 编码与 Base64
来源：http://tt.shxzskj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ha.hahajie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://vg.chemitech.net.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fq.wgjwhj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wx.9csxet.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bc.gzmigu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://uv.colortex.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://co.jctech888.com.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sm.huanxung.cn

[E15] HTML 转义 / 反转义
来源：http://ap.asd995.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://gm.yuntaijiaju.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ow.yuntaijiaju.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lb.jianghongdianzi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ny.panjiajie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qs.shxzskj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qd.shtwfgs.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wb.muxihuayi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jj.lnxyls.cn

[E16] 数字千分位
来源：http://fq.newstarts.cn

Py:   f"{1234567:,}"
来源：http://ce.haigaiapp.cn

PHP:  number_format(1234567);
来源：http://fv.521024.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://xz.huixiangedu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://sf.huixiangedu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fn.asd995.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://oz.jctech888.com.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kg.panjiajie.cn

C#:   1234567.ToString("N0")
来源：http://tr.asd995.cn

[E17] 首字母大写
来源：http://mk.9csxet.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mx.szxytkj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://qk.shtwfgs.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ci.hahajie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qp.huixinmuqiang.cn


<!-- 参考信息 -->