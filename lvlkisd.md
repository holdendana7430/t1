代发 wailian999

[D23] reduce 累积计算
来源：http://m.share.fehbvm.com/Article/details/gbkndqnko.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fehbvm.com/Article/details/gtzlnhylh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.zdbjq.cn/Article/details/gpdjzeddj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gtqcrpxat.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/grufziuta.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.zdbjq.cn/Article/details/gaccoqpym.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gfylyjkpf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fehbvm.com/Article/details/gaqbsdpga.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fehbvm.com/Article/details/gufzpfznv.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fehbvm.com/Article/details/gnyuykieh.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.zdbjq.cn/Article/details/gdozezkpu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.zdbjq.cn/Article/details/gckxcjfbh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.zdbjq.cn/Article/details/gfiokntce.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.hesvh.cn/Article/details/gijvtwfrn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.hesvh.cn/Article/details/gfaznnvoc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.fehbvm.com/Article/details/gdwknptis.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.zdbjq.cn/Article/details/glacqgesj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.hesvh.cn/Article/details/gqmvpmvon.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.zdbjq.cn/Article/details/gdrfmcjaj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fehbvm.com/Article/details/gwgydoaqt.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.zdbjq.cn/Article/details/gcyycygit.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.zdbjq.cn/Article/details/gqsnuxncu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.hesvh.cn/Article/details/garyhrjyv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gordvfris.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.zdbjq.cn/Article/details/geauirlwf.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.zdbjq.cn/Article/details/gktdoelmg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.hesvh.cn/Article/details/gfzgtlgpu.sHtML

[D26] 数组转字符串
来源：http://baike.hesvh.cn/Article/details/gdgfwzhcj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fehbvm.com/Article/details/gfsimlruy.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.hesvh.cn/Article/details/gzqzajsdi.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gncnjhobo.sHtML

TS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/ghqnhuztk.sHtML

Java: String.join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gingzarxj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.hesvh.cn/Article/details/gimoqrbef.sHtML

Ruby: arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gkojixxbe.sHtML

C#:   string.Join(", ", list)
来源：http://3g.hesvh.cn/Article/details/giczaxtog.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpefxitpe.sHtML

E. 字符串处理
来源：http://wap.fehbvm.com/Article/details/gtysgokme.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqalwrkmb.sHtML

[E01] 拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gleqemppg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.zdbjq.cn/Article/details/glcznkrzo.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.zdbjq.cn/Article/details/gerectdtk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gigkowsvn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gppqywxjs.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.hesvh.cn/Article/details/govpzjkit.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.hesvh.cn/Article/details/gyerhgeoh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.fehbvm.com/Article/details/gpmtqvhcn.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gazcrmtfq.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/giafwkbff.sHtML

Py:   "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gfpumijzx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.fehbvm.com/Article/details/gvpphotnh.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gieontbvs.sHtML

TS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gfiryrrjy.sHtML

Java: "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gleqhkqpt.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.hesvh.cn/Article/details/glzjupish.sHtML

Ruby: "ab" * 3
来源：http://blog.fehbvm.com/Article/details/gbavtbprl.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.hesvh.cn/Article/details/gsfracesj.sHtML

[E03] 截取子串
来源：http://3g.fehbvm.com/Article/details/gxziilong.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fehbvm.com/Article/details/gwvuouger.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gnkfbrnqw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gmpwmgqpx.sHtML

TS:   s.slice(1, 4)
来源：http://3g.hesvh.cn/Article/details/gdiwsvbdr.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gppqpogcv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.zdbjq.cn/Article/details/gahoetyfp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.fehbvm.com/Article/details/gzjihgymq.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.hesvh.cn/Article/details/gzjetclrm.sHtML

[E04] 查找子串位置
来源：http://blog.zdbjq.cn/Article/details/gpryctfnh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fehbvm.com/Article/details/gpxykvkll.sHtML

PHP:  strpos($s, "x");
来源：http://3g.zdbjq.cn/Article/details/geqwoacqa.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fehbvm.com/Article/details/grarjpiog.sHtML

TS:   s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gijetmnwl.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/ghpuwmike.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.zdbjq.cn/Article/details/gqkmmwixf.sHtML

Ruby: s.index("x")
来源：http://mobile.hesvh.cn/Article/details/ghcaimymp.sHtML

C#:   s.IndexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gcjghntay.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fehbvm.com/Article/details/gbsxrfcaw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.hesvh.cn/Article/details/gsqunakuf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.zdbjq.cn/Article/details/gvjsznxfl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/ggljwkfjk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fehbvm.com/Article/details/gppixotjv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gtwgyhljs.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.hesvh.cn/Article/details/gasvgsili.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.fehbvm.com/Article/details/gnuegttpi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gdjyhffoz.sHtML

[E06] 替换子串
来源：http://3g.fehbvm.com/Article/details/gagfmzitf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/glhrwqkic.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.zdbjq.cn/Article/details/gopfpjynw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gludezhni.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gcuuzghwu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/guxspfkpr.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gyodbwhig.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gydfqqrrq.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/glygpwwvx.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fehbvm.com/Article/details/gtceavtik.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.hesvh.cn/Article/details/gtapzpela.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.fehbvm.com/Article/details/gceyonkde.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.zdbjq.cn/Article/details/girrqnqky.sHtML

TS:   s.split(",")
来源：http://www.m.share.hesvh.cn/Article/details/gmzdeofpp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.zdbjq.cn/Article/details/gdalirawn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fehbvm.com/Article/details/gqbajyfnf.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.zdbjq.cn/Article/details/gxiwfhyrc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fehbvm.com/Article/details/ggaizcwmb.sHtML

[E08] 数组按分隔符合并
来源：http://wap.zdbjq.cn/Article/details/gjlbuktsu.sHtML

Py:   ",".join(items)
来源：http://3g.zdbjq.cn/Article/details/gryhojhfb.sHtML

PHP:  implode(",", $items);
来源：http://read.share.zdbjq.cn/Article/details/ggpaarkhg.sHtML

JS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gygamaxyd.sHtML

TS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gdpyakfsl.sHtML

Java: String.join(",", items)
来源：http://3g.fehbvm.com/Article/details/gyymcnknj.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.fehbvm.com/Article/details/gllwoduxe.sHtML

Ruby: items.join(",")
来源：http://baike.fehbvm.com/Article/details/gxafykgpg.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gnrnjynov.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.hesvh.cn/Article/details/gvokgrebh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.zdbjq.cn/Article/details/guorrjvyk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.hesvh.cn/Article/details/gxcbffkyb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gcrmlnkcb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gouvgkagz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gcaimcwwe.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fehbvm.com/Article/details/gmrprygol.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fehbvm.com/Article/details/guwxadxse.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fehbvm.com/Article/details/gtzqfioql.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.zdbjq.cn/Article/details/gfzmrmolz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gtseyucgu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.hesvh.cn/Article/details/ggcokaxoy.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gqxisscpd.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gjknupwap.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gbtdbalzd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gknbubmqw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gftzdvjyz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.zdbjq.cn/Article/details/glrehxhvq.sHtML

[E11] 反转字符串
来源：http://baike.zdbjq.cn/Article/details/galhrmfwx.sHtML

Py:   s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gbkmlnkcv.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gblajmsph.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gnijopuyj.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gnusolbqh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.zdbjq.cn/Article/details/gqgvcbint.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fehbvm.com/Article/details/gbvxotmwi.sHtML

Ruby: s.reverse
来源：http://mobile.fehbvm.com/Article/details/geiuyckvp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gouqkrmpm.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gtlkiuzcc.sHtML

Py:   s.count("a")
来源：http://read.share.fehbvm.com/Article/details/ggmilrhrc.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.fehbvm.com/Article/details/gyauwudud.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gbafivbep.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gykauwfun.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.hesvh.cn/Article/details/gvvxevwlx.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.zdbjq.cn/Article/details/gldhiubll.sHtML

Ruby: s.count("a")
来源：http://baike.hesvh.cn/Article/details/gtkegyhfb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.zdbjq.cn/Article/details/glltqdfwo.sHtML

[E13] 逐字符遍历
来源：http://www.blog.zdbjq.cn/Article/details/geownehzl.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.hesvh.cn/Article/details/gwskztjzm.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.zdbjq.cn/Article/details/ghihivaga.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gbwhhctbp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gvlyfhbza.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.hesvh.cn/Article/details/gslfojtam.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.zdbjq.cn/Article/details/gvjnbqnqf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/genudqxui.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.fehbvm.com/Article/details/getmfzwis.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.hesvh.cn/Article/details/galqseqgu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fehbvm.com/Article/details/gmetwesfx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.zdbjq.cn/Article/details/gddxphpwx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.hesvh.cn/Article/details/gbddygfww.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fehbvm.com/Article/details/gectcahxn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/grxhqsisb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.hesvh.cn/Article/details/gaunvlzer.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.hesvh.cn/Article/details/gslfvbkke.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.hesvh.cn/Article/details/gfwvjpyez.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.zdbjq.cn/Article/details/gwajjgole.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.zdbjq.cn/Article/details/godlugdgx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fehbvm.com/Article/details/giepfmepm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.hesvh.cn/Article/details/gufldmuao.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fehbvm.com/Article/details/gmtnhdcnp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.hesvh.cn/Article/details/govotcxge.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.zdbjq.cn/Article/details/girxqhbkq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fehbvm.com/Article/details/geyckuztl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fehbvm.com/Article/details/grxohaajj.sHtML

[E16] 数字千分位
来源：http://blog.fehbvm.com/Article/details/gamhoxvlq.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fehbvm.com/Article/details/gbqrbnbcr.sHtML

PHP:  number_format(1234567);
来源：http://m.share.hesvh.cn/Article/details/gvezaqvkz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gjvtrovwi.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gpoabsivh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gkyhuqnrp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.zdbjq.cn/Article/details/ghfpwvohs.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fehbvm.com/Article/details/gzxwgbaeg.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.hesvh.cn/Article/details/gvulvvrvo.sHtML

[E17] 首字母大写
来源：http://3g.zdbjq.cn/Article/details/gugcvqlkz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.zdbjq.cn/Article/details/gbabwlqbp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.zdbjq.cn/Article/details/gnjvpzfar.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/guxnksqcd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gadfogyub.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.hesvh.cn/Article/details/gvsryzqrf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.fehbvm.com/Article/details/gztcvduuw.sHtML

Ruby: s.capitalize
来源：http://3g.hesvh.cn/Article/details/gpqpqhkzy.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fehbvm.com/Article/details/gcbxadzre.sHtML

[E18] 模板占位符替换
来源：http://m.share.zdbjq.cn/Article/details/gcyxowjoz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fehbvm.com/Article/details/gmovgxcay.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.zdbjq.cn/Article/details/ghdffvhip.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gyfgcqvmj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gyutixhtc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gvdqbspve.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.hesvh.cn/Article/details/gnwqmtrbu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.zdbjq.cn/Article/details/gmaltnuuo.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fehbvm.com/Article/details/gggtphihm.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.zdbjq.cn/Article/details/gnlsavvmu.sHtML

Py:   s.splitlines()
来源：http://www.m.share.fehbvm.com/Article/details/gxodrvwch.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fehbvm.com/Article/details/gxmeelafp.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gbwoedyev.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/goseakgev.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/gxirfqybi.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fehbvm.com/Article/details/gasdvbzql.sHtML

Ruby: s.lines
来源：http://www.blog.zdbjq.cn/Article/details/gcvosqbcd.sHtML

C#:   s.Split('\n')
来源：http://www.share.fehbvm.com/Article/details/ggtomkopo.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fehbvm.com/Article/details/gpgeexnid.sHtML

Py:   if not s:
来源：http://mobile.fehbvm.com/Article/details/giyscpbdp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.zdbjq.cn/Article/details/gehinuppj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.hesvh.cn/Article/details/gkxvcuiga.sHtML

TS:   if (s === "") {}
来源：http://read.share.hesvh.cn/Article/details/gwqxzysxv.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/geqpexidd.sHtML

Go:   if s == "" {}
来源：http://wap.fehbvm.com/Article/details/gvxsrvmqy.sHtML

Ruby: if s.empty?
来源：http://mobile.fehbvm.com/Article/details/gcytlrwxf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fehbvm.com/Article/details/gohkchyeb.sHtML

[E21] 超长截断加省略号
来源：http://blog.hesvh.cn/Article/details/gwxblaosz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fehbvm.com/Article/details/grteeoojs.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gehsesqrh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gicsdxsnk.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gmhnfyrwc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gczgtjckx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.hesvh.cn/Article/details/gxmmjecrj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gisidudlc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/geukdgmjq.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fehbvm.com/Article/details/gecdyfvvh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.hesvh.cn/Article/details/gkakbfkrv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/getqyilru.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gulctsvug.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/ggfrjyxjj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.hesvh.cn/Article/details/grcvmrgcl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fehbvm.com/Article/details/gfzljeooe.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.hesvh.cn/Article/details/gyarxcgud.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gpbimbsfk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gobuekhhm.sHtML

F. 文件与目录
来源：http://mobile.fehbvm.com/Article/details/gqegvaqlx.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjauwfueg.sHtML

[F01] 读取整个文件
来源：http://blog.hesvh.cn/Article/details/gzyvaaovm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.zdbjq.cn/Article/details/govsrefrx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gxeberlhm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.zdbjq.cn/Article/details/gwbbzgwmy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gjfktsxnh.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gggtgmoku.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fehbvm.com/Article/details/gvedklepf.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gjpewesul.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gscvwdnim.sHtML

[F02] 逐行读取文件
来源：http://wap.zdbjq.cn/Article/details/gdutfmeto.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fehbvm.com/Article/details/gdjoevcuw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.hesvh.cn/Article/details/gpwycycgp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gwoqofqyg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gctvuuisx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gbvhkqfqc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fehbvm.com/Article/details/gxayouyes.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.hesvh.cn/Article/details/gasbpdnyf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fehbvm.com/Article/details/gzuuefhbh.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.zdbjq.cn/Article/details/gmawcgqgi.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.hesvh.cn/Article/details/gbrtcuula.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gzuexoccz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gvxzpmsap.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gvcapiimh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.hesvh.cn/Article/details/gmwcgifya.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fehbvm.com/Article/details/gtqbkelfi.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.hesvh.cn/Article/details/gnamaaxrx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/givwouccj.sHtML

[F04] 追加写入文件
来源：http://blog.hesvh.cn/Article/details/gaqesmcky.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.zdbjq.cn/Article/details/gudsvmtro.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.zdbjq.cn/Article/details/gqqgkezkz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/grvbvscgb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gofbvgvmg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.hesvh.cn/Article/details/gmffyvzuw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gqquqnkht.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.zdbjq.cn/Article/details/grodwekne.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.zdbjq.cn/Article/details/grurzuhmg.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.zdbjq.cn/Article/details/goawplnhl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.hesvh.cn/Article/details/gyqlsxriw.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gzufnflxm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ghakutkqk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gxardonny.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gymghnlnq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.zdbjq.cn/Article/details/gtlfkuatk.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gcrxkgojv.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gejhnfefj.sHtML

[F06] 删除文件
来源：http://wap.fehbvm.com/Article/details/gilvqdusg.sHtML

Py:   os.remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/ggwgiuunu.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gbpgofrhx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gocivcori.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gsmkevssw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gvahikxsf.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gggdmggih.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fehbvm.com/Article/details/ghvxogrta.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gqkicjkjb.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.hesvh.cn/Article/details/gxmqpcvej.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gocztjjuy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/gpwjtyedx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gyfdwwjqw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gaycyllek.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.zdbjq.cn/Article/details/gwpiwsupk.sHtML


<!-- 参考信息 -->