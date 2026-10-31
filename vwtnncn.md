代发 wailian999

[D19] 按字段分组
来源：http://ld.panjiajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://et.yuexingan06.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bp.9csxet.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ky.yuntaijiaju.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://yr.nicolike.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ba.hnjuh.cn

Go:   // 手写 map[string][]T
来源：http://zh.shtwfgs.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ei.hnjuh.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lm.wgjwhj.cn

[D20] 统计每个元素出现次数
来源：http://ti.hnjuh.cn

Py:   Counter(arr)
来源：http://be.bjjhwx.cn

PHP:  array_count_values($arr);
来源：http://yz.huixinmuqiang.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xs.9csxet.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xj.gzmigu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ji.bjjhwx.cn

Go:   // 手写 map[T]int
来源：http://jy.jctech888.com.cn

Ruby: arr.tally
来源：http://kz.asd995.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tj.huanxung.cn

[D21] 判断是否包含某元素
来源：http://pr.huixinmuqiang.cn

Py:   x in arr
来源：http://fk.asd995.cn

PHP:  in_array($x, $arr, true);
来源：http://ng.szxytkj.cn

JS:   arr.includes(x)
来源：http://jk.shtwfgs.cn

TS:   arr.includes(x)
来源：http://ql.9csxet.cn

Java: list.contains(x)
来源：http://wi.bookmarksfly.cn

Go:   slices.Contains(arr, x)
来源：http://hc.newstarts.cn

Ruby: arr.include?(x)
来源：http://wy.newstarts.cn

C#:   list.Contains(x)
来源：http://do.yuntaijiaju.cn

[D22] 复制数组（避免共享引用）
来源：http://vk.9csxet.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://io.gzmigu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://es.muxihuayi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ka.newstarts.cn

TS:   [...arr];
来源：http://yd.newstarts.cn

Java: new ArrayList<>(list);
来源：http://or.hahajie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://dj.9csxet.cn

Ruby: arr.dup;  arr.clone
来源：http://xq.bookmarksfly.cn

C#:   new List<int>(list);
来源：http://dy.bjjhwx.cn

[D23] reduce 累积计算
来源：http://ur.huixinmuqiang.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lf.huixinmuqiang.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://sj.hnjuh.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yv.asd995.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gu.hnjuh.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://jv.newstarts.cn

Go:   // 手写循环
来源：http://kp.bjjhwx.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tc.jctech888.com.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gn.hnjuh.cn

[D24] 字典 / Map 基本操作
来源：http://es.lnxyls.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ev.colortex.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dz.huanxung.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://me.panjiajie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://iq.nszjky.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fz.wgjwhj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ip.shtwfgs.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xk.haigaiapp.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hm.yuexingan06.cn

[D25] Set 集合去重与交并差
来源：http://av.huanxung.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xz.bjjhwx.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kv.panjiajie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hm.9csxet.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ir.huixiangedu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dx.yuexingan06.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ho.wgjwhj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cj.szsharing.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qh.yuntaijiaju.cn

[D26] 数组转字符串
来源：http://yu.chemitech.net.cn

Py:   ", ".join(map(str, arr))
来源：http://lk.muxihuayi.cn

PHP:  implode(", ", $arr);
来源：http://pf.panjiajie.cn

JS:   arr.join(", ")
来源：http://so.gzmigu.cn

TS:   arr.join(", ")
来源：http://vh.yuexingan06.cn

Java: String.join(", ", list)
来源：http://ee.huixinmuqiang.cn

Go:   strings.Join(strs, ", ")
来源：http://kf.haigaiapp.cn

Ruby: arr.join(", ")
来源：http://vl.colortex.cn

C#:   string.Join(", ", list)
来源：http://ng.muxihuayi.cn

================================================================================
来源：http://av.haigaiapp.cn

E. 字符串处理
来源：http://yi.521024.cn

================================================================================
来源：http://ya.nicolike.cn

[E01] 拼接字符串
来源：http://pc.huixinmuqiang.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://up.huixiangedu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://po.colortex.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mx.gzmigu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://iq.yuexingan06.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ob.lnxyls.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://il.hahajie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://to.bookmarksfly.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://du.colortex.cn

[E02] 重复字符串
来源：http://pz.colortex.cn

Py:   "ab" * 3
来源：http://ow.szsharing.cn

PHP:  str_repeat("ab", 3);
来源：http://um.hahajie.cn

JS:   "ab".repeat(3)
来源：http://uq.huixinmuqiang.cn

TS:   "ab".repeat(3)
来源：http://lu.panjiajie.cn

Java: "ab".repeat(3)
来源：http://zu.521024.cn

Go:   strings.Repeat("ab", 3)
来源：http://ad.colortex.cn

Ruby: "ab" * 3
来源：http://zc.huixiangedu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ry.shxzskj.cn

[E03] 截取子串
来源：http://bq.hahajie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qw.szxytkj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yc.asd995.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lt.hahajie.cn

TS:   s.slice(1, 4)
来源：http://cl.hnjuh.cn

Java: s.substring(1, 4)
来源：http://if.szsharing.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yd.9csxet.cn

Ruby: s[1, 3];  s[1..3]
来源：http://sj.haigaiapp.cn

C#:   s.Substring(1, 3)
来源：http://gl.szxytkj.cn

[E04] 查找子串位置
来源：http://js.haigaiapp.cn

Py:   s.find("x");  s.index("x")
来源：http://fw.szsharing.cn

PHP:  strpos($s, "x");
来源：http://ld.521024.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ry.huixiangedu.cn

TS:   s.indexOf("x")
来源：http://bg.panjiajie.cn

Java: s.indexOf("x")
来源：http://ja.bjjhwx.cn

Go:   strings.Index(s, "x")
来源：http://ir.jctech888.com.cn

Ruby: s.index("x")
来源：http://ud.newstarts.cn

C#:   s.IndexOf("x")
来源：http://hn.huixiangedu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://jf.bookmarksfly.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pb.szxytkj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hg.yuntaijiaju.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nx.asd995.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ci.gzmigu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gm.bookmarksfly.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ql.lnxyls.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://md.gzmigu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kr.yuexingan06.cn

[E06] 替换子串
来源：http://nr.yuexingan06.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ky.hahajie.cn

PHP:  str_replace("a", "b", $s);
来源：http://yz.asd995.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://na.lnxyls.cn

TS:   s.replaceAll("a", "b")
来源：http://uu.jianghongdianzi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uc.shxzskj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zh.szxytkj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ru.jctech888.com.cn

C#:   s.Replace("a", "b")
来源：http://gp.521024.cn

[E07] 按分隔符拆分
来源：http://za.nicolike.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jz.huixinmuqiang.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cc.chemitech.net.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://wk.lnxyls.cn

TS:   s.split(",")
来源：http://qz.yuexingan06.cn

Java: s.split(",");  s.split("\\s+")
来源：http://wx.bookmarksfly.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lt.hahajie.cn

Ruby: s.split(",");  s.split
来源：http://cj.huixinmuqiang.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mo.nicolike.cn

[E08] 数组按分隔符合并
来源：http://ep.nszjky.cn

Py:   ",".join(items)
来源：http://py.lnxyls.cn

PHP:  implode(",", $items);
来源：http://na.hahajie.cn

JS:   items.join(",")
来源：http://kq.bookmarksfly.cn

TS:   items.join(",")
来源：http://tr.shxzukj.cn

Java: String.join(",", items)
来源：http://xa.yuexingan06.cn

Go:   strings.Join(items, ",")
来源：http://db.asd995.cn

Ruby: items.join(",")
来源：http://jq.nicolike.cn

C#:   string.Join(",", items)
来源：http://vo.521024.cn

[E09] 去除所有空白字符
来源：http://sn.nszjky.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rq.nszjky.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tn.wgjwhj.cn

JS:   s.replace(/\s+/g, "")
来源：http://xa.colortex.cn

TS:   s.replace(/\s+/g, "")
来源：http://xa.shtwfgs.cn

Java: s.replaceAll("\\s+", "")
来源：http://ll.shxzukj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ro.shxzukj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://jk.szsharing.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mb.newstarts.cn

[E10] 左侧补零 / 定长填充
来源：http://fj.nszjky.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bf.shxzukj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://di.yuntaijiaju.cn

JS:   "7".padStart(3, "0")
来源：http://sc.jctech888.com.cn

TS:   "7".padStart(3, "0")
来源：http://ov.521024.cn

Java: String.format("%03d", 7)
来源：http://hq.jctech888.com.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://nd.hahajie.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wy.haigaiapp.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ri.szsharing.cn

[E11] 反转字符串
来源：http://kc.huanxung.cn

Py:   s[::-1]
来源：http://tk.hahajie.cn

PHP:  strrev($s);
来源：http://yz.panjiajie.cn

JS:   [...s].reverse().join("")
来源：http://ej.nicolike.cn

TS:   [...s].reverse().join("")
来源：http://mj.bjjhwx.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zh.hahajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://sv.haigaiapp.cn

Ruby: s.reverse
来源：http://qe.haigaiapp.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ug.szxytkj.cn

[E12] 统计某字符出现次数
来源：http://lz.huixinmuqiang.cn

Py:   s.count("a")
来源：http://ih.huixinmuqiang.cn

PHP:  substr_count($s, "a");
来源：http://ii.szsharing.cn

JS:   s.split("a").length - 1
来源：http://qe.huixinmuqiang.cn

TS:   s.split("a").length - 1
来源：http://uf.huixinmuqiang.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://co.lnxyls.cn

Go:   strings.Count(s, "a")
来源：http://lt.shtwfgs.cn

Ruby: s.count("a")
来源：http://lj.shxzskj.cn

C#:   s.Count(c => c == 'a')
来源：http://ok.huixinmuqiang.cn

[E13] 逐字符遍历
来源：http://ze.jctech888.com.cn

Py:   for ch in s: print(ch)
来源：http://ea.9csxet.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lb.hahajie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://dt.bjjhwx.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://jg.jctech888.com.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ug.bjjhwx.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fx.9csxet.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://xt.wgjwhj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xj.colortex.cn

[E14] URL 编码与 Base64
来源：http://vx.bookmarksfly.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cy.nszjky.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ch.bookmarksfly.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ia.521024.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lx.huixinmuqiang.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xn.nszjky.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://aa.shxzukj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xj.wgjwhj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zp.huanxung.cn

[E15] HTML 转义 / 反转义
来源：http://fr.szsharing.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://az.nszjky.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://on.9csxet.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xp.asd995.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://rh.hahajie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://nk.huanxung.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xg.shxzskj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jj.lnxyls.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bo.szsharing.cn

[E16] 数字千分位
来源：http://xh.colortex.cn

Py:   f"{1234567:,}"
来源：http://bi.newstarts.cn

PHP:  number_format(1234567);
来源：http://bz.shxzukj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ht.huixiangedu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://li.newstarts.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fa.panjiajie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vy.huanxung.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://sq.gzmigu.cn

C#:   1234567.ToString("N0")
来源：http://vo.shxzukj.cn

[E17] 首字母大写
来源：http://ug.chemitech.net.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pp.521024.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ty.panjiajie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tn.521024.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://in.huixiangedu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://au.huanxung.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fx.muxihuayi.cn

Ruby: s.capitalize
来源：http://ed.huanxung.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tu.9csxet.cn

[E18] 模板占位符替换
来源：http://xz.hnjuh.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ok.hnjuh.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://my.bookmarksfly.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ti.jianghongdianzi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://oz.newstarts.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mo.huixinmuqiang.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://od.colortex.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rm.asd995.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fw.nicolike.cn

[E19] 多行文本按行拆分
来源：http://nz.haigaiapp.cn

Py:   s.splitlines()
来源：http://sf.szxytkj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fg.bjjhwx.cn

JS:   s.split(/\r?\n/)
来源：http://dn.shtwfgs.cn

TS:   s.split(/\r?\n/)
来源：http://jd.yuntaijiaju.cn

Java: s.lines().toList()
来源：http://mu.muxihuayi.cn

Go:   strings.Split(s, "\n")
来源：http://jr.hahajie.cn

Ruby: s.lines
来源：http://zp.huanxung.cn

C#:   s.Split('\n')
来源：http://hn.shxzskj.cn

[E20] 判断字符串是否为空
来源：http://vf.yuexingan06.cn

Py:   if not s:
来源：http://rm.muxihuayi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ka.huixinmuqiang.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://if.hnjuh.cn

TS:   if (s === "") {}
来源：http://nd.wgjwhj.cn

Java: if (s.isEmpty()) {}
来源：http://ro.lnxyls.cn

Go:   if s == "" {}
来源：http://bq.yuexingan06.cn

Ruby: if s.empty?
来源：http://zl.shxzukj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xk.panjiajie.cn

[E21] 超长截断加省略号
来源：http://vu.wgjwhj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://om.colortex.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wq.yuntaijiaju.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xc.szsharing.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rn.jctech888.com.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ud.chemitech.net.cn

Go:   // 按 rune 判断长度后截断
来源：http://jj.hnjuh.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mo.hahajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ia.huanxung.cn

[E22] 字节长度与字符长度
来源：http://dr.asd995.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ql.gzmigu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uw.nszjky.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fd.jianghongdianzi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ku.panjiajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ca.chemitech.net.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vb.yuexingan06.cn

Ruby: s.bytesize;  s.length
来源：http://cz.521024.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sp.huixiangedu.cn

================================================================================
来源：http://ta.wgjwhj.cn

F. 文件与目录
来源：http://gl.jianghongdianzi.cn

================================================================================
来源：http://ma.jctech888.com.cn

[F01] 读取整个文件
来源：http://po.szsharing.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qh.shxzukj.cn

PHP:  file_get_contents("a.txt");
来源：http://bn.colortex.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nv.nicolike.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://oh.jctech888.com.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://dq.yuexingan06.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pa.chemitech.net.cn

Ruby: File.read("a.txt")
来源：http://da.hahajie.cn

C#:   File.ReadAllText("a.txt");
来源：http://vg.9csxet.cn

[F02] 逐行读取文件
来源：http://ok.lnxyls.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://be.wgjwhj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fv.szsharing.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bu.newstarts.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ef.jianghongdianzi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vr.shxzukj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bi.haigaiapp.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://sk.bjjhwx.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rx.yuntaijiaju.cn

[F03] 写入文件（覆盖）
来源：http://cs.bjjhwx.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mf.jianghongdianzi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://bg.yuexingan06.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zn.521024.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ov.jctech888.com.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yh.wgjwhj.cn


<!-- 参考信息 -->