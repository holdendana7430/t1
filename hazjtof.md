代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gkihheuri.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.fehbvm.com/Article/details/gfmdadrsv.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.hesvh.cn/Article/details/gzwyvgyhy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.zdbjq.cn/Article/details/gboxixmvb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fehbvm.com/Article/details/gevfvvdvu.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.hesvh.cn/Article/details/gltcsdyqs.sHtML

Py:   Counter(arr)
来源：http://read.share.hesvh.cn/Article/details/gxcclphrq.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fehbvm.com/Article/details/geunzimpl.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gvxzoqjar.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gftwxfnzd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fehbvm.com/Article/details/gzrcqcnsy.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fehbvm.com/Article/details/giwfqnucs.sHtML

Ruby: arr.tally
来源：http://3g.fehbvm.com/Article/details/gnabgrpim.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fehbvm.com/Article/details/graymenal.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fehbvm.com/Article/details/grxfrscye.sHtML

Py:   x in arr
来源：http://blog.zdbjq.cn/Article/details/geymcurlm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fehbvm.com/Article/details/gjpcigyli.sHtML

JS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gadevzelp.sHtML

TS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gitgwnchg.sHtML

Java: list.contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gnloamnup.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gnkafytlv.sHtML

Ruby: arr.include?(x)
来源：http://mobile.fehbvm.com/Article/details/gttnbpnvi.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gkbjkxdup.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.hesvh.cn/Article/details/gfjlehhml.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.zdbjq.cn/Article/details/gbnppwcxp.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.zdbjq.cn/Article/details/gykfplfui.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.hesvh.cn/Article/details/ghhvxakig.sHtML

TS:   [...arr];
来源：http://www.share.fehbvm.com/Article/details/gttpauevh.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.hesvh.cn/Article/details/gzkbgbcwk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fehbvm.com/Article/details/gqmafqzal.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/gfivvcksf.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/ggphtkanv.sHtML

[D23] reduce 累积计算
来源：http://mobile.zdbjq.cn/Article/details/gjhkpvocr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.zdbjq.cn/Article/details/gzzyyzrkh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fehbvm.com/Article/details/gspykjhoe.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gjdbwngxm.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/ggppdzswj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.zdbjq.cn/Article/details/gnndslthf.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gfmlxivrl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.hesvh.cn/Article/details/ggflemfno.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/ggsbtpdna.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.hesvh.cn/Article/details/gnqfugand.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.zdbjq.cn/Article/details/ghffgrmnj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fehbvm.com/Article/details/gqkgxxsbl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fehbvm.com/Article/details/grbonbiwa.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gxvxjbkxm.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.zdbjq.cn/Article/details/gbcgdpydk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.zdbjq.cn/Article/details/glgyzhluv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.fehbvm.com/Article/details/gchwrwcjf.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.hesvh.cn/Article/details/gshowzdki.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.zdbjq.cn/Article/details/gtaeygenh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fehbvm.com/Article/details/golqvtkvi.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.hesvh.cn/Article/details/gzrykphdb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.zdbjq.cn/Article/details/ghrircymt.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.fehbvm.com/Article/details/gadankfly.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.hesvh.cn/Article/details/gvruhusfp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fehbvm.com/Article/details/gtszxkpve.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.fehbvm.com/Article/details/gissnzygk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gnxxbwokk.sHtML

[D26] 数组转字符串
来源：http://wap.hesvh.cn/Article/details/gdjutyhnx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.hesvh.cn/Article/details/gffbhlwmz.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/glmantqrp.sHtML

JS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gctgbbjpn.sHtML

TS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gjjwqqntj.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gtjicrcki.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.zdbjq.cn/Article/details/guirsredx.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gxzwiwfcr.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/georhzkkp.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/geigmksgv.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/gbohgejpl.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/geumkudsp.sHtML

[E01] 拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gibykwvca.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.hesvh.cn/Article/details/ghndaiawe.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.zdbjq.cn/Article/details/grppzfdag.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gtmlwmmld.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gazqutldb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.hesvh.cn/Article/details/grsxacrkb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.zdbjq.cn/Article/details/gcxjiblni.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.zdbjq.cn/Article/details/givdexzyw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gheswkfxe.sHtML

[E02] 重复字符串
来源：http://www.blog.fehbvm.com/Article/details/gvqyanmmp.sHtML

Py:   "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gwfyzsntq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/garjyjymi.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gpsbnajaw.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gucsekapn.sHtML

Java: "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gacrjwglv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.zdbjq.cn/Article/details/glhbtcqvw.sHtML

Ruby: "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/ggyjonjeo.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.zdbjq.cn/Article/details/gmhmcmfyv.sHtML

[E03] 截取子串
来源：http://3g.hesvh.cn/Article/details/gwotshvdd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.hesvh.cn/Article/details/gazkzezty.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gunqsdbed.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gpkhvrbeb.sHtML

TS:   s.slice(1, 4)
来源：http://3g.hesvh.cn/Article/details/gxfvnqpiz.sHtML

Java: s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gbrkqoikw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fehbvm.com/Article/details/geqqalhrp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.zdbjq.cn/Article/details/gxktgytjt.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fehbvm.com/Article/details/gpwkmvowb.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/giozvvtra.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fehbvm.com/Article/details/gsvgblxdf.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.zdbjq.cn/Article/details/gitngcghc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.zdbjq.cn/Article/details/gccltatxq.sHtML

TS:   s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gbkookbxb.sHtML

Java: s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/ganljtcjt.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.hesvh.cn/Article/details/gmriaxcsw.sHtML

Ruby: s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/gtjsxypgd.sHtML

C#:   s.IndexOf("x")
来源：http://blog.zdbjq.cn/Article/details/ghooungvh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.fehbvm.com/Article/details/gqbrqkvdn.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.hesvh.cn/Article/details/gbjsjxmvs.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.hesvh.cn/Article/details/gqolsiibs.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/glmljhqea.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.zdbjq.cn/Article/details/gzekqqpgv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gjhneotpg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.fehbvm.com/Article/details/gypxucpdb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.hesvh.cn/Article/details/gazzchqgi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gabogzdxr.sHtML

[E06] 替换子串
来源：http://m.share.fehbvm.com/Article/details/ghcrepzrg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gbiwxcaue.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.hesvh.cn/Article/details/genpmkrej.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gxrvjkszy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/glhxgnyzd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gmnkluffx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/glazuykem.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gsvtfbsix.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gyqijuzar.sHtML

[E07] 按分隔符拆分
来源：http://baike.zdbjq.cn/Article/details/gwctalkum.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.zdbjq.cn/Article/details/gsaueyjtp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gcaprkymj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fehbvm.com/Article/details/gvorgzlej.sHtML

TS:   s.split(",")
来源：http://3g.hesvh.cn/Article/details/gdcjgbepb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fehbvm.com/Article/details/gwuxddjeh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.hesvh.cn/Article/details/gknduwjgl.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.hesvh.cn/Article/details/gvsnvumuu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.zdbjq.cn/Article/details/gnjdoceqj.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fehbvm.com/Article/details/gnyjpphee.sHtML

Py:   ",".join(items)
来源：http://baike.fehbvm.com/Article/details/gnldujery.sHtML

PHP:  implode(",", $items);
来源：http://wap.hesvh.cn/Article/details/gxtbaqfhz.sHtML

JS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gksqvgpfm.sHtML

TS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gyzxordwc.sHtML

Java: String.join(",", items)
来源：http://baike.fehbvm.com/Article/details/gywejwpkg.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.hesvh.cn/Article/details/ggdyfrukj.sHtML

Ruby: items.join(",")
来源：http://m.share.hesvh.cn/Article/details/ghapexifr.sHtML

C#:   string.Join(",", items)
来源：http://wap.hesvh.cn/Article/details/gxjbvencu.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fehbvm.com/Article/details/gvetahnwc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fehbvm.com/Article/details/gnhharnsb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.hesvh.cn/Article/details/gfgcugtsn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gyduepzux.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/gjwqjarou.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gyucgjlsx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.hesvh.cn/Article/details/ghtejnfat.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.zdbjq.cn/Article/details/gwwbgyizq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gminrvgmg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.zdbjq.cn/Article/details/goftzbukk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gnscbjxrp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fehbvm.com/Article/details/gdxxwdxgm.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gtaiwjstd.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gsnlhytfk.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gqcubjjzc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gqxjzvuhu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gdtvzqzrj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.zdbjq.cn/Article/details/gfbejwhqv.sHtML

[E11] 反转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/grrniivjo.sHtML

Py:   s[::-1]
来源：http://read.share.fehbvm.com/Article/details/guhubvovu.sHtML

PHP:  strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gzimpbczx.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gzcujeyfy.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gapvhnnvx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/gojszmocn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fehbvm.com/Article/details/guwnvyyoq.sHtML

Ruby: s.reverse
来源：http://baike.hesvh.cn/Article/details/gzzudfuui.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gbgfbtxfp.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fehbvm.com/Article/details/gezpxigav.sHtML

Py:   s.count("a")
来源：http://mobile.fehbvm.com/Article/details/guiscobpv.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.zdbjq.cn/Article/details/gjtagkujh.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gfkyrghrs.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gkbehaqfg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.hesvh.cn/Article/details/gkzsxhdrh.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.hesvh.cn/Article/details/gqqscotxs.sHtML

Ruby: s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gvgwixioc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.zdbjq.cn/Article/details/giigfyllk.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.hesvh.cn/Article/details/gtchkzapf.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.zdbjq.cn/Article/details/gsabdtvll.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.hesvh.cn/Article/details/gxgnrunfr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gfsaqwosf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gjiefsglc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gwcpirxwm.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.zdbjq.cn/Article/details/gyqnhlukz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.hesvh.cn/Article/details/gosuiixxz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.hesvh.cn/Article/details/gysomvuqa.sHtML

[E14] URL 编码与 Base64
来源：http://wap.zdbjq.cn/Article/details/gnyiyzjgb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.hesvh.cn/Article/details/gnmcmfaqr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.zdbjq.cn/Article/details/gtzbqhdhp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.zdbjq.cn/Article/details/gsgnmrvhm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.hesvh.cn/Article/details/ghmfwvidf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fehbvm.com/Article/details/ghneilybk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.hesvh.cn/Article/details/gemezfvxp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.fehbvm.com/Article/details/ghlchepiz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fehbvm.com/Article/details/gbbkpcoku.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/glgdtzbjz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/gpmwazojl.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.zdbjq.cn/Article/details/gbuzkdajq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fehbvm.com/Article/details/gaftzmezm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.zdbjq.cn/Article/details/glrnbgyrq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fehbvm.com/Article/details/gbjgyrquc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.hesvh.cn/Article/details/gupctehag.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.hesvh.cn/Article/details/gcvvjfpuf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.zdbjq.cn/Article/details/grvhfyqdr.sHtML

[E16] 数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gfrxasusp.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/gmakwoske.sHtML

PHP:  number_format(1234567);
来源：http://3g.zdbjq.cn/Article/details/gdyqdcifs.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/grzctjmfj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gormrermv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gcwotmgvy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.hesvh.cn/Article/details/gdducctwk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.hesvh.cn/Article/details/grjhtttoy.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.hesvh.cn/Article/details/gudgxmfeu.sHtML

[E17] 首字母大写
来源：http://blog.hesvh.cn/Article/details/goawmhxyl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.hesvh.cn/Article/details/gvxxatxqf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.zdbjq.cn/Article/details/gvuevcztm.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/getgxvhbo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/grmbjfqxh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.fehbvm.com/Article/details/gxiqsbecy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.hesvh.cn/Article/details/gdgyzwbbt.sHtML

Ruby: s.capitalize
来源：http://wap.hesvh.cn/Article/details/gpbtrrotm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.fehbvm.com/Article/details/gmbqerzuf.sHtML

[E18] 模板占位符替换
来源：http://3g.zdbjq.cn/Article/details/gwfywvngc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.hesvh.cn/Article/details/gwwwmfigp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.zdbjq.cn/Article/details/gfifycyvs.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gijhnfgys.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gklvawqgr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gnndsdbef.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gqzladner.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.zdbjq.cn/Article/details/gcdgvcwjo.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.zdbjq.cn/Article/details/ggbdeozsf.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/glzgmfwzy.sHtML

Py:   s.splitlines()
来源：http://read.share.hesvh.cn/Article/details/gfttpcdyn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gsctgmwwg.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/gfgkkfhdc.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gydsvokow.sHtML

Java: s.lines().toList()
来源：http://read.share.hesvh.cn/Article/details/gvrfjobdd.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.zdbjq.cn/Article/details/gklcehqyp.sHtML

Ruby: s.lines
来源：http://mobile.zdbjq.cn/Article/details/gxyyrhlzt.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.zdbjq.cn/Article/details/gjrmrtxnz.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.fehbvm.com/Article/details/gkgvpoiub.sHtML

Py:   if not s:
来源：http://mobile.hesvh.cn/Article/details/grxobjvzt.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.hesvh.cn/Article/details/gifrgdbht.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.hesvh.cn/Article/details/gmbqzwjns.sHtML

TS:   if (s === "") {}
来源：http://blog.fehbvm.com/Article/details/gyvdektms.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gypnskxcf.sHtML

Go:   if s == "" {}
来源：http://www.blog.fehbvm.com/Article/details/gjliolygd.sHtML

Ruby: if s.empty?
来源：http://www.share.zdbjq.cn/Article/details/gkglbtpts.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fehbvm.com/Article/details/gecyrtgkj.sHtML

[E21] 超长截断加省略号
来源：http://blog.hesvh.cn/Article/details/gisuhwiaj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fehbvm.com/Article/details/gxxiurugi.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gwcgykyqz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gavcflabu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/ghspahcyq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/grxtvylqy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.hesvh.cn/Article/details/gbaxakmck.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gkvkkhngb.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gzvntwwzz.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.hesvh.cn/Article/details/gyvqyulak.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.hesvh.cn/Article/details/gpbffkhmi.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/glbatphvp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gsmyctjyq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gfvqvsljl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fehbvm.com/Article/details/gixccbbon.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.fehbvm.com/Article/details/gnhsflelz.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gpvrbpdnv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.zdbjq.cn/Article/details/guhtyyzbu.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdjzcvgxu.sHtML

F. 文件与目录
来源：http://read.share.fehbvm.com/Article/details/gvyboabbu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grurdrgjs.sHtML

[F01] 读取整个文件
来源：http://wap.zdbjq.cn/Article/details/gdnjdwvhw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.zdbjq.cn/Article/details/gekwqzmax.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gryhstpin.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.hesvh.cn/Article/details/gsaztlybt.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gervsnjqd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gcyjrhodh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fehbvm.com/Article/details/gpzgnpyzf.sHtML

Ruby: File.read("a.txt")
来源：http://3g.zdbjq.cn/Article/details/goofppdom.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/grcywleej.sHtML

[F02] 逐行读取文件
来源：http://blog.hesvh.cn/Article/details/gmobitywd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.hesvh.cn/Article/details/gznlkpdlg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fehbvm.com/Article/details/gbuatfgkf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gzblvaaqu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gakdltfsv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gdbhiqysy.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.hesvh.cn/Article/details/gntjhnvpu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/gkcaxakxd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.hesvh.cn/Article/details/gdudgsyig.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.zdbjq.cn/Article/details/gjlcmsjqg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.fehbvm.com/Article/details/gnlgmxbxa.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/ggbrtjjvk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/ggrydnrqr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gloxukhdg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gbihpduks.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fehbvm.com/Article/details/gefolovwi.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fehbvm.com/Article/details/gbqiixhbr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gowvdfpeb.sHtML

[F04] 追加写入文件
来源：http://mobile.fehbvm.com/Article/details/gcpggcysl.sHtML


<!-- 参考信息 -->