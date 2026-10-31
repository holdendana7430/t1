代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yb.huixiangedu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oh.chemitech.net.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xs.hahajie.cn

Go:   slices.Index(arr, x)
来源：http://mm.hahajie.cn

Ruby: arr.index(x)
来源：http://zt.bjjhwx.cn

C#:   list.IndexOf(x);
来源：http://vl.shxzskj.cn

[D13] 过滤（保留满足条件的）
来源：http://fs.yuexingan06.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gs.asd995.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kp.nszjky.cn

JS:   arr.filter(x => x > 3)
来源：http://io.yuntaijiaju.cn

TS:   arr.filter(x => x > 3)
来源：http://cr.shtwfgs.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mc.nszjky.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gb.bookmarksfly.cn

Ruby: arr.select { |x| x > 3 }
来源：http://lt.521024.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://sb.huixiangedu.cn

[D14] 映射转换（每个元素变形）
来源：http://ho.szsharing.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ak.shtwfgs.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://me.huixiangedu.cn

JS:   arr.map(x => x * 2)
来源：http://tc.shxzskj.cn

TS:   arr.map(x => x * 2)
来源：http://hh.colortex.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://nd.hnjuh.cn

Go:   // 手写循环
来源：http://yp.shxzukj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://go.colortex.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zw.gzmigu.cn

[D15] 去重
来源：http://rf.huixiangedu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://uc.nszjky.cn

PHP:  array_unique($arr);
来源：http://fc.szsharing.cn

JS:   [...new Set(arr)]
来源：http://wu.bookmarksfly.cn

TS:   [...new Set(arr)]
来源：http://ik.chemitech.net.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://td.jianghongdianzi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://eg.9csxet.cn

Ruby: arr.uniq
来源：http://wj.bjjhwx.cn

C#:   list.Distinct().ToList()
来源：http://fz.panjiajie.cn

[D16] 求和与平均值
来源：http://za.shxzukj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jb.521024.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://um.huixiangedu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xg.bookmarksfly.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vb.asd995.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://td.muxihuayi.cn

Go:   // 手写循环累加
来源：http://og.haigaiapp.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jl.colortex.cn

C#:   list.Sum();  list.Average()
来源：http://ts.bookmarksfly.cn

[D17] 最大值与最小值
来源：http://mo.bookmarksfly.cn

Py:   max(arr);  min(arr)
来源：http://dn.nszjky.cn

PHP:  max($arr);  min($arr);
来源：http://fr.bookmarksfly.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qc.yuexingan06.cn

TS:   Math.max(...arr);
来源：http://pn.shtwfgs.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jy.chemitech.net.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ku.yuexingan06.cn

Ruby: arr.max;  arr.min
来源：http://vo.haigaiapp.cn

C#:   list.Max();  list.Min()
来源：http://gu.chemitech.net.cn

[D18] 扁平化嵌套数组
来源：http://qj.bjjhwx.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fq.hnjuh.cn

PHP:  array_merge(...$nested);
来源：http://ot.gzmigu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hl.yuexingan06.cn

TS:   nested.flat();
来源：http://bf.hnjuh.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dx.huixinmuqiang.cn

Go:   // 手写双层循环
来源：http://yr.huanxung.cn

Ruby: nested.flatten
来源：http://fg.panjiajie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ky.gzmigu.cn

[D19] 按字段分组
来源：http://jn.wgjwhj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://in.haigaiapp.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bn.szsharing.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wy.yuexingan06.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://bj.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ce.wgjwhj.cn

Go:   // 手写 map[string][]T
来源：http://bv.huixiangedu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://in.huixiangedu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kf.shtwfgs.cn

[D20] 统计每个元素出现次数
来源：http://iv.yuntaijiaju.cn

Py:   Counter(arr)
来源：http://go.jctech888.com.cn

PHP:  array_count_values($arr);
来源：http://il.haigaiapp.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uh.huanxung.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kd.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qx.nszjky.cn

Go:   // 手写 map[T]int
来源：http://bn.muxihuayi.cn

Ruby: arr.tally
来源：http://cp.shxzskj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ct.shxzskj.cn

[D21] 判断是否包含某元素
来源：http://qf.shxzskj.cn

Py:   x in arr
来源：http://ee.bookmarksfly.cn

PHP:  in_array($x, $arr, true);
来源：http://so.huanxung.cn

JS:   arr.includes(x)
来源：http://lq.wgjwhj.cn

TS:   arr.includes(x)
来源：http://sa.panjiajie.cn

Java: list.contains(x)
来源：http://hk.nicolike.cn

Go:   slices.Contains(arr, x)
来源：http://gc.muxihuayi.cn

Ruby: arr.include?(x)
来源：http://pp.muxihuayi.cn

C#:   list.Contains(x)
来源：http://gn.szsharing.cn

[D22] 复制数组（避免共享引用）
来源：http://xy.chemitech.net.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rl.jianghongdianzi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kh.huanxung.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ke.bjjhwx.cn

TS:   [...arr];
来源：http://rz.bjjhwx.cn

Java: new ArrayList<>(list);
来源：http://sz.asd995.cn

Go:   copied := append([]int(nil), arr...)
来源：http://hv.asd995.cn

Ruby: arr.dup;  arr.clone
来源：http://bo.huixiangedu.cn

C#:   new List<int>(list);
来源：http://gy.haigaiapp.cn

[D23] reduce 累积计算
来源：http://jb.huanxung.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zg.jianghongdianzi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zt.hnjuh.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zh.lnxyls.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oo.hnjuh.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://lv.szxytkj.cn

Go:   // 手写循环
来源：http://ml.9csxet.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tj.asd995.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vp.colortex.cn

[D24] 字典 / Map 基本操作
来源：http://hw.asd995.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://sm.huanxung.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ga.yuexingan06.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bk.hnjuh.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tt.asd995.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xq.shxzukj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yw.huixiangedu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jp.asd995.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nh.panjiajie.cn

[D25] Set 集合去重与交并差
来源：http://ac.muxihuayi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tu.wgjwhj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lq.nicolike.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ac.szsharing.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nw.lnxyls.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mb.521024.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://oh.panjiajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nb.chemitech.net.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jo.hnjuh.cn

[D26] 数组转字符串
来源：http://bk.gzmigu.cn

Py:   ", ".join(map(str, arr))
来源：http://pm.shtwfgs.cn

PHP:  implode(", ", $arr);
来源：http://qr.shtwfgs.cn

JS:   arr.join(", ")
来源：http://ox.huanxung.cn

TS:   arr.join(", ")
来源：http://bp.asd995.cn

Java: String.join(", ", list)
来源：http://am.shxzskj.cn

Go:   strings.Join(strs, ", ")
来源：http://xw.shxzukj.cn

Ruby: arr.join(", ")
来源：http://eg.bjjhwx.cn

C#:   string.Join(", ", list)
来源：http://le.521024.cn

================================================================================
来源：http://vq.wgjwhj.cn

E. 字符串处理
来源：http://in.wgjwhj.cn

================================================================================
来源：http://nd.nszjky.cn

[E01] 拼接字符串
来源：http://qq.521024.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://uu.huanxung.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ow.newstarts.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kp.huanxung.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xd.huixinmuqiang.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://me.muxihuayi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ux.9csxet.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wy.chemitech.net.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qf.jianghongdianzi.cn

[E02] 重复字符串
来源：http://ty.huixinmuqiang.cn

Py:   "ab" * 3
来源：http://za.wgjwhj.cn

PHP:  str_repeat("ab", 3);
来源：http://ag.yuntaijiaju.cn

JS:   "ab".repeat(3)
来源：http://ak.huixiangedu.cn

TS:   "ab".repeat(3)
来源：http://vv.colortex.cn

Java: "ab".repeat(3)
来源：http://dr.haigaiapp.cn

Go:   strings.Repeat("ab", 3)
来源：http://pl.shxzskj.cn

Ruby: "ab" * 3
来源：http://gn.521024.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://aw.szsharing.cn

[E03] 截取子串
来源：http://gi.panjiajie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://iz.nicolike.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dh.jianghongdianzi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fq.colortex.cn

TS:   s.slice(1, 4)
来源：http://qf.shtwfgs.cn

Java: s.substring(1, 4)
来源：http://rj.gzmigu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://et.lnxyls.cn

Ruby: s[1, 3];  s[1..3]
来源：http://rc.szsharing.cn

C#:   s.Substring(1, 3)
来源：http://ev.panjiajie.cn

[E04] 查找子串位置
来源：http://jk.yuexingan06.cn

Py:   s.find("x");  s.index("x")
来源：http://yi.shxzukj.cn

PHP:  strpos($s, "x");
来源：http://vj.shtwfgs.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lz.shtwfgs.cn

TS:   s.indexOf("x")
来源：http://ci.jianghongdianzi.cn

Java: s.indexOf("x")
来源：http://er.colortex.cn

Go:   strings.Index(s, "x")
来源：http://hy.szxytkj.cn

Ruby: s.index("x")
来源：http://pc.szxytkj.cn

C#:   s.IndexOf("x")
来源：http://qm.jianghongdianzi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://hw.shtwfgs.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://sv.newstarts.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tm.nicolike.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gy.lnxyls.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hc.9csxet.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ke.shxzskj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mn.nicolike.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://td.huixiangedu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ix.colortex.cn

[E06] 替换子串
来源：http://ho.jctech888.com.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://us.wgjwhj.cn

PHP:  str_replace("a", "b", $s);
来源：http://nr.bjjhwx.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kw.yuexingan06.cn

TS:   s.replaceAll("a", "b")
来源：http://qa.newstarts.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iv.bjjhwx.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mh.huanxung.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hi.szxytkj.cn

C#:   s.Replace("a", "b")
来源：http://mq.haigaiapp.cn

[E07] 按分隔符拆分
来源：http://zq.panjiajie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lo.shxzskj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fz.szxytkj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://jb.hnjuh.cn

TS:   s.split(",")
来源：http://en.hnjuh.cn

Java: s.split(",");  s.split("\\s+")
来源：http://hu.nicolike.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kq.szsharing.cn

Ruby: s.split(",");  s.split
来源：http://ct.muxihuayi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vr.newstarts.cn

[E08] 数组按分隔符合并
来源：http://fo.haigaiapp.cn

Py:   ",".join(items)
来源：http://de.hahajie.cn

PHP:  implode(",", $items);
来源：http://zm.shxzskj.cn

JS:   items.join(",")
来源：http://lw.shtwfgs.cn

TS:   items.join(",")
来源：http://qf.bjjhwx.cn

Java: String.join(",", items)
来源：http://na.haigaiapp.cn

Go:   strings.Join(items, ",")
来源：http://ub.wgjwhj.cn

Ruby: items.join(",")
来源：http://jc.shxzskj.cn

C#:   string.Join(",", items)
来源：http://qf.nicolike.cn

[E09] 去除所有空白字符
来源：http://gb.521024.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rc.shxzskj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wf.newstarts.cn

JS:   s.replace(/\s+/g, "")
来源：http://rg.lnxyls.cn

TS:   s.replace(/\s+/g, "")
来源：http://cp.huixiangedu.cn

Java: s.replaceAll("\\s+", "")
来源：http://zf.shxzskj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ug.szxytkj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ai.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kq.asd995.cn

[E10] 左侧补零 / 定长填充
来源：http://zi.muxihuayi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wq.shxzukj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xj.jctech888.com.cn

JS:   "7".padStart(3, "0")
来源：http://mm.haigaiapp.cn

TS:   "7".padStart(3, "0")
来源：http://qq.jctech888.com.cn

Java: String.format("%03d", 7)
来源：http://mu.gzmigu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://hk.szxytkj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yl.bjjhwx.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ar.gzmigu.cn

[E11] 反转字符串
来源：http://os.gzmigu.cn

Py:   s[::-1]
来源：http://sf.chemitech.net.cn

PHP:  strrev($s);
来源：http://jb.jctech888.com.cn

JS:   [...s].reverse().join("")
来源：http://ax.muxihuayi.cn

TS:   [...s].reverse().join("")
来源：http://cu.jianghongdianzi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://su.huanxung.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://mw.shtwfgs.cn

Ruby: s.reverse
来源：http://ky.szxytkj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://rt.shtwfgs.cn

[E12] 统计某字符出现次数
来源：http://hp.szsharing.cn

Py:   s.count("a")
来源：http://sv.9csxet.cn

PHP:  substr_count($s, "a");
来源：http://wb.shxzskj.cn

JS:   s.split("a").length - 1
来源：http://qx.colortex.cn

TS:   s.split("a").length - 1
来源：http://fh.wgjwhj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://eb.gzmigu.cn

Go:   strings.Count(s, "a")
来源：http://zf.shxzskj.cn

Ruby: s.count("a")
来源：http://lt.asd995.cn

C#:   s.Count(c => c == 'a')
来源：http://it.shxzukj.cn

[E13] 逐字符遍历
来源：http://uj.shxzukj.cn

Py:   for ch in s: print(ch)
来源：http://ri.muxihuayi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lb.9csxet.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://jv.nszjky.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ia.chemitech.net.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zm.jianghongdianzi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kw.nszjky.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://oq.nszjky.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bd.shxzskj.cn

[E14] URL 编码与 Base64
来源：http://ac.huanxung.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gx.hnjuh.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://vn.bjjhwx.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yl.haigaiapp.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dh.shtwfgs.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gq.jianghongdianzi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cn.newstarts.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://sr.huanxung.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://je.asd995.cn

[E15] HTML 转义 / 反转义
来源：http://fz.szsharing.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://mn.chemitech.net.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fd.chemitech.net.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ye.nicolike.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://xt.yuntaijiaju.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pb.huanxung.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://la.shxzskj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bq.wgjwhj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ib.yuexingan06.cn

[E16] 数字千分位
来源：http://ve.nszjky.cn

Py:   f"{1234567:,}"
来源：http://qu.chemitech.net.cn

PHP:  number_format(1234567);
来源：http://pv.jctech888.com.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://yt.hnjuh.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://fi.wgjwhj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jt.chemitech.net.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xh.jctech888.com.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hs.jianghongdianzi.cn

C#:   1234567.ToString("N0")
来源：http://es.chemitech.net.cn

[E17] 首字母大写
来源：http://tx.wgjwhj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zl.nicolike.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://dw.colortex.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dh.colortex.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jw.gzmigu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qj.panjiajie.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nj.bjjhwx.cn

Ruby: s.capitalize
来源：http://bc.asd995.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pc.gzmigu.cn

[E18] 模板占位符替换
来源：http://uo.newstarts.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lu.9csxet.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ks.huixinmuqiang.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zw.shtwfgs.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://qn.shxzskj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vb.bookmarksfly.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gy.chemitech.net.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ub.shxzukj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://eg.chemitech.net.cn

[E19] 多行文本按行拆分
来源：http://pt.chemitech.net.cn

Py:   s.splitlines()
来源：http://sa.colortex.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nl.wgjwhj.cn


<!-- 参考信息 -->