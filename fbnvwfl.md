代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://uf.haigaiapp.cn

Ruby: arr.select { |x| x > 3 }
来源：http://og.muxihuayi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://yy.panjiajie.cn

[D14] 映射转换（每个元素变形）
来源：http://bd.shxzukj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mj.haigaiapp.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gl.yuexingan06.cn

JS:   arr.map(x => x * 2)
来源：http://iu.bookmarksfly.cn

TS:   arr.map(x => x * 2)
来源：http://cr.bookmarksfly.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ds.wgjwhj.cn

Go:   // 手写循环
来源：http://gp.jctech888.com.cn

Ruby: arr.map { |x| x * 2 }
来源：http://bw.hnjuh.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ak.szsharing.cn

[D15] 去重
来源：http://vl.wgjwhj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qk.shxzskj.cn

PHP:  array_unique($arr);
来源：http://it.huixiangedu.cn

JS:   [...new Set(arr)]
来源：http://rt.bjjhwx.cn

TS:   [...new Set(arr)]
来源：http://fd.szxytkj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bo.jianghongdianzi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://nz.yuntaijiaju.cn

Ruby: arr.uniq
来源：http://qa.chemitech.net.cn

C#:   list.Distinct().ToList()
来源：http://mz.chemitech.net.cn

[D16] 求和与平均值
来源：http://jt.shtwfgs.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zm.bookmarksfly.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xb.nszjky.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vo.huixinmuqiang.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mj.gzmigu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gh.hahajie.cn

Go:   // 手写循环累加
来源：http://wt.jianghongdianzi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mm.521024.cn

C#:   list.Sum();  list.Average()
来源：http://mg.haigaiapp.cn

[D17] 最大值与最小值
来源：http://nr.nszjky.cn

Py:   max(arr);  min(arr)
来源：http://ou.huanxung.cn

PHP:  max($arr);  min($arr);
来源：http://so.asd995.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dn.jianghongdianzi.cn

TS:   Math.max(...arr);
来源：http://yf.yuexingan06.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://fr.chemitech.net.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mu.bookmarksfly.cn

Ruby: arr.max;  arr.min
来源：http://jb.haigaiapp.cn

C#:   list.Max();  list.Min()
来源：http://ng.521024.cn

[D18] 扁平化嵌套数组
来源：http://xo.haigaiapp.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nv.shxzskj.cn

PHP:  array_merge(...$nested);
来源：http://qh.yuexingan06.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mn.gzmigu.cn

TS:   nested.flat();
来源：http://tr.gzmigu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://my.jctech888.com.cn

Go:   // 手写双层循环
来源：http://jf.lnxyls.cn

Ruby: nested.flatten
来源：http://zf.jianghongdianzi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://fn.shtwfgs.cn

[D19] 按字段分组
来源：http://uo.nszjky.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bc.521024.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mp.huixiangedu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://et.asd995.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://zq.yuntaijiaju.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hj.shxzukj.cn

Go:   // 手写 map[string][]T
来源：http://ky.newstarts.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ub.gzmigu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lx.szxytkj.cn

[D20] 统计每个元素出现次数
来源：http://dt.asd995.cn

Py:   Counter(arr)
来源：http://ti.asd995.cn

PHP:  array_count_values($arr);
来源：http://ft.gzmigu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://aq.yuntaijiaju.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bm.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zl.huanxung.cn

Go:   // 手写 map[T]int
来源：http://qz.nszjky.cn

Ruby: arr.tally
来源：http://op.yuexingan06.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bh.hahajie.cn

[D21] 判断是否包含某元素
来源：http://cy.szsharing.cn

Py:   x in arr
来源：http://ua.huixinmuqiang.cn

PHP:  in_array($x, $arr, true);
来源：http://uv.huanxung.cn

JS:   arr.includes(x)
来源：http://ag.jianghongdianzi.cn

TS:   arr.includes(x)
来源：http://yz.huanxung.cn

Java: list.contains(x)
来源：http://kq.szxytkj.cn

Go:   slices.Contains(arr, x)
来源：http://mb.szsharing.cn

Ruby: arr.include?(x)
来源：http://nv.hnjuh.cn

C#:   list.Contains(x)
来源：http://zb.szxytkj.cn

[D22] 复制数组（避免共享引用）
来源：http://pa.huanxung.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://su.haigaiapp.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://no.nszjky.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qe.chemitech.net.cn

TS:   [...arr];
来源：http://fe.nszjky.cn

Java: new ArrayList<>(list);
来源：http://mt.haigaiapp.cn

Go:   copied := append([]int(nil), arr...)
来源：http://gn.bookmarksfly.cn

Ruby: arr.dup;  arr.clone
来源：http://pm.lnxyls.cn

C#:   new List<int>(list);
来源：http://fp.newstarts.cn

[D23] reduce 累积计算
来源：http://jg.shtwfgs.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nc.jctech888.com.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yt.huixinmuqiang.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eq.521024.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uz.gzmigu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ut.colortex.cn

Go:   // 手写循环
来源：http://ey.huanxung.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vr.panjiajie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wp.colortex.cn

[D24] 字典 / Map 基本操作
来源：http://pd.yuexingan06.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yu.nicolike.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qw.asd995.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hd.huixinmuqiang.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://we.yuntaijiaju.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://io.hahajie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ka.hahajie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ln.yuntaijiaju.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yp.wgjwhj.cn

[D25] Set 集合去重与交并差
来源：http://ff.huanxung.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ho.szxytkj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ev.yuntaijiaju.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gl.nszjky.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ep.colortex.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cy.szxytkj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nc.huanxung.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vp.yuexingan06.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pt.9csxet.cn

[D26] 数组转字符串
来源：http://ip.bookmarksfly.cn

Py:   ", ".join(map(str, arr))
来源：http://zm.521024.cn

PHP:  implode(", ", $arr);
来源：http://ix.bjjhwx.cn

JS:   arr.join(", ")
来源：http://am.newstarts.cn

TS:   arr.join(", ")
来源：http://hc.lnxyls.cn

Java: String.join(", ", list)
来源：http://by.bjjhwx.cn

Go:   strings.Join(strs, ", ")
来源：http://gk.huixinmuqiang.cn

Ruby: arr.join(", ")
来源：http://nk.muxihuayi.cn

C#:   string.Join(", ", list)
来源：http://iw.9csxet.cn

================================================================================
来源：http://um.huixiangedu.cn

E. 字符串处理
来源：http://xs.szxytkj.cn

================================================================================
来源：http://rf.521024.cn

[E01] 拼接字符串
来源：http://gh.yuexingan06.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kn.hnjuh.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://te.haigaiapp.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://om.bookmarksfly.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bl.bookmarksfly.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://id.szsharing.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://md.bjjhwx.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://la.hnjuh.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cu.panjiajie.cn

[E02] 重复字符串
来源：http://xm.nicolike.cn

Py:   "ab" * 3
来源：http://az.muxihuayi.cn

PHP:  str_repeat("ab", 3);
来源：http://aq.hahajie.cn

JS:   "ab".repeat(3)
来源：http://vk.yuexingan06.cn

TS:   "ab".repeat(3)
来源：http://pu.bjjhwx.cn

Java: "ab".repeat(3)
来源：http://uu.nszjky.cn

Go:   strings.Repeat("ab", 3)
来源：http://re.bjjhwx.cn

Ruby: "ab" * 3
来源：http://rp.huixiangedu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://si.lnxyls.cn

[E03] 截取子串
来源：http://cg.bookmarksfly.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wd.szsharing.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xg.lnxyls.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ma.9csxet.cn

TS:   s.slice(1, 4)
来源：http://pg.hahajie.cn

Java: s.substring(1, 4)
来源：http://fm.szsharing.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://di.wgjwhj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ll.jianghongdianzi.cn

C#:   s.Substring(1, 3)
来源：http://pl.wgjwhj.cn

[E04] 查找子串位置
来源：http://oe.yuexingan06.cn

Py:   s.find("x");  s.index("x")
来源：http://bm.huanxung.cn

PHP:  strpos($s, "x");
来源：http://rm.bookmarksfly.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tr.521024.cn

TS:   s.indexOf("x")
来源：http://vh.bjjhwx.cn

Java: s.indexOf("x")
来源：http://gr.haigaiapp.cn

Go:   strings.Index(s, "x")
来源：http://lm.gzmigu.cn

Ruby: s.index("x")
来源：http://ht.wgjwhj.cn

C#:   s.IndexOf("x")
来源：http://jb.huixiangedu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gc.huixiangedu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uj.yuexingan06.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xv.muxihuayi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zl.newstarts.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://nb.huanxung.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lh.bjjhwx.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://iw.jctech888.com.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cl.hnjuh.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sw.yuexingan06.cn

[E06] 替换子串
来源：http://am.huixiangedu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://oo.huanxung.cn

PHP:  str_replace("a", "b", $s);
来源：http://oy.nszjky.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://st.asd995.cn

TS:   s.replaceAll("a", "b")
来源：http://ki.yuexingan06.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://aq.szxytkj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ud.muxihuayi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lh.wgjwhj.cn

C#:   s.Replace("a", "b")
来源：http://we.wgjwhj.cn

[E07] 按分隔符拆分
来源：http://qc.haigaiapp.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ca.hnjuh.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pc.gzmigu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://tm.nicolike.cn

TS:   s.split(",")
来源：http://uq.haigaiapp.cn

Java: s.split(",");  s.split("\\s+")
来源：http://cp.huixiangedu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://aa.muxihuayi.cn

Ruby: s.split(",");  s.split
来源：http://jz.shtwfgs.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://td.lnxyls.cn

[E08] 数组按分隔符合并
来源：http://ij.newstarts.cn

Py:   ",".join(items)
来源：http://wi.muxihuayi.cn

PHP:  implode(",", $items);
来源：http://yt.521024.cn

JS:   items.join(",")
来源：http://qo.panjiajie.cn

TS:   items.join(",")
来源：http://ft.panjiajie.cn

Java: String.join(",", items)
来源：http://ww.hahajie.cn

Go:   strings.Join(items, ",")
来源：http://kn.muxihuayi.cn

Ruby: items.join(",")
来源：http://ma.haigaiapp.cn

C#:   string.Join(",", items)
来源：http://ig.shxzskj.cn

[E09] 去除所有空白字符
来源：http://cg.asd995.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ai.shxzskj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zz.9csxet.cn

JS:   s.replace(/\s+/g, "")
来源：http://mu.muxihuayi.cn

TS:   s.replace(/\s+/g, "")
来源：http://oe.9csxet.cn

Java: s.replaceAll("\\s+", "")
来源：http://qx.szxytkj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://oz.asd995.cn

Ruby: s.gsub(/\s+/, "")
来源：http://lt.asd995.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tj.yuexingan06.cn

[E10] 左侧补零 / 定长填充
来源：http://cn.yuntaijiaju.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tg.yuexingan06.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mu.huanxung.cn

JS:   "7".padStart(3, "0")
来源：http://dw.asd995.cn

TS:   "7".padStart(3, "0")
来源：http://md.hahajie.cn

Java: String.format("%03d", 7)
来源：http://fv.gzmigu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ac.wgjwhj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zh.yuexingan06.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ud.muxihuayi.cn

[E11] 反转字符串
来源：http://ja.colortex.cn

Py:   s[::-1]
来源：http://vq.huanxung.cn

PHP:  strrev($s);
来源：http://zb.szxytkj.cn

JS:   [...s].reverse().join("")
来源：http://vt.colortex.cn

TS:   [...s].reverse().join("")
来源：http://bs.yuntaijiaju.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ec.jctech888.com.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://gs.jctech888.com.cn

Ruby: s.reverse
来源：http://bj.huixinmuqiang.cn

C#:   new string(s.Reverse().ToArray())
来源：http://su.muxihuayi.cn

[E12] 统计某字符出现次数
来源：http://ee.szsharing.cn

Py:   s.count("a")
来源：http://zf.bjjhwx.cn

PHP:  substr_count($s, "a");
来源：http://sf.nszjky.cn

JS:   s.split("a").length - 1
来源：http://tu.colortex.cn

TS:   s.split("a").length - 1
来源：http://yr.panjiajie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gz.shxzskj.cn

Go:   strings.Count(s, "a")
来源：http://vm.gzmigu.cn

Ruby: s.count("a")
来源：http://dl.jianghongdianzi.cn

C#:   s.Count(c => c == 'a')
来源：http://jv.521024.cn

[E13] 逐字符遍历
来源：http://is.huixiangedu.cn

Py:   for ch in s: print(ch)
来源：http://lg.yuntaijiaju.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zt.hahajie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://hm.szxytkj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://id.gzmigu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://eb.nszjky.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wx.9csxet.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://wl.nicolike.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://aq.huanxung.cn

[E14] URL 编码与 Base64
来源：http://ac.yuntaijiaju.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ee.chemitech.net.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://tm.jianghongdianzi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lq.gzmigu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://su.shtwfgs.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cd.huanxung.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zy.jianghongdianzi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jn.hnjuh.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rb.hnjuh.cn

[E15] HTML 转义 / 反转义
来源：http://zn.521024.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ak.szsharing.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yp.shxzskj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jq.huixinmuqiang.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://qb.nszjky.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mz.bjjhwx.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gt.nszjky.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xa.shtwfgs.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jm.haigaiapp.cn

[E16] 数字千分位
来源：http://cw.panjiajie.cn

Py:   f"{1234567:,}"
来源：http://tl.nicolike.cn

PHP:  number_format(1234567);
来源：http://bp.9csxet.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://og.yuexingan06.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://fm.shtwfgs.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ey.huixinmuqiang.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jo.nszjky.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ma.shtwfgs.cn

C#:   1234567.ToString("N0")
来源：http://kf.jctech888.com.cn

[E17] 首字母大写
来源：http://cy.nszjky.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ic.nszjky.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://yw.szsharing.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rb.lnxyls.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ue.wgjwhj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gb.nicolike.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tf.haigaiapp.cn

Ruby: s.capitalize
来源：http://mn.bookmarksfly.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://va.huanxung.cn

[E18] 模板占位符替换
来源：http://kr.huixinmuqiang.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ql.9csxet.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rt.nszjky.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://eh.panjiajie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://bh.bjjhwx.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://iu.huanxung.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dq.shtwfgs.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mp.muxihuayi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qy.hahajie.cn

[E19] 多行文本按行拆分
来源：http://zb.panjiajie.cn

Py:   s.splitlines()
来源：http://ra.gzmigu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kj.jianghongdianzi.cn

JS:   s.split(/\r?\n/)
来源：http://fz.bjjhwx.cn

TS:   s.split(/\r?\n/)
来源：http://fb.yuntaijiaju.cn

Java: s.lines().toList()
来源：http://dw.colortex.cn

Go:   strings.Split(s, "\n")
来源：http://rb.521024.cn

Ruby: s.lines
来源：http://fo.haigaiapp.cn

C#:   s.Split('\n')
来源：http://zv.hahajie.cn

[E20] 判断字符串是否为空
来源：http://uf.shxzskj.cn

Py:   if not s:
来源：http://vg.jctech888.com.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ku.chemitech.net.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vp.colortex.cn

TS:   if (s === "") {}
来源：http://aa.nszjky.cn

Java: if (s.isEmpty()) {}
来源：http://tu.gzmigu.cn


<!-- 参考信息 -->