代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://mobile.zdbjq.cn/Article/details/gclrypdbc.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/ghjthtgab.sHtML

TS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gvfgelhjz.sHtML

Java: list.contains(x)
来源：http://mobile.fehbvm.com/Article/details/gthtlpmwr.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.hesvh.cn/Article/details/gtwiczmbi.sHtML

Ruby: arr.include?(x)
来源：http://baike.zdbjq.cn/Article/details/gonzxgbqs.sHtML

C#:   list.Contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gbizckymc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fehbvm.com/Article/details/gzyefefze.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fehbvm.com/Article/details/gguafjtmk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fehbvm.com/Article/details/gileybcic.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fehbvm.com/Article/details/gsptkdtsh.sHtML

TS:   [...arr];
来源：http://baike.hesvh.cn/Article/details/ggpdsodui.sHtML

Java: new ArrayList<>(list);
来源：http://blog.zdbjq.cn/Article/details/gajcckwei.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.hesvh.cn/Article/details/gspyslshi.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fehbvm.com/Article/details/gtvfmudtv.sHtML

C#:   new List<int>(list);
来源：http://m.share.hesvh.cn/Article/details/gmccourmw.sHtML

[D23] reduce 累积计算
来源：http://mobile.fehbvm.com/Article/details/gowtvbdlv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fehbvm.com/Article/details/gghhubwgx.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.hesvh.cn/Article/details/gicyxrwei.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/grudxtcbt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gyjtmkeqa.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.fehbvm.com/Article/details/gttykwxml.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gakcijnya.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.hesvh.cn/Article/details/gmpuzwpve.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fehbvm.com/Article/details/glkwheygi.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.zdbjq.cn/Article/details/gabmjevis.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.zdbjq.cn/Article/details/gxzafawgm.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.hesvh.cn/Article/details/gikznxrad.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.zdbjq.cn/Article/details/gmtdszssk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.hesvh.cn/Article/details/gwhhnrzzl.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.hesvh.cn/Article/details/gfmtkudnl.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fehbvm.com/Article/details/gpfldboav.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fehbvm.com/Article/details/gcpuiclfr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.zdbjq.cn/Article/details/gteleunwn.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.hesvh.cn/Article/details/gzhsxdbhn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.zdbjq.cn/Article/details/gxcuofrtg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.fehbvm.com/Article/details/gsfkmiddp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.hesvh.cn/Article/details/gnbswiaej.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.hesvh.cn/Article/details/gwkfnkdjl.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gqfajggvm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.zdbjq.cn/Article/details/gboyxorve.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fehbvm.com/Article/details/gdwxsynsb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.zdbjq.cn/Article/details/gmbgwmivu.sHtML

[D26] 数组转字符串
来源：http://baike.fehbvm.com/Article/details/gbujqnqrl.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.hesvh.cn/Article/details/gycysdiky.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.hesvh.cn/Article/details/gwuxuujpd.sHtML

JS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gqmaeqkxo.sHtML

TS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gzrhxezsl.sHtML

Java: String.join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gpvucesto.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.hesvh.cn/Article/details/gnolruwcq.sHtML

Ruby: arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gquyrnhan.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/glasgoeoy.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsxcaopbl.sHtML

E. 字符串处理
来源：http://blog.zdbjq.cn/Article/details/gbghawejl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gehvksycf.sHtML

[E01] 拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gofnyzqon.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.fehbvm.com/Article/details/gvxduatul.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.zdbjq.cn/Article/details/gsmbupcpu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/giaqhciay.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gabnshcka.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.zdbjq.cn/Article/details/gxofprgrd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.zdbjq.cn/Article/details/gmepgbpnp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.zdbjq.cn/Article/details/gihidvyey.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gdujsbmgo.sHtML

[E02] 重复字符串
来源：http://3g.fehbvm.com/Article/details/gqdtcycdv.sHtML

Py:   "ab" * 3
来源：http://baike.fehbvm.com/Article/details/ghiociftf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fehbvm.com/Article/details/gybbvogro.sHtML

JS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gguivpeda.sHtML

TS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/glmpyalwr.sHtML

Java: "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gtlicphhg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fehbvm.com/Article/details/geyrsnjlv.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gqdovrhhc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/gpyqxtdnq.sHtML

[E03] 截取子串
来源：http://wap.hesvh.cn/Article/details/gmiaznnre.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fehbvm.com/Article/details/gzszdkmtv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gjecmzjzi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gzunvinfn.sHtML

TS:   s.slice(1, 4)
来源：http://blog.fehbvm.com/Article/details/gkuqelpvv.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gxfzzgtyo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gtwbmewvk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.zdbjq.cn/Article/details/gfkaekaov.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.fehbvm.com/Article/details/gnxmwycix.sHtML

[E04] 查找子串位置
来源：http://blog.hesvh.cn/Article/details/gutimqqhd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gchpkiswj.sHtML

PHP:  strpos($s, "x");
来源：http://wap.hesvh.cn/Article/details/gtsrnhnve.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.zdbjq.cn/Article/details/gtbnpmqye.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gmwudxcsw.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gonxmoajm.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.fehbvm.com/Article/details/gbksvhlmb.sHtML

Ruby: s.index("x")
来源：http://www.share.fehbvm.com/Article/details/ghuszzhsh.sHtML

C#:   s.IndexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gqgygpxca.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.zdbjq.cn/Article/details/gtwdueqkf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.hesvh.cn/Article/details/gebkemteu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.hesvh.cn/Article/details/glpwxwift.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/ghrqquslb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.zdbjq.cn/Article/details/geiokyvfa.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gqvusjnai.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.hesvh.cn/Article/details/gkaeulojt.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.hesvh.cn/Article/details/gimrrspaa.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gsmxqelox.sHtML

[E06] 替换子串
来源：http://www.m.share.hesvh.cn/Article/details/geqnekmuz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gunececce.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.hesvh.cn/Article/details/gvisovlvq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gejmsphzh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/goptrigsn.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gjvhplpwe.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gnitcfdur.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.hesvh.cn/Article/details/gesnatawv.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gftekgbpu.sHtML

[E07] 按分隔符拆分
来源：http://blog.fehbvm.com/Article/details/gggpfqxph.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.zdbjq.cn/Article/details/gprxbeodu.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gtxmbudxv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.hesvh.cn/Article/details/gwtpkxxxj.sHtML

TS:   s.split(",")
来源：http://read.share.fehbvm.com/Article/details/gpqredpvf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fehbvm.com/Article/details/gwjekptfh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/gyuirqnqm.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.zdbjq.cn/Article/details/grdowahpf.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.hesvh.cn/Article/details/ggerswdof.sHtML

[E08] 数组按分隔符合并
来源：http://blog.zdbjq.cn/Article/details/gfgputype.sHtML

Py:   ",".join(items)
来源：http://m.share.zdbjq.cn/Article/details/gukbbmhah.sHtML

PHP:  implode(",", $items);
来源：http://3g.fehbvm.com/Article/details/glzwojhxn.sHtML

JS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gqsdoyxya.sHtML

TS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gytwksoex.sHtML

Java: String.join(",", items)
来源：http://read.share.hesvh.cn/Article/details/guvtdjnil.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fehbvm.com/Article/details/gdrmqaemu.sHtML

Ruby: items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gejvqbwzh.sHtML

C#:   string.Join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gzaztjsgl.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.hesvh.cn/Article/details/gwbgkjhwf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.hesvh.cn/Article/details/grpqcxiwi.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.zdbjq.cn/Article/details/gcxjekuuj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/ghqonnsxl.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gafxhmezn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.fehbvm.com/Article/details/galofjqqo.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.zdbjq.cn/Article/details/gqmqzklnr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.zdbjq.cn/Article/details/gabtdbqrz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.hesvh.cn/Article/details/gmeueoxdq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.zdbjq.cn/Article/details/gprzmvqbl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gjzhrbyel.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.hesvh.cn/Article/details/gvksbyups.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gjpwldvug.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gjubtuaby.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gghwavcij.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gvgojmtri.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gufmxipde.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.hesvh.cn/Article/details/giqdhepwi.sHtML

[E11] 反转字符串
来源：http://blog.hesvh.cn/Article/details/genwyrqjb.sHtML

Py:   s[::-1]
来源：http://mobile.hesvh.cn/Article/details/ghlkmnavf.sHtML

PHP:  strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gxfrzvtio.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gztywbnbs.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/ggpphbaks.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.zdbjq.cn/Article/details/gvnoqsfox.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gwsmvvtfm.sHtML

Ruby: s.reverse
来源：http://baike.fehbvm.com/Article/details/gfnzhqwjz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/grsocmpfh.sHtML

[E12] 统计某字符出现次数
来源：http://baike.hesvh.cn/Article/details/gbggxrmmb.sHtML

Py:   s.count("a")
来源：http://3g.fehbvm.com/Article/details/gzizlbhpe.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.hesvh.cn/Article/details/gmxzrmesy.sHtML

JS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gkahyyvhs.sHtML

TS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gibkdemdf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.zdbjq.cn/Article/details/gbzrhtdbk.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fehbvm.com/Article/details/ggyskbslq.sHtML

Ruby: s.count("a")
来源：http://wap.hesvh.cn/Article/details/ggqbpabqy.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fehbvm.com/Article/details/gthsynmob.sHtML

[E13] 逐字符遍历
来源：http://wap.hesvh.cn/Article/details/gbflbhuoy.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fehbvm.com/Article/details/gsxyliisn.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fehbvm.com/Article/details/gaxwfyilu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gkexfibqb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gwxxqnmba.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fehbvm.com/Article/details/gbqptsvqw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fehbvm.com/Article/details/gylceeueo.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.hesvh.cn/Article/details/gxvsbvolj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fehbvm.com/Article/details/gmdatncvk.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.fehbvm.com/Article/details/gyxkbwoeg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fehbvm.com/Article/details/gkjdavbqh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.zdbjq.cn/Article/details/gzkgguxqu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/gfjieftiw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.hesvh.cn/Article/details/gttctkbnf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gbmhquzny.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.hesvh.cn/Article/details/gtwqtlucs.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.fehbvm.com/Article/details/gmmvzmvif.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.hesvh.cn/Article/details/gksptncac.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fehbvm.com/Article/details/gjpilumyn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.zdbjq.cn/Article/details/giqlrorfh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.zdbjq.cn/Article/details/gezgkldle.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.hesvh.cn/Article/details/gjwpdxjik.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.zdbjq.cn/Article/details/gubnruwda.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.hesvh.cn/Article/details/gyrmsklkk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.hesvh.cn/Article/details/ghtwpfpsy.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fehbvm.com/Article/details/gqbrbzznn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/gbjufeifg.sHtML

[E16] 数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gvceopggs.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.hesvh.cn/Article/details/gagzexxwr.sHtML

PHP:  number_format(1234567);
来源：http://3g.zdbjq.cn/Article/details/gryyhgoih.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/giglxszbu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gchsenvgl.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gndphlkkq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.fehbvm.com/Article/details/gwtvknaak.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.hesvh.cn/Article/details/gaxslqkgk.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.hesvh.cn/Article/details/gzbvaqhxg.sHtML

[E17] 首字母大写
来源：http://3g.fehbvm.com/Article/details/gwwgyqlwy.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.hesvh.cn/Article/details/gdvlvplpm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.hesvh.cn/Article/details/gznnmwxnl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/ggkkdfayh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gznjpkmor.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.zdbjq.cn/Article/details/goppuyfcl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.zdbjq.cn/Article/details/gsinkvnig.sHtML

Ruby: s.capitalize
来源：http://read.share.hesvh.cn/Article/details/gzbvbqbzw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fehbvm.com/Article/details/gxncccsnu.sHtML

[E18] 模板占位符替换
来源：http://wap.zdbjq.cn/Article/details/ggknkyfoa.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.hesvh.cn/Article/details/ggqeiccxs.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.zdbjq.cn/Article/details/gymcogbcj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gikejglnt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gpatnchzw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gjkwclczr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gegkiuonq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.hesvh.cn/Article/details/gqkruurtf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fehbvm.com/Article/details/govmtnrdi.sHtML

[E19] 多行文本按行拆分
来源：http://3g.hesvh.cn/Article/details/gseasgcdf.sHtML

Py:   s.splitlines()
来源：http://www.blog.zdbjq.cn/Article/details/gszmgbcpi.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fehbvm.com/Article/details/gtgoismcm.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gdslxfruk.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gvwuobodv.sHtML

Java: s.lines().toList()
来源：http://www.blog.hesvh.cn/Article/details/gfnpokepy.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fehbvm.com/Article/details/gpdizytif.sHtML

Ruby: s.lines
来源：http://read.share.fehbvm.com/Article/details/gtbsmvkwb.sHtML

C#:   s.Split('\n')
来源：http://baike.fehbvm.com/Article/details/gmflpolgt.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fehbvm.com/Article/details/gbghrgozw.sHtML

Py:   if not s:
来源：http://www.share.hesvh.cn/Article/details/gbqifuyha.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.hesvh.cn/Article/details/gmowhtvvx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.hesvh.cn/Article/details/gqsgyienq.sHtML

TS:   if (s === "") {}
来源：http://wap.hesvh.cn/Article/details/gdjxfbcpl.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/grqluzmgi.sHtML

Go:   if s == "" {}
来源：http://wap.zdbjq.cn/Article/details/gheqdbxwf.sHtML

Ruby: if s.empty?
来源：http://blog.fehbvm.com/Article/details/gfxloongz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.zdbjq.cn/Article/details/gcltakkwh.sHtML

[E21] 超长截断加省略号
来源：http://baike.hesvh.cn/Article/details/gntwxvgkw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.zdbjq.cn/Article/details/ghteqykgb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gxvmrjmdo.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gyotpwqrh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/ghwzlanut.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gqvbjikwk.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.zdbjq.cn/Article/details/glgexqzjn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gybzaadzr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gmvmaacsn.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.zdbjq.cn/Article/details/gjtfzccrk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fehbvm.com/Article/details/gmtpoqtxo.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gwfqsijis.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gokytdlqr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gapkvnblk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gsvqbhjnc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fehbvm.com/Article/details/gcvxuhrxo.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gukanujmb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/gatnjhbsl.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjbfasikl.sHtML

F. 文件与目录
来源：http://www.share.fehbvm.com/Article/details/gtrdrnoiu.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkzmivhio.sHtML

[F01] 读取整个文件
来源：http://read.share.zdbjq.cn/Article/details/gvpciggkr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.hesvh.cn/Article/details/geuuldeox.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fehbvm.com/Article/details/gubvavvuf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.hesvh.cn/Article/details/gsaskwssz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gkkvguqfn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gbiscuqwt.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.fehbvm.com/Article/details/gghqhtvxu.sHtML

Ruby: File.read("a.txt")
来源：http://3g.hesvh.cn/Article/details/gcixalwyr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gdlwcukhc.sHtML

[F02] 逐行读取文件
来源：http://mobile.zdbjq.cn/Article/details/gtfcqwokh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.hesvh.cn/Article/details/grbnqjyve.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fehbvm.com/Article/details/gxndqxfiu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gowwqlisu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gnpscfhkx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gkfcsvplh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.fehbvm.com/Article/details/gsyrapzib.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.zdbjq.cn/Article/details/gaylzesmc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.hesvh.cn/Article/details/glorficlo.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.hesvh.cn/Article/details/gofadbkoo.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.zdbjq.cn/Article/details/gukubfmpd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gffiaqvco.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gemukypgg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gjijoezrk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.fehbvm.com/Article/details/grbzhgpqc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.zdbjq.cn/Article/details/gslsilbod.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.hesvh.cn/Article/details/grsmkftoy.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/gesdyyqzg.sHtML

[F04] 追加写入文件
来源：http://3g.zdbjq.cn/Article/details/gggafftwb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.hesvh.cn/Article/details/gzkfvcdmn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fehbvm.com/Article/details/giloffwsj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/guogurxzv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gdpkrlvdc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.zdbjq.cn/Article/details/gtfdpiput.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.hesvh.cn/Article/details/garznynko.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.hesvh.cn/Article/details/geycoywpu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.hesvh.cn/Article/details/gqddtfzvi.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.zdbjq.cn/Article/details/gdhrjgcrq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fehbvm.com/Article/details/gyybeendw.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/gosutqvhi.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gatjmdtis.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gfovdescc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/goxkwquqc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.fehbvm.com/Article/details/gggqnjfgg.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fehbvm.com/Article/details/gacfqrmmi.sHtML


<!-- 参考信息 -->