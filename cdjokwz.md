代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gnapsvidd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gnxnbjoog.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fehbvm.com/Article/details/gbjqhpweh.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fehbvm.com/Article/details/gqguslhnq.sHtML

Ruby: arr.tally
来源：http://read.share.hesvh.cn/Article/details/gaojtumin.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.hesvh.cn/Article/details/grcqswanx.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fehbvm.com/Article/details/gumgytxwy.sHtML

Py:   x in arr
来源：http://3g.fehbvm.com/Article/details/gbadhiphf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.zdbjq.cn/Article/details/gzmxhfhug.sHtML

JS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gyffbleha.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gxpecvsoo.sHtML

Java: list.contains(x)
来源：http://www.share.fehbvm.com/Article/details/gpkujrgtk.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.zdbjq.cn/Article/details/grarbpeks.sHtML

Ruby: arr.include?(x)
来源：http://baike.fehbvm.com/Article/details/gjrjhibih.sHtML

C#:   list.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gotzvhkeg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.zdbjq.cn/Article/details/ginflggrv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fehbvm.com/Article/details/gfgaavenc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fehbvm.com/Article/details/golcukjjf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fehbvm.com/Article/details/gvjakoqqr.sHtML

TS:   [...arr];
来源：http://m.share.zdbjq.cn/Article/details/glmrxiecq.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fehbvm.com/Article/details/gqfymquhm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fehbvm.com/Article/details/gqnnaoqmj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.hesvh.cn/Article/details/geshemfde.sHtML

C#:   new List<int>(list);
来源：http://www.share.zdbjq.cn/Article/details/gutdbelwc.sHtML

[D23] reduce 累积计算
来源：http://baike.zdbjq.cn/Article/details/gmfgqehqw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gxerlbxln.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.hesvh.cn/Article/details/gowrxmznx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gsmizmhif.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gchedcujp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.hesvh.cn/Article/details/gqqibvirp.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gygkydvjq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fehbvm.com/Article/details/gjmagvxnz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.zdbjq.cn/Article/details/gntojpqbz.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fehbvm.com/Article/details/gnqlflzcs.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.hesvh.cn/Article/details/goavzboyl.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.zdbjq.cn/Article/details/gtfkppnmx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gqmhhnfmf.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gldxfgovc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.hesvh.cn/Article/details/gbbernguw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.zdbjq.cn/Article/details/gqguxszpi.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.zdbjq.cn/Article/details/ggiqedtxs.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.zdbjq.cn/Article/details/gzryietsh.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.hesvh.cn/Article/details/gijniyowj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.zdbjq.cn/Article/details/gronowkee.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fehbvm.com/Article/details/gsasbaydy.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.fehbvm.com/Article/details/gqvaiphns.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.zdbjq.cn/Article/details/goepqnoby.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gfgoxwlmo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.hesvh.cn/Article/details/gczneusfm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.hesvh.cn/Article/details/gmyehiiab.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gfncegmjk.sHtML

[D26] 数组转字符串
来源：http://www.share.hesvh.cn/Article/details/gcmtoabck.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.zdbjq.cn/Article/details/gapnlitfe.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/gfzbbwcvz.sHtML

JS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gzakabxph.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gnanqdtnw.sHtML

Java: String.join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gwjbednfl.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.hesvh.cn/Article/details/gxccakieq.sHtML

Ruby: arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gxqaofhfp.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gevpapxjc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gcvnuacvs.sHtML

E. 字符串处理
来源：http://baike.hesvh.cn/Article/details/gyuorfzyv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjtbfkdgz.sHtML

[E01] 拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gpynhlvtr.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.hesvh.cn/Article/details/gotkueqtw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.zdbjq.cn/Article/details/gpyoajrgn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gacsdflsp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gocvdgmjk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.fehbvm.com/Article/details/gfqufswxo.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gwigcsagr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.hesvh.cn/Article/details/gzapqwsnc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gduuyrvoi.sHtML

[E02] 重复字符串
来源：http://www.share.zdbjq.cn/Article/details/gxllljjmo.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/goyohbadk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fehbvm.com/Article/details/gpicgkohe.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gqzlbhafk.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/giyjupxpv.sHtML

Java: "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gpfpakkbk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.zdbjq.cn/Article/details/gxyacpyzg.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gqsbrfssu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.zdbjq.cn/Article/details/gebsnsfvk.sHtML

[E03] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gzqqyjpdd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.zdbjq.cn/Article/details/gsasfrfiw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gpxacwnqz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gyhncolrf.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/ghobathzg.sHtML

Java: s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/goukfcwhs.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gqbnqxccw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.fehbvm.com/Article/details/gmgttoyse.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.zdbjq.cn/Article/details/gpfnjvyll.sHtML

[E04] 查找子串位置
来源：http://m.share.fehbvm.com/Article/details/gkoidlvkx.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gcujsjfxs.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fehbvm.com/Article/details/gizpwfsxl.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.hesvh.cn/Article/details/gunhkuilk.sHtML

TS:   s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gmkhwbmei.sHtML

Java: s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gvrutbkbs.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.zdbjq.cn/Article/details/gqatcrijq.sHtML

Ruby: s.index("x")
来源：http://baike.hesvh.cn/Article/details/gfjkfpmag.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gtafmgvns.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fehbvm.com/Article/details/gbebuyvir.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.fehbvm.com/Article/details/gqriabgvh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.hesvh.cn/Article/details/gbvjjzeaa.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gwdzfxeao.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.hesvh.cn/Article/details/gvjothpgf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gyjfnahff.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.fehbvm.com/Article/details/gfhywrwkc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fehbvm.com/Article/details/gfsyudxjf.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gyzqitwvp.sHtML

[E06] 替换子串
来源：http://wap.zdbjq.cn/Article/details/gickfnnqy.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gmgswaagn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.zdbjq.cn/Article/details/gdatdgtcl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gtkbimtju.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/ghorpdqdy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/glwnatxdp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gaaiylcjx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.hesvh.cn/Article/details/gctmyupdj.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gtkgjeudx.sHtML

[E07] 按分隔符拆分
来源：http://mobile.zdbjq.cn/Article/details/gonrhfmwz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.fehbvm.com/Article/details/gjlhqemvu.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.hesvh.cn/Article/details/gmsavlyuk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.zdbjq.cn/Article/details/gneyyxsrl.sHtML

TS:   s.split(",")
来源：http://3g.hesvh.cn/Article/details/gxqnesfqt.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.fehbvm.com/Article/details/gcmoodymv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.zdbjq.cn/Article/details/gdiayydot.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.fehbvm.com/Article/details/ggxrvghre.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.hesvh.cn/Article/details/gjkayipuj.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fehbvm.com/Article/details/ggcwcltsk.sHtML

Py:   ",".join(items)
来源：http://3g.hesvh.cn/Article/details/gxuwqmcxi.sHtML

PHP:  implode(",", $items);
来源：http://3g.hesvh.cn/Article/details/glakgmfyg.sHtML

JS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/ggtjynarw.sHtML

TS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gkpzexbrw.sHtML

Java: String.join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gbajgbwgc.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.hesvh.cn/Article/details/gattpudir.sHtML

Ruby: items.join(",")
来源：http://baike.fehbvm.com/Article/details/gxgwkxifp.sHtML

C#:   string.Join(",", items)
来源：http://baike.hesvh.cn/Article/details/gnltzdigy.sHtML

[E09] 去除所有空白字符
来源：http://3g.zdbjq.cn/Article/details/gkkqgwiso.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.hesvh.cn/Article/details/glxihzali.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fehbvm.com/Article/details/gwxuuquxm.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gblnuaukz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gnomtkkcz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/ghlmcihyo.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.hesvh.cn/Article/details/gvkhyvhah.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fehbvm.com/Article/details/gwputhmnx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gmuwjskmw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fehbvm.com/Article/details/gsljkylag.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gawhnghzp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fehbvm.com/Article/details/ggsklncbz.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/glzfwosry.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/ghfnjjvvc.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gnatsduqp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gegyybjol.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/glvkxbbor.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.fehbvm.com/Article/details/gbrkqzvjc.sHtML

[E11] 反转字符串
来源：http://blog.hesvh.cn/Article/details/grpsscrlr.sHtML

Py:   s[::-1]
来源：http://blog.hesvh.cn/Article/details/gciensfzq.sHtML

PHP:  strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gcgtqbbxu.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/glotjylcy.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/geznpbsxl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gyrrlxaih.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gcaweppme.sHtML

Ruby: s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gpgsepwmj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/golzttmru.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fehbvm.com/Article/details/ghhwmtrhb.sHtML

Py:   s.count("a")
来源：http://blog.hesvh.cn/Article/details/gnmchffmd.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.zdbjq.cn/Article/details/govxpbmsc.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gakdxznhu.sHtML

TS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/ghmrvirfk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.hesvh.cn/Article/details/gsodmohus.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fehbvm.com/Article/details/gzynjwnmu.sHtML

Ruby: s.count("a")
来源：http://www.share.hesvh.cn/Article/details/glcxbafty.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.hesvh.cn/Article/details/gnuntwhei.sHtML

[E13] 逐字符遍历
来源：http://www.blog.hesvh.cn/Article/details/guhjpivgj.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.hesvh.cn/Article/details/gxqjzwndm.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.hesvh.cn/Article/details/grwhpfegt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gqqgrnmdr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gnpnwcxwv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/ggfhdliaj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.zdbjq.cn/Article/details/grfqehzgz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.fehbvm.com/Article/details/gqixtvozi.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fehbvm.com/Article/details/grsxfpzws.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fehbvm.com/Article/details/ggzpkeayf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fehbvm.com/Article/details/ggkkbxwwu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.hesvh.cn/Article/details/grqwpzwot.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.hesvh.cn/Article/details/gbyxyjoxv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.zdbjq.cn/Article/details/ggtdghgim.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gruldplak.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.zdbjq.cn/Article/details/gaulqwogl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.zdbjq.cn/Article/details/gacliejrr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.zdbjq.cn/Article/details/gfcruyrtb.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.zdbjq.cn/Article/details/goarlcmdt.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.zdbjq.cn/Article/details/ggsdrdqmk.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.hesvh.cn/Article/details/guqhoqrqv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.zdbjq.cn/Article/details/gdtbafgmh.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fehbvm.com/Article/details/gtoyrbrrn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.zdbjq.cn/Article/details/gefqedibt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fehbvm.com/Article/details/ggpewuenx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.hesvh.cn/Article/details/gapdfnotm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.hesvh.cn/Article/details/gtvhfqmey.sHtML

[E16] 数字千分位
来源：http://3g.hesvh.cn/Article/details/gqkistidx.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.zdbjq.cn/Article/details/gymnccctj.sHtML

PHP:  number_format(1234567);
来源：http://www.share.zdbjq.cn/Article/details/gpveqolei.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gqlunszld.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gtiuavldy.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gokvsfjvt.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.hesvh.cn/Article/details/gohkbfpre.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gxultdpkg.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.zdbjq.cn/Article/details/gqxccoyco.sHtML

[E17] 首字母大写
来源：http://blog.hesvh.cn/Article/details/gaargrepn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.fehbvm.com/Article/details/gzpfgqrhn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fehbvm.com/Article/details/ghvsjaxwp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gytwzortn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gvxdrupfq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.zdbjq.cn/Article/details/givoniqzh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fehbvm.com/Article/details/gvumhprxo.sHtML

Ruby: s.capitalize
来源：http://www.m.share.fehbvm.com/Article/details/gmydyfyuo.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.zdbjq.cn/Article/details/gkdxmxjvx.sHtML

[E18] 模板占位符替换
来源：http://wap.zdbjq.cn/Article/details/gozposjrh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.zdbjq.cn/Article/details/gumwvfups.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.hesvh.cn/Article/details/grsxthive.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gnnfvvulr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/ggalrtpkl.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gjuzrqdkb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gztxstovl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fehbvm.com/Article/details/gufxpqfmw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.zdbjq.cn/Article/details/gvhmrikea.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.zdbjq.cn/Article/details/gqrhqomyj.sHtML

Py:   s.splitlines()
来源：http://mobile.fehbvm.com/Article/details/gganymnwx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fehbvm.com/Article/details/gvbvjobxx.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gswbjrwjm.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/gmjhjjiix.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/gwuxgwiqv.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.zdbjq.cn/Article/details/gcepyzlpp.sHtML

Ruby: s.lines
来源：http://read.share.hesvh.cn/Article/details/guhsdoucm.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.hesvh.cn/Article/details/gdzmapmku.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.hesvh.cn/Article/details/gpdpgxkgv.sHtML

Py:   if not s:
来源：http://m.share.hesvh.cn/Article/details/gtmijlgmg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fehbvm.com/Article/details/gcopxcpgz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.hesvh.cn/Article/details/gqmbmodry.sHtML

TS:   if (s === "") {}
来源：http://wap.hesvh.cn/Article/details/gppjlmeta.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gprvjwbkg.sHtML

Go:   if s == "" {}
来源：http://blog.hesvh.cn/Article/details/gtqabviou.sHtML

Ruby: if s.empty?
来源：http://mobile.zdbjq.cn/Article/details/gsstpefiy.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdujgjjjs.sHtML

[E21] 超长截断加省略号
来源：http://blog.fehbvm.com/Article/details/ghmwnfzdc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/gsgoilafu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gcnkhwohv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gbvjggjnz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gljcuxjze.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/ghmyrwvlr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fehbvm.com/Article/details/glfdqtfum.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gzwbackog.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gtttcpqtf.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fehbvm.com/Article/details/gfdedjsjx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.hesvh.cn/Article/details/gahkccwht.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gzdaqdzgb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gborwzjlj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gyauertlg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gzyqsslrc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.zdbjq.cn/Article/details/grizdoffa.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gesagryjt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gojiuiusx.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdukbhlep.sHtML

F. 文件与目录
来源：http://mobile.fehbvm.com/Article/details/gbnkrbzvo.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxcqbvaeq.sHtML

[F01] 读取整个文件
来源：http://wap.fehbvm.com/Article/details/gohfbccze.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fehbvm.com/Article/details/gugrjqrmy.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.hesvh.cn/Article/details/glzmpolnu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fehbvm.com/Article/details/gazxlcxxb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fehbvm.com/Article/details/giiwztjas.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gsdtjhmbf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fehbvm.com/Article/details/gcdbuvafg.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gaaybhrir.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.fehbvm.com/Article/details/gnqokbjud.sHtML

[F02] 逐行读取文件
来源：http://blog.hesvh.cn/Article/details/gnoitklmy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/gqboeicaw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.hesvh.cn/Article/details/gwzctzzcj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gjstbgbfb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gwdyqeygd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gtnthqmpq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.fehbvm.com/Article/details/ggckqeopp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.zdbjq.cn/Article/details/gtlkiogqh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fehbvm.com/Article/details/ghnhhpunm.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fehbvm.com/Article/details/gxtssghbz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.zdbjq.cn/Article/details/gahjgwgim.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gbldaygex.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gdayypsid.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gfeocilet.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gifzqbabq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fehbvm.com/Article/details/glppxryvf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.hesvh.cn/Article/details/gwbisjsww.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gosdshqdy.sHtML

[F04] 追加写入文件
来源：http://baike.hesvh.cn/Article/details/grlxxljvi.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gjmcsdbyn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.zdbjq.cn/Article/details/guzqdepbw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/ghxcuacqx.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gdxfnlxoe.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.hesvh.cn/Article/details/gxnschdgi.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gnlosxoqw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/ghjczdelk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.hesvh.cn/Article/details/gzfeayfmv.sHtML


<!-- 参考信息 -->