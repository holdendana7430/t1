代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ww.panjiajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sp.hnjuh.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vw.chemitech.net.cn

Go:   slices.Index(arr, x)
来源：http://zm.nicolike.cn

Ruby: arr.index(x)
来源：http://lr.newstarts.cn

C#:   list.IndexOf(x);
来源：http://lx.shxzukj.cn

[D13] 过滤（保留满足条件的）
来源：http://el.szxytkj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ul.shxzukj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bn.huixiangedu.cn

JS:   arr.filter(x => x > 3)
来源：http://az.hahajie.cn

TS:   arr.filter(x => x > 3)
来源：http://jo.521024.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wh.hahajie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://in.bookmarksfly.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ph.521024.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://of.shxzskj.cn

[D14] 映射转换（每个元素变形）
来源：http://jc.jctech888.com.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gj.bjjhwx.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sl.huixinmuqiang.cn

JS:   arr.map(x => x * 2)
来源：http://cj.asd995.cn

TS:   arr.map(x => x * 2)
来源：http://na.huanxung.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://dj.gzmigu.cn

Go:   // 手写循环
来源：http://nv.bookmarksfly.cn

Ruby: arr.map { |x| x * 2 }
来源：http://lj.szxytkj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://rq.haigaiapp.cn

[D15] 去重
来源：http://ry.yuntaijiaju.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lt.gzmigu.cn

PHP:  array_unique($arr);
来源：http://uz.szsharing.cn

JS:   [...new Set(arr)]
来源：http://gn.szxytkj.cn

TS:   [...new Set(arr)]
来源：http://vo.nicolike.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lt.shtwfgs.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ch.huixinmuqiang.cn

Ruby: arr.uniq
来源：http://fv.521024.cn

C#:   list.Distinct().ToList()
来源：http://xz.jianghongdianzi.cn

[D16] 求和与平均值
来源：http://ms.panjiajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gw.shtwfgs.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sj.wgjwhj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rr.huixinmuqiang.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lt.hnjuh.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wm.yuexingan06.cn

Go:   // 手写循环累加
来源：http://su.jianghongdianzi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cg.huixiangedu.cn

C#:   list.Sum();  list.Average()
来源：http://ax.colortex.cn

[D17] 最大值与最小值
来源：http://zj.wgjwhj.cn

Py:   max(arr);  min(arr)
来源：http://fe.colortex.cn

PHP:  max($arr);  min($arr);
来源：http://ps.huixiangedu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://iv.shtwfgs.cn

TS:   Math.max(...arr);
来源：http://ei.521024.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ny.panjiajie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tq.nszjky.cn

Ruby: arr.max;  arr.min
来源：http://qo.newstarts.cn

C#:   list.Max();  list.Min()
来源：http://wz.9csxet.cn

[D18] 扁平化嵌套数组
来源：http://cm.szxytkj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ud.chemitech.net.cn

PHP:  array_merge(...$nested);
来源：http://dd.hahajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zy.hahajie.cn

TS:   nested.flat();
来源：http://vm.yuexingan06.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://om.wgjwhj.cn

Go:   // 手写双层循环
来源：http://ks.wgjwhj.cn

Ruby: nested.flatten
来源：http://um.colortex.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://vg.shxzukj.cn

[D19] 按字段分组
来源：http://lj.chemitech.net.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yn.shtwfgs.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://oa.bjjhwx.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ng.9csxet.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://df.chemitech.net.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://uz.huanxung.cn

Go:   // 手写 map[string][]T
来源：http://ma.521024.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://jb.wgjwhj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vr.lnxyls.cn

[D20] 统计每个元素出现次数
来源：http://gh.huixiangedu.cn

Py:   Counter(arr)
来源：http://lp.hahajie.cn

PHP:  array_count_values($arr);
来源：http://sg.shxzukj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gd.521024.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vi.shtwfgs.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ud.bjjhwx.cn

Go:   // 手写 map[T]int
来源：http://kr.huixiangedu.cn

Ruby: arr.tally
来源：http://zn.bjjhwx.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://id.shtwfgs.cn

[D21] 判断是否包含某元素
来源：http://qp.hahajie.cn

Py:   x in arr
来源：http://yk.colortex.cn

PHP:  in_array($x, $arr, true);
来源：http://kz.nszjky.cn

JS:   arr.includes(x)
来源：http://pp.wgjwhj.cn

TS:   arr.includes(x)
来源：http://bu.hnjuh.cn

Java: list.contains(x)
来源：http://dz.newstarts.cn

Go:   slices.Contains(arr, x)
来源：http://tn.jianghongdianzi.cn

Ruby: arr.include?(x)
来源：http://yw.newstarts.cn

C#:   list.Contains(x)
来源：http://vl.shxzukj.cn

[D22] 复制数组（避免共享引用）
来源：http://mv.haigaiapp.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zt.huixinmuqiang.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dx.jctech888.com.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://he.shxzskj.cn

TS:   [...arr];
来源：http://ws.huixiangedu.cn

Java: new ArrayList<>(list);
来源：http://fi.yuntaijiaju.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qw.521024.cn

Ruby: arr.dup;  arr.clone
来源：http://vy.nszjky.cn

C#:   new List<int>(list);
来源：http://xk.gzmigu.cn

[D23] reduce 累积计算
来源：http://yq.nicolike.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gw.wgjwhj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://aw.gzmigu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hl.panjiajie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wu.lnxyls.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://lv.szxytkj.cn

Go:   // 手写循环
来源：http://zf.lnxyls.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jd.shxzukj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bb.newstarts.cn

[D24] 字典 / Map 基本操作
来源：http://vz.jctech888.com.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ns.hahajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gu.hnjuh.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://us.muxihuayi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fn.muxihuayi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kp.newstarts.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hw.bookmarksfly.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cw.lnxyls.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qv.huixiangedu.cn

[D25] Set 集合去重与交并差
来源：http://vn.asd995.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hc.jctech888.com.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://aq.shtwfgs.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://sd.shxzskj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rd.shtwfgs.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ft.panjiajie.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ly.shtwfgs.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bj.chemitech.net.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xz.jctech888.com.cn

[D26] 数组转字符串
来源：http://xl.nszjky.cn

Py:   ", ".join(map(str, arr))
来源：http://pg.9csxet.cn

PHP:  implode(", ", $arr);
来源：http://mc.szxytkj.cn

JS:   arr.join(", ")
来源：http://gh.shxzukj.cn

TS:   arr.join(", ")
来源：http://jr.gzmigu.cn

Java: String.join(", ", list)
来源：http://eb.szsharing.cn

Go:   strings.Join(strs, ", ")
来源：http://gq.bookmarksfly.cn

Ruby: arr.join(", ")
来源：http://tj.bookmarksfly.cn

C#:   string.Join(", ", list)
来源：http://wv.wgjwhj.cn

================================================================================
来源：http://eg.jianghongdianzi.cn

E. 字符串处理
来源：http://lh.hnjuh.cn

================================================================================
来源：http://xv.hnjuh.cn

[E01] 拼接字符串
来源：http://xu.jianghongdianzi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xl.szxytkj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sa.9csxet.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ye.colortex.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ma.jctech888.com.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://os.bjjhwx.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ph.huixiangedu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pi.huanxung.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vx.newstarts.cn

[E02] 重复字符串
来源：http://id.hnjuh.cn

Py:   "ab" * 3
来源：http://fw.newstarts.cn

PHP:  str_repeat("ab", 3);
来源：http://el.jianghongdianzi.cn

JS:   "ab".repeat(3)
来源：http://up.9csxet.cn

TS:   "ab".repeat(3)
来源：http://jg.asd995.cn

Java: "ab".repeat(3)
来源：http://xm.bjjhwx.cn

Go:   strings.Repeat("ab", 3)
来源：http://yt.huixinmuqiang.cn

Ruby: "ab" * 3
来源：http://pz.chemitech.net.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xq.colortex.cn

[E03] 截取子串
来源：http://zj.nszjky.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://km.panjiajie.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lg.muxihuayi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fa.haigaiapp.cn

TS:   s.slice(1, 4)
来源：http://xg.521024.cn

Java: s.substring(1, 4)
来源：http://rc.bookmarksfly.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wp.jianghongdianzi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://rh.bookmarksfly.cn

C#:   s.Substring(1, 3)
来源：http://mo.lnxyls.cn

[E04] 查找子串位置
来源：http://nv.hnjuh.cn

Py:   s.find("x");  s.index("x")
来源：http://oc.gzmigu.cn

PHP:  strpos($s, "x");
来源：http://ss.shxzskj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qe.bookmarksfly.cn

TS:   s.indexOf("x")
来源：http://sx.szxytkj.cn

Java: s.indexOf("x")
来源：http://sq.wgjwhj.cn

Go:   strings.Index(s, "x")
来源：http://nc.yuntaijiaju.cn

Ruby: s.index("x")
来源：http://fr.wgjwhj.cn

C#:   s.IndexOf("x")
来源：http://bw.shtwfgs.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://wc.nszjky.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fz.shxzskj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fl.shxzskj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xl.huixinmuqiang.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://tx.panjiajie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wt.lnxyls.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vy.huanxung.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xb.jianghongdianzi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ih.muxihuayi.cn

[E06] 替换子串
来源：http://sh.muxihuayi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ti.bjjhwx.cn

PHP:  str_replace("a", "b", $s);
来源：http://sx.newstarts.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jg.szsharing.cn

TS:   s.replaceAll("a", "b")
来源：http://gp.shtwfgs.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jn.haigaiapp.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tb.9csxet.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bf.huanxung.cn

C#:   s.Replace("a", "b")
来源：http://uk.hahajie.cn

[E07] 按分隔符拆分
来源：http://yb.haigaiapp.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bm.521024.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wu.asd995.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://di.hnjuh.cn

TS:   s.split(",")
来源：http://vf.lnxyls.cn

Java: s.split(",");  s.split("\\s+")
来源：http://fz.shxzukj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://sd.shxzukj.cn

Ruby: s.split(",");  s.split
来源：http://nc.jctech888.com.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dq.gzmigu.cn

[E08] 数组按分隔符合并
来源：http://vu.jctech888.com.cn

Py:   ",".join(items)
来源：http://up.yuexingan06.cn

PHP:  implode(",", $items);
来源：http://iw.huixiangedu.cn

JS:   items.join(",")
来源：http://jt.panjiajie.cn

TS:   items.join(",")
来源：http://li.bjjhwx.cn

Java: String.join(",", items)
来源：http://rj.lnxyls.cn

Go:   strings.Join(items, ",")
来源：http://hc.jianghongdianzi.cn

Ruby: items.join(",")
来源：http://eq.bookmarksfly.cn

C#:   string.Join(",", items)
来源：http://tj.muxihuayi.cn

[E09] 去除所有空白字符
来源：http://go.asd995.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://th.jianghongdianzi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ml.hahajie.cn

JS:   s.replace(/\s+/g, "")
来源：http://ob.muxihuayi.cn

TS:   s.replace(/\s+/g, "")
来源：http://fb.newstarts.cn

Java: s.replaceAll("\\s+", "")
来源：http://as.gzmigu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qe.shtwfgs.cn

Ruby: s.gsub(/\s+/, "")
来源：http://wp.nszjky.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uf.bookmarksfly.cn

[E10] 左侧补零 / 定长填充
来源：http://bl.shtwfgs.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://st.wgjwhj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tj.haigaiapp.cn

JS:   "7".padStart(3, "0")
来源：http://ks.bookmarksfly.cn

TS:   "7".padStart(3, "0")
来源：http://xe.asd995.cn

Java: String.format("%03d", 7)
来源：http://al.huixinmuqiang.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ff.jianghongdianzi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gm.huanxung.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://re.szxytkj.cn

[E11] 反转字符串
来源：http://pw.shtwfgs.cn

Py:   s[::-1]
来源：http://bs.jctech888.com.cn

PHP:  strrev($s);
来源：http://hp.huixiangedu.cn

JS:   [...s].reverse().join("")
来源：http://vo.huixiangedu.cn

TS:   [...s].reverse().join("")
来源：http://hm.shxzukj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://tw.9csxet.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://xp.huixinmuqiang.cn

Ruby: s.reverse
来源：http://fy.colortex.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ob.shxzukj.cn

[E12] 统计某字符出现次数
来源：http://qg.bjjhwx.cn

Py:   s.count("a")
来源：http://jf.chemitech.net.cn

PHP:  substr_count($s, "a");
来源：http://yi.jctech888.com.cn

JS:   s.split("a").length - 1
来源：http://ef.521024.cn

TS:   s.split("a").length - 1
来源：http://to.521024.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://er.wgjwhj.cn

Go:   strings.Count(s, "a")
来源：http://qr.asd995.cn

Ruby: s.count("a")
来源：http://dy.bjjhwx.cn

C#:   s.Count(c => c == 'a')
来源：http://tu.huanxung.cn

[E13] 逐字符遍历
来源：http://sd.bjjhwx.cn

Py:   for ch in s: print(ch)
来源：http://bk.chemitech.net.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://br.szxytkj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://re.bjjhwx.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ng.wgjwhj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tv.huixiangedu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sy.newstarts.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://il.nicolike.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yh.lnxyls.cn

[E14] URL 编码与 Base64
来源：http://rs.nszjky.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yq.muxihuayi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ad.nszjky.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vu.bjjhwx.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://az.521024.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fh.colortex.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qj.nicolike.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cw.newstarts.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wx.gzmigu.cn

[E15] HTML 转义 / 反转义
来源：http://en.wgjwhj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://jf.jianghongdianzi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ty.bookmarksfly.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yu.muxihuayi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ki.huixiangedu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mg.shxzskj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yk.yuexingan06.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mc.521024.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://sp.jctech888.com.cn

[E16] 数字千分位
来源：http://es.newstarts.cn

Py:   f"{1234567:,}"
来源：http://iv.lnxyls.cn

PHP:  number_format(1234567);
来源：http://ea.asd995.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://za.521024.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ao.shxzskj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://at.muxihuayi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tw.panjiajie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://yt.bjjhwx.cn

C#:   1234567.ToString("N0")
来源：http://kn.muxihuayi.cn

[E17] 首字母大写
来源：http://zr.bookmarksfly.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vq.yuntaijiaju.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://vc.jianghongdianzi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hj.nszjky.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dt.jctech888.com.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zg.521024.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jl.chemitech.net.cn

Ruby: s.capitalize
来源：http://ju.yuexingan06.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zq.yuntaijiaju.cn

[E18] 模板占位符替换
来源：http://tx.newstarts.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mw.lnxyls.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tf.shxzukj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zi.muxihuayi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ze.huixinmuqiang.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://an.chemitech.net.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kn.szsharing.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://oj.9csxet.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qu.jctech888.com.cn

[E19] 多行文本按行拆分
来源：http://lw.jctech888.com.cn

Py:   s.splitlines()
来源：http://pq.lnxyls.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mf.521024.cn


<!-- 参考信息 -->