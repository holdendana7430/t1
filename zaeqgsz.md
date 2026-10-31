代发 wailian999

Java: new ArrayList<>(list);
来源：http://hb.huixiangedu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ku.521024.cn

Ruby: arr.dup;  arr.clone
来源：http://sd.newstarts.cn

C#:   new List<int>(list);
来源：http://yp.wgjwhj.cn

[D23] reduce 累积计算
来源：http://gd.shxzukj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ju.shxzukj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qr.bjjhwx.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://or.bjjhwx.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dz.huixinmuqiang.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://pt.panjiajie.cn

Go:   // 手写循环
来源：http://qu.hnjuh.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ch.hnjuh.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mu.chemitech.net.cn

[D24] 字典 / Map 基本操作
来源：http://ap.asd995.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://eo.newstarts.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sf.panjiajie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zm.521024.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zq.hnjuh.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://os.521024.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sy.nicolike.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lo.colortex.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://uk.nszjky.cn

[D25] Set 集合去重与交并差
来源：http://ux.nicolike.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bb.bookmarksfly.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hq.9csxet.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://su.jctech888.com.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qo.panjiajie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lt.9csxet.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sv.yuexingan06.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zk.huixiangedu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qm.shxzskj.cn

[D26] 数组转字符串
来源：http://fr.newstarts.cn

Py:   ", ".join(map(str, arr))
来源：http://ic.muxihuayi.cn

PHP:  implode(", ", $arr);
来源：http://hf.newstarts.cn

JS:   arr.join(", ")
来源：http://yb.huixiangedu.cn

TS:   arr.join(", ")
来源：http://vt.haigaiapp.cn

Java: String.join(", ", list)
来源：http://cs.huixinmuqiang.cn

Go:   strings.Join(strs, ", ")
来源：http://dp.chemitech.net.cn

Ruby: arr.join(", ")
来源：http://sw.wgjwhj.cn

C#:   string.Join(", ", list)
来源：http://lq.newstarts.cn

================================================================================
来源：http://gc.huanxung.cn

E. 字符串处理
来源：http://bf.hnjuh.cn

================================================================================
来源：http://pr.hahajie.cn

[E01] 拼接字符串
来源：http://li.hnjuh.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wy.newstarts.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gc.yuexingan06.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vw.jctech888.com.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cl.chemitech.net.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fq.bookmarksfly.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nm.asd995.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fv.gzmigu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kq.nszjky.cn

[E02] 重复字符串
来源：http://zt.huixinmuqiang.cn

Py:   "ab" * 3
来源：http://yv.hahajie.cn

PHP:  str_repeat("ab", 3);
来源：http://xl.gzmigu.cn

JS:   "ab".repeat(3)
来源：http://on.jianghongdianzi.cn

TS:   "ab".repeat(3)
来源：http://qo.haigaiapp.cn

Java: "ab".repeat(3)
来源：http://kl.jctech888.com.cn

Go:   strings.Repeat("ab", 3)
来源：http://me.gzmigu.cn

Ruby: "ab" * 3
来源：http://vl.9csxet.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uu.shxzukj.cn

[E03] 截取子串
来源：http://rg.muxihuayi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://sv.wgjwhj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lj.szsharing.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zn.haigaiapp.cn

TS:   s.slice(1, 4)
来源：http://fq.shxzukj.cn

Java: s.substring(1, 4)
来源：http://db.haigaiapp.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hn.yuntaijiaju.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ki.jianghongdianzi.cn

C#:   s.Substring(1, 3)
来源：http://kx.521024.cn

[E04] 查找子串位置
来源：http://ug.jianghongdianzi.cn

Py:   s.find("x");  s.index("x")
来源：http://sc.haigaiapp.cn

PHP:  strpos($s, "x");
来源：http://rm.jctech888.com.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qi.szxytkj.cn

TS:   s.indexOf("x")
来源：http://mk.nszjky.cn

Java: s.indexOf("x")
来源：http://ds.shxzskj.cn

Go:   strings.Index(s, "x")
来源：http://yu.szxytkj.cn

Ruby: s.index("x")
来源：http://lo.wgjwhj.cn

C#:   s.IndexOf("x")
来源：http://wd.9csxet.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://mt.haigaiapp.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hg.wgjwhj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://gb.wgjwhj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bo.huanxung.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://yk.521024.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dw.nicolike.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uj.yuntaijiaju.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ct.hnjuh.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yb.szsharing.cn

[E06] 替换子串
来源：http://ft.hnjuh.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ox.yuntaijiaju.cn

PHP:  str_replace("a", "b", $s);
来源：http://ai.szxytkj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ji.wgjwhj.cn

TS:   s.replaceAll("a", "b")
来源：http://nx.colortex.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tf.wgjwhj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hg.szsharing.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jg.lnxyls.cn

C#:   s.Replace("a", "b")
来源：http://sr.shtwfgs.cn

[E07] 按分隔符拆分
来源：http://ae.shtwfgs.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nn.hahajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cl.nicolike.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://kn.huixinmuqiang.cn

TS:   s.split(",")
来源：http://kl.colortex.cn

Java: s.split(",");  s.split("\\s+")
来源：http://gk.9csxet.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jj.szsharing.cn

Ruby: s.split(",");  s.split
来源：http://rs.huixiangedu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mq.asd995.cn

[E08] 数组按分隔符合并
来源：http://qk.muxihuayi.cn

Py:   ",".join(items)
来源：http://ma.gzmigu.cn

PHP:  implode(",", $items);
来源：http://zx.shxzukj.cn

JS:   items.join(",")
来源：http://ge.huanxung.cn

TS:   items.join(",")
来源：http://kw.shxzukj.cn

Java: String.join(",", items)
来源：http://qf.nszjky.cn

Go:   strings.Join(items, ",")
来源：http://ny.jianghongdianzi.cn

Ruby: items.join(",")
来源：http://wr.bjjhwx.cn

C#:   string.Join(",", items)
来源：http://nj.chemitech.net.cn

[E09] 去除所有空白字符
来源：http://tn.shtwfgs.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zn.haigaiapp.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nz.wgjwhj.cn

JS:   s.replace(/\s+/g, "")
来源：http://yz.bjjhwx.cn

TS:   s.replace(/\s+/g, "")
来源：http://gx.yuexingan06.cn

Java: s.replaceAll("\\s+", "")
来源：http://hn.yuexingan06.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://in.nszjky.cn

Ruby: s.gsub(/\s+/, "")
来源：http://zy.shtwfgs.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bs.wgjwhj.cn

[E10] 左侧补零 / 定长填充
来源：http://oj.shtwfgs.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ju.huixinmuqiang.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://sq.szxytkj.cn

JS:   "7".padStart(3, "0")
来源：http://wb.gzmigu.cn

TS:   "7".padStart(3, "0")
来源：http://cj.huanxung.cn

Java: String.format("%03d", 7)
来源：http://gf.yuntaijiaju.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://qp.newstarts.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bt.szsharing.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://se.haigaiapp.cn

[E11] 反转字符串
来源：http://aa.szsharing.cn

Py:   s[::-1]
来源：http://mh.szxytkj.cn

PHP:  strrev($s);
来源：http://uc.bjjhwx.cn

JS:   [...s].reverse().join("")
来源：http://ce.huanxung.cn

TS:   [...s].reverse().join("")
来源：http://ym.yuexingan06.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://mv.wgjwhj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://au.jctech888.com.cn

Ruby: s.reverse
来源：http://qu.yuntaijiaju.cn

C#:   new string(s.Reverse().ToArray())
来源：http://dj.gzmigu.cn

[E12] 统计某字符出现次数
来源：http://ik.colortex.cn

Py:   s.count("a")
来源：http://tj.shxzukj.cn

PHP:  substr_count($s, "a");
来源：http://rg.jianghongdianzi.cn

JS:   s.split("a").length - 1
来源：http://pe.huixinmuqiang.cn

TS:   s.split("a").length - 1
来源：http://ja.hahajie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wm.bookmarksfly.cn

Go:   strings.Count(s, "a")
来源：http://bm.jianghongdianzi.cn

Ruby: s.count("a")
来源：http://ie.huanxung.cn

C#:   s.Count(c => c == 'a')
来源：http://aa.chemitech.net.cn

[E13] 逐字符遍历
来源：http://cw.shxzskj.cn

Py:   for ch in s: print(ch)
来源：http://qf.newstarts.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jg.szsharing.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://gd.muxihuayi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wx.yuntaijiaju.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qc.newstarts.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yf.lnxyls.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://fh.lnxyls.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://id.lnxyls.cn

[E14] URL 编码与 Base64
来源：http://yb.9csxet.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wb.newstarts.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://hy.szsharing.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fs.szsharing.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nz.huixiangedu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://az.wgjwhj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://am.hahajie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zt.panjiajie.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xd.wgjwhj.cn

[E15] HTML 转义 / 反转义
来源：http://yp.shxzskj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://nm.nszjky.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pm.colortex.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bp.9csxet.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wz.muxihuayi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://sj.colortex.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zh.asd995.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rg.asd995.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vi.newstarts.cn

[E16] 数字千分位
来源：http://sk.lnxyls.cn

Py:   f"{1234567:,}"
来源：http://eg.9csxet.cn

PHP:  number_format(1234567);
来源：http://ru.huixinmuqiang.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://jq.newstarts.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://lb.nicolike.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fy.jianghongdianzi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lj.nicolike.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pi.huixiangedu.cn

C#:   1234567.ToString("N0")
来源：http://ik.shtwfgs.cn

[E17] 首字母大写
来源：http://nu.shxzskj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nx.jianghongdianzi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://bh.muxihuayi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lu.huixinmuqiang.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dm.gzmigu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ur.nszjky.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ax.hnjuh.cn

Ruby: s.capitalize
来源：http://hw.haigaiapp.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rg.yuexingan06.cn

[E18] 模板占位符替换
来源：http://zh.nicolike.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yw.haigaiapp.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hr.asd995.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://us.hnjuh.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://sv.jctech888.com.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ye.bjjhwx.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kx.bjjhwx.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cq.wgjwhj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ex.521024.cn

[E19] 多行文本按行拆分
来源：http://nq.shxzskj.cn

Py:   s.splitlines()
来源：http://kq.shxzukj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tf.jctech888.com.cn

JS:   s.split(/\r?\n/)
来源：http://uh.huixiangedu.cn

TS:   s.split(/\r?\n/)
来源：http://pb.szsharing.cn

Java: s.lines().toList()
来源：http://yz.huanxung.cn

Go:   strings.Split(s, "\n")
来源：http://ti.wgjwhj.cn

Ruby: s.lines
来源：http://ki.shtwfgs.cn

C#:   s.Split('\n')
来源：http://ls.bjjhwx.cn

[E20] 判断字符串是否为空
来源：http://vn.colortex.cn

Py:   if not s:
来源：http://az.jianghongdianzi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vu.wgjwhj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://en.yuntaijiaju.cn

TS:   if (s === "") {}
来源：http://sc.bjjhwx.cn

Java: if (s.isEmpty()) {}
来源：http://jd.lnxyls.cn

Go:   if s == "" {}
来源：http://oh.gzmigu.cn

Ruby: if s.empty?
来源：http://tb.panjiajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://uq.szsharing.cn

[E21] 超长截断加省略号
来源：http://ob.bookmarksfly.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pe.huanxung.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zy.haigaiapp.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ca.bjjhwx.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bt.huixinmuqiang.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zl.huixinmuqiang.cn

Go:   // 按 rune 判断长度后截断
来源：http://pd.huixiangedu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fd.nszjky.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://if.jianghongdianzi.cn

[E22] 字节长度与字符长度
来源：http://nq.shtwfgs.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yn.huanxung.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ee.muxihuayi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zl.colortex.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://td.lnxyls.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://oq.colortex.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yv.yuexingan06.cn

Ruby: s.bytesize;  s.length
来源：http://hh.haigaiapp.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uc.szsharing.cn

================================================================================
来源：http://xr.panjiajie.cn

F. 文件与目录
来源：http://cd.nszjky.cn

================================================================================
来源：http://wb.gzmigu.cn

[F01] 读取整个文件
来源：http://pq.521024.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://sx.haigaiapp.cn

PHP:  file_get_contents("a.txt");
来源：http://du.521024.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ly.bjjhwx.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cg.shxzskj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jt.huanxung.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mw.yuntaijiaju.cn

Ruby: File.read("a.txt")
来源：http://cb.szsharing.cn

C#:   File.ReadAllText("a.txt");
来源：http://rs.wgjwhj.cn

[F02] 逐行读取文件
来源：http://ql.shxzukj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pl.nszjky.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qv.hnjuh.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fq.szxytkj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wt.panjiajie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pb.shtwfgs.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gz.szxytkj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bk.9csxet.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yv.chemitech.net.cn

[F03] 写入文件（覆盖）
来源：http://bp.huanxung.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cu.wgjwhj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ca.muxihuayi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ke.haigaiapp.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ih.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://in.chemitech.net.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kr.jctech888.com.cn

Ruby: File.write("a.txt", "hi")
来源：http://pf.nicolike.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cy.huixiangedu.cn

[F04] 追加写入文件
来源：http://vj.muxihuayi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nc.521024.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vn.lnxyls.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ci.asd995.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nh.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://de.yuntaijiaju.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zb.nszjky.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zy.chemitech.net.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mb.huixinmuqiang.cn

[F05] 判断文件或目录是否存在
来源：http://uf.bjjhwx.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ok.shtwfgs.cn

PHP:  file_exists("a.txt");
来源：http://pd.jianghongdianzi.cn

JS:   fs.existsSync("a.txt")
来源：http://wr.hahajie.cn

TS:   fs.existsSync("a.txt")
来源：http://os.szxytkj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ci.szxytkj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://se.nszjky.cn

Ruby: File.exist?("a.txt")
来源：http://vt.shxzskj.cn

C#:   File.Exists("a.txt")
来源：http://nl.panjiajie.cn

[F06] 删除文件
来源：http://fo.lnxyls.cn

Py:   os.remove("a.txt")
来源：http://kl.nicolike.cn

PHP:  unlink("a.txt");
来源：http://fa.yuexingan06.cn

JS:   fs.unlinkSync("a.txt")
来源：http://lk.nszjky.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fk.panjiajie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bu.yuexingan06.cn

Go:   os.Remove("a.txt")
来源：http://vk.colortex.cn

Ruby: File.delete("a.txt")
来源：http://iy.jianghongdianzi.cn

C#:   File.Delete("a.txt");
来源：http://ga.huixiangedu.cn

[F07] 创建目录（含多级）
来源：http://rv.huixiangedu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://yr.hahajie.cn


<!-- 参考信息 -->