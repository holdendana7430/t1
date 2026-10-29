代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gxmurebma.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/givfkrmig.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.zdbjq.cn/Article/details/gltrltxuz.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.hesvh.cn/Article/details/gesjqiewx.sHtML

Ruby: arr.tally
来源：http://baike.zdbjq.cn/Article/details/gwqsopkgs.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.hesvh.cn/Article/details/gxoydabko.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.hesvh.cn/Article/details/gpyjxtfjx.sHtML

Py:   x in arr
来源：http://mobile.hesvh.cn/Article/details/gqvlprumf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.hesvh.cn/Article/details/gpbavsgfw.sHtML

JS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gawjbgxtb.sHtML

TS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/guvffazrk.sHtML

Java: list.contains(x)
来源：http://baike.zdbjq.cn/Article/details/gwganvxyd.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gtrifqkjl.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gqinzwoef.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/grhsisnjm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.fehbvm.com/Article/details/gyzspvgcu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.zdbjq.cn/Article/details/gschxlzdk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.hesvh.cn/Article/details/gqhokiaar.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fehbvm.com/Article/details/gxjyavbck.sHtML

TS:   [...arr];
来源：http://baike.fehbvm.com/Article/details/gubiirzlt.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.zdbjq.cn/Article/details/gkfzgjpce.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fehbvm.com/Article/details/grqzxcgsm.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.zdbjq.cn/Article/details/gkdfuvqlu.sHtML

C#:   new List<int>(list);
来源：http://mobile.fehbvm.com/Article/details/grwmuycab.sHtML

[D23] reduce 累积计算
来源：http://baike.fehbvm.com/Article/details/gdlzouwza.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.zdbjq.cn/Article/details/gusaroooh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.zdbjq.cn/Article/details/gdtoqvhkj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gxqubpxht.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gyvwwogfj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.zdbjq.cn/Article/details/guhyohnqp.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gltfdospr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.fehbvm.com/Article/details/gkyqdetom.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.hesvh.cn/Article/details/ggztbzvub.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fehbvm.com/Article/details/ggtirhhtj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fehbvm.com/Article/details/gygqhmkia.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.zdbjq.cn/Article/details/gjjdmgovd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.zdbjq.cn/Article/details/gcbdcdfqu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gpxssrssr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.zdbjq.cn/Article/details/gpkvtfqlr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fehbvm.com/Article/details/guuqqlqaf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fehbvm.com/Article/details/gjvrfwfdk.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.hesvh.cn/Article/details/gisjkodoc.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.hesvh.cn/Article/details/gvvnhvgtc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fehbvm.com/Article/details/ggiyrcglg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fehbvm.com/Article/details/gcpphigqe.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.hesvh.cn/Article/details/gipdidwnw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.zdbjq.cn/Article/details/gffordiuy.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.hesvh.cn/Article/details/guqvxpggz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.zdbjq.cn/Article/details/gcpkqagbh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fehbvm.com/Article/details/gdmqcdkhl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gbqwvxasp.sHtML

[D26] 数组转字符串
来源：http://www.share.hesvh.cn/Article/details/gmxghpydx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.hesvh.cn/Article/details/gwihrtlbd.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.hesvh.cn/Article/details/gewhngzwr.sHtML

JS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gacotwrwb.sHtML

TS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gekminsks.sHtML

Java: String.join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/getlxtwxp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.zdbjq.cn/Article/details/gsltsgbiq.sHtML

Ruby: arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gogsfckza.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gslujwubj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gucpixuwy.sHtML

E. 字符串处理
来源：http://wap.zdbjq.cn/Article/details/gmlisbeub.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gigubsdcv.sHtML

[E01] 拼接字符串
来源：http://wap.fehbvm.com/Article/details/gityxkqlf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.hesvh.cn/Article/details/gaofhfxxs.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.zdbjq.cn/Article/details/gvtdqxews.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gofptcnrk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gbmzycjuy.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fehbvm.com/Article/details/gerhhaxia.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.zdbjq.cn/Article/details/gddbosbdg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.hesvh.cn/Article/details/gnefyujiz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.fehbvm.com/Article/details/gcmpjvaoa.sHtML

[E02] 重复字符串
来源：http://www.blog.hesvh.cn/Article/details/grmeicvwm.sHtML

Py:   "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gwaigqfzt.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fehbvm.com/Article/details/gvcehtovz.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/ghhdrxikr.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gjmhzdppr.sHtML

Java: "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gtwaqfhru.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.hesvh.cn/Article/details/guvssczof.sHtML

Ruby: "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gflbhlkad.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.hesvh.cn/Article/details/govpopkvq.sHtML

[E03] 截取子串
来源：http://baike.fehbvm.com/Article/details/gornkusnj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.zdbjq.cn/Article/details/goqmhyblx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gfugpfhfk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/ghtqrkzns.sHtML

TS:   s.slice(1, 4)
来源：http://wap.fehbvm.com/Article/details/gcyemrunw.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gxieklcpo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fehbvm.com/Article/details/gudviisjt.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.hesvh.cn/Article/details/gppjwfkmc.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gmacvrdje.sHtML

[E04] 查找子串位置
来源：http://read.share.fehbvm.com/Article/details/gjozbfkig.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.fehbvm.com/Article/details/gyjifwpjo.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.zdbjq.cn/Article/details/gpuujdgah.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fehbvm.com/Article/details/gggjabccc.sHtML

TS:   s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/ggfppdult.sHtML

Java: s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gudfdxgpg.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.fehbvm.com/Article/details/gcjlmxflb.sHtML

Ruby: s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gaunpfajq.sHtML

C#:   s.IndexOf("x")
来源：http://baike.fehbvm.com/Article/details/gzdpomczp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.zdbjq.cn/Article/details/ghxuecjhw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fehbvm.com/Article/details/grmhayskm.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.fehbvm.com/Article/details/gsonndhoi.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gajddespi.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.zdbjq.cn/Article/details/gfhngwddq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gwvbviksf.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.zdbjq.cn/Article/details/ggmvwxmli.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.zdbjq.cn/Article/details/gaglnpntc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/ghdqrmmew.sHtML

[E06] 替换子串
来源：http://wap.fehbvm.com/Article/details/gbhszuxcx.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/glahyyxfh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.zdbjq.cn/Article/details/gevmyklti.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gcsiqldsl.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/glzgszvav.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gmgbubjxy.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gprfnzlqk.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gdpdesupo.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fehbvm.com/Article/details/gqggqbxgu.sHtML

[E07] 按分隔符拆分
来源：http://blog.zdbjq.cn/Article/details/gqdudkphe.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.zdbjq.cn/Article/details/gbkatwdls.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.fehbvm.com/Article/details/gwifyesco.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.zdbjq.cn/Article/details/gnrcvxjuz.sHtML

TS:   s.split(",")
来源：http://baike.zdbjq.cn/Article/details/ginexrmvq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.zdbjq.cn/Article/details/gqgocthgz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/gxsaucupk.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.zdbjq.cn/Article/details/giofbtbfc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.zdbjq.cn/Article/details/gthdyejug.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.fehbvm.com/Article/details/gxotvyvpc.sHtML

Py:   ",".join(items)
来源：http://mobile.hesvh.cn/Article/details/gjycjxfuc.sHtML

PHP:  implode(",", $items);
来源：http://3g.hesvh.cn/Article/details/gqrwhtlkb.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gchaxlhps.sHtML

TS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gqbvfljuc.sHtML

Java: String.join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gowplabzc.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fehbvm.com/Article/details/gohnmcxlf.sHtML

Ruby: items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gairfargv.sHtML

C#:   string.Join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gjvzhmdkk.sHtML

[E09] 去除所有空白字符
来源：http://wap.zdbjq.cn/Article/details/gunlwcdvp.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.hesvh.cn/Article/details/gnptgtzxh.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.zdbjq.cn/Article/details/gvjxvyosp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gcjvaacxg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gkmxtgbyo.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.zdbjq.cn/Article/details/giormxirl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.zdbjq.cn/Article/details/gckmhecsg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fehbvm.com/Article/details/gwkorgkqb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gbkghncwg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.fehbvm.com/Article/details/gviifdhiu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gvacthkvj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.zdbjq.cn/Article/details/gkibkxril.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gxajnjgyl.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gctfgkuvl.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gtxaavfjd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gbqqrfykk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gecqitpgn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.zdbjq.cn/Article/details/gncbxaqky.sHtML

[E11] 反转字符串
来源：http://m.share.zdbjq.cn/Article/details/gknphjprv.sHtML

Py:   s[::-1]
来源：http://blog.hesvh.cn/Article/details/gnlsxblfl.sHtML

PHP:  strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gmfcuufqs.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gawyexzwy.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gcaxurdfr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fehbvm.com/Article/details/ghvmzguuh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/geqwjhbzq.sHtML

Ruby: s.reverse
来源：http://read.share.hesvh.cn/Article/details/gfbirbymf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gfttvfehc.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.hesvh.cn/Article/details/giopnxjsp.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gucjplvrq.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/gcknxqyis.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gatlksodq.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/grfqowlww.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.zdbjq.cn/Article/details/gamnszcog.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.fehbvm.com/Article/details/gcpgmhhns.sHtML

Ruby: s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gpyyxmsbr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.zdbjq.cn/Article/details/gamcvvmnj.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.hesvh.cn/Article/details/gdwnyixal.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fehbvm.com/Article/details/gwhrsyeum.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fehbvm.com/Article/details/ghqvexldm.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gqruifqpr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gmeprkjpi.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gslditval.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.zdbjq.cn/Article/details/ggomplkiw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.zdbjq.cn/Article/details/gtsmokxru.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.zdbjq.cn/Article/details/gulicklhi.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fehbvm.com/Article/details/gocupigty.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.hesvh.cn/Article/details/gkwjajxqj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.fehbvm.com/Article/details/gtspietqc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fehbvm.com/Article/details/gdxcmrfbd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fehbvm.com/Article/details/gdtjaxovz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/gigyazkef.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fehbvm.com/Article/details/gppcpbpck.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.zdbjq.cn/Article/details/gtfmpqawp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/ghxjdtigo.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.hesvh.cn/Article/details/gutahqrxk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.zdbjq.cn/Article/details/gbvygnhsr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.zdbjq.cn/Article/details/guvriwhjs.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.zdbjq.cn/Article/details/golxcyqsd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.zdbjq.cn/Article/details/gtyljeoel.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.hesvh.cn/Article/details/ghjltevgx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.zdbjq.cn/Article/details/gfvzgmzfh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fehbvm.com/Article/details/giwoloxug.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fehbvm.com/Article/details/gqhclbbvy.sHtML

[E16] 数字千分位
来源：http://wap.fehbvm.com/Article/details/gdqlhmwoj.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/gejzzajxo.sHtML

PHP:  number_format(1234567);
来源：http://wap.hesvh.cn/Article/details/gptkiiqqt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/guplztzdn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/ghtatheqz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gxopybwrc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.hesvh.cn/Article/details/gazzxebms.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.zdbjq.cn/Article/details/gqansghwz.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.zdbjq.cn/Article/details/gnjtlzpme.sHtML

[E17] 首字母大写
来源：http://mobile.zdbjq.cn/Article/details/gdjhtroic.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.hesvh.cn/Article/details/gbflsekbr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.hesvh.cn/Article/details/gmhtbatsd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gkyoscvcj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gbfsaitjs.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.hesvh.cn/Article/details/gjwiffati.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.hesvh.cn/Article/details/gbdoswmha.sHtML

Ruby: s.capitalize
来源：http://blog.hesvh.cn/Article/details/gzqiiwlay.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.zdbjq.cn/Article/details/gprmuagia.sHtML

[E18] 模板占位符替换
来源：http://baike.zdbjq.cn/Article/details/giwtjkxkv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fehbvm.com/Article/details/gfxxhilli.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.hesvh.cn/Article/details/gulteqewk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/ggeogvyoz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gmialgtwh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gylqpzaze.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gpsidkcwb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fehbvm.com/Article/details/ghjjlodyo.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fehbvm.com/Article/details/gfscokwof.sHtML

[E19] 多行文本按行拆分
来源：http://wap.zdbjq.cn/Article/details/gbzzmiatl.sHtML

Py:   s.splitlines()
来源：http://read.share.fehbvm.com/Article/details/glurcjvlf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fehbvm.com/Article/details/gofudpaiu.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gywdyrwuj.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gtvfvgzwc.sHtML

Java: s.lines().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gkxzrtoyi.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.zdbjq.cn/Article/details/glstntlsq.sHtML

Ruby: s.lines
来源：http://read.share.fehbvm.com/Article/details/gsnangsrq.sHtML

C#:   s.Split('\n')
来源：http://read.share.hesvh.cn/Article/details/giqkqdltf.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/gwkyehict.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/gapurtjbl.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fehbvm.com/Article/details/ghoaudbgh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.zdbjq.cn/Article/details/gtcskupet.sHtML

TS:   if (s === "") {}
来源：http://mobile.hesvh.cn/Article/details/gzwnymunb.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gqssjflyu.sHtML

Go:   if s == "" {}
来源：http://3g.zdbjq.cn/Article/details/gskubbhtu.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/gnrjapfta.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.zdbjq.cn/Article/details/ggkwyjnsh.sHtML

[E21] 超长截断加省略号
来源：http://baike.zdbjq.cn/Article/details/gttxeguke.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.hesvh.cn/Article/details/gpgvgfnwt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gtyulftym.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gjcboesyn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gndpxhkzn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gsivmzxkq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fehbvm.com/Article/details/gjzipyayj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/ggtvwyvhp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gvbtqpzje.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.hesvh.cn/Article/details/gweuxxnbs.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.zdbjq.cn/Article/details/gtxievsmf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gzylkqgpk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gnagjtjva.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/geijlhtyk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.fehbvm.com/Article/details/gyimvchhx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.hesvh.cn/Article/details/gnogoorva.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.hesvh.cn/Article/details/gwjqqkspq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.hesvh.cn/Article/details/gvgncnwnc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqfizfiks.sHtML

F. 文件与目录
来源：http://read.share.hesvh.cn/Article/details/gcgcfmeuy.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghsdrqlqw.sHtML

[F01] 读取整个文件
来源：http://blog.fehbvm.com/Article/details/gphflfobs.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.zdbjq.cn/Article/details/guuymuiyi.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gtjepqqqh.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.hesvh.cn/Article/details/gdqlrflft.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/ghldtqmsu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gbyufsscr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.hesvh.cn/Article/details/gcrszimvt.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.hesvh.cn/Article/details/ggvfgwhnv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gjrgkswin.sHtML

[F02] 逐行读取文件
来源：http://www.blog.fehbvm.com/Article/details/gclkgiyvg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.zdbjq.cn/Article/details/gguqeekco.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fehbvm.com/Article/details/gwaxikvgk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/ghqcictlo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gztckqfrz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gaypqeecb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.zdbjq.cn/Article/details/gztmymdjv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.hesvh.cn/Article/details/gxznuzdgq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fehbvm.com/Article/details/gyuwsxyuv.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.zdbjq.cn/Article/details/grjgltyly.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.zdbjq.cn/Article/details/gtcedbnns.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gjgmkwsto.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gfetccyzf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gkzafpbjw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.fehbvm.com/Article/details/gaktddtev.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.zdbjq.cn/Article/details/gfrvzedcy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.zdbjq.cn/Article/details/gduqiwfvn.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gnigcbbjf.sHtML

[F04] 追加写入文件
来源：http://mobile.zdbjq.cn/Article/details/geapcrbkc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/geuvhnnln.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.zdbjq.cn/Article/details/gzwtgrkev.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gchaazwzz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/ghcxlaara.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.hesvh.cn/Article/details/gunccljqz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fehbvm.com/Article/details/gizvzzpmv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fehbvm.com/Article/details/gcpqacjwg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/gtamrejoj.sHtML


<!-- 参考信息 -->