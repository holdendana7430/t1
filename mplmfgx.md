代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://gh.hahajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yl.jctech888.com.cn

Go:   // 手写 map[string][]T
来源：http://gu.nszjky.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rw.jctech888.com.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hu.huixinmuqiang.cn

[D20] 统计每个元素出现次数
来源：http://ns.colortex.cn

Py:   Counter(arr)
来源：http://rq.wgjwhj.cn

PHP:  array_count_values($arr);
来源：http://qe.hahajie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nb.shtwfgs.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iy.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gk.wgjwhj.cn

Go:   // 手写 map[T]int
来源：http://mw.wgjwhj.cn

Ruby: arr.tally
来源：http://fk.lnxyls.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xv.bookmarksfly.cn

[D21] 判断是否包含某元素
来源：http://zq.lnxyls.cn

Py:   x in arr
来源：http://sy.hnjuh.cn

PHP:  in_array($x, $arr, true);
来源：http://yh.bjjhwx.cn

JS:   arr.includes(x)
来源：http://yx.9csxet.cn

TS:   arr.includes(x)
来源：http://da.asd995.cn

Java: list.contains(x)
来源：http://vm.yuntaijiaju.cn

Go:   slices.Contains(arr, x)
来源：http://zy.9csxet.cn

Ruby: arr.include?(x)
来源：http://kj.chemitech.net.cn

C#:   list.Contains(x)
来源：http://xd.shxzukj.cn

[D22] 复制数组（避免共享引用）
来源：http://zw.newstarts.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://uq.hahajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vk.colortex.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://du.szxytkj.cn

TS:   [...arr];
来源：http://wt.colortex.cn

Java: new ArrayList<>(list);
来源：http://yz.huixiangedu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://jh.shxzskj.cn

Ruby: arr.dup;  arr.clone
来源：http://ov.chemitech.net.cn

C#:   new List<int>(list);
来源：http://da.shxzukj.cn

[D23] reduce 累积计算
来源：http://re.shxzukj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://va.wgjwhj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hn.bjjhwx.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lc.colortex.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fr.hnjuh.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ti.chemitech.net.cn

Go:   // 手写循环
来源：http://vx.nszjky.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://sj.shtwfgs.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tb.muxihuayi.cn

[D24] 字典 / Map 基本操作
来源：http://wz.chemitech.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://sa.panjiajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ht.haigaiapp.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://br.jianghongdianzi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qk.jianghongdianzi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cw.shxzskj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://to.gzmigu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qh.lnxyls.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jv.muxihuayi.cn

[D25] Set 集合去重与交并差
来源：http://pz.shxzukj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ov.nszjky.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vn.shtwfgs.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hd.chemitech.net.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://id.521024.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ll.newstarts.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://uv.bookmarksfly.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sq.huixinmuqiang.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vi.521024.cn

[D26] 数组转字符串
来源：http://fp.9csxet.cn

Py:   ", ".join(map(str, arr))
来源：http://ha.yuntaijiaju.cn

PHP:  implode(", ", $arr);
来源：http://nj.wgjwhj.cn

JS:   arr.join(", ")
来源：http://ww.shxzskj.cn

TS:   arr.join(", ")
来源：http://yv.haigaiapp.cn

Java: String.join(", ", list)
来源：http://al.lnxyls.cn

Go:   strings.Join(strs, ", ")
来源：http://tt.asd995.cn

Ruby: arr.join(", ")
来源：http://xk.huanxung.cn

C#:   string.Join(", ", list)
来源：http://bo.asd995.cn

================================================================================
来源：http://ep.bjjhwx.cn

E. 字符串处理
来源：http://oj.wgjwhj.cn

================================================================================
来源：http://ns.shxzukj.cn

[E01] 拼接字符串
来源：http://cx.nszjky.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cy.chemitech.net.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://aw.jctech888.com.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bx.haigaiapp.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rh.huanxung.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bx.newstarts.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ew.asd995.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xk.muxihuayi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zp.jianghongdianzi.cn

[E02] 重复字符串
来源：http://bs.wgjwhj.cn

Py:   "ab" * 3
来源：http://ls.hahajie.cn

PHP:  str_repeat("ab", 3);
来源：http://ej.colortex.cn

JS:   "ab".repeat(3)
来源：http://in.gzmigu.cn

TS:   "ab".repeat(3)
来源：http://gr.bjjhwx.cn

Java: "ab".repeat(3)
来源：http://sw.shxzukj.cn

Go:   strings.Repeat("ab", 3)
来源：http://xk.colortex.cn

Ruby: "ab" * 3
来源：http://hr.newstarts.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mh.szsharing.cn

[E03] 截取子串
来源：http://sf.hahajie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fp.lnxyls.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bg.szxytkj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nc.jianghongdianzi.cn

TS:   s.slice(1, 4)
来源：http://qy.haigaiapp.cn

Java: s.substring(1, 4)
来源：http://ja.haigaiapp.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xj.yuexingan06.cn

Ruby: s[1, 3];  s[1..3]
来源：http://hf.shxzukj.cn

C#:   s.Substring(1, 3)
来源：http://eo.bjjhwx.cn

[E04] 查找子串位置
来源：http://so.9csxet.cn

Py:   s.find("x");  s.index("x")
来源：http://xt.lnxyls.cn

PHP:  strpos($s, "x");
来源：http://cd.huixiangedu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://em.asd995.cn

TS:   s.indexOf("x")
来源：http://vc.muxihuayi.cn

Java: s.indexOf("x")
来源：http://xy.chemitech.net.cn

Go:   strings.Index(s, "x")
来源：http://jq.jianghongdianzi.cn

Ruby: s.index("x")
来源：http://fe.shxzskj.cn

C#:   s.IndexOf("x")
来源：http://jo.jctech888.com.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://yy.yuntaijiaju.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fe.newstarts.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lv.bookmarksfly.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sy.yuntaijiaju.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://iw.haigaiapp.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://la.wgjwhj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://we.nszjky.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xx.newstarts.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ui.shxzukj.cn

[E06] 替换子串
来源：http://uw.shtwfgs.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xr.shtwfgs.cn

PHP:  str_replace("a", "b", $s);
来源：http://ke.haigaiapp.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cy.szsharing.cn

TS:   s.replaceAll("a", "b")
来源：http://kv.nicolike.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wp.521024.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://an.huixiangedu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tq.jianghongdianzi.cn

C#:   s.Replace("a", "b")
来源：http://jt.huixinmuqiang.cn

[E07] 按分隔符拆分
来源：http://nt.gzmigu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yl.muxihuayi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qw.colortex.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://nk.hahajie.cn

TS:   s.split(",")
来源：http://ur.shtwfgs.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xu.wgjwhj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zl.yuexingan06.cn

Ruby: s.split(",");  s.split
来源：http://jv.asd995.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lz.haigaiapp.cn

[E08] 数组按分隔符合并
来源：http://po.colortex.cn

Py:   ",".join(items)
来源：http://vi.shxzskj.cn

PHP:  implode(",", $items);
来源：http://zl.huixiangedu.cn

JS:   items.join(",")
来源：http://lt.shxzukj.cn

TS:   items.join(",")
来源：http://pt.shtwfgs.cn

Java: String.join(",", items)
来源：http://ey.huixinmuqiang.cn

Go:   strings.Join(items, ",")
来源：http://rh.szsharing.cn

Ruby: items.join(",")
来源：http://dz.jctech888.com.cn

C#:   string.Join(",", items)
来源：http://uu.9csxet.cn

[E09] 去除所有空白字符
来源：http://yh.bookmarksfly.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vm.colortex.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dw.9csxet.cn

JS:   s.replace(/\s+/g, "")
来源：http://ld.huixiangedu.cn

TS:   s.replace(/\s+/g, "")
来源：http://kz.yuntaijiaju.cn

Java: s.replaceAll("\\s+", "")
来源：http://er.shtwfgs.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://zc.nszjky.cn

Ruby: s.gsub(/\s+/, "")
来源：http://pc.asd995.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wq.shtwfgs.cn

[E10] 左侧补零 / 定长填充
来源：http://vs.szxytkj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://av.jctech888.com.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cu.shtwfgs.cn

JS:   "7".padStart(3, "0")
来源：http://rs.panjiajie.cn

TS:   "7".padStart(3, "0")
来源：http://ci.jctech888.com.cn

Java: String.format("%03d", 7)
来源：http://hh.lnxyls.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://db.9csxet.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ep.lnxyls.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lz.bjjhwx.cn

[E11] 反转字符串
来源：http://rs.yuntaijiaju.cn

Py:   s[::-1]
来源：http://mm.hahajie.cn

PHP:  strrev($s);
来源：http://fh.bookmarksfly.cn

JS:   [...s].reverse().join("")
来源：http://yx.asd995.cn

TS:   [...s].reverse().join("")
来源：http://yh.lnxyls.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://yl.lnxyls.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ef.nszjky.cn

Ruby: s.reverse
来源：http://vl.haigaiapp.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ny.gzmigu.cn

[E12] 统计某字符出现次数
来源：http://bg.shxzskj.cn

Py:   s.count("a")
来源：http://pf.szsharing.cn

PHP:  substr_count($s, "a");
来源：http://un.muxihuayi.cn

JS:   s.split("a").length - 1
来源：http://qf.jianghongdianzi.cn

TS:   s.split("a").length - 1
来源：http://aj.bjjhwx.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vq.nicolike.cn

Go:   strings.Count(s, "a")
来源：http://ck.wgjwhj.cn

Ruby: s.count("a")
来源：http://tg.huixinmuqiang.cn

C#:   s.Count(c => c == 'a')
来源：http://or.colortex.cn

[E13] 逐字符遍历
来源：http://ip.shxzskj.cn

Py:   for ch in s: print(ch)
来源：http://jh.muxihuayi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zn.panjiajie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://az.hnjuh.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://zm.jctech888.com.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ef.shxzskj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fv.newstarts.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://tw.yuexingan06.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://db.shtwfgs.cn

[E14] URL 编码与 Base64
来源：http://fp.jianghongdianzi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cw.muxihuayi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ph.jctech888.com.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://io.yuexingan06.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cx.gzmigu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uv.nicolike.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ko.bookmarksfly.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ej.yuntaijiaju.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qf.huixinmuqiang.cn

[E15] HTML 转义 / 反转义
来源：http://wy.wgjwhj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://lh.yuexingan06.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ex.panjiajie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ty.shtwfgs.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://na.newstarts.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ni.wgjwhj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pr.wgjwhj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ss.yuntaijiaju.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hf.nszjky.cn

[E16] 数字千分位
来源：http://kh.nicolike.cn

Py:   f"{1234567:,}"
来源：http://sj.colortex.cn

PHP:  number_format(1234567);
来源：http://qd.haigaiapp.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://cr.shxzskj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://cu.chemitech.net.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dk.hahajie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://px.lnxyls.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ez.hahajie.cn

C#:   1234567.ToString("N0")
来源：http://lk.panjiajie.cn

[E17] 首字母大写
来源：http://hp.asd995.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://oe.huixinmuqiang.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://us.gzmigu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oj.521024.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kv.chemitech.net.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sl.panjiajie.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://og.yuexingan06.cn

Ruby: s.capitalize
来源：http://pr.huanxung.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tr.huanxung.cn

[E18] 模板占位符替换
来源：http://nu.lnxyls.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qk.shxzskj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nv.muxihuayi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://fq.nicolike.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://qh.lnxyls.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cc.colortex.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vp.chemitech.net.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fn.chemitech.net.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gw.panjiajie.cn

[E19] 多行文本按行拆分
来源：http://pi.nicolike.cn

Py:   s.splitlines()
来源：http://nj.wgjwhj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kj.lnxyls.cn

JS:   s.split(/\r?\n/)
来源：http://tw.colortex.cn

TS:   s.split(/\r?\n/)
来源：http://le.shxzukj.cn

Java: s.lines().toList()
来源：http://gz.colortex.cn

Go:   strings.Split(s, "\n")
来源：http://rr.shtwfgs.cn

Ruby: s.lines
来源：http://uc.yuntaijiaju.cn

C#:   s.Split('\n')
来源：http://cj.asd995.cn

[E20] 判断字符串是否为空
来源：http://xq.bjjhwx.cn

Py:   if not s:
来源：http://hu.muxihuayi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gk.huanxung.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ju.panjiajie.cn

TS:   if (s === "") {}
来源：http://dx.521024.cn

Java: if (s.isEmpty()) {}
来源：http://yh.huanxung.cn

Go:   if s == "" {}
来源：http://np.521024.cn

Ruby: if s.empty?
来源：http://sx.szsharing.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xh.colortex.cn

[E21] 超长截断加省略号
来源：http://di.colortex.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vy.nszjky.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ju.9csxet.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qn.jctech888.com.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://la.yuntaijiaju.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ov.jianghongdianzi.cn

Go:   // 按 rune 判断长度后截断
来源：http://zg.panjiajie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ae.panjiajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lv.nicolike.cn

[E22] 字节长度与字符长度
来源：http://dx.hnjuh.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ty.huanxung.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hu.shtwfgs.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://le.newstarts.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bl.chemitech.net.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zk.newstarts.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mj.szxytkj.cn

Ruby: s.bytesize;  s.length
来源：http://ig.jianghongdianzi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://aj.yuexingan06.cn

================================================================================
来源：http://xq.521024.cn

F. 文件与目录
来源：http://tu.huixinmuqiang.cn

================================================================================
来源：http://vu.jianghongdianzi.cn

[F01] 读取整个文件
来源：http://ei.nicolike.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tr.wgjwhj.cn

PHP:  file_get_contents("a.txt");
来源：http://oz.szxytkj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nt.newstarts.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xt.huixinmuqiang.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://bf.jianghongdianzi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gm.asd995.cn

Ruby: File.read("a.txt")
来源：http://an.hahajie.cn

C#:   File.ReadAllText("a.txt");
来源：http://qc.szxytkj.cn

[F02] 逐行读取文件
来源：http://ka.shtwfgs.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wt.wgjwhj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nq.shtwfgs.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qh.panjiajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vg.huixiangedu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hj.shxzskj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bw.nszjky.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fj.muxihuayi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://na.haigaiapp.cn

[F03] 写入文件（覆盖）
来源：http://nv.yuntaijiaju.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jj.lnxyls.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://er.bjjhwx.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://us.szsharing.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bn.jianghongdianzi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ot.asd995.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lv.hnjuh.cn

Ruby: File.write("a.txt", "hi")
来源：http://qo.huixiangedu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://oz.huixinmuqiang.cn

[F04] 追加写入文件
来源：http://ir.lnxyls.cn


<!-- 参考信息 -->