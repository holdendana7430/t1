代发 wailian999

Ruby: arr.index(x)
来源：http://nu.huanxung.cn

C#:   list.IndexOf(x);
来源：http://yq.shxzukj.cn

[D13] 过滤（保留满足条件的）
来源：http://cb.lnxyls.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jh.gzmigu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yu.shtwfgs.cn

JS:   arr.filter(x => x > 3)
来源：http://cr.wgjwhj.cn

TS:   arr.filter(x => x > 3)
来源：http://el.szsharing.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wp.nicolike.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ml.lnxyls.cn

Ruby: arr.select { |x| x > 3 }
来源：http://cx.nszjky.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://zx.shxzskj.cn

[D14] 映射转换（每个元素变形）
来源：http://og.huixinmuqiang.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wf.haigaiapp.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zz.9csxet.cn

JS:   arr.map(x => x * 2)
来源：http://ge.szxytkj.cn

TS:   arr.map(x => x * 2)
来源：http://dj.9csxet.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://jf.lnxyls.cn

Go:   // 手写循环
来源：http://xu.jctech888.com.cn

Ruby: arr.map { |x| x * 2 }
来源：http://zp.szsharing.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://jt.asd995.cn

[D15] 去重
来源：http://bg.szxytkj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xa.hahajie.cn

PHP:  array_unique($arr);
来源：http://fg.yuntaijiaju.cn

JS:   [...new Set(arr)]
来源：http://pd.huixinmuqiang.cn

TS:   [...new Set(arr)]
来源：http://wn.szxytkj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://av.panjiajie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://uv.huixiangedu.cn

Ruby: arr.uniq
来源：http://le.yuexingan06.cn

C#:   list.Distinct().ToList()
来源：http://pr.colortex.cn

[D16] 求和与平均值
来源：http://yo.bjjhwx.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vm.yuntaijiaju.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://uv.yuntaijiaju.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xt.hnjuh.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://at.huixinmuqiang.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jt.shxzskj.cn

Go:   // 手写循环累加
来源：http://kn.chemitech.net.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mv.chemitech.net.cn

C#:   list.Sum();  list.Average()
来源：http://ow.haigaiapp.cn

[D17] 最大值与最小值
来源：http://dl.muxihuayi.cn

Py:   max(arr);  min(arr)
来源：http://ny.huanxung.cn

PHP:  max($arr);  min($arr);
来源：http://xl.bookmarksfly.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yg.colortex.cn

TS:   Math.max(...arr);
来源：http://bw.huanxung.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ie.jctech888.com.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lm.shxzskj.cn

Ruby: arr.max;  arr.min
来源：http://vk.chemitech.net.cn

C#:   list.Max();  list.Min()
来源：http://la.huixinmuqiang.cn

[D18] 扁平化嵌套数组
来源：http://ot.panjiajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ah.chemitech.net.cn

PHP:  array_merge(...$nested);
来源：http://it.hnjuh.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wa.shxzskj.cn

TS:   nested.flat();
来源：http://eb.muxihuayi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wf.521024.cn

Go:   // 手写双层循环
来源：http://ru.jianghongdianzi.cn

Ruby: nested.flatten
来源：http://nb.newstarts.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://tb.huixiangedu.cn

[D19] 按字段分组
来源：http://pp.panjiajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://se.huixinmuqiang.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mp.huanxung.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ve.9csxet.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ip.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qy.huanxung.cn

Go:   // 手写 map[string][]T
来源：http://ym.asd995.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ru.szxytkj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fz.nszjky.cn

[D20] 统计每个元素出现次数
来源：http://sb.shxzukj.cn

Py:   Counter(arr)
来源：http://dw.szxytkj.cn

PHP:  array_count_values($arr);
来源：http://uu.huixiangedu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kx.newstarts.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gy.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://oh.muxihuayi.cn

Go:   // 手写 map[T]int
来源：http://ni.szxytkj.cn

Ruby: arr.tally
来源：http://bs.asd995.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ne.gzmigu.cn

[D21] 判断是否包含某元素
来源：http://yo.yuexingan06.cn

Py:   x in arr
来源：http://lh.panjiajie.cn

PHP:  in_array($x, $arr, true);
来源：http://uv.jianghongdianzi.cn

JS:   arr.includes(x)
来源：http://ed.asd995.cn

TS:   arr.includes(x)
来源：http://iz.jianghongdianzi.cn

Java: list.contains(x)
来源：http://qt.521024.cn

Go:   slices.Contains(arr, x)
来源：http://xv.colortex.cn

Ruby: arr.include?(x)
来源：http://lf.nszjky.cn

C#:   list.Contains(x)
来源：http://sv.hahajie.cn

[D22] 复制数组（避免共享引用）
来源：http://cm.gzmigu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://us.bjjhwx.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xi.shxzukj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://if.huixinmuqiang.cn

TS:   [...arr];
来源：http://rq.bookmarksfly.cn

Java: new ArrayList<>(list);
来源：http://ty.shxzskj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ju.jctech888.com.cn

Ruby: arr.dup;  arr.clone
来源：http://yy.wgjwhj.cn

C#:   new List<int>(list);
来源：http://ys.nicolike.cn

[D23] reduce 累积计算
来源：http://ot.yuntaijiaju.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cv.newstarts.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rc.huixinmuqiang.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ap.asd995.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rf.yuntaijiaju.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://jo.colortex.cn

Go:   // 手写循环
来源：http://gk.shxzskj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ih.lnxyls.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://re.gzmigu.cn

[D24] 字典 / Map 基本操作
来源：http://tw.hnjuh.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tl.hahajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ff.lnxyls.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ac.bookmarksfly.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ib.hnjuh.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ju.nszjky.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ae.nicolike.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pa.wgjwhj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://au.colortex.cn

[D25] Set 集合去重与交并差
来源：http://pu.huixiangedu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dn.yuexingan06.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://td.asd995.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xy.nicolike.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ek.newstarts.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ii.jianghongdianzi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fk.hahajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pv.shtwfgs.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ef.muxihuayi.cn

[D26] 数组转字符串
来源：http://fn.shxzskj.cn

Py:   ", ".join(map(str, arr))
来源：http://ou.yuntaijiaju.cn

PHP:  implode(", ", $arr);
来源：http://mx.huixinmuqiang.cn

JS:   arr.join(", ")
来源：http://fa.huanxung.cn

TS:   arr.join(", ")
来源：http://kl.yuexingan06.cn

Java: String.join(", ", list)
来源：http://gs.newstarts.cn

Go:   strings.Join(strs, ", ")
来源：http://qt.huixiangedu.cn

Ruby: arr.join(", ")
来源：http://za.newstarts.cn

C#:   string.Join(", ", list)
来源：http://jn.hahajie.cn

================================================================================
来源：http://fd.huanxung.cn

E. 字符串处理
来源：http://xk.yuntaijiaju.cn

================================================================================
来源：http://fd.huanxung.cn

[E01] 拼接字符串
来源：http://sw.gzmigu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kv.hnjuh.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jb.jctech888.com.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fk.huixinmuqiang.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cr.nszjky.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yq.bookmarksfly.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ji.shxzukj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xz.shtwfgs.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tv.chemitech.net.cn

[E02] 重复字符串
来源：http://hr.shxzskj.cn

Py:   "ab" * 3
来源：http://qp.huanxung.cn

PHP:  str_repeat("ab", 3);
来源：http://hd.shxzskj.cn

JS:   "ab".repeat(3)
来源：http://zt.9csxet.cn

TS:   "ab".repeat(3)
来源：http://tz.gzmigu.cn

Java: "ab".repeat(3)
来源：http://bl.yuntaijiaju.cn

Go:   strings.Repeat("ab", 3)
来源：http://wu.colortex.cn

Ruby: "ab" * 3
来源：http://lx.huanxung.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ga.muxihuayi.cn

[E03] 截取子串
来源：http://yy.shxzukj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gu.wgjwhj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pn.chemitech.net.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lg.lnxyls.cn

TS:   s.slice(1, 4)
来源：http://ek.lnxyls.cn

Java: s.substring(1, 4)
来源：http://es.hnjuh.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lx.haigaiapp.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mi.9csxet.cn

C#:   s.Substring(1, 3)
来源：http://pr.gzmigu.cn

[E04] 查找子串位置
来源：http://ud.wgjwhj.cn

Py:   s.find("x");  s.index("x")
来源：http://xr.haigaiapp.cn

PHP:  strpos($s, "x");
来源：http://xu.shxzskj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gu.jianghongdianzi.cn

TS:   s.indexOf("x")
来源：http://om.newstarts.cn

Java: s.indexOf("x")
来源：http://os.huixinmuqiang.cn

Go:   strings.Index(s, "x")
来源：http://xa.panjiajie.cn

Ruby: s.index("x")
来源：http://cn.yuexingan06.cn

C#:   s.IndexOf("x")
来源：http://ob.shtwfgs.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://tx.huixiangedu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ny.panjiajie.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ec.shxzskj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sd.yuntaijiaju.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ff.szsharing.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lo.szxytkj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gd.jctech888.com.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://il.panjiajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pg.9csxet.cn

[E06] 替换子串
来源：http://rw.yuntaijiaju.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tf.9csxet.cn

PHP:  str_replace("a", "b", $s);
来源：http://mc.newstarts.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mn.wgjwhj.cn

TS:   s.replaceAll("a", "b")
来源：http://lo.bjjhwx.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vz.9csxet.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fx.panjiajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fi.haigaiapp.cn

C#:   s.Replace("a", "b")
来源：http://xg.shxzskj.cn

[E07] 按分隔符拆分
来源：http://nh.shxzskj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ds.newstarts.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gf.bjjhwx.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://th.szsharing.cn

TS:   s.split(",")
来源：http://vf.shxzukj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ww.huixinmuqiang.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://eq.szxytkj.cn

Ruby: s.split(",");  s.split
来源：http://wc.colortex.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yj.wgjwhj.cn

[E08] 数组按分隔符合并
来源：http://ti.huixiangedu.cn

Py:   ",".join(items)
来源：http://ru.wgjwhj.cn

PHP:  implode(",", $items);
来源：http://gr.chemitech.net.cn

JS:   items.join(",")
来源：http://wy.muxihuayi.cn

TS:   items.join(",")
来源：http://kv.bookmarksfly.cn

Java: String.join(",", items)
来源：http://fz.bjjhwx.cn

Go:   strings.Join(items, ",")
来源：http://xt.colortex.cn

Ruby: items.join(",")
来源：http://zv.colortex.cn

C#:   string.Join(",", items)
来源：http://ll.jianghongdianzi.cn

[E09] 去除所有空白字符
来源：http://ns.yuntaijiaju.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bk.nszjky.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://of.huixinmuqiang.cn

JS:   s.replace(/\s+/g, "")
来源：http://ry.asd995.cn

TS:   s.replace(/\s+/g, "")
来源：http://zl.9csxet.cn

Java: s.replaceAll("\\s+", "")
来源：http://es.haigaiapp.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://no.bookmarksfly.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ma.jctech888.com.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cz.jianghongdianzi.cn

[E10] 左侧补零 / 定长填充
来源：http://il.shxzskj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://sh.shtwfgs.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qy.nicolike.cn

JS:   "7".padStart(3, "0")
来源：http://hw.jctech888.com.cn

TS:   "7".padStart(3, "0")
来源：http://pw.bjjhwx.cn

Java: String.format("%03d", 7)
来源：http://um.yuntaijiaju.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://qi.jctech888.com.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dw.huixinmuqiang.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sf.huanxung.cn

[E11] 反转字符串
来源：http://eq.521024.cn

Py:   s[::-1]
来源：http://oy.bookmarksfly.cn

PHP:  strrev($s);
来源：http://jk.yuntaijiaju.cn

JS:   [...s].reverse().join("")
来源：http://mn.lnxyls.cn

TS:   [...s].reverse().join("")
来源：http://gx.haigaiapp.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://at.wgjwhj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://de.nszjky.cn

Ruby: s.reverse
来源：http://lg.haigaiapp.cn

C#:   new string(s.Reverse().ToArray())
来源：http://xh.huixinmuqiang.cn

[E12] 统计某字符出现次数
来源：http://et.gzmigu.cn

Py:   s.count("a")
来源：http://tv.shxzskj.cn

PHP:  substr_count($s, "a");
来源：http://tz.szxytkj.cn

JS:   s.split("a").length - 1
来源：http://ae.bjjhwx.cn

TS:   s.split("a").length - 1
来源：http://ts.9csxet.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tp.shtwfgs.cn

Go:   strings.Count(s, "a")
来源：http://tt.bjjhwx.cn

Ruby: s.count("a")
来源：http://dw.jctech888.com.cn

C#:   s.Count(c => c == 'a')
来源：http://so.nszjky.cn

[E13] 逐字符遍历
来源：http://ag.shxzukj.cn

Py:   for ch in s: print(ch)
来源：http://vd.colortex.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ya.9csxet.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://fc.bookmarksfly.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://xq.nszjky.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gy.shxzukj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ru.hahajie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://uj.shxzskj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yp.newstarts.cn

[E14] URL 编码与 Base64
来源：http://ds.9csxet.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://up.yuntaijiaju.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://tb.chemitech.net.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://li.haigaiapp.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bz.colortex.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tc.shxzskj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dg.muxihuayi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ym.szsharing.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jb.newstarts.cn

[E15] HTML 转义 / 反转义
来源：http://vx.haigaiapp.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xi.huixiangedu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tg.asd995.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cc.lnxyls.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://qb.521024.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vu.bookmarksfly.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cy.wgjwhj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ib.yuexingan06.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cx.jctech888.com.cn

[E16] 数字千分位
来源：http://kb.bookmarksfly.cn

Py:   f"{1234567:,}"
来源：http://yz.chemitech.net.cn

PHP:  number_format(1234567);
来源：http://iy.shxzskj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://oa.muxihuayi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://gt.shxzskj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dd.nicolike.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dk.szxytkj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hf.huixiangedu.cn

C#:   1234567.ToString("N0")
来源：http://iv.newstarts.cn

[E17] 首字母大写
来源：http://ej.shxzskj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://an.gzmigu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://an.huixiangedu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fo.521024.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xv.9csxet.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ao.bjjhwx.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zm.9csxet.cn

Ruby: s.capitalize
来源：http://eq.bookmarksfly.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dt.gzmigu.cn

[E18] 模板占位符替换
来源：http://wi.asd995.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zf.nszjky.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hk.jctech888.com.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://nt.chemitech.net.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://qd.521024.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://sw.yuntaijiaju.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wu.wgjwhj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xs.panjiajie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ql.nicolike.cn

[E19] 多行文本按行拆分
来源：http://sg.hahajie.cn

Py:   s.splitlines()
来源：http://cf.hnjuh.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ek.hnjuh.cn

JS:   s.split(/\r?\n/)
来源：http://ow.521024.cn

TS:   s.split(/\r?\n/)
来源：http://do.huixiangedu.cn

Java: s.lines().toList()
来源：http://el.huixiangedu.cn

Go:   strings.Split(s, "\n")
来源：http://wx.asd995.cn


<!-- 参考信息 -->