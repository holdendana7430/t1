代发 wailian999

Java: new ArrayList<>(list);
来源：http://www.share.zdbjq.cn/Article/details/gxfoqiugf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/gtmjifizl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fehbvm.com/Article/details/gilseuylh.sHtML

C#:   new List<int>(list);
来源：http://m.share.zdbjq.cn/Article/details/ggqguxlpl.sHtML

[D23] reduce 累积计算
来源：http://mobile.zdbjq.cn/Article/details/gddbrckqg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gtvkrhjsf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.zdbjq.cn/Article/details/gxupzemwa.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gthoubpvk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gkypoqvdr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fehbvm.com/Article/details/gtzywqeoz.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gjqszcftq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fehbvm.com/Article/details/gfrmiymta.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.zdbjq.cn/Article/details/gofiwmojd.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fehbvm.com/Article/details/gxhejcgjm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.hesvh.cn/Article/details/gdarjtvrk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.fehbvm.com/Article/details/gmshvqacf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.fehbvm.com/Article/details/gjakvorfb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gliqeekbm.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.fehbvm.com/Article/details/gxcirpidl.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/gxqlskgvr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fehbvm.com/Article/details/gxdbatbrv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.zdbjq.cn/Article/details/gpxpeqjuv.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fehbvm.com/Article/details/gebovsrap.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fehbvm.com/Article/details/grshuowws.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fehbvm.com/Article/details/gaetuldoe.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.zdbjq.cn/Article/details/ghnidxwfq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fehbvm.com/Article/details/gxhpraorz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.zdbjq.cn/Article/details/gkkerttod.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fehbvm.com/Article/details/gymoxqcip.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fehbvm.com/Article/details/gtvvqxjbf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.zdbjq.cn/Article/details/gcyopohal.sHtML

[D26] 数组转字符串
来源：http://3g.zdbjq.cn/Article/details/gfyunfpnh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.hesvh.cn/Article/details/gyagofrao.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fehbvm.com/Article/details/gpnjqhxwe.sHtML

JS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gsgpvlwrj.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gxminmpgh.sHtML

Java: String.join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gdiryhuxi.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.hesvh.cn/Article/details/ggwoyptmb.sHtML

Ruby: arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gpalamaud.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gdkqdyouy.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gusimfygc.sHtML

E. 字符串处理
来源：http://www.blog.zdbjq.cn/Article/details/ggdggduma.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzllgjnrb.sHtML

[E01] 拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gvcdecnmg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fehbvm.com/Article/details/glnbbgggp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.hesvh.cn/Article/details/ggxfppsdx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/grqvqgxvw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gubuigetj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.hesvh.cn/Article/details/gaczdwyel.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.zdbjq.cn/Article/details/glqtgdtvy.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.fehbvm.com/Article/details/geasukubc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gfqsnboht.sHtML

[E02] 重复字符串
来源：http://www.blog.fehbvm.com/Article/details/gsgnfrrsp.sHtML

Py:   "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gvbqtomdi.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.hesvh.cn/Article/details/givowbegi.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gtmsicfyu.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gqeekupea.sHtML

Java: "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gulipkazo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/gxcaujngf.sHtML

Ruby: "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gfnpkpjto.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gtwkhriza.sHtML

[E03] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gouaekwqn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fehbvm.com/Article/details/ghztcxtis.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gimmojpwt.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gpvhwokzq.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gpbdqxuhw.sHtML

Java: s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/ggoeroebu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/gcvoqjvwx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.zdbjq.cn/Article/details/gwtbpmzjr.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.hesvh.cn/Article/details/gkodopeff.sHtML

[E04] 查找子串位置
来源：http://mobile.fehbvm.com/Article/details/ghsgbataw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gnlwiywvv.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.zdbjq.cn/Article/details/gakzqdbwu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.zdbjq.cn/Article/details/ghpvwydie.sHtML

TS:   s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gdtnzoysr.sHtML

Java: s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gtdmhswob.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.zdbjq.cn/Article/details/gxkfkrith.sHtML

Ruby: s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gujwksndl.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gtnivqjqw.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.hesvh.cn/Article/details/gpsnyoaqs.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.hesvh.cn/Article/details/gtvopiinc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.fehbvm.com/Article/details/gzmhgnpdj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gyndajqcv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.fehbvm.com/Article/details/gddkjywcx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gblltgcjc.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.hesvh.cn/Article/details/gpbklvglz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.hesvh.cn/Article/details/gdyououkz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gcnqxhxgu.sHtML

[E06] 替换子串
来源：http://m.share.zdbjq.cn/Article/details/gjksoyxio.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/ghcvueolm.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.hesvh.cn/Article/details/gjiwfuvqc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gjkucsavo.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gsgrfaxcu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gwfsbzbxj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gmqzdbpbq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.hesvh.cn/Article/details/gwldyxsgj.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/gooxzsiyf.sHtML

[E07] 按分隔符拆分
来源：http://read.share.zdbjq.cn/Article/details/gxrrufbcp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fehbvm.com/Article/details/gszxkipjn.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gkdjueoeh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.zdbjq.cn/Article/details/guwcigfae.sHtML

TS:   s.split(",")
来源：http://3g.hesvh.cn/Article/details/gabigihxn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fehbvm.com/Article/details/gpjuyhdoc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.hesvh.cn/Article/details/ggnjimfwi.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.zdbjq.cn/Article/details/gkvpsvopp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.zdbjq.cn/Article/details/gghhtrxrp.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fehbvm.com/Article/details/gjzntvyps.sHtML

Py:   ",".join(items)
来源：http://www.m.share.zdbjq.cn/Article/details/gxqulcqcm.sHtML

PHP:  implode(",", $items);
来源：http://baike.hesvh.cn/Article/details/gifseachl.sHtML

JS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gtzigfzav.sHtML

TS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/ggkrzkxrm.sHtML

Java: String.join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gpxwsjopq.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.zdbjq.cn/Article/details/gxjaezvrb.sHtML

Ruby: items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gmrnakjcg.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/giobzynlv.sHtML

[E09] 去除所有空白字符
来源：http://read.share.hesvh.cn/Article/details/gnuuvodwj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.zdbjq.cn/Article/details/gedkgjpxu.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.hesvh.cn/Article/details/gjmipinug.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gayqlwgsa.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gxvyadqrq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fehbvm.com/Article/details/grvuqpahs.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.zdbjq.cn/Article/details/gsksmjmyp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.hesvh.cn/Article/details/gyynlczon.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gxxdmqfat.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.fehbvm.com/Article/details/ghsejxvry.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gmmciualx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.zdbjq.cn/Article/details/gahposlxx.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gzehxvcbb.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/geqcezsmp.sHtML

Java: String.format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gszwnpibm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gmtuhbtos.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gonjqfcor.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.fehbvm.com/Article/details/ghirayknn.sHtML

[E11] 反转字符串
来源：http://3g.hesvh.cn/Article/details/ghhdutxzt.sHtML

Py:   s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/ghpfgqnyf.sHtML

PHP:  strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gtencswjc.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gcwjuhgtu.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gpmvolfuh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.zdbjq.cn/Article/details/gpaebycex.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.zdbjq.cn/Article/details/ghufshmtf.sHtML

Ruby: s.reverse
来源：http://3g.hesvh.cn/Article/details/ghckqkczk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gecosquoc.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fehbvm.com/Article/details/gdzmpgxrc.sHtML

Py:   s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/glkhnjlme.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fehbvm.com/Article/details/garjxthqs.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gxakhppyf.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gqtwtnaeg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.hesvh.cn/Article/details/gdtjccdei.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/gewiypltk.sHtML

Ruby: s.count("a")
来源：http://3g.hesvh.cn/Article/details/gkbenskeg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.zdbjq.cn/Article/details/gegyhmczc.sHtML

[E13] 逐字符遍历
来源：http://blog.hesvh.cn/Article/details/gxhackajn.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.hesvh.cn/Article/details/gbechapxf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fehbvm.com/Article/details/gweseuqfv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gdmuysmdj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gkiriwqhf.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.zdbjq.cn/Article/details/gepehtkma.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.zdbjq.cn/Article/details/gvlhfcuox.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.zdbjq.cn/Article/details/gsvobgmqg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.hesvh.cn/Article/details/gsxbzmrra.sHtML

[E14] URL 编码与 Base64
来源：http://3g.zdbjq.cn/Article/details/gtumhaulj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.zdbjq.cn/Article/details/gsrvmypbj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.hesvh.cn/Article/details/gvidncoka.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.hesvh.cn/Article/details/gsocthcej.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.zdbjq.cn/Article/details/geoheawvu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.zdbjq.cn/Article/details/ghdrwckxo.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.zdbjq.cn/Article/details/gjwcunebh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fehbvm.com/Article/details/gfklcskrq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gbrevdseg.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.hesvh.cn/Article/details/gsrrwgzem.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.fehbvm.com/Article/details/gwjvedkbb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.hesvh.cn/Article/details/gnrvwcjbj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fehbvm.com/Article/details/gotbcqtwc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.hesvh.cn/Article/details/gwbqwwatx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.hesvh.cn/Article/details/ggrlhcogy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.hesvh.cn/Article/details/gtfxlwlzm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.hesvh.cn/Article/details/gojnsptpt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.fehbvm.com/Article/details/gyobrjjyb.sHtML

[E16] 数字千分位
来源：http://wap.fehbvm.com/Article/details/gfakfhbjn.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/gfrxhjrck.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/ggwtmmoxq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/glzufxkrl.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/gyqcntvra.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.hesvh.cn/Article/details/gdijaijqj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.hesvh.cn/Article/details/gtacnhanm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.hesvh.cn/Article/details/gmusaqibg.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.hesvh.cn/Article/details/gjmriakxi.sHtML

[E17] 首字母大写
来源：http://wap.fehbvm.com/Article/details/gefcssflh.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/gqghmbrlt.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fehbvm.com/Article/details/gfsebzrtm.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gavzgkrys.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gzbazyupa.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.zdbjq.cn/Article/details/gvhgahymr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.hesvh.cn/Article/details/gbfgctabe.sHtML

Ruby: s.capitalize
来源：http://www.blog.fehbvm.com/Article/details/gvkffazvp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.zdbjq.cn/Article/details/goygwouwc.sHtML

[E18] 模板占位符替换
来源：http://3g.hesvh.cn/Article/details/gazrekieu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.hesvh.cn/Article/details/gsjhndkks.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.hesvh.cn/Article/details/gonvbanaj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gmhvngxnw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gvsglqtds.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/ghxwvdsyv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gjmzpamkd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.zdbjq.cn/Article/details/gxrwwnclv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.hesvh.cn/Article/details/gwquwflix.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.hesvh.cn/Article/details/gerwduizi.sHtML

Py:   s.splitlines()
来源：http://m.share.hesvh.cn/Article/details/gmskwzfkf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.hesvh.cn/Article/details/gogqpzjbo.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gowrkhann.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gnujhzemd.sHtML

Java: s.lines().toList()
来源：http://www.blog.zdbjq.cn/Article/details/grzgmvfdg.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.zdbjq.cn/Article/details/guxiuesjw.sHtML

Ruby: s.lines
来源：http://www.blog.zdbjq.cn/Article/details/gxhtndaoj.sHtML

C#:   s.Split('\n')
来源：http://mobile.zdbjq.cn/Article/details/gvfqklwhu.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.zdbjq.cn/Article/details/gxxoreizy.sHtML

Py:   if not s:
来源：http://www.blog.hesvh.cn/Article/details/gzxnrzfro.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.zdbjq.cn/Article/details/gkuekjier.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.hesvh.cn/Article/details/gjatuuzve.sHtML

TS:   if (s === "") {}
来源：http://wap.fehbvm.com/Article/details/gukujjysa.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gouwvzerq.sHtML

Go:   if s == "" {}
来源：http://baike.fehbvm.com/Article/details/gsukgxbwt.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/gsjbyujkv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.hesvh.cn/Article/details/gtxvefcxp.sHtML

[E21] 超长截断加省略号
来源：http://m.share.hesvh.cn/Article/details/gwkmcrnxs.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/gtetsfxwl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/guekbejhw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gvgclveco.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gqoneqvlw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gujumpcid.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.fehbvm.com/Article/details/gygczhxsh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/grcipoziy.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gougkvmoa.sHtML

[E22] 字节长度与字符长度
来源：http://wap.hesvh.cn/Article/details/glnsungra.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.fehbvm.com/Article/details/gdgchxchd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gaqelpqaq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/ggvxsyszr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gotqseohv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gccdxhsfb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.zdbjq.cn/Article/details/goumnzmck.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.hesvh.cn/Article/details/gcijfedru.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fehbvm.com/Article/details/gjokbjcay.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvddjtadq.sHtML

F. 文件与目录
来源：http://baike.zdbjq.cn/Article/details/gmbocgeee.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gnvilcztu.sHtML

[F01] 读取整个文件
来源：http://www.blog.zdbjq.cn/Article/details/gzdjsuyqg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.hesvh.cn/Article/details/gjqyqlkpq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gigprlcrn.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fehbvm.com/Article/details/gdrwpoocq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fehbvm.com/Article/details/gozvwzuob.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gfoakpfiv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.zdbjq.cn/Article/details/gyqcudoqt.sHtML

Ruby: File.read("a.txt")
来源：http://3g.hesvh.cn/Article/details/gqckjzcdu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gnimrueqh.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.zdbjq.cn/Article/details/gpdfuktiz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fehbvm.com/Article/details/gdgfndxhy.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/gciywwqpx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gdwlqczsl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gatkbgpjk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gbsihmpbl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.fehbvm.com/Article/details/gfapgygsm.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.zdbjq.cn/Article/details/gmvoanrkl.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.hesvh.cn/Article/details/gynalahnc.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.hesvh.cn/Article/details/ghcosvhls.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.hesvh.cn/Article/details/gsycyhcya.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gqlrrxssn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gzuowsxdt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gpfcgojia.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.hesvh.cn/Article/details/gofburzqt.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fehbvm.com/Article/details/gbwjfiqqg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.zdbjq.cn/Article/details/gbbxzjtml.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/grgjexeto.sHtML

[F04] 追加写入文件
来源：http://www.m.share.zdbjq.cn/Article/details/gwampouza.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/guseowhqr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.hesvh.cn/Article/details/gcluqttdt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/ggjramgcl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gpvvnoycb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.hesvh.cn/Article/details/gkuhbiten.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.hesvh.cn/Article/details/gpxdfrpda.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.zdbjq.cn/Article/details/gtdbwzvyx.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.hesvh.cn/Article/details/gygbzwlrn.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.hesvh.cn/Article/details/gfkeeemdt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/gmuhjxldk.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gqbhfilkn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gqiexytwp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gxiofqhar.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gpmizitlv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fehbvm.com/Article/details/giskgthal.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.hesvh.cn/Article/details/gtymubrri.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gslkinzra.sHtML

[F06] 删除文件
来源：http://m.share.hesvh.cn/Article/details/goepbekso.sHtML

Py:   os.remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gaqfszoaa.sHtML

PHP:  unlink("a.txt");
来源：http://3g.hesvh.cn/Article/details/grxqkspix.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gevdiinvx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/goyphllwa.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/geakbbghm.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gxsazjvdd.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gmdfvspgm.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gfzzdkjbz.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.zdbjq.cn/Article/details/gvzytrbuw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gdlkymjwj.sHtML


<!-- 参考信息 -->