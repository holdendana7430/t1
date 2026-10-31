代发 wailian999

Java: new ArrayList<>(list);
来源：http://jc.nicolike.cn

Go:   copied := append([]int(nil), arr...)
来源：http://jw.huixinmuqiang.cn

Ruby: arr.dup;  arr.clone
来源：http://mi.szxytkj.cn

C#:   new List<int>(list);
来源：http://jx.bookmarksfly.cn

[D23] reduce 累积计算
来源：http://fn.huixiangedu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lx.yuntaijiaju.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fl.bookmarksfly.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fx.nicolike.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://md.bookmarksfly.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qq.jctech888.com.cn

Go:   // 手写循环
来源：http://un.bjjhwx.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rj.panjiajie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mg.yuntaijiaju.cn

[D24] 字典 / Map 基本操作
来源：http://aa.jctech888.com.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vy.bookmarksfly.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wo.jctech888.com.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qn.huixinmuqiang.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kb.nszjky.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bc.chemitech.net.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ym.colortex.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bu.haigaiapp.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wq.haigaiapp.cn

[D25] Set 集合去重与交并差
来源：http://bm.shxzukj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qg.bjjhwx.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kc.521024.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cm.hahajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://op.yuexingan06.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qf.szsharing.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://aj.521024.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jx.shtwfgs.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tv.9csxet.cn

[D26] 数组转字符串
来源：http://kx.newstarts.cn

Py:   ", ".join(map(str, arr))
来源：http://nn.lnxyls.cn

PHP:  implode(", ", $arr);
来源：http://ga.colortex.cn

JS:   arr.join(", ")
来源：http://nj.nszjky.cn

TS:   arr.join(", ")
来源：http://ne.chemitech.net.cn

Java: String.join(", ", list)
来源：http://rp.chemitech.net.cn

Go:   strings.Join(strs, ", ")
来源：http://lh.yuntaijiaju.cn

Ruby: arr.join(", ")
来源：http://zd.huixiangedu.cn

C#:   string.Join(", ", list)
来源：http://og.chemitech.net.cn

================================================================================
来源：http://jw.hnjuh.cn

E. 字符串处理
来源：http://ur.huanxung.cn

================================================================================
来源：http://dh.muxihuayi.cn

[E01] 拼接字符串
来源：http://vo.gzmigu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cw.szxytkj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cc.muxihuayi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wr.nicolike.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tk.chemitech.net.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sb.wgjwhj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mb.muxihuayi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ae.muxihuayi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qi.hnjuh.cn

[E02] 重复字符串
来源：http://ed.hahajie.cn

Py:   "ab" * 3
来源：http://sb.muxihuayi.cn

PHP:  str_repeat("ab", 3);
来源：http://go.bjjhwx.cn

JS:   "ab".repeat(3)
来源：http://oq.jctech888.com.cn

TS:   "ab".repeat(3)
来源：http://uu.lnxyls.cn

Java: "ab".repeat(3)
来源：http://dc.hnjuh.cn

Go:   strings.Repeat("ab", 3)
来源：http://bu.chemitech.net.cn

Ruby: "ab" * 3
来源：http://dl.521024.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://se.panjiajie.cn

[E03] 截取子串
来源：http://ky.nicolike.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tl.huixinmuqiang.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pj.hahajie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://al.szxytkj.cn

TS:   s.slice(1, 4)
来源：http://sy.colortex.cn

Java: s.substring(1, 4)
来源：http://sb.shtwfgs.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vo.szsharing.cn

Ruby: s[1, 3];  s[1..3]
来源：http://pa.jctech888.com.cn

C#:   s.Substring(1, 3)
来源：http://rn.bjjhwx.cn

[E04] 查找子串位置
来源：http://xq.hnjuh.cn

Py:   s.find("x");  s.index("x")
来源：http://tf.wgjwhj.cn

PHP:  strpos($s, "x");
来源：http://en.shxzukj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yz.bookmarksfly.cn

TS:   s.indexOf("x")
来源：http://bd.huixiangedu.cn

Java: s.indexOf("x")
来源：http://vf.jianghongdianzi.cn

Go:   strings.Index(s, "x")
来源：http://pt.bookmarksfly.cn

Ruby: s.index("x")
来源：http://ij.colortex.cn

C#:   s.IndexOf("x")
来源：http://vo.chemitech.net.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://je.bookmarksfly.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cl.nicolike.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jp.szsharing.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://il.haigaiapp.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ne.9csxet.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://to.colortex.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rp.newstarts.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://sf.yuexingan06.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ah.colortex.cn

[E06] 替换子串
来源：http://im.bjjhwx.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dc.shxzukj.cn

PHP:  str_replace("a", "b", $s);
来源：http://mr.szsharing.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dz.yuexingan06.cn

TS:   s.replaceAll("a", "b")
来源：http://af.bjjhwx.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wy.muxihuayi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ub.huixinmuqiang.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://go.yuntaijiaju.cn

C#:   s.Replace("a", "b")
来源：http://xi.yuntaijiaju.cn

[E07] 按分隔符拆分
来源：http://cb.szsharing.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lt.nicolike.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gb.panjiajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://si.bookmarksfly.cn

TS:   s.split(",")
来源：http://vm.shtwfgs.cn

Java: s.split(",");  s.split("\\s+")
来源：http://vs.asd995.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ze.shxzskj.cn

Ruby: s.split(",");  s.split
来源：http://ck.bookmarksfly.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qq.hahajie.cn

[E08] 数组按分隔符合并
来源：http://qk.nicolike.cn

Py:   ",".join(items)
来源：http://cs.521024.cn

PHP:  implode(",", $items);
来源：http://vl.panjiajie.cn

JS:   items.join(",")
来源：http://rh.szxytkj.cn

TS:   items.join(",")
来源：http://vh.bjjhwx.cn

Java: String.join(",", items)
来源：http://ri.yuexingan06.cn

Go:   strings.Join(items, ",")
来源：http://ro.gzmigu.cn

Ruby: items.join(",")
来源：http://ue.hnjuh.cn

C#:   string.Join(",", items)
来源：http://qg.szxytkj.cn

[E09] 去除所有空白字符
来源：http://go.asd995.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://yw.newstarts.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hw.521024.cn

JS:   s.replace(/\s+/g, "")
来源：http://cg.jctech888.com.cn

TS:   s.replace(/\s+/g, "")
来源：http://eg.colortex.cn

Java: s.replaceAll("\\s+", "")
来源：http://rk.521024.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://tx.hahajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://uo.hnjuh.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sj.bookmarksfly.cn

[E10] 左侧补零 / 定长填充
来源：http://wu.shtwfgs.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qg.yuntaijiaju.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zb.newstarts.cn

JS:   "7".padStart(3, "0")
来源：http://dt.huixiangedu.cn

TS:   "7".padStart(3, "0")
来源：http://hg.colortex.cn

Java: String.format("%03d", 7)
来源：http://hd.haigaiapp.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://bp.shxzskj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cz.9csxet.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bb.yuntaijiaju.cn

[E11] 反转字符串
来源：http://ek.jianghongdianzi.cn

Py:   s[::-1]
来源：http://fa.bjjhwx.cn

PHP:  strrev($s);
来源：http://yy.jianghongdianzi.cn

JS:   [...s].reverse().join("")
来源：http://ic.521024.cn

TS:   [...s].reverse().join("")
来源：http://ml.shxzskj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://md.szxytkj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ni.jianghongdianzi.cn

Ruby: s.reverse
来源：http://ry.hahajie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://dx.jctech888.com.cn

[E12] 统计某字符出现次数
来源：http://cb.chemitech.net.cn

Py:   s.count("a")
来源：http://se.asd995.cn

PHP:  substr_count($s, "a");
来源：http://sn.lnxyls.cn

JS:   s.split("a").length - 1
来源：http://uf.hahajie.cn

TS:   s.split("a").length - 1
来源：http://ex.panjiajie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gc.szsharing.cn

Go:   strings.Count(s, "a")
来源：http://dd.huanxung.cn

Ruby: s.count("a")
来源：http://rl.asd995.cn

C#:   s.Count(c => c == 'a')
来源：http://ha.huixiangedu.cn

[E13] 逐字符遍历
来源：http://od.bjjhwx.cn

Py:   for ch in s: print(ch)
来源：http://bq.shxzukj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wm.gzmigu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xw.9csxet.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://kz.yuntaijiaju.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://uj.newstarts.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vz.shxzskj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ag.asd995.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mr.jctech888.com.cn

[E14] URL 编码与 Base64
来源：http://fq.nszjky.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://li.asd995.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://lh.haigaiapp.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ro.huixiangedu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://er.colortex.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ek.newstarts.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sf.chemitech.net.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yj.jianghongdianzi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rp.huanxung.cn

[E15] HTML 转义 / 反转义
来源：http://ny.jianghongdianzi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://pb.huixinmuqiang.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yh.szxytkj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xw.bookmarksfly.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ow.chemitech.net.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lt.bjjhwx.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wy.haigaiapp.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tc.huixiangedu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lj.bookmarksfly.cn

[E16] 数字千分位
来源：http://ez.521024.cn

Py:   f"{1234567:,}"
来源：http://hw.yuntaijiaju.cn

PHP:  number_format(1234567);
来源：http://cs.lnxyls.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://oc.nszjky.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ac.bjjhwx.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tl.huixinmuqiang.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cc.wgjwhj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mq.wgjwhj.cn

C#:   1234567.ToString("N0")
来源：http://nv.yuntaijiaju.cn

[E17] 首字母大写
来源：http://ba.szxytkj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pe.jianghongdianzi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://oh.shxzukj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gn.haigaiapp.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kt.lnxyls.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ep.newstarts.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wy.bookmarksfly.cn

Ruby: s.capitalize
来源：http://zr.shtwfgs.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://me.huixinmuqiang.cn

[E18] 模板占位符替换
来源：http://ra.lnxyls.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hw.521024.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yd.bookmarksfly.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://fg.lnxyls.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ux.521024.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://al.muxihuayi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lr.bookmarksfly.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bi.gzmigu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dw.bookmarksfly.cn

[E19] 多行文本按行拆分
来源：http://bi.haigaiapp.cn

Py:   s.splitlines()
来源：http://wy.muxihuayi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ll.hnjuh.cn

JS:   s.split(/\r?\n/)
来源：http://ve.jianghongdianzi.cn

TS:   s.split(/\r?\n/)
来源：http://rg.nicolike.cn

Java: s.lines().toList()
来源：http://ir.haigaiapp.cn

Go:   strings.Split(s, "\n")
来源：http://gm.lnxyls.cn

Ruby: s.lines
来源：http://zn.bookmarksfly.cn

C#:   s.Split('\n')
来源：http://vx.yuexingan06.cn

[E20] 判断字符串是否为空
来源：http://wl.hahajie.cn

Py:   if not s:
来源：http://tb.hahajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jy.shxzskj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wc.muxihuayi.cn

TS:   if (s === "") {}
来源：http://ff.colortex.cn

Java: if (s.isEmpty()) {}
来源：http://zq.lnxyls.cn

Go:   if s == "" {}
来源：http://fy.huanxung.cn

Ruby: if s.empty?
来源：http://uc.521024.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ls.szxytkj.cn

[E21] 超长截断加省略号
来源：http://gp.gzmigu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ql.jianghongdianzi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yv.yuexingan06.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pp.nszjky.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kj.szsharing.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gp.jctech888.com.cn

Go:   // 按 rune 判断长度后截断
来源：http://ve.colortex.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lu.szxytkj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bg.szxytkj.cn

[E22] 字节长度与字符长度
来源：http://nf.lnxyls.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bi.colortex.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ef.bjjhwx.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mr.huixiangedu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tg.gzmigu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cj.shxzukj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://es.szxytkj.cn

Ruby: s.bytesize;  s.length
来源：http://zr.nszjky.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fj.nszjky.cn

================================================================================
来源：http://bw.yuntaijiaju.cn

F. 文件与目录
来源：http://hb.colortex.cn

================================================================================
来源：http://ib.asd995.cn

[F01] 读取整个文件
来源：http://be.nszjky.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mm.huixinmuqiang.cn

PHP:  file_get_contents("a.txt");
来源：http://ei.hahajie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lp.szsharing.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wa.jianghongdianzi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vj.hnjuh.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ge.szxytkj.cn

Ruby: File.read("a.txt")
来源：http://eh.nicolike.cn

C#:   File.ReadAllText("a.txt");
来源：http://ox.muxihuayi.cn

[F02] 逐行读取文件
来源：http://sf.shtwfgs.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mn.9csxet.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ex.shtwfgs.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bo.9csxet.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ub.shxzskj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yo.asd995.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yk.nszjky.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dl.chemitech.net.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hp.hahajie.cn

[F03] 写入文件（覆盖）
来源：http://vw.hnjuh.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xr.bookmarksfly.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://bf.jctech888.com.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://as.shxzskj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hi.shtwfgs.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ng.nicolike.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rz.huixinmuqiang.cn

Ruby: File.write("a.txt", "hi")
来源：http://kv.jctech888.com.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://sq.9csxet.cn

[F04] 追加写入文件
来源：http://ns.gzmigu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vw.muxihuayi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cc.wgjwhj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dx.muxihuayi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lc.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jv.szsharing.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vq.hahajie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wp.yuexingan06.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ip.bjjhwx.cn

[F05] 判断文件或目录是否存在
来源：http://ig.521024.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://cn.newstarts.cn

PHP:  file_exists("a.txt");
来源：http://ax.521024.cn

JS:   fs.existsSync("a.txt")
来源：http://vi.shtwfgs.cn

TS:   fs.existsSync("a.txt")
来源：http://vf.huanxung.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ek.haigaiapp.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ea.shxzskj.cn

Ruby: File.exist?("a.txt")
来源：http://hh.bookmarksfly.cn

C#:   File.Exists("a.txt")
来源：http://bf.huixinmuqiang.cn

[F06] 删除文件
来源：http://sm.haigaiapp.cn

Py:   os.remove("a.txt")
来源：http://rl.wgjwhj.cn

PHP:  unlink("a.txt");
来源：http://af.haigaiapp.cn

JS:   fs.unlinkSync("a.txt")
来源：http://mu.newstarts.cn

TS:   fs.unlinkSync("a.txt")
来源：http://xi.huixiangedu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uo.wgjwhj.cn

Go:   os.Remove("a.txt")
来源：http://vr.huixinmuqiang.cn

Ruby: File.delete("a.txt")
来源：http://vz.newstarts.cn

C#:   File.Delete("a.txt");
来源：http://qe.bookmarksfly.cn

[F07] 创建目录（含多级）
来源：http://eb.huixiangedu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nt.bjjhwx.cn


<!-- 参考信息 -->