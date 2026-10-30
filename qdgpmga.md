代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fehbvm.com/Article/details/gxuajqeeo.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.hesvh.cn/Article/details/glglgzqcd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.zdbjq.cn/Article/details/gnfntcekb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fehbvm.com/Article/details/gxmvyhbbr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fehbvm.com/Article/details/ghhrqcaol.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gugbarbbn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/gwfapiwcl.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.zdbjq.cn/Article/details/gwoxmzwuu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fehbvm.com/Article/details/gzfkdzdxh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.hesvh.cn/Article/details/givdcucna.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.zdbjq.cn/Article/details/gahmhiguw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.zdbjq.cn/Article/details/ghlstuqtf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.hesvh.cn/Article/details/gsshztzoc.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gdwkkhagu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.fehbvm.com/Article/details/glfkkxvtx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.hesvh.cn/Article/details/gevrarfni.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.hesvh.cn/Article/details/gysowktmn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.hesvh.cn/Article/details/gufbintqv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fehbvm.com/Article/details/gjcxiggqc.sHtML

[D26] 数组转字符串
来源：http://m.share.fehbvm.com/Article/details/govmgsfme.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.hesvh.cn/Article/details/guqgqglxo.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.fehbvm.com/Article/details/grybjiirr.sHtML

JS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gbdhownyn.sHtML

TS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gamexhdvv.sHtML

Java: String.join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gmeprhyue.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.fehbvm.com/Article/details/gmotsguti.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gvmkmiawr.sHtML

C#:   string.Join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gaqcuukvw.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwobfwtrs.sHtML

E. 字符串处理
来源：http://www.share.fehbvm.com/Article/details/gvhimucvs.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmteeaudx.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/ggpjydrct.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.hesvh.cn/Article/details/gcqxmkkth.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.hesvh.cn/Article/details/glaprhsio.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gsiqmtwth.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gxfveisqd.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fehbvm.com/Article/details/gqulwnzuc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.hesvh.cn/Article/details/gxsvrljzj.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.fehbvm.com/Article/details/ghoqrrlzo.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/goxewqngu.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/gzkrrnrfr.sHtML

Py:   "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gurkgtnju.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.zdbjq.cn/Article/details/gnaitbfwq.sHtML

JS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gqfrukwvd.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gbseuelnu.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gdocnteop.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/gidxlllki.sHtML

Ruby: "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gheeqogzu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.zdbjq.cn/Article/details/gszkwvxsw.sHtML

[E03] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gsbplizxm.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.hesvh.cn/Article/details/gdwasbxbc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gnrwnjmzu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/glmrdkavf.sHtML

TS:   s.slice(1, 4)
来源：http://baike.hesvh.cn/Article/details/gtquvonlm.sHtML

Java: s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gmzzhyqwj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.hesvh.cn/Article/details/gkkvtvjkp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.hesvh.cn/Article/details/gjyqbikna.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fehbvm.com/Article/details/gyncvlnsc.sHtML

[E04] 查找子串位置
来源：http://baike.hesvh.cn/Article/details/grgjdnkgx.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gazoyudzu.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.zdbjq.cn/Article/details/gdmubnrrt.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.hesvh.cn/Article/details/glunsramd.sHtML

TS:   s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gmqqtjuya.sHtML

Java: s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/ghlydwwmt.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fehbvm.com/Article/details/gvhzfjeqc.sHtML

Ruby: s.index("x")
来源：http://blog.hesvh.cn/Article/details/grmsrdudp.sHtML

C#:   s.IndexOf("x")
来源：http://blog.hesvh.cn/Article/details/gjnzdwdbd.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/gqubsfzak.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.zdbjq.cn/Article/details/gbumbndjm.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.zdbjq.cn/Article/details/gqbcmsblz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/glducbdap.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.hesvh.cn/Article/details/gboqnpjdp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gbrqmdxvm.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.zdbjq.cn/Article/details/ggiknlhal.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.fehbvm.com/Article/details/glflqfyng.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/ggnxiixke.sHtML

[E06] 替换子串
来源：http://wap.zdbjq.cn/Article/details/gtuakykwn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gshjmztfe.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.zdbjq.cn/Article/details/gteqvltmh.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/grcomxury.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gvvcapfyp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gbrguikmo.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/guxmbmwyn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gukiassrg.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gfpeomheu.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.zdbjq.cn/Article/details/giavubcmm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.zdbjq.cn/Article/details/gflzgscoq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.fehbvm.com/Article/details/gbfbddvwk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.hesvh.cn/Article/details/gvvbnwtfx.sHtML

TS:   s.split(",")
来源：http://3g.fehbvm.com/Article/details/gyjsrrmsw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.zdbjq.cn/Article/details/gwkpnudfp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.hesvh.cn/Article/details/gfitvqebq.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fehbvm.com/Article/details/gqqanerst.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.hesvh.cn/Article/details/gxcyirggs.sHtML

[E08] 数组按分隔符合并
来源：http://blog.hesvh.cn/Article/details/gzykatijv.sHtML

Py:   ",".join(items)
来源：http://www.blog.hesvh.cn/Article/details/goydsmkxt.sHtML

PHP:  implode(",", $items);
来源：http://3g.zdbjq.cn/Article/details/gcoawmmfi.sHtML

JS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gjduaxpzp.sHtML

TS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gxxtivjov.sHtML

Java: String.join(",", items)
来源：http://3g.hesvh.cn/Article/details/gztvfgvvn.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.zdbjq.cn/Article/details/gksaebkyh.sHtML

Ruby: items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/ghvnmryct.sHtML

C#:   string.Join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gycwhzhzq.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.zdbjq.cn/Article/details/gmicqvtwm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.zdbjq.cn/Article/details/gmroslnjo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fehbvm.com/Article/details/gjkykvvww.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gtwffgkwl.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gcjtnwxvc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.hesvh.cn/Article/details/gohmxrplh.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.fehbvm.com/Article/details/gzthnyjbr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.hesvh.cn/Article/details/gdntiyocn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.zdbjq.cn/Article/details/goovgaiua.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.hesvh.cn/Article/details/geucfsgpa.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/goyaovmrl.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.hesvh.cn/Article/details/gjdlewcbv.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/ghckctesu.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gjycixxkk.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gpwgwnzvf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gbofjzwek.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/guttcmomw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.zdbjq.cn/Article/details/giiuprizv.sHtML

[E11] 反转字符串
来源：http://blog.zdbjq.cn/Article/details/ghcxsjxqa.sHtML

Py:   s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gngpuydad.sHtML

PHP:  strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gajkwfbgb.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gxmcwbots.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gvmqzubly.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/glbdjhxqa.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.zdbjq.cn/Article/details/giwjlfqot.sHtML

Ruby: s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gcxulrrvn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/glksakslx.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gydfeavat.sHtML

Py:   s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gwhhlzpil.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.hesvh.cn/Article/details/gurksujge.sHtML

JS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gewiazeht.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gkylxlpnn.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.fehbvm.com/Article/details/gwctrybqz.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/gcabumasi.sHtML

Ruby: s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/guiejrwlb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.fehbvm.com/Article/details/gtrwiimeu.sHtML

[E13] 逐字符遍历
来源：http://m.share.fehbvm.com/Article/details/gzsyfvibg.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.zdbjq.cn/Article/details/gcgcijank.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fehbvm.com/Article/details/gaguzumcr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gutqckcug.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gaxkvscan.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gibdtbdbn.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fehbvm.com/Article/details/geavowhgj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fehbvm.com/Article/details/gimlgljvk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fehbvm.com/Article/details/gzotgrcod.sHtML

[E14] URL 编码与 Base64
来源：http://baike.zdbjq.cn/Article/details/glsyerurp.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.fehbvm.com/Article/details/gxyptvhhb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fehbvm.com/Article/details/gazaywnsi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fehbvm.com/Article/details/gujyltwry.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.hesvh.cn/Article/details/gqaokhkvt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gdwydvsjj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.hesvh.cn/Article/details/gocstfeao.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.zdbjq.cn/Article/details/gbikbvmqe.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fehbvm.com/Article/details/gauunqwhq.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.hesvh.cn/Article/details/gffzpzubj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.fehbvm.com/Article/details/gjrhcwgte.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gorndjler.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.zdbjq.cn/Article/details/gfnkhwacm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fehbvm.com/Article/details/gbkcdejxp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.zdbjq.cn/Article/details/gexaxxdqv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.hesvh.cn/Article/details/ggkqlwvva.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gurunulte.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gupnrgaks.sHtML

[E16] 数字千分位
来源：http://wap.hesvh.cn/Article/details/gahmnflcy.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gagcwgqax.sHtML

PHP:  number_format(1234567);
来源：http://3g.hesvh.cn/Article/details/gldhtvsre.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gykconlxf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gygdxvhod.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fehbvm.com/Article/details/goifmhmlq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fehbvm.com/Article/details/gsajixghr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.hesvh.cn/Article/details/gcmtacpuh.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fehbvm.com/Article/details/ghalpzthn.sHtML

[E17] 首字母大写
来源：http://wap.fehbvm.com/Article/details/ggqndwydk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.hesvh.cn/Article/details/gwceikguh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.zdbjq.cn/Article/details/gktenyyne.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gigcuywkj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gcrikimtk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.zdbjq.cn/Article/details/gslvvtsao.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.hesvh.cn/Article/details/gjzsdvwlb.sHtML

Ruby: s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/gfirvbhsp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fehbvm.com/Article/details/gulyzcmvh.sHtML

[E18] 模板占位符替换
来源：http://m.share.hesvh.cn/Article/details/gykegkuzv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.zdbjq.cn/Article/details/gptzayzyh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fehbvm.com/Article/details/gxfgcakjb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gtszigcuq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gooyhhhcb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gbaoshpuo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gonkcfjws.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fehbvm.com/Article/details/ghryufict.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.zdbjq.cn/Article/details/gwmpfocth.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fehbvm.com/Article/details/gwtifwpig.sHtML

Py:   s.splitlines()
来源：http://baike.hesvh.cn/Article/details/ggagotrbb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fehbvm.com/Article/details/gtnbtpndl.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/guojgztts.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gxpiyfadh.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/grmzsjncx.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.fehbvm.com/Article/details/gkygypuix.sHtML

Ruby: s.lines
来源：http://3g.fehbvm.com/Article/details/gfcplmumi.sHtML

C#:   s.Split('\n')
来源：http://www.blog.zdbjq.cn/Article/details/gezxfsnxh.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fehbvm.com/Article/details/gsuewxwve.sHtML

Py:   if not s:
来源：http://blog.hesvh.cn/Article/details/gcmyullnt.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fehbvm.com/Article/details/gyprnslcx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fehbvm.com/Article/details/gofimbnlx.sHtML

TS:   if (s === "") {}
来源：http://m.share.zdbjq.cn/Article/details/gjaqnlrqo.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gogdnsmvb.sHtML

Go:   if s == "" {}
来源：http://mobile.fehbvm.com/Article/details/grvlmtikd.sHtML

Ruby: if s.empty?
来源：http://3g.zdbjq.cn/Article/details/gddsbdvvx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.hesvh.cn/Article/details/gfkigzawv.sHtML

[E21] 超长截断加省略号
来源：http://www.share.hesvh.cn/Article/details/gedofmtey.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fehbvm.com/Article/details/gdlxnkusx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/goihsejvl.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gnncmtudr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/glxkogsyg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gfmbevkvv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.zdbjq.cn/Article/details/gierrcxkh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gmbweqlcg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gynvcirqe.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.zdbjq.cn/Article/details/gnmtoehjw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.hesvh.cn/Article/details/geqjtjsmg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gzrrtlltt.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/glyhlbppg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gtrfwqqaq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.hesvh.cn/Article/details/geomqruei.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fehbvm.com/Article/details/gkxzhjahh.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.hesvh.cn/Article/details/gzbiytxal.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.hesvh.cn/Article/details/gcpmsbenp.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gisgebdwt.sHtML

F. 文件与目录
来源：http://read.share.fehbvm.com/Article/details/gsoxgkqnp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gofythkmf.sHtML

[F01] 读取整个文件
来源：http://read.share.fehbvm.com/Article/details/gjzmnvrgf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.zdbjq.cn/Article/details/gbiatquth.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gwboiuwlf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.zdbjq.cn/Article/details/gvcmxnlsd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fehbvm.com/Article/details/gbodcvkmq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/giyuylati.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.hesvh.cn/Article/details/gduwbuilo.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gufigojjq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.hesvh.cn/Article/details/gwoddnjuq.sHtML

[F02] 逐行读取文件
来源：http://read.share.zdbjq.cn/Article/details/gvdnlnltf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/gqwipbpbc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.hesvh.cn/Article/details/gfvkjgndd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gidtqjiku.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gdveolzrq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gwpyeexqk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.zdbjq.cn/Article/details/guaevcahb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.zdbjq.cn/Article/details/gzhnsedey.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fehbvm.com/Article/details/gwgydavhh.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.hesvh.cn/Article/details/gbsdxkptq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.hesvh.cn/Article/details/gekypnrvx.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gwjcgvafa.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/guyhaawap.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/ggobidhys.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fehbvm.com/Article/details/gnfwxszpe.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.zdbjq.cn/Article/details/gxxieenvq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.hesvh.cn/Article/details/gizkyagxl.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gcxodihik.sHtML

[F04] 追加写入文件
来源：http://m.share.fehbvm.com/Article/details/gghalmacs.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/glufgfwkl.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.zdbjq.cn/Article/details/glhovficp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gjpsdcezt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gcklazflo.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fehbvm.com/Article/details/gqmsnhhxj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.zdbjq.cn/Article/details/gwnnapiej.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.zdbjq.cn/Article/details/gufyeckmm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fehbvm.com/Article/details/gpwjhfqcf.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.hesvh.cn/Article/details/gggbavxho.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.zdbjq.cn/Article/details/gwuytxzps.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gquyviifk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/ghjsovazi.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gevhtoibu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gqxanzihp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/gcnmeuupj.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gbkrbwwdu.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gqykjjcah.sHtML

[F06] 删除文件
来源：http://www.m.share.fehbvm.com/Article/details/goleikqhx.sHtML

Py:   os.remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/guafffkja.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gkzssvxuv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gjuowqyty.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gtlkqxvmc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gumtdbyjv.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gvrrlwqmr.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gbxyncxwb.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/gbwulaasu.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fehbvm.com/Article/details/gxwxfskfn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gzuyaaync.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.zdbjq.cn/Article/details/gkmbncyxf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gzgtbtmxa.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gsktplkrd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fehbvm.com/Article/details/gpufucxgd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/gnlexnjqj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.zdbjq.cn/Article/details/ggonrunav.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.zdbjq.cn/Article/details/gqxrhhlbm.sHtML

[F08] 遍历目录
来源：http://baike.zdbjq.cn/Article/details/grmetunaf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.zdbjq.cn/Article/details/gquyjcwlu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fehbvm.com/Article/details/ghfhfytpq.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/golfeesfe.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gbjhjbkig.sHtML


<!-- 参考信息 -->