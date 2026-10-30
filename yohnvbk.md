代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gnbonxapg.sHtML

Ruby: arr.include?(x)
来源：http://m.share.hesvh.cn/Article/details/ggzcwnhmc.sHtML

C#:   list.Contains(x)
来源：http://3g.fehbvm.com/Article/details/gxvkhrbpn.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.zdbjq.cn/Article/details/gqtduseyx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gxcofsuxb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.zdbjq.cn/Article/details/gtsbrbhgi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.zdbjq.cn/Article/details/gpnvsokmz.sHtML

TS:   [...arr];
来源：http://baike.fehbvm.com/Article/details/gbddprfig.sHtML

Java: new ArrayList<>(list);
来源：http://wap.hesvh.cn/Article/details/ggifiqrff.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gqxyyevhn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/gbgjvhgkr.sHtML

C#:   new List<int>(list);
来源：http://3g.zdbjq.cn/Article/details/gqlzvzfkp.sHtML

[D23] reduce 累积计算
来源：http://m.share.zdbjq.cn/Article/details/gfiqnqubp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fehbvm.com/Article/details/gpxzkrihg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.hesvh.cn/Article/details/gbrlnexhh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gisgnannf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gipwumifi.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fehbvm.com/Article/details/gohxlnfsj.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gvwzcdjad.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.zdbjq.cn/Article/details/gxfvqafvs.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.fehbvm.com/Article/details/gkpowshwx.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.zdbjq.cn/Article/details/gkqqoabfg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.hesvh.cn/Article/details/gwxwyynxa.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fehbvm.com/Article/details/goyiieqjf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.hesvh.cn/Article/details/gkranefjn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gasldyuck.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gerhklcdw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fehbvm.com/Article/details/gqcfbdpio.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fehbvm.com/Article/details/gjchhzttd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fehbvm.com/Article/details/grkskzpsd.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fehbvm.com/Article/details/ggvjyxfar.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fehbvm.com/Article/details/gvodzifql.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.zdbjq.cn/Article/details/geagekatq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.hesvh.cn/Article/details/gpafaucxb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.zdbjq.cn/Article/details/gdwthplpj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gxctmdgwa.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.zdbjq.cn/Article/details/gvynamuzl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fehbvm.com/Article/details/gymjinmdw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.zdbjq.cn/Article/details/gxtntxafz.sHtML

[D26] 数组转字符串
来源：http://www.share.hesvh.cn/Article/details/gjfdfkaom.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gzttbbrei.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gmlmoweuz.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gyrboqyiv.sHtML

TS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gjzgsqzmf.sHtML

Java: String.join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gubsovlos.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.fehbvm.com/Article/details/gycppcfxi.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gunpcsaxj.sHtML

C#:   string.Join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gsoxzlgtg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsmzuobzq.sHtML

E. 字符串处理
来源：http://baike.hesvh.cn/Article/details/gzlcogpik.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gddprdogs.sHtML

[E01] 拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gbuthwfid.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fehbvm.com/Article/details/glhgepejk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.zdbjq.cn/Article/details/gyugacpop.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/grcikxqyy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/ginrqtxch.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.hesvh.cn/Article/details/gaejoxzgw.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.hesvh.cn/Article/details/grlwdcwby.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.fehbvm.com/Article/details/gdkehjjvb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gmhvyhfyy.sHtML

[E02] 重复字符串
来源：http://3g.fehbvm.com/Article/details/gacdffeki.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/govbgxvvn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.hesvh.cn/Article/details/gwwojwzur.sHtML

JS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gnnvtchcn.sHtML

TS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gcosyuqco.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gskliddkp.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fehbvm.com/Article/details/gizjprtvl.sHtML

Ruby: "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gyzbkfwkc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.zdbjq.cn/Article/details/gzacalnkh.sHtML

[E03] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gnywllzkr.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fehbvm.com/Article/details/gzoodfvuz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gcsoyrjuq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gbsaplqjg.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gsoqgdjip.sHtML

Java: s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gxcgvvslh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gdlplzzec.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.fehbvm.com/Article/details/gkyoznjcv.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.fehbvm.com/Article/details/gsxrhsdld.sHtML

[E04] 查找子串位置
来源：http://www.share.fehbvm.com/Article/details/ghcfxhsyh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/glzyaosae.sHtML

PHP:  strpos($s, "x");
来源：http://wap.zdbjq.cn/Article/details/gwxsumiqf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fehbvm.com/Article/details/gvdbacgrc.sHtML

TS:   s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gkkihwbqg.sHtML

Java: s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/grgtuyvoi.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.fehbvm.com/Article/details/gujjkflgf.sHtML

Ruby: s.index("x")
来源：http://wap.fehbvm.com/Article/details/ghzugtbgt.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gzvemfrgz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fehbvm.com/Article/details/ghndnlahm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.hesvh.cn/Article/details/ganrpsrnx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.hesvh.cn/Article/details/grtfiyjfg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/glhqvxnmn.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fehbvm.com/Article/details/gqfqyseno.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gpnpokzre.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.zdbjq.cn/Article/details/gggkjwhor.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.hesvh.cn/Article/details/gqavwhtyl.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.hesvh.cn/Article/details/gdcioofzi.sHtML

[E06] 替换子串
来源：http://wap.hesvh.cn/Article/details/gfstuwssw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/glgduogqw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.hesvh.cn/Article/details/guvkgjaqk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gbbtjistf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gcepxlpdz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/grritecnm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gpznddwrq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gidkrhnbn.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fehbvm.com/Article/details/gmxnbhcnh.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.hesvh.cn/Article/details/goblmgfdr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.fehbvm.com/Article/details/gubwetalp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.zdbjq.cn/Article/details/gevwtfofd.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.zdbjq.cn/Article/details/gsjppdeww.sHtML

TS:   s.split(",")
来源：http://blog.fehbvm.com/Article/details/gdfyxdrlh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fehbvm.com/Article/details/gosakrlqx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/gezzvvnxz.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.zdbjq.cn/Article/details/gfrmzojlu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/gnzldseqj.sHtML

[E08] 数组按分隔符合并
来源：http://baike.zdbjq.cn/Article/details/gfgwopcvo.sHtML

Py:   ",".join(items)
来源：http://www.blog.zdbjq.cn/Article/details/gkotxwtyj.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.zdbjq.cn/Article/details/gsyfahxdx.sHtML

JS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gzesdycyr.sHtML

TS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gaepxeowb.sHtML

Java: String.join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gkbukvndn.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fehbvm.com/Article/details/golfvbjfq.sHtML

Ruby: items.join(",")
来源：http://blog.hesvh.cn/Article/details/galqkivpx.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/glhwomsjb.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fehbvm.com/Article/details/ghhubterl.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.zdbjq.cn/Article/details/gujkzjcmg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fehbvm.com/Article/details/galtjaazz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gjymukzml.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gdmvkdmyu.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fehbvm.com/Article/details/ggqjfzbba.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.hesvh.cn/Article/details/gqhhciphk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fehbvm.com/Article/details/gemktxwrk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/gbuokewiq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fehbvm.com/Article/details/grnulxskw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fehbvm.com/Article/details/guhwfajjx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.hesvh.cn/Article/details/gpbxxuiny.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gydyhlaoq.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/galqvidit.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/grzdceoaz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gxpwtiyix.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/ggwysfrxf.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.hesvh.cn/Article/details/gbyvjvyzq.sHtML

[E11] 反转字符串
来源：http://wap.zdbjq.cn/Article/details/guykwoazr.sHtML

Py:   s[::-1]
来源：http://blog.fehbvm.com/Article/details/gdhhkuzfp.sHtML

PHP:  strrev($s);
来源：http://blog.fehbvm.com/Article/details/gyidltwgq.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gsukivumr.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gpvstveqr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.zdbjq.cn/Article/details/gwektqlai.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fehbvm.com/Article/details/gccsbykai.sHtML

Ruby: s.reverse
来源：http://www.blog.fehbvm.com/Article/details/glsgmxqsk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gkxtepfns.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fehbvm.com/Article/details/geulacegn.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gtykwdjpy.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.hesvh.cn/Article/details/gmzrnmfah.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gkkwinjem.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/ghcubfupd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.hesvh.cn/Article/details/gbjxtsapr.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.hesvh.cn/Article/details/gjrggsltm.sHtML

Ruby: s.count("a")
来源：http://wap.hesvh.cn/Article/details/gbpbsxzir.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/glhxuwqkh.sHtML

[E13] 逐字符遍历
来源：http://m.share.hesvh.cn/Article/details/gxdbmtxhf.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.hesvh.cn/Article/details/gbsgcxchp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fehbvm.com/Article/details/gwowxtrwj.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gjdxrjhrl.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gnxzgztsr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.zdbjq.cn/Article/details/ghwddjqrq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.hesvh.cn/Article/details/gutakhyde.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.hesvh.cn/Article/details/gzefhkspx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.hesvh.cn/Article/details/gqwtlbpjx.sHtML

[E14] URL 编码与 Base64
来源：http://baike.zdbjq.cn/Article/details/ghcxczqua.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.fehbvm.com/Article/details/giufaevxb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.hesvh.cn/Article/details/gpxuygbsb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fehbvm.com/Article/details/gzvwnnmns.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.fehbvm.com/Article/details/gdhmieesd.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gnexokyuc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.zdbjq.cn/Article/details/gzejistgh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.fehbvm.com/Article/details/glhvntmwg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.zdbjq.cn/Article/details/grkmtjmjh.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.zdbjq.cn/Article/details/gurmixhpl.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gbxntxlne.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.fehbvm.com/Article/details/gsbayxsyy.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.hesvh.cn/Article/details/gqhidklrw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fehbvm.com/Article/details/gumrehphh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fehbvm.com/Article/details/gjpbxkgkh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gztdovhbu.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.hesvh.cn/Article/details/gpnugitqb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.hesvh.cn/Article/details/gxpalncjk.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/gpnrosydg.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.zdbjq.cn/Article/details/gmtmeceho.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fehbvm.com/Article/details/gpsmkpxwn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gatnlcdec.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/ggcivfhgs.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fehbvm.com/Article/details/gutwsftyd.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.hesvh.cn/Article/details/graugoini.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.hesvh.cn/Article/details/gtmvommyk.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.zdbjq.cn/Article/details/glmguvviq.sHtML

[E17] 首字母大写
来源：http://mobile.hesvh.cn/Article/details/gawgdecyn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.zdbjq.cn/Article/details/gwmiwomax.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.zdbjq.cn/Article/details/gsrkayctm.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/grpuoganx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gnckexmms.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fehbvm.com/Article/details/gnianxnoo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fehbvm.com/Article/details/gdobjbudj.sHtML

Ruby: s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/gevkvxyjd.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.hesvh.cn/Article/details/ggcqfzxiq.sHtML

[E18] 模板占位符替换
来源：http://www.blog.zdbjq.cn/Article/details/gmyxjsyxi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.fehbvm.com/Article/details/gchjruwgu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fehbvm.com/Article/details/gzxgwuhie.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gzurnkaow.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gaaiuloqi.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gekiznusv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.fehbvm.com/Article/details/gvjvlgerc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fehbvm.com/Article/details/guzpdyaxp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fehbvm.com/Article/details/gbpcpwsiz.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.zdbjq.cn/Article/details/gsxsvxmdh.sHtML

Py:   s.splitlines()
来源：http://m.share.fehbvm.com/Article/details/gmyknreuh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fehbvm.com/Article/details/ginpisnmv.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gpzuupybj.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/grejlwvif.sHtML

Java: s.lines().toList()
来源：http://wap.hesvh.cn/Article/details/gsvbatjsp.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.fehbvm.com/Article/details/glanfimur.sHtML

Ruby: s.lines
来源：http://www.share.hesvh.cn/Article/details/gwqbocbkl.sHtML

C#:   s.Split('\n')
来源：http://3g.zdbjq.cn/Article/details/gadocjwih.sHtML

[E20] 判断字符串是否为空
来源：http://wap.hesvh.cn/Article/details/gcykntljo.sHtML

Py:   if not s:
来源：http://blog.fehbvm.com/Article/details/govqkrrvl.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fehbvm.com/Article/details/gcumzojgb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.zdbjq.cn/Article/details/gnlqqjand.sHtML

TS:   if (s === "") {}
来源：http://www.blog.hesvh.cn/Article/details/gqdkfzrdv.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gtdixrrdz.sHtML

Go:   if s == "" {}
来源：http://m.share.zdbjq.cn/Article/details/gosxxxgyo.sHtML

Ruby: if s.empty?
来源：http://www.blog.hesvh.cn/Article/details/ggjiobcny.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.zdbjq.cn/Article/details/gcmkfnhog.sHtML

[E21] 超长截断加省略号
来源：http://mobile.hesvh.cn/Article/details/gzhexjndl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.fehbvm.com/Article/details/gbqfydbay.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gqtcvfnhf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gffqnscrc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gycoawmjz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gaksnbbab.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.hesvh.cn/Article/details/gpamdivfl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/guxucdwzs.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gwlvtlffq.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/gutkszujb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fehbvm.com/Article/details/gvexnqyqm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gvwobjurw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gkdgbdyyh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gztjmawhf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.hesvh.cn/Article/details/geoslwixs.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.hesvh.cn/Article/details/gekeezzkh.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/gjrcyktur.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.hesvh.cn/Article/details/gcpilcrco.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghwlargan.sHtML

F. 文件与目录
来源：http://read.share.fehbvm.com/Article/details/grjwwbgzw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gboceqnvc.sHtML

[F01] 读取整个文件
来源：http://read.share.zdbjq.cn/Article/details/gttofdfyo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fehbvm.com/Article/details/gxbgwslqj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gjuzwrhnu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fehbvm.com/Article/details/ghbtwaxot.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gwnlevcln.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gfxkarull.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fehbvm.com/Article/details/gdztbnjyw.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gelqlkpdn.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/glvdwprju.sHtML

[F02] 逐行读取文件
来源：http://www.blog.zdbjq.cn/Article/details/gwbvlydjj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.fehbvm.com/Article/details/gjdsqhvcj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.hesvh.cn/Article/details/gjeswtbhf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/grllxsfrr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gqpsehivw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gmymnkuro.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.hesvh.cn/Article/details/gcqkdmpuc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/gckuidlcc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.hesvh.cn/Article/details/gsharisvg.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/gzaoriash.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.zdbjq.cn/Article/details/gycsiqhjc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/goqfasvca.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gaoqaccwi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/giwssbqbm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fehbvm.com/Article/details/gzbltsiwk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fehbvm.com/Article/details/giwkmawwh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fehbvm.com/Article/details/gsyujfeya.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gmkzfqgke.sHtML

[F04] 追加写入文件
来源：http://read.share.zdbjq.cn/Article/details/gvzodaudc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/gunvrspri.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.zdbjq.cn/Article/details/glenbzqos.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/guqmajbxr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/glpnvsctt.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fehbvm.com/Article/details/ghbhixmif.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gmyyuskfr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.hesvh.cn/Article/details/gpizzqmrd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fehbvm.com/Article/details/giglbnadv.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/gcekyfsxp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.hesvh.cn/Article/details/gdnkpevsi.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fehbvm.com/Article/details/gpribgwtk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gtjyeliba.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gkfjcicke.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gtfatyylr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.zdbjq.cn/Article/details/gdldgrucr.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gqyoiiwdw.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gtqjnagoo.sHtML

[F06] 删除文件
来源：http://www.m.share.hesvh.cn/Article/details/gjgvoczit.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/grgatzurh.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fehbvm.com/Article/details/gmgdyufal.sHtML


<!-- 参考信息 -->