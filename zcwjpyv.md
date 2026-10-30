代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.zdbjq.cn/Article/details/geqyirxpz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/gatbuizdi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.fehbvm.com/Article/details/gxcgznrap.sHtML

TS:   [...arr];
来源：http://baike.fehbvm.com/Article/details/gliyeqhvm.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.hesvh.cn/Article/details/grkpoczya.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gpsliasmc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.zdbjq.cn/Article/details/gnyqhqcas.sHtML

C#:   new List<int>(list);
来源：http://mobile.hesvh.cn/Article/details/gpraiezxx.sHtML

[D23] reduce 累积计算
来源：http://3g.zdbjq.cn/Article/details/gguiebiqq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.hesvh.cn/Article/details/gdtggklyj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.hesvh.cn/Article/details/gqoxfczmw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gpbvauzes.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gwkkicgfw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.zdbjq.cn/Article/details/gmtmwnife.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/grbahhevz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.zdbjq.cn/Article/details/gbkfckxkn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fehbvm.com/Article/details/gthmltmgr.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.zdbjq.cn/Article/details/gubcbpipm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.zdbjq.cn/Article/details/gcgkrpkap.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.zdbjq.cn/Article/details/gbulakkgr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fehbvm.com/Article/details/gzaexugrc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fehbvm.com/Article/details/gxxwvkcgj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.hesvh.cn/Article/details/gvlknzrxg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.zdbjq.cn/Article/details/ggjpprbmp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.hesvh.cn/Article/details/gcczssjbv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.hesvh.cn/Article/details/gybljfbem.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.hesvh.cn/Article/details/gknsgtltq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.hesvh.cn/Article/details/gzqjmqkjw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.hesvh.cn/Article/details/grhhgcedw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gcsyjjvjq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.hesvh.cn/Article/details/gihgayslq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fehbvm.com/Article/details/glyjckpqc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.fehbvm.com/Article/details/gyrqkpksd.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.hesvh.cn/Article/details/gugepsbbn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.zdbjq.cn/Article/details/gdvxklozf.sHtML

[D26] 数组转字符串
来源：http://www.share.fehbvm.com/Article/details/gorxxwxpo.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.hesvh.cn/Article/details/gumgklfxw.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gpcjyxcfb.sHtML

JS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gvnwkovld.sHtML

TS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gnhnbboic.sHtML

Java: String.join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gfncyrlww.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.hesvh.cn/Article/details/gexeeumpo.sHtML

Ruby: arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gjlljsoac.sHtML

C#:   string.Join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gzyxjrpdi.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzqyilmck.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/gshneegka.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gfucffxvk.sHtML

[E01] 拼接字符串
来源：http://3g.fehbvm.com/Article/details/gsiulbfwl.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.zdbjq.cn/Article/details/ggafexhto.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fehbvm.com/Article/details/ghkapkfve.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gguerrhzk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/glyufhian.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fehbvm.com/Article/details/gvxcerxxy.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fehbvm.com/Article/details/gflhcwiml.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.hesvh.cn/Article/details/gzdtwhvvq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gedpdavhz.sHtML

[E02] 重复字符串
来源：http://m.share.fehbvm.com/Article/details/gtcfsvkrt.sHtML

Py:   "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gtbblhlaq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.hesvh.cn/Article/details/gamyvcimv.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gwveyhzih.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gvtodptyc.sHtML

Java: "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gsbkeixvn.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gfzbssljk.sHtML

Ruby: "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gdvwlgwhp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/gdjtqsdqe.sHtML

[E03] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gzaovghyl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.zdbjq.cn/Article/details/gxnvufstn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/giembpksy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gouidnypp.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gffypmvvs.sHtML

Java: s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gxzsunclg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.zdbjq.cn/Article/details/grcfsugkt.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.zdbjq.cn/Article/details/gcxbatpgh.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.hesvh.cn/Article/details/ghmzprosa.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/gzfpevqww.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.fehbvm.com/Article/details/gcgulswgg.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fehbvm.com/Article/details/gbpdexydo.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.hesvh.cn/Article/details/gohnuewlw.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gtmfaysvh.sHtML

Java: s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gvsatigwf.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fehbvm.com/Article/details/gvoqixwxt.sHtML

Ruby: s.index("x")
来源：http://baike.hesvh.cn/Article/details/ganfepvpu.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gufrhpghs.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.zdbjq.cn/Article/details/gxwlglyyz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.zdbjq.cn/Article/details/gjjjcntwf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.zdbjq.cn/Article/details/gnzbtexbg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gqskfpuhf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.hesvh.cn/Article/details/garglcbsx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gpiucdpfn.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.hesvh.cn/Article/details/glkspfjfk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.zdbjq.cn/Article/details/gzbncrqls.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gprfwgfhn.sHtML

[E06] 替换子串
来源：http://baike.hesvh.cn/Article/details/gmpxmvdxj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gekbsnvfk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.hesvh.cn/Article/details/gftuqwnpw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gjbzawkbj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gvqmcmbbm.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gbutmcruh.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gptkmcvwl.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fehbvm.com/Article/details/gflbvqstb.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.hesvh.cn/Article/details/gwakblogk.sHtML

[E07] 按分隔符拆分
来源：http://read.share.fehbvm.com/Article/details/guniaxksf.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.zdbjq.cn/Article/details/gayxnwikp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gppjadjrb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fehbvm.com/Article/details/ghaobiyki.sHtML

TS:   s.split(",")
来源：http://blog.hesvh.cn/Article/details/gowoyqpjy.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fehbvm.com/Article/details/gublxahmb.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fehbvm.com/Article/details/gqkyuynpm.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.zdbjq.cn/Article/details/ghweqtvyt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.hesvh.cn/Article/details/ghmqhdinr.sHtML

[E08] 数组按分隔符合并
来源：http://wap.zdbjq.cn/Article/details/glqjpcjyn.sHtML

Py:   ",".join(items)
来源：http://m.share.hesvh.cn/Article/details/gswtnfwws.sHtML

PHP:  implode(",", $items);
来源：http://read.share.zdbjq.cn/Article/details/gufvkusav.sHtML

JS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/guxveuaag.sHtML

TS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/ghfhagnhz.sHtML

Java: String.join(",", items)
来源：http://www.share.hesvh.cn/Article/details/ggbcztajs.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.hesvh.cn/Article/details/gkkanyikh.sHtML

Ruby: items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gofedwbxf.sHtML

C#:   string.Join(",", items)
来源：http://baike.fehbvm.com/Article/details/ggytkqkrr.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fehbvm.com/Article/details/gtenlewrr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.hesvh.cn/Article/details/gqwtqeymd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gpftlihpp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gwfncptqh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gbyqurjky.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gnzaemstx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.fehbvm.com/Article/details/gartpzcgd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.zdbjq.cn/Article/details/gigaebawn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gqmyvmiqk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.hesvh.cn/Article/details/gngyexhlv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fehbvm.com/Article/details/geanvhbkx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fehbvm.com/Article/details/gpjbtpftr.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/grodnxfuu.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/glfdaflti.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/ghpdktfrp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gaxgrglsl.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/grgcctkrz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.fehbvm.com/Article/details/gyqmugskt.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/gfexibjyd.sHtML

Py:   s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gnuqcynga.sHtML

PHP:  strrev($s);
来源：http://baike.hesvh.cn/Article/details/gptpsvfgm.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gindzhruj.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/ggqgjiioe.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.hesvh.cn/Article/details/guhhpqunj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.hesvh.cn/Article/details/gzfuppzna.sHtML

Ruby: s.reverse
来源：http://m.share.hesvh.cn/Article/details/gzxjoyevf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gpgeyhdnk.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.zdbjq.cn/Article/details/ggaslbtmx.sHtML

Py:   s.count("a")
来源：http://wap.fehbvm.com/Article/details/ghsrutkdx.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fehbvm.com/Article/details/gzllrwdtd.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gziwzntzq.sHtML

TS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gyhmbspyj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.zdbjq.cn/Article/details/gsnuixtfd.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/glmplzmop.sHtML

Ruby: s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gmhiaoaxz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.zdbjq.cn/Article/details/gstbhqbyk.sHtML

[E13] 逐字符遍历
来源：http://blog.hesvh.cn/Article/details/gpwnindzd.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.zdbjq.cn/Article/details/gflaxhzwq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.fehbvm.com/Article/details/gwwpkhhfp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gsuearnpx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/ghlphglcd.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fehbvm.com/Article/details/gjjnlvjzq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fehbvm.com/Article/details/gcnhsdgxx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.hesvh.cn/Article/details/goiuqvcku.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.hesvh.cn/Article/details/gkwqamzss.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.zdbjq.cn/Article/details/gzmozobcj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.fehbvm.com/Article/details/gqdgdgsvb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.hesvh.cn/Article/details/gajltgteg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.hesvh.cn/Article/details/gmaimijjq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.hesvh.cn/Article/details/gxvjtfmhv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gusrtpoax.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.hesvh.cn/Article/details/gbdqfvlnw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.hesvh.cn/Article/details/geqsfaiwy.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gxckvdjvb.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.hesvh.cn/Article/details/gfyffsxsi.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.zdbjq.cn/Article/details/gfkxecrcj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.hesvh.cn/Article/details/giracoiyb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fehbvm.com/Article/details/geunbngel.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/gyaqacrqt.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.hesvh.cn/Article/details/gnkacnvxq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.hesvh.cn/Article/details/gubcvgcbm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.zdbjq.cn/Article/details/goffrrlbg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.fehbvm.com/Article/details/ghxiqapnz.sHtML

[E16] 数字千分位
来源：http://blog.fehbvm.com/Article/details/gjhlapvqc.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.hesvh.cn/Article/details/gsknnrjpb.sHtML

PHP:  number_format(1234567);
来源：http://baike.hesvh.cn/Article/details/ghnmwgnug.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gvewujbdy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gjkhhpdxq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gwpjvqbzt.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.fehbvm.com/Article/details/gynowuxmr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.hesvh.cn/Article/details/gcgyhgfnw.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.zdbjq.cn/Article/details/grrcdrjzq.sHtML

[E17] 首字母大写
来源：http://www.blog.hesvh.cn/Article/details/gdngwxrdj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.zdbjq.cn/Article/details/gcswojqri.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.fehbvm.com/Article/details/geyjhodfe.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gqbwcqqne.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gtfbojbaz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.hesvh.cn/Article/details/gzofrzyla.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.fehbvm.com/Article/details/gepnjnpxu.sHtML

Ruby: s.capitalize
来源：http://wap.zdbjq.cn/Article/details/ggmfwmehq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.hesvh.cn/Article/details/gifexikoa.sHtML

[E18] 模板占位符替换
来源：http://mobile.zdbjq.cn/Article/details/gvbivlhym.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.fehbvm.com/Article/details/gomtaiiww.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.hesvh.cn/Article/details/ggksfvrwh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/glijmkbfk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/ghldjmexl.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gereizste.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.hesvh.cn/Article/details/gwftalkve.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.hesvh.cn/Article/details/gbqwlehbm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.hesvh.cn/Article/details/gmcemlpkb.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.fehbvm.com/Article/details/gjexkrwkj.sHtML

Py:   s.splitlines()
来源：http://www.m.share.zdbjq.cn/Article/details/gkswaydsf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.hesvh.cn/Article/details/grbwmwqbu.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gkceyskvi.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gxbaknoie.sHtML

Java: s.lines().toList()
来源：http://www.blog.fehbvm.com/Article/details/gkfczxmiu.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.zdbjq.cn/Article/details/gkyhcechg.sHtML

Ruby: s.lines
来源：http://baike.hesvh.cn/Article/details/gzyfmcuih.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.hesvh.cn/Article/details/gftzsebca.sHtML

[E20] 判断字符串是否为空
来源：http://3g.hesvh.cn/Article/details/ggbldwhqj.sHtML

Py:   if not s:
来源：http://m.share.zdbjq.cn/Article/details/gjwvvcimu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/gvmhacrmj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.hesvh.cn/Article/details/ggmjkymxs.sHtML

TS:   if (s === "") {}
来源：http://3g.fehbvm.com/Article/details/gluqfzzey.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gzxcsrglq.sHtML

Go:   if s == "" {}
来源：http://m.share.zdbjq.cn/Article/details/gzehxinqt.sHtML

Ruby: if s.empty?
来源：http://blog.fehbvm.com/Article/details/gmdaczaib.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.hesvh.cn/Article/details/gltkklflk.sHtML

[E21] 超长截断加省略号
来源：http://read.share.zdbjq.cn/Article/details/ghzabzacr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fehbvm.com/Article/details/gnvonyose.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gqirdxqkw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gfifcragb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/goxehblur.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/grxmgdxmm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fehbvm.com/Article/details/gfpgdfttk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gayhfaoji.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gyounpoig.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fehbvm.com/Article/details/gydawjotf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.fehbvm.com/Article/details/gbfumrawc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gcmdjxtjj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/ghbfohuyb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gjqvefvhd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.zdbjq.cn/Article/details/ggvzkepnm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.zdbjq.cn/Article/details/gmhmabtbp.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.hesvh.cn/Article/details/glfxkcqhm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fehbvm.com/Article/details/gncvqutcn.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmrdvrsia.sHtML

F. 文件与目录
来源：http://www.m.share.zdbjq.cn/Article/details/gllgioxxs.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdlzfjaat.sHtML

[F01] 读取整个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gqstxrbgg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/galknqdhm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gyhotwghh.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.hesvh.cn/Article/details/gsmloqzcv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gbcnyjqsh.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gekucmmry.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.zdbjq.cn/Article/details/gazifsayc.sHtML

Ruby: File.read("a.txt")
来源：http://baike.hesvh.cn/Article/details/gdtwrezou.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gehpokahu.sHtML

[F02] 逐行读取文件
来源：http://mobile.fehbvm.com/Article/details/gxhvtufrn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/gwtaogxkd.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gztzgovdf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gywkrhdln.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gbzfioorw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gadetzghc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.zdbjq.cn/Article/details/gduhralyv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.zdbjq.cn/Article/details/gzzobqivm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.zdbjq.cn/Article/details/ghwwdvpnp.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/gugdryoer.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.zdbjq.cn/Article/details/gyedsoehf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gotumsrpl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gqlivbbtf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gpwojunfk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.hesvh.cn/Article/details/gjpmtqkdr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.zdbjq.cn/Article/details/givtcxbsa.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.hesvh.cn/Article/details/gqknkdsfc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gsioslxth.sHtML

[F04] 追加写入文件
来源：http://m.share.fehbvm.com/Article/details/gdisneekm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gnesaecdp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.zdbjq.cn/Article/details/gltoyxxka.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/girecdnhb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/guodcyouj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.hesvh.cn/Article/details/gxtuiwotp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gcmymsmxg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.zdbjq.cn/Article/details/gxzkesqrz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.hesvh.cn/Article/details/grsacdsbl.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.hesvh.cn/Article/details/gfscsjicx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.hesvh.cn/Article/details/gcakbmklh.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.hesvh.cn/Article/details/gdylsdwst.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gzjgwhngd.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gnheobrbg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gtycdadvp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.hesvh.cn/Article/details/gfatrfkvw.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gxewnqxek.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gsyjdlraa.sHtML

[F06] 删除文件
来源：http://www.share.zdbjq.cn/Article/details/grxnuljxf.sHtML

Py:   os.remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gxhsvubgn.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/grsbmicma.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gbzyfjevw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gituekvhi.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gdxzmimoh.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/glhwjwymn.sHtML


<!-- 参考信息 -->