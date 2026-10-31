代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ox.haigaiapp.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://du.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qo.huanxung.cn

Go:   // 手写 map[T]int
来源：http://ow.hnjuh.cn

Ruby: arr.tally
来源：http://qm.nszjky.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yk.gzmigu.cn

[D21] 判断是否包含某元素
来源：http://oe.newstarts.cn

Py:   x in arr
来源：http://zt.chemitech.net.cn

PHP:  in_array($x, $arr, true);
来源：http://lu.bookmarksfly.cn

JS:   arr.includes(x)
来源：http://qx.lnxyls.cn

TS:   arr.includes(x)
来源：http://zg.wgjwhj.cn

Java: list.contains(x)
来源：http://yw.9csxet.cn

Go:   slices.Contains(arr, x)
来源：http://an.szxytkj.cn

Ruby: arr.include?(x)
来源：http://rn.wgjwhj.cn

C#:   list.Contains(x)
来源：http://zn.shxzukj.cn

[D22] 复制数组（避免共享引用）
来源：http://ge.hahajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://im.jctech888.com.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sw.newstarts.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vo.huixiangedu.cn

TS:   [...arr];
来源：http://ey.hahajie.cn

Java: new ArrayList<>(list);
来源：http://bm.bookmarksfly.cn

Go:   copied := append([]int(nil), arr...)
来源：http://sk.huixiangedu.cn

Ruby: arr.dup;  arr.clone
来源：http://ej.yuexingan06.cn

C#:   new List<int>(list);
来源：http://nc.yuexingan06.cn

[D23] reduce 累积计算
来源：http://gl.hahajie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tp.wgjwhj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cm.9csxet.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ir.jctech888.com.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wa.colortex.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ty.chemitech.net.cn

Go:   // 手写循环
来源：http://vz.lnxyls.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ux.shxzukj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ll.bjjhwx.cn

[D24] 字典 / Map 基本操作
来源：http://yw.newstarts.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gk.nszjky.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ss.hnjuh.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mz.shxzskj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pb.asd995.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zu.huixinmuqiang.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wx.wgjwhj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vw.huixiangedu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nx.jctech888.com.cn

[D25] Set 集合去重与交并差
来源：http://ke.szsharing.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ml.szsharing.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gl.asd995.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fz.panjiajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fe.huanxung.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nw.shxzukj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tf.bjjhwx.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sj.wgjwhj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rl.chemitech.net.cn

[D26] 数组转字符串
来源：http://fm.lnxyls.cn

Py:   ", ".join(map(str, arr))
来源：http://ji.colortex.cn

PHP:  implode(", ", $arr);
来源：http://lb.yuntaijiaju.cn

JS:   arr.join(", ")
来源：http://gy.newstarts.cn

TS:   arr.join(", ")
来源：http://al.muxihuayi.cn

Java: String.join(", ", list)
来源：http://na.shxzukj.cn

Go:   strings.Join(strs, ", ")
来源：http://op.huanxung.cn

Ruby: arr.join(", ")
来源：http://yq.hnjuh.cn

C#:   string.Join(", ", list)
来源：http://ng.haigaiapp.cn

================================================================================
来源：http://ju.panjiajie.cn

E. 字符串处理
来源：http://dj.szsharing.cn

================================================================================
来源：http://za.asd995.cn

[E01] 拼接字符串
来源：http://hv.huixinmuqiang.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tt.hahajie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xe.huixiangedu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ke.szsharing.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bj.jctech888.com.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cf.panjiajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yk.asd995.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ft.jianghongdianzi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vy.yuexingan06.cn

[E02] 重复字符串
来源：http://cj.colortex.cn

Py:   "ab" * 3
来源：http://qv.shtwfgs.cn

PHP:  str_repeat("ab", 3);
来源：http://zt.jctech888.com.cn

JS:   "ab".repeat(3)
来源：http://oz.huanxung.cn

TS:   "ab".repeat(3)
来源：http://hd.szxytkj.cn

Java: "ab".repeat(3)
来源：http://mg.asd995.cn

Go:   strings.Repeat("ab", 3)
来源：http://nn.nicolike.cn

Ruby: "ab" * 3
来源：http://ij.huanxung.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://di.yuntaijiaju.cn

[E03] 截取子串
来源：http://wi.newstarts.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tv.wgjwhj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ba.shxzskj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ic.yuexingan06.cn

TS:   s.slice(1, 4)
来源：http://nb.colortex.cn

Java: s.substring(1, 4)
来源：http://tw.huixiangedu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://do.shxzskj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ds.shxzukj.cn

C#:   s.Substring(1, 3)
来源：http://db.huixinmuqiang.cn

[E04] 查找子串位置
来源：http://oa.lnxyls.cn

Py:   s.find("x");  s.index("x")
来源：http://hp.huixiangedu.cn

PHP:  strpos($s, "x");
来源：http://iv.gzmigu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mt.nszjky.cn

TS:   s.indexOf("x")
来源：http://kk.yuntaijiaju.cn

Java: s.indexOf("x")
来源：http://pz.nicolike.cn

Go:   strings.Index(s, "x")
来源：http://mr.hahajie.cn

Ruby: s.index("x")
来源：http://gn.jianghongdianzi.cn

C#:   s.IndexOf("x")
来源：http://ta.shxzskj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://mk.huixinmuqiang.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://px.nszjky.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vk.haigaiapp.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yn.shtwfgs.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://me.shxzukj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cn.chemitech.net.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pk.nicolike.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wa.hahajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fu.panjiajie.cn

[E06] 替换子串
来源：http://pw.chemitech.net.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sa.bookmarksfly.cn

PHP:  str_replace("a", "b", $s);
来源：http://cg.panjiajie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fv.bjjhwx.cn

TS:   s.replaceAll("a", "b")
来源：http://xy.shtwfgs.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ld.yuexingan06.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://du.huixinmuqiang.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ck.newstarts.cn

C#:   s.Replace("a", "b")
来源：http://is.szsharing.cn

[E07] 按分隔符拆分
来源：http://sw.colortex.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bc.huixiangedu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://et.521024.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://nz.chemitech.net.cn

TS:   s.split(",")
来源：http://kk.asd995.cn

Java: s.split(",");  s.split("\\s+")
来源：http://bk.shtwfgs.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://sm.wgjwhj.cn

Ruby: s.split(",");  s.split
来源：http://ak.shxzukj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ma.9csxet.cn

[E08] 数组按分隔符合并
来源：http://rw.9csxet.cn

Py:   ",".join(items)
来源：http://jp.colortex.cn

PHP:  implode(",", $items);
来源：http://ga.shxzukj.cn

JS:   items.join(",")
来源：http://fn.newstarts.cn

TS:   items.join(",")
来源：http://nm.huixiangedu.cn

Java: String.join(",", items)
来源：http://op.haigaiapp.cn

Go:   strings.Join(items, ",")
来源：http://wv.colortex.cn

Ruby: items.join(",")
来源：http://bt.szxytkj.cn

C#:   string.Join(",", items)
来源：http://vy.yuexingan06.cn

[E09] 去除所有空白字符
来源：http://ge.jianghongdianzi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ky.gzmigu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kg.muxihuayi.cn

JS:   s.replace(/\s+/g, "")
来源：http://ji.chemitech.net.cn

TS:   s.replace(/\s+/g, "")
来源：http://qn.hnjuh.cn

Java: s.replaceAll("\\s+", "")
来源：http://ds.chemitech.net.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qg.jctech888.com.cn

Ruby: s.gsub(/\s+/, "")
来源：http://mq.9csxet.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vs.huanxung.cn

[E10] 左侧补零 / 定长填充
来源：http://nr.hnjuh.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kp.nszjky.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://if.chemitech.net.cn

JS:   "7".padStart(3, "0")
来源：http://kl.chemitech.net.cn

TS:   "7".padStart(3, "0")
来源：http://gm.szxytkj.cn

Java: String.format("%03d", 7)
来源：http://po.huixiangedu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ki.bookmarksfly.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://im.panjiajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wy.shxzukj.cn

[E11] 反转字符串
来源：http://bc.huanxung.cn

Py:   s[::-1]
来源：http://xw.szxytkj.cn

PHP:  strrev($s);
来源：http://gc.shtwfgs.cn

JS:   [...s].reverse().join("")
来源：http://aq.hnjuh.cn

TS:   [...s].reverse().join("")
来源：http://yf.wgjwhj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ph.9csxet.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://bg.wgjwhj.cn

Ruby: s.reverse
来源：http://aw.huanxung.cn

C#:   new string(s.Reverse().ToArray())
来源：http://tm.hahajie.cn

[E12] 统计某字符出现次数
来源：http://rq.bjjhwx.cn

Py:   s.count("a")
来源：http://tv.newstarts.cn

PHP:  substr_count($s, "a");
来源：http://yg.jctech888.com.cn

JS:   s.split("a").length - 1
来源：http://fh.chemitech.net.cn

TS:   s.split("a").length - 1
来源：http://mo.newstarts.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ag.huixiangedu.cn

Go:   strings.Count(s, "a")
来源：http://bj.yuntaijiaju.cn

Ruby: s.count("a")
来源：http://ez.shxzukj.cn

C#:   s.Count(c => c == 'a')
来源：http://lf.huanxung.cn

[E13] 逐字符遍历
来源：http://ml.521024.cn

Py:   for ch in s: print(ch)
来源：http://en.wgjwhj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ii.nszjky.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://zz.huixinmuqiang.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://xt.muxihuayi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://aj.gzmigu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vy.9csxet.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ml.chemitech.net.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tp.szsharing.cn

[E14] URL 编码与 Base64
来源：http://wy.szxytkj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fb.jianghongdianzi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ai.huixinmuqiang.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://aj.asd995.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pc.colortex.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ta.szsharing.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pr.shtwfgs.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hk.shxzskj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://te.yuexingan06.cn

[E15] HTML 转义 / 反转义
来源：http://zy.jianghongdianzi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://il.yuexingan06.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pu.bjjhwx.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xm.shxzskj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://yg.haigaiapp.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fo.newstarts.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cr.hahajie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zi.muxihuayi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nr.szsharing.cn

[E16] 数字千分位
来源：http://xt.yuexingan06.cn

Py:   f"{1234567:,}"
来源：http://ol.521024.cn

PHP:  number_format(1234567);
来源：http://vt.huixinmuqiang.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vl.szxytkj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://cv.lnxyls.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qt.lnxyls.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zj.asd995.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pk.wgjwhj.cn

C#:   1234567.ToString("N0")
来源：http://bf.bookmarksfly.cn

[E17] 首字母大写
来源：http://cn.jctech888.com.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dc.yuexingan06.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://nl.asd995.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kf.jianghongdianzi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://am.lnxyls.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nj.shxzskj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cr.muxihuayi.cn

Ruby: s.capitalize
来源：http://ra.asd995.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://by.newstarts.cn

[E18] 模板占位符替换
来源：http://py.hnjuh.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kk.hahajie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hj.shxzukj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://wg.shtwfgs.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://mo.haigaiapp.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hr.szsharing.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gc.jctech888.com.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vd.hahajie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://oj.gzmigu.cn

[E19] 多行文本按行拆分
来源：http://de.wgjwhj.cn

Py:   s.splitlines()
来源：http://hr.lnxyls.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vg.szsharing.cn

JS:   s.split(/\r?\n/)
来源：http://nl.huixinmuqiang.cn

TS:   s.split(/\r?\n/)
来源：http://nx.shxzukj.cn

Java: s.lines().toList()
来源：http://gp.huixinmuqiang.cn

Go:   strings.Split(s, "\n")
来源：http://bn.521024.cn

Ruby: s.lines
来源：http://yg.nicolike.cn

C#:   s.Split('\n')
来源：http://wx.9csxet.cn

[E20] 判断字符串是否为空
来源：http://ie.panjiajie.cn

Py:   if not s:
来源：http://vi.huixinmuqiang.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://km.colortex.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xw.chemitech.net.cn

TS:   if (s === "") {}
来源：http://yg.asd995.cn

Java: if (s.isEmpty()) {}
来源：http://ep.huanxung.cn

Go:   if s == "" {}
来源：http://px.jctech888.com.cn

Ruby: if s.empty?
来源：http://pn.huixinmuqiang.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ex.jianghongdianzi.cn

[E21] 超长截断加省略号
来源：http://un.bookmarksfly.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://su.gzmigu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jz.hnjuh.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qp.szxytkj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cm.szsharing.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://va.huixinmuqiang.cn

Go:   // 按 rune 判断长度后截断
来源：http://ds.haigaiapp.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bq.huixiangedu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://he.nicolike.cn

[E22] 字节长度与字符长度
来源：http://er.szxytkj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tu.bookmarksfly.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hn.nszjky.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://in.nicolike.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jo.lnxyls.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://js.wgjwhj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vp.yuexingan06.cn

Ruby: s.bytesize;  s.length
来源：http://jo.shxzskj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tv.huixinmuqiang.cn

================================================================================
来源：http://tj.huixinmuqiang.cn

F. 文件与目录
来源：http://xy.panjiajie.cn

================================================================================
来源：http://lr.szsharing.cn

[F01] 读取整个文件
来源：http://ci.yuntaijiaju.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ig.wgjwhj.cn

PHP:  file_get_contents("a.txt");
来源：http://td.shxzukj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ds.nicolike.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bg.shtwfgs.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ze.wgjwhj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vp.haigaiapp.cn

Ruby: File.read("a.txt")
来源：http://qq.wgjwhj.cn

C#:   File.ReadAllText("a.txt");
来源：http://dv.yuexingan06.cn

[F02] 逐行读取文件
来源：http://il.9csxet.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fa.yuexingan06.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pd.nicolike.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.huanxung.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jx.yuntaijiaju.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qf.gzmigu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rg.hahajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kl.lnxyls.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ix.newstarts.cn

[F03] 写入文件（覆盖）
来源：http://kw.huixiangedu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qj.szsharing.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://bb.hahajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mo.nicolike.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jr.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vb.nszjky.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://al.gzmigu.cn

Ruby: File.write("a.txt", "hi")
来源：http://cj.hahajie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hg.hnjuh.cn

[F04] 追加写入文件
来源：http://mc.haigaiapp.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bs.asd995.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cm.muxihuayi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ov.muxihuayi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://us.bjjhwx.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hu.lnxyls.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://aw.yuntaijiaju.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nk.huixinmuqiang.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ze.jctech888.com.cn


<!-- 参考信息 -->