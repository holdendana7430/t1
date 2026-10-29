代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.hesvh.cn/Article/details/gzyrfestc.sHtML

JS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gyumkkfgl.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gjedbjayi.sHtML

Java: list.contains(x)
来源：http://mobile.fehbvm.com/Article/details/gibqceqfa.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gjtyzmoep.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gohwzbxzt.sHtML

C#:   list.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/gglllqnti.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.zdbjq.cn/Article/details/gqpnifvyx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fehbvm.com/Article/details/gaoibxkaa.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.zdbjq.cn/Article/details/gvkpqxqcr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.hesvh.cn/Article/details/gtsvtkdzc.sHtML

TS:   [...arr];
来源：http://wap.hesvh.cn/Article/details/gyznengaj.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gjfmtufqu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fehbvm.com/Article/details/gptdhlels.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.hesvh.cn/Article/details/gfviyrtmk.sHtML

C#:   new List<int>(list);
来源：http://read.share.zdbjq.cn/Article/details/gvlnbxcsw.sHtML

[D23] reduce 累积计算
来源：http://3g.zdbjq.cn/Article/details/ggclrjzzi.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/gtjwavuzz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.fehbvm.com/Article/details/gnmktrzdw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gzcapiwbm.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gtkdubnwf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.hesvh.cn/Article/details/gdjqfykjo.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/goqthevgx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.zdbjq.cn/Article/details/gitgoaonr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.zdbjq.cn/Article/details/gjljtgzgn.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.fehbvm.com/Article/details/gmzyrkeww.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.hesvh.cn/Article/details/gbyiesieh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fehbvm.com/Article/details/gqyudposw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fehbvm.com/Article/details/gubswbflv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gczndlncc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fehbvm.com/Article/details/gxwqexbdh.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.hesvh.cn/Article/details/gljzenkwu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.zdbjq.cn/Article/details/gssexgrue.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.zdbjq.cn/Article/details/gufzpepjb.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.zdbjq.cn/Article/details/gusfdqwgt.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fehbvm.com/Article/details/gszmykhrz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.fehbvm.com/Article/details/gimhxynou.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.zdbjq.cn/Article/details/glvbpxhpt.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fehbvm.com/Article/details/gjlfpgzme.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.fehbvm.com/Article/details/gtmfvifoh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.hesvh.cn/Article/details/gmdwemgrh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.hesvh.cn/Article/details/gydzdyzzy.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gpunlovmc.sHtML

[D26] 数组转字符串
来源：http://3g.fehbvm.com/Article/details/gycfwhkka.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.fehbvm.com/Article/details/gweuyhief.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fehbvm.com/Article/details/glbsfxuan.sHtML

JS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gkksyoezu.sHtML

TS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gvwfnfjxs.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gxlcvwize.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.hesvh.cn/Article/details/gkaaixzzi.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gijfnkzmz.sHtML

C#:   string.Join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gmmawgwuv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gifauaixd.sHtML

E. 字符串处理
来源：http://3g.hesvh.cn/Article/details/gjnmlsmzs.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ggtelbftc.sHtML

[E01] 拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gcimpryza.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.fehbvm.com/Article/details/gcgcspbla.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.hesvh.cn/Article/details/gjmopdpkx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gcigvkekc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gqwywtzwm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fehbvm.com/Article/details/gmkynmfqs.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fehbvm.com/Article/details/gwqhtklyu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.hesvh.cn/Article/details/gqepxxsrp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fehbvm.com/Article/details/ghcsgpxku.sHtML

[E02] 重复字符串
来源：http://www.share.zdbjq.cn/Article/details/galpkkytd.sHtML

Py:   "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gcbbpguyr.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.fehbvm.com/Article/details/guxtoifbz.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gejcqbtra.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gyhogomar.sHtML

Java: "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gcqorccaj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.hesvh.cn/Article/details/gpippwlvp.sHtML

Ruby: "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gslgutjsu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.hesvh.cn/Article/details/geselfhdt.sHtML

[E03] 截取子串
来源：http://blog.hesvh.cn/Article/details/gjtqbqmhr.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.zdbjq.cn/Article/details/gacmthsmy.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/guedwfpmi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gblnxcndp.sHtML

TS:   s.slice(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gsbxlyesq.sHtML

Java: s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/glxjaragc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.hesvh.cn/Article/details/ggwwxcdug.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fehbvm.com/Article/details/ghohhbzke.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.hesvh.cn/Article/details/gqaxulnvt.sHtML

[E04] 查找子串位置
来源：http://blog.hesvh.cn/Article/details/gvfebiprq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/grsqrbpxa.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.hesvh.cn/Article/details/gbokfzlly.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.fehbvm.com/Article/details/gwrtbfhsf.sHtML

TS:   s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gfqtxkcxq.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gtpdvvphm.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fehbvm.com/Article/details/gpwfthghf.sHtML

Ruby: s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gclmdqvff.sHtML

C#:   s.IndexOf("x")
来源：http://3g.hesvh.cn/Article/details/grjvhicxh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.zdbjq.cn/Article/details/glauatydn.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fehbvm.com/Article/details/gdiltzcny.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.zdbjq.cn/Article/details/gmwgtkcjc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gpxoqmkdk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.fehbvm.com/Article/details/goowppvgk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gncenzujn.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fehbvm.com/Article/details/gkpjfknam.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.hesvh.cn/Article/details/gfvewwyrk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.hesvh.cn/Article/details/gwnagwrxf.sHtML

[E06] 替换子串
来源：http://read.share.fehbvm.com/Article/details/gndysjwip.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gamlfgwqt.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.zdbjq.cn/Article/details/gwwosyyzm.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gzaktuufm.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gikrlwtrl.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/ghzufomxh.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gyfgfjgpn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gphzeafbb.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gdxzgpwhv.sHtML

[E07] 按分隔符拆分
来源：http://wap.hesvh.cn/Article/details/gviofxdqc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.hesvh.cn/Article/details/gjcxrpdrk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.hesvh.cn/Article/details/gbohavgix.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.zdbjq.cn/Article/details/gaqbrcmxp.sHtML

TS:   s.split(",")
来源：http://www.blog.zdbjq.cn/Article/details/glrgtuzds.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fehbvm.com/Article/details/gbcbpycyj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.zdbjq.cn/Article/details/glfiacfhc.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.zdbjq.cn/Article/details/gkvfsnnjo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.hesvh.cn/Article/details/gkncwlqbj.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.fehbvm.com/Article/details/gvzdhwanw.sHtML

Py:   ",".join(items)
来源：http://read.share.hesvh.cn/Article/details/giclxbhcg.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fehbvm.com/Article/details/gbprelhmt.sHtML

JS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gekwraivz.sHtML

TS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gqhdjalna.sHtML

Java: String.join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gglryyllw.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fehbvm.com/Article/details/gemahaqxm.sHtML

Ruby: items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gfswsdjtr.sHtML

C#:   string.Join(",", items)
来源：http://mobile.hesvh.cn/Article/details/glsogaljq.sHtML

[E09] 去除所有空白字符
来源：http://mobile.hesvh.cn/Article/details/gyajjeute.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.zdbjq.cn/Article/details/gjgtqgjqq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.zdbjq.cn/Article/details/gwfoymrys.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gmflxbodx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gkklmomzg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.fehbvm.com/Article/details/gqdzpupck.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.hesvh.cn/Article/details/guhrwtxrr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.hesvh.cn/Article/details/gdwciqukb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gnahqxflj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.zdbjq.cn/Article/details/gxartfbwz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.hesvh.cn/Article/details/guncktfdh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.hesvh.cn/Article/details/gznmdfigl.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gwhiolmze.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/geetqsdhq.sHtML

Java: String.format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gbrdrrbhw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gedyliadj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gpuilmcvi.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/gljiugzvd.sHtML

[E11] 反转字符串
来源：http://www.blog.hesvh.cn/Article/details/gqrfhubxn.sHtML

Py:   s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gqtmflelc.sHtML

PHP:  strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gwzbkgtym.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gehyqblyq.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/grfchlboq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fehbvm.com/Article/details/gnyvynoct.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.zdbjq.cn/Article/details/glnyrhwjf.sHtML

Ruby: s.reverse
来源：http://read.share.fehbvm.com/Article/details/gfijdtlnk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gzkuqkvpe.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.zdbjq.cn/Article/details/gjvidicnd.sHtML

Py:   s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gpzjxgkdd.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.hesvh.cn/Article/details/gsvhdvxfz.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/glrztlqlc.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gzvmmnfby.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.zdbjq.cn/Article/details/gymqhvztd.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fehbvm.com/Article/details/ghtxixbjf.sHtML

Ruby: s.count("a")
来源：http://wap.fehbvm.com/Article/details/gdamkbzmb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.hesvh.cn/Article/details/gcifgrhnl.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fehbvm.com/Article/details/goukfdkvr.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.zdbjq.cn/Article/details/gzptitzxy.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.fehbvm.com/Article/details/gmvrgxeyq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/ggjqhcpqr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gejnrujji.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.fehbvm.com/Article/details/gamoartux.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.zdbjq.cn/Article/details/gzsapfluk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.fehbvm.com/Article/details/gsjjhzdgy.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fehbvm.com/Article/details/gxprgkipm.sHtML

[E14] URL 编码与 Base64
来源：http://wap.hesvh.cn/Article/details/giqtbckgr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.hesvh.cn/Article/details/gnwvkrjzz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.zdbjq.cn/Article/details/ghnzputgy.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.zdbjq.cn/Article/details/gcutfvyvv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.zdbjq.cn/Article/details/gwieaeukp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.zdbjq.cn/Article/details/gyogwvasy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.zdbjq.cn/Article/details/gjgrjkvpg.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.hesvh.cn/Article/details/gcmonwebp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gsscwnjky.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.zdbjq.cn/Article/details/gsmztkjrs.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fehbvm.com/Article/details/gckhbgryz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.zdbjq.cn/Article/details/gxgefwhuw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.hesvh.cn/Article/details/giomjgeao.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/gwxoyplqi.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.hesvh.cn/Article/details/gwnksbiij.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.hesvh.cn/Article/details/gbxlcgiwz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.hesvh.cn/Article/details/gonzityqy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.zdbjq.cn/Article/details/gtnadyyen.sHtML

[E16] 数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gzuciwuso.sHtML

Py:   f"{1234567:,}"
来源：http://wap.zdbjq.cn/Article/details/gqxbsvxix.sHtML

PHP:  number_format(1234567);
来源：http://3g.fehbvm.com/Article/details/gixvibpqw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gqkbatwer.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gkzrootlh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fehbvm.com/Article/details/glutliits.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.zdbjq.cn/Article/details/gknkoojjx.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.fehbvm.com/Article/details/gbemxkqmr.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.zdbjq.cn/Article/details/gmyzsvgjs.sHtML

[E17] 首字母大写
来源：http://3g.fehbvm.com/Article/details/geundruob.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.fehbvm.com/Article/details/gfzdybleb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.hesvh.cn/Article/details/gghxxhbff.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gdgdebiev.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gsszferby.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fehbvm.com/Article/details/ghcbvvami.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.zdbjq.cn/Article/details/ggetcnekb.sHtML

Ruby: s.capitalize
来源：http://www.m.share.hesvh.cn/Article/details/gogjickbf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.hesvh.cn/Article/details/gjeratckt.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.zdbjq.cn/Article/details/giwfbbuge.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.fehbvm.com/Article/details/gtbihipyk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.zdbjq.cn/Article/details/gwihimrsc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gvabfbpuc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gwditponq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gquunnked.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gqlsigfiv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.hesvh.cn/Article/details/gakkmibkn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.hesvh.cn/Article/details/gebiqjpkl.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.hesvh.cn/Article/details/gupcaiail.sHtML

Py:   s.splitlines()
来源：http://www.share.hesvh.cn/Article/details/gjpqsfjip.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gtizcvqyp.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gbtndupoy.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/glqgbniue.sHtML

Java: s.lines().toList()
来源：http://read.share.fehbvm.com/Article/details/giksjeqrh.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fehbvm.com/Article/details/goyaqrnnd.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/ghkumpbck.sHtML

C#:   s.Split('\n')
来源：http://3g.zdbjq.cn/Article/details/ggiocpubw.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fehbvm.com/Article/details/ghzymtafh.sHtML

Py:   if not s:
来源：http://www.blog.zdbjq.cn/Article/details/gboylsedn.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fehbvm.com/Article/details/glacqvyjw.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fehbvm.com/Article/details/gwjlmhdia.sHtML

TS:   if (s === "") {}
来源：http://wap.fehbvm.com/Article/details/grywmcqoi.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/giefqstnq.sHtML

Go:   if s == "" {}
来源：http://www.m.share.hesvh.cn/Article/details/ghxaxzplh.sHtML

Ruby: if s.empty?
来源：http://www.share.fehbvm.com/Article/details/glpkxepux.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.zdbjq.cn/Article/details/genndldfx.sHtML

[E21] 超长截断加省略号
来源：http://baike.hesvh.cn/Article/details/gqodvcrym.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/grscrxpod.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gzeqyqxnj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/giqzzlhhc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gpwsgbyxe.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/godxdhkyv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.zdbjq.cn/Article/details/gpavpenfb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gytmgeoku.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gpzxdspnk.sHtML

[E22] 字节长度与字符长度
来源：http://wap.zdbjq.cn/Article/details/gckpkcwxe.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.hesvh.cn/Article/details/gwqygvodo.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gsoctgbqs.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/goaqjbgca.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gogbkiffl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fehbvm.com/Article/details/gtqygqncs.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.zdbjq.cn/Article/details/guvdtvtpu.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.zdbjq.cn/Article/details/gxgjcrrod.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fehbvm.com/Article/details/guehmuzlh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grlmkaayz.sHtML

F. 文件与目录
来源：http://blog.zdbjq.cn/Article/details/gqmsyhtnd.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gikltcwcw.sHtML

[F01] 读取整个文件
来源：http://www.blog.zdbjq.cn/Article/details/ginvlvjbu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.zdbjq.cn/Article/details/gobksqmdy.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.hesvh.cn/Article/details/gisfabcly.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.hesvh.cn/Article/details/gddlvthag.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gssejxani.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/geibihzqr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.zdbjq.cn/Article/details/gfescdmot.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.hesvh.cn/Article/details/ggjkodypj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gjgabgxlp.sHtML

[F02] 逐行读取文件
来源：http://mobile.fehbvm.com/Article/details/gxonatvbo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.zdbjq.cn/Article/details/gblrtekzh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.zdbjq.cn/Article/details/ghebgifaa.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gfeuiwqxd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/glimiwcco.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/ggzsjpoqv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.hesvh.cn/Article/details/gcpqzjubm.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.hesvh.cn/Article/details/gnidltudc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.zdbjq.cn/Article/details/gbnjrsynh.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.hesvh.cn/Article/details/gduzinekm.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.zdbjq.cn/Article/details/gvwrqxhdv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gtpzbbisf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gjwkqecgu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gdpkvsjke.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fehbvm.com/Article/details/gxjoscswf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.hesvh.cn/Article/details/gcqgazepg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.hesvh.cn/Article/details/gjqnonbfo.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/ggazxhunu.sHtML

[F04] 追加写入文件
来源：http://wap.hesvh.cn/Article/details/gnfscnnnz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gknskwhtn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.zdbjq.cn/Article/details/gsrocuwfa.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/grremwkah.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gpvvpzomb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.zdbjq.cn/Article/details/gysiiszyw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.hesvh.cn/Article/details/guehcfagp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.hesvh.cn/Article/details/ggrpqdlbt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fehbvm.com/Article/details/ghwdfwbcp.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fehbvm.com/Article/details/gvupoqhrr.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fehbvm.com/Article/details/giuwdlxdl.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gkgexrnnk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gsuajngbc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gxerckesc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gbdvgixgo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.zdbjq.cn/Article/details/guajexqsj.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gqgndqfhp.sHtML


<!-- 参考信息 -->