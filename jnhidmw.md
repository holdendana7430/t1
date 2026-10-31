代发 wailian999

Ruby: arr.index(x)
来源：http://ni.lnxyls.cn

C#:   list.IndexOf(x);
来源：http://em.shtwfgs.cn

[D13] 过滤（保留满足条件的）
来源：http://ry.huixiangedu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ys.jctech888.com.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jj.521024.cn

JS:   arr.filter(x => x > 3)
来源：http://fm.jctech888.com.cn

TS:   arr.filter(x => x > 3)
来源：http://ii.shtwfgs.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ht.muxihuayi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ca.huanxung.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fq.nicolike.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://og.shxzskj.cn

[D14] 映射转换（每个元素变形）
来源：http://ql.huixiangedu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rn.panjiajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tr.gzmigu.cn

JS:   arr.map(x => x * 2)
来源：http://pn.newstarts.cn

TS:   arr.map(x => x * 2)
来源：http://pr.huixiangedu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://at.bookmarksfly.cn

Go:   // 手写循环
来源：http://ia.yuexingan06.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qr.nicolike.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://bd.yuexingan06.cn

[D15] 去重
来源：http://ty.nicolike.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fp.bookmarksfly.cn

PHP:  array_unique($arr);
来源：http://jq.haigaiapp.cn

JS:   [...new Set(arr)]
来源：http://ru.newstarts.cn

TS:   [...new Set(arr)]
来源：http://ba.bookmarksfly.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cu.jctech888.com.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zl.newstarts.cn

Ruby: arr.uniq
来源：http://ji.521024.cn

C#:   list.Distinct().ToList()
来源：http://hz.colortex.cn

[D16] 求和与平均值
来源：http://sf.shtwfgs.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wz.yuexingan06.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dg.shxzukj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jy.lnxyls.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ri.hahajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vw.jctech888.com.cn

Go:   // 手写循环累加
来源：http://sm.newstarts.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mu.chemitech.net.cn

C#:   list.Sum();  list.Average()
来源：http://ri.jianghongdianzi.cn

[D17] 最大值与最小值
来源：http://cy.szxytkj.cn

Py:   max(arr);  min(arr)
来源：http://ge.hahajie.cn

PHP:  max($arr);  min($arr);
来源：http://ge.asd995.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xi.newstarts.cn

TS:   Math.max(...arr);
来源：http://sj.521024.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jn.wgjwhj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.bjjhwx.cn

Ruby: arr.max;  arr.min
来源：http://qr.shtwfgs.cn

C#:   list.Max();  list.Min()
来源：http://bl.asd995.cn

[D18] 扁平化嵌套数组
来源：http://ln.gzmigu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nm.szxytkj.cn

PHP:  array_merge(...$nested);
来源：http://xm.chemitech.net.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jx.wgjwhj.cn

TS:   nested.flat();
来源：http://ug.huixiangedu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gu.bookmarksfly.cn

Go:   // 手写双层循环
来源：http://dw.bookmarksfly.cn

Ruby: nested.flatten
来源：http://rx.nicolike.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://qr.newstarts.cn

[D19] 按字段分组
来源：http://zx.hnjuh.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fb.yuntaijiaju.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wc.panjiajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ia.yuntaijiaju.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://oc.newstarts.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yg.asd995.cn

Go:   // 手写 map[string][]T
来源：http://ib.jianghongdianzi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://zn.shxzskj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xs.colortex.cn

[D20] 统计每个元素出现次数
来源：http://yz.gzmigu.cn

Py:   Counter(arr)
来源：http://nf.haigaiapp.cn

PHP:  array_count_values($arr);
来源：http://rz.yuexingan06.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ws.hnjuh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ua.newstarts.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nn.nicolike.cn

Go:   // 手写 map[T]int
来源：http://qd.muxihuayi.cn

Ruby: arr.tally
来源：http://ub.yuexingan06.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mq.yuexingan06.cn

[D21] 判断是否包含某元素
来源：http://ko.panjiajie.cn

Py:   x in arr
来源：http://bn.nszjky.cn

PHP:  in_array($x, $arr, true);
来源：http://wn.bjjhwx.cn

JS:   arr.includes(x)
来源：http://va.nszjky.cn

TS:   arr.includes(x)
来源：http://sn.lnxyls.cn

Java: list.contains(x)
来源：http://nh.shtwfgs.cn

Go:   slices.Contains(arr, x)
来源：http://ad.wgjwhj.cn

Ruby: arr.include?(x)
来源：http://hf.jctech888.com.cn

C#:   list.Contains(x)
来源：http://su.hahajie.cn

[D22] 复制数组（避免共享引用）
来源：http://hy.nszjky.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rh.gzmigu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sg.bookmarksfly.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lu.yuntaijiaju.cn

TS:   [...arr];
来源：http://hr.nicolike.cn

Java: new ArrayList<>(list);
来源：http://hk.haigaiapp.cn

Go:   copied := append([]int(nil), arr...)
来源：http://pc.panjiajie.cn

Ruby: arr.dup;  arr.clone
来源：http://ke.huanxung.cn

C#:   new List<int>(list);
来源：http://gy.huixiangedu.cn

[D23] reduce 累积计算
来源：http://yv.haigaiapp.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cv.muxihuayi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nm.chemitech.net.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ow.szxytkj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kv.yuntaijiaju.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://id.colortex.cn

Go:   // 手写循环
来源：http://il.shxzukj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ro.bookmarksfly.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xt.bookmarksfly.cn

[D24] 字典 / Map 基本操作
来源：http://op.huanxung.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vr.bjjhwx.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sa.huanxung.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bz.bjjhwx.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cc.wgjwhj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fa.yuexingan06.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ai.jctech888.com.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jz.nszjky.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://da.yuexingan06.cn

[D25] Set 集合去重与交并差
来源：http://im.jctech888.com.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dk.szxytkj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sm.gzmigu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qx.bookmarksfly.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hn.huixiangedu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://td.haigaiapp.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://et.panjiajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qh.shxzskj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lz.lnxyls.cn

[D26] 数组转字符串
来源：http://ik.colortex.cn

Py:   ", ".join(map(str, arr))
来源：http://gk.huanxung.cn

PHP:  implode(", ", $arr);
来源：http://ir.huixinmuqiang.cn

JS:   arr.join(", ")
来源：http://gm.wgjwhj.cn

TS:   arr.join(", ")
来源：http://tl.huixiangedu.cn

Java: String.join(", ", list)
来源：http://jo.521024.cn

Go:   strings.Join(strs, ", ")
来源：http://ip.lnxyls.cn

Ruby: arr.join(", ")
来源：http://za.bjjhwx.cn

C#:   string.Join(", ", list)
来源：http://wl.huanxung.cn

================================================================================
来源：http://vl.521024.cn

E. 字符串处理
来源：http://hr.bookmarksfly.cn

================================================================================
来源：http://zh.shtwfgs.cn

[E01] 拼接字符串
来源：http://bl.nicolike.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bm.colortex.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rt.huixinmuqiang.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://sh.shxzukj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://om.haigaiapp.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hf.huixinmuqiang.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dy.nszjky.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ik.bookmarksfly.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sk.hnjuh.cn

[E02] 重复字符串
来源：http://my.521024.cn

Py:   "ab" * 3
来源：http://wa.asd995.cn

PHP:  str_repeat("ab", 3);
来源：http://rf.bookmarksfly.cn

JS:   "ab".repeat(3)
来源：http://ay.szxytkj.cn

TS:   "ab".repeat(3)
来源：http://kq.colortex.cn

Java: "ab".repeat(3)
来源：http://af.shxzukj.cn

Go:   strings.Repeat("ab", 3)
来源：http://fa.521024.cn

Ruby: "ab" * 3
来源：http://rl.shtwfgs.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ja.bjjhwx.cn

[E03] 截取子串
来源：http://kn.muxihuayi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vs.colortex.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xb.jctech888.com.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://iq.shxzskj.cn

TS:   s.slice(1, 4)
来源：http://no.9csxet.cn

Java: s.substring(1, 4)
来源：http://wd.huixinmuqiang.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://oc.shxzskj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://lf.asd995.cn

C#:   s.Substring(1, 3)
来源：http://ms.huixinmuqiang.cn

[E04] 查找子串位置
来源：http://ti.bjjhwx.cn

Py:   s.find("x");  s.index("x")
来源：http://do.jianghongdianzi.cn

PHP:  strpos($s, "x");
来源：http://nm.wgjwhj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ka.huixiangedu.cn

TS:   s.indexOf("x")
来源：http://fb.gzmigu.cn

Java: s.indexOf("x")
来源：http://dd.muxihuayi.cn

Go:   strings.Index(s, "x")
来源：http://az.yuexingan06.cn

Ruby: s.index("x")
来源：http://pb.muxihuayi.cn

C#:   s.IndexOf("x")
来源：http://vp.9csxet.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://eu.9csxet.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ho.szsharing.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ac.jianghongdianzi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vy.asd995.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://th.huixinmuqiang.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ik.gzmigu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ti.huanxung.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zz.colortex.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ug.huixiangedu.cn

[E06] 替换子串
来源：http://bj.bookmarksfly.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://im.huixinmuqiang.cn

PHP:  str_replace("a", "b", $s);
来源：http://sc.huixiangedu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rf.yuntaijiaju.cn

TS:   s.replaceAll("a", "b")
来源：http://gk.521024.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://li.jctech888.com.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xr.chemitech.net.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rd.521024.cn

C#:   s.Replace("a", "b")
来源：http://ut.muxihuayi.cn

[E07] 按分隔符拆分
来源：http://nw.yuntaijiaju.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ok.nszjky.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fz.haigaiapp.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://er.huixiangedu.cn

TS:   s.split(",")
来源：http://tz.9csxet.cn

Java: s.split(",");  s.split("\\s+")
来源：http://go.bookmarksfly.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jo.bookmarksfly.cn

Ruby: s.split(",");  s.split
来源：http://qy.szsharing.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://al.hnjuh.cn

[E08] 数组按分隔符合并
来源：http://oe.9csxet.cn

Py:   ",".join(items)
来源：http://hc.huixiangedu.cn

PHP:  implode(",", $items);
来源：http://ds.wgjwhj.cn

JS:   items.join(",")
来源：http://dz.shxzukj.cn

TS:   items.join(",")
来源：http://lg.szsharing.cn

Java: String.join(",", items)
来源：http://ue.yuexingan06.cn

Go:   strings.Join(items, ",")
来源：http://kb.asd995.cn

Ruby: items.join(",")
来源：http://rz.521024.cn

C#:   string.Join(",", items)
来源：http://ac.yuexingan06.cn

[E09] 去除所有空白字符
来源：http://wz.wgjwhj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mn.szxytkj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gl.shxzskj.cn

JS:   s.replace(/\s+/g, "")
来源：http://lu.nszjky.cn

TS:   s.replace(/\s+/g, "")
来源：http://qy.chemitech.net.cn

Java: s.replaceAll("\\s+", "")
来源：http://gs.panjiajie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://xg.haigaiapp.cn

Ruby: s.gsub(/\s+/, "")
来源：http://wt.nszjky.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xx.shxzskj.cn

[E10] 左侧补零 / 定长填充
来源：http://yz.panjiajie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ow.hnjuh.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ql.jianghongdianzi.cn

JS:   "7".padStart(3, "0")
来源：http://gq.huixiangedu.cn

TS:   "7".padStart(3, "0")
来源：http://mf.hahajie.cn

Java: String.format("%03d", 7)
来源：http://ng.huixinmuqiang.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://js.huixinmuqiang.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sa.shxzskj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rj.nicolike.cn

[E11] 反转字符串
来源：http://gy.huanxung.cn

Py:   s[::-1]
来源：http://eg.colortex.cn

PHP:  strrev($s);
来源：http://qz.yuexingan06.cn

JS:   [...s].reverse().join("")
来源：http://hj.bjjhwx.cn

TS:   [...s].reverse().join("")
来源：http://yr.9csxet.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://yi.newstarts.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://gs.gzmigu.cn

Ruby: s.reverse
来源：http://zz.nicolike.cn

C#:   new string(s.Reverse().ToArray())
来源：http://pc.huixiangedu.cn

[E12] 统计某字符出现次数
来源：http://dq.huanxung.cn

Py:   s.count("a")
来源：http://kf.shtwfgs.cn

PHP:  substr_count($s, "a");
来源：http://wi.521024.cn

JS:   s.split("a").length - 1
来源：http://ud.asd995.cn

TS:   s.split("a").length - 1
来源：http://dq.9csxet.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xk.newstarts.cn

Go:   strings.Count(s, "a")
来源：http://yg.shxzskj.cn

Ruby: s.count("a")
来源：http://ck.521024.cn

C#:   s.Count(c => c == 'a')
来源：http://oq.bookmarksfly.cn

[E13] 逐字符遍历
来源：http://yr.shxzskj.cn

Py:   for ch in s: print(ch)
来源：http://lh.hnjuh.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cp.muxihuayi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://he.521024.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://vb.bjjhwx.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tc.huixinmuqiang.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://uz.shxzskj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ym.nicolike.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dh.wgjwhj.cn

[E14] URL 编码与 Base64
来源：http://sp.huanxung.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fz.panjiajie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://iz.hnjuh.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ot.yuntaijiaju.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://py.szsharing.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uv.panjiajie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pz.hnjuh.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ls.chemitech.net.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hp.521024.cn

[E15] HTML 转义 / 反转义
来源：http://lq.wgjwhj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://iv.bookmarksfly.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ft.lnxyls.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tc.huixiangedu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://jt.bjjhwx.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fj.hnjuh.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cr.nicolike.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bx.lnxyls.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://op.huixiangedu.cn

[E16] 数字千分位
来源：http://xi.hnjuh.cn

Py:   f"{1234567:,}"
来源：http://sn.newstarts.cn

PHP:  number_format(1234567);
来源：http://zr.huixinmuqiang.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://nu.newstarts.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wz.newstarts.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ug.lnxyls.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://uj.yuexingan06.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://at.muxihuayi.cn

C#:   1234567.ToString("N0")
来源：http://bl.shxzukj.cn

[E17] 首字母大写
来源：http://bk.muxihuayi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vq.shxzukj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://mp.huanxung.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cq.shxzskj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hx.nszjky.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vf.huixinmuqiang.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kz.bookmarksfly.cn

Ruby: s.capitalize
来源：http://uo.shtwfgs.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nw.jianghongdianzi.cn

[E18] 模板占位符替换
来源：http://la.hnjuh.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://oq.nszjky.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ug.gzmigu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://gy.hahajie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://br.lnxyls.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://au.szxytkj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wq.szsharing.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bt.huixinmuqiang.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gq.lnxyls.cn

[E19] 多行文本按行拆分
来源：http://ra.bjjhwx.cn

Py:   s.splitlines()
来源：http://da.521024.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kt.jianghongdianzi.cn

JS:   s.split(/\r?\n/)
来源：http://xv.asd995.cn

TS:   s.split(/\r?\n/)
来源：http://xs.521024.cn

Java: s.lines().toList()
来源：http://vs.yuntaijiaju.cn

Go:   strings.Split(s, "\n")
来源：http://sf.lnxyls.cn


<!-- 参考信息 -->