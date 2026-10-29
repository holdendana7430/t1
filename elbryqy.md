代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/ggcgycvpg.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gjqroslgd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fehbvm.com/Article/details/gilsopwvv.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fehbvm.com/Article/details/gpiiblfwk.sHtML

Ruby: arr.tally
来源：http://3g.fehbvm.com/Article/details/gltmfrjnk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.zdbjq.cn/Article/details/gfaiflkio.sHtML

[D21] 判断是否包含某元素
来源：http://baike.zdbjq.cn/Article/details/gswqktqpc.sHtML

Py:   x in arr
来源：http://baike.zdbjq.cn/Article/details/gpohxeltc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.zdbjq.cn/Article/details/goyqnaoqn.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gaiomsvph.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/ggoiqffnn.sHtML

Java: list.contains(x)
来源：http://www.share.fehbvm.com/Article/details/gcvulxoqn.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/grnnsiprp.sHtML

Ruby: arr.include?(x)
来源：http://3g.fehbvm.com/Article/details/gkodulptm.sHtML

C#:   list.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/guixgmace.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fehbvm.com/Article/details/gljsavjuv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.zdbjq.cn/Article/details/gepicjbum.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fehbvm.com/Article/details/gjysjhpyo.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.fehbvm.com/Article/details/gkuuhskoz.sHtML

TS:   [...arr];
来源：http://wap.fehbvm.com/Article/details/gjwabmeog.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fehbvm.com/Article/details/gelicrgmt.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fehbvm.com/Article/details/grteuukyu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fehbvm.com/Article/details/gmglpurkd.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gvqomneie.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/giljitony.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.hesvh.cn/Article/details/ggneqdkos.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.hesvh.cn/Article/details/gowjttiik.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gyprwsyyx.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/ghwbdcflc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.hesvh.cn/Article/details/gplyuexdy.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gxqmwksjd.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.zdbjq.cn/Article/details/geqjinnwt.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fehbvm.com/Article/details/gbhxprfzq.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.zdbjq.cn/Article/details/gmzptsuqx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.hesvh.cn/Article/details/gjacjkkwc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.hesvh.cn/Article/details/gthmzqodi.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.hesvh.cn/Article/details/gytgzahur.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.hesvh.cn/Article/details/gqojitovg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.zdbjq.cn/Article/details/gznikdieh.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.hesvh.cn/Article/details/guzgnucnz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.hesvh.cn/Article/details/gzraqfyfb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.zdbjq.cn/Article/details/gyhquxdvs.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fehbvm.com/Article/details/gyejtahye.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.fehbvm.com/Article/details/guxascaoy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.zdbjq.cn/Article/details/gpqzptocv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.hesvh.cn/Article/details/gzapxgnjz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/gyzhydgpy.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.hesvh.cn/Article/details/goyyebznp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.hesvh.cn/Article/details/gknmeztnc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.zdbjq.cn/Article/details/gioejxros.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fehbvm.com/Article/details/ggwjjbpha.sHtML

[D26] 数组转字符串
来源：http://read.share.fehbvm.com/Article/details/gvluzdpvb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.hesvh.cn/Article/details/gbcqguaof.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.fehbvm.com/Article/details/gwzeivfeb.sHtML

JS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gyxoyhvtc.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gkgoliqso.sHtML

Java: String.join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gnzezkubb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fehbvm.com/Article/details/gkgfdpogs.sHtML

Ruby: arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gezurywkm.sHtML

C#:   string.Join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gontioujg.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghzizbyrm.sHtML

E. 字符串处理
来源：http://3g.fehbvm.com/Article/details/gbmrcbzby.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gaduahrie.sHtML

[E01] 拼接字符串
来源：http://baike.fehbvm.com/Article/details/guuzwaole.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fehbvm.com/Article/details/gcyciozhy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.hesvh.cn/Article/details/ghwezpxvi.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gbgadmmzd.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gzpxiemod.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.zdbjq.cn/Article/details/gbifpnhwy.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fehbvm.com/Article/details/ghsivmani.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.zdbjq.cn/Article/details/ghkkvwglf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.hesvh.cn/Article/details/godsemmid.sHtML

[E02] 重复字符串
来源：http://blog.zdbjq.cn/Article/details/guyzulntl.sHtML

Py:   "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/googkkmhs.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.hesvh.cn/Article/details/gzqibvapn.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/ghmizkcfc.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gvflolhyg.sHtML

Java: "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gcbwrfcmu.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fehbvm.com/Article/details/gxxvqtgtu.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gtogdeqso.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.hesvh.cn/Article/details/gkjzelsuq.sHtML

[E03] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gcdqgsukf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.zdbjq.cn/Article/details/ggvwetxah.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gqoccgcwt.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gmcmzdmjg.sHtML

TS:   s.slice(1, 4)
来源：http://3g.fehbvm.com/Article/details/gyrgasjvb.sHtML

Java: s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gtohhvued.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/glcssgrci.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.zdbjq.cn/Article/details/gssbzfcfc.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.zdbjq.cn/Article/details/giabcbype.sHtML

[E04] 查找子串位置
来源：http://www.m.share.zdbjq.cn/Article/details/gbdiltdcs.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.hesvh.cn/Article/details/guxeljbhm.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fehbvm.com/Article/details/gmxqlozfq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.fehbvm.com/Article/details/gafveqbeg.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/ggydfhzgu.sHtML

Java: s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gpbszqwib.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.hesvh.cn/Article/details/giukuierk.sHtML

Ruby: s.index("x")
来源：http://3g.fehbvm.com/Article/details/gsedwwbko.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fehbvm.com/Article/details/gtwhsmump.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.hesvh.cn/Article/details/gjmzebqgd.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.fehbvm.com/Article/details/gtwptxhfr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.zdbjq.cn/Article/details/gmgxqxxsx.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gogftjgsj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.zdbjq.cn/Article/details/gjqxueepx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gpzpboylk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.zdbjq.cn/Article/details/gtqzihatz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.hesvh.cn/Article/details/gmcgdpnsx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gviyvfniw.sHtML

[E06] 替换子串
来源：http://read.share.fehbvm.com/Article/details/gttrlpiuu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gitvdsrkk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.hesvh.cn/Article/details/gqbxkoqoc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gityjmnge.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gfvdnnkqv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gyqanzmsg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gbeyrhavg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gqnjuryxe.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gjokzuatb.sHtML

[E07] 按分隔符拆分
来源：http://baike.zdbjq.cn/Article/details/gtvsbhdfw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.zdbjq.cn/Article/details/ggyfouxcl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.zdbjq.cn/Article/details/grbkcigeu.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.hesvh.cn/Article/details/gitjzeydp.sHtML

TS:   s.split(",")
来源：http://mobile.zdbjq.cn/Article/details/gqleakawd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.hesvh.cn/Article/details/gdrlzqahs.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fehbvm.com/Article/details/gjsploflp.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.fehbvm.com/Article/details/guoxgdooo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fehbvm.com/Article/details/gfxbfbzyw.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.hesvh.cn/Article/details/guwkidxby.sHtML

Py:   ",".join(items)
来源：http://m.share.hesvh.cn/Article/details/gwrkmzhvc.sHtML

PHP:  implode(",", $items);
来源：http://baike.zdbjq.cn/Article/details/gufodilep.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gwkbjelvb.sHtML

TS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gcwmmheoq.sHtML

Java: String.join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gnfzllakj.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.hesvh.cn/Article/details/gmggqhbfn.sHtML

Ruby: items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gyvfypreu.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gphduzibn.sHtML

[E09] 去除所有空白字符
来源：http://www.share.hesvh.cn/Article/details/gdxnvzmnz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.hesvh.cn/Article/details/gaaqlewan.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.hesvh.cn/Article/details/gqtqgkdvq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gtviljoec.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gcyvshdyt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/guooxuane.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.hesvh.cn/Article/details/gqndyljle.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.fehbvm.com/Article/details/gntaxmzfk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.hesvh.cn/Article/details/giooktnfk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fehbvm.com/Article/details/gchfnpudd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gfdkfctmf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.zdbjq.cn/Article/details/gsfqynkew.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gtkpceyzl.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gxfvldvdh.sHtML

Java: String.format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gqjrstmah.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gpulrafxz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gwclfrhmq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.zdbjq.cn/Article/details/gthfbubvi.sHtML

[E11] 反转字符串
来源：http://3g.fehbvm.com/Article/details/gylnbxrxl.sHtML

Py:   s[::-1]
来源：http://read.share.fehbvm.com/Article/details/guwcyxsgv.sHtML

PHP:  strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gewugbthd.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/ghvxluqdq.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gktbjnahu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gbowwjqhh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gpwpebqfj.sHtML

Ruby: s.reverse
来源：http://blog.hesvh.cn/Article/details/ggrsxdczu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/guvbovaqt.sHtML

[E12] 统计某字符出现次数
来源：http://wap.hesvh.cn/Article/details/ggueaayoj.sHtML

Py:   s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gswycaued.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.zdbjq.cn/Article/details/gidvwibjo.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gtdmfyzgo.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/ghendhglt.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fehbvm.com/Article/details/gkmugbvfh.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.zdbjq.cn/Article/details/gntkvkycn.sHtML

Ruby: s.count("a")
来源：http://m.share.fehbvm.com/Article/details/ghiynxtad.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.zdbjq.cn/Article/details/gvodnkdmg.sHtML

[E13] 逐字符遍历
来源：http://www.share.fehbvm.com/Article/details/gelizcilf.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.hesvh.cn/Article/details/gvxpvfjgs.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fehbvm.com/Article/details/gjbxumjav.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gzrrcpihf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwxzxqdzf.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gqnwzdrrq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.zdbjq.cn/Article/details/glnjgnsmf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.zdbjq.cn/Article/details/grbcvtlzp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.hesvh.cn/Article/details/ghcxzzrgv.sHtML

[E14] URL 编码与 Base64
来源：http://baike.fehbvm.com/Article/details/gjntfykas.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fehbvm.com/Article/details/gjxzbiash.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.hesvh.cn/Article/details/gpqjjjuuj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.hesvh.cn/Article/details/gfykcxtrw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.hesvh.cn/Article/details/gzzpvutjh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/gptyngdag.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.zdbjq.cn/Article/details/gachbqbgp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fehbvm.com/Article/details/gyplyyvdw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gyqcciiht.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fehbvm.com/Article/details/gumdpaxey.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.zdbjq.cn/Article/details/gmvcfatnm.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.hesvh.cn/Article/details/ghqkkgzyr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/gtuscsuuf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.hesvh.cn/Article/details/gjgmybies.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.zdbjq.cn/Article/details/gbrhkrevq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.hesvh.cn/Article/details/gfsxbiysb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fehbvm.com/Article/details/gitebcfeh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fehbvm.com/Article/details/grgxgfqzn.sHtML

[E16] 数字千分位
来源：http://blog.zdbjq.cn/Article/details/gzoakukra.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fehbvm.com/Article/details/gkxjvugdc.sHtML

PHP:  number_format(1234567);
来源：http://read.share.hesvh.cn/Article/details/geehrkoyw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gfjqjxvcl.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gcwgklpwe.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gmagdodzq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.zdbjq.cn/Article/details/glslotvto.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.hesvh.cn/Article/details/gygfpxmwy.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.hesvh.cn/Article/details/gvamebtyg.sHtML

[E17] 首字母大写
来源：http://3g.fehbvm.com/Article/details/gijigcfjo.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.hesvh.cn/Article/details/grerhpgsp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.hesvh.cn/Article/details/gzggfiylg.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gaabelsau.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gerceuayu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.hesvh.cn/Article/details/geqjjqqkw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fehbvm.com/Article/details/gsyddrlde.sHtML

Ruby: s.capitalize
来源：http://www.m.share.fehbvm.com/Article/details/gxfhwmeqd.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.zdbjq.cn/Article/details/girzhtwos.sHtML

[E18] 模板占位符替换
来源：http://wap.hesvh.cn/Article/details/gcecysewe.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.zdbjq.cn/Article/details/gwziulsgr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.fehbvm.com/Article/details/gbpajsdtp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/glzmmizpn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/glryiolkc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gybjpgbwy.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gzovbhhvd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.zdbjq.cn/Article/details/grxmofkoa.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.hesvh.cn/Article/details/gdwvftwjt.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.fehbvm.com/Article/details/giaauxrqm.sHtML

Py:   s.splitlines()
来源：http://read.share.zdbjq.cn/Article/details/gjeupjlkw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gpncnmfql.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gcmoojmoc.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/guirmhzzu.sHtML

Java: s.lines().toList()
来源：http://read.share.hesvh.cn/Article/details/gxzgwivyb.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.hesvh.cn/Article/details/gkbawfalx.sHtML

Ruby: s.lines
来源：http://www.share.zdbjq.cn/Article/details/gvcqnbngn.sHtML

C#:   s.Split('\n')
来源：http://mobile.hesvh.cn/Article/details/grgzwzcgu.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.fehbvm.com/Article/details/gqdxthzip.sHtML

Py:   if not s:
来源：http://blog.zdbjq.cn/Article/details/gpxukbgpq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/gxnyiqbne.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.zdbjq.cn/Article/details/gofavsdmj.sHtML

TS:   if (s === "") {}
来源：http://wap.zdbjq.cn/Article/details/gjberjygg.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gbiuxwrgb.sHtML

Go:   if s == "" {}
来源：http://baike.hesvh.cn/Article/details/grqozmoth.sHtML

Ruby: if s.empty?
来源：http://read.share.fehbvm.com/Article/details/gypsfmkug.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.zdbjq.cn/Article/details/gsznfnnbf.sHtML

[E21] 超长截断加省略号
来源：http://wap.zdbjq.cn/Article/details/gmczphadt.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fehbvm.com/Article/details/grnutmejj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.hesvh.cn/Article/details/ggajwkorz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/ggzdowsrr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/guensfwvs.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gumqbuarp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/gmispwjlg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gvzqrqllw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gjtnlzcap.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fehbvm.com/Article/details/gdmspbgmq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.zdbjq.cn/Article/details/gebhgsjda.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gpdzelpyr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gdjclnsld.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gtnevuaal.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gatwalgyl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fehbvm.com/Article/details/gqbjfyuer.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.zdbjq.cn/Article/details/gmhvywtwk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gnygfpzdn.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfdqgecrv.sHtML

F. 文件与目录
来源：http://3g.fehbvm.com/Article/details/gdqndbhag.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/genzfgtjm.sHtML

[F01] 读取整个文件
来源：http://mobile.zdbjq.cn/Article/details/gitkrudeb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.zdbjq.cn/Article/details/gygjvmxeo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gefhzlojj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fehbvm.com/Article/details/ggrqalnon.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.hesvh.cn/Article/details/gtgleycjk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gcvdrvivg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.zdbjq.cn/Article/details/gvbzmixlx.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fehbvm.com/Article/details/gbmxmsond.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gbyypybnl.sHtML

[F02] 逐行读取文件
来源：http://www.share.fehbvm.com/Article/details/gwslumjnt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.zdbjq.cn/Article/details/ggwkpypps.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.hesvh.cn/Article/details/gtdjnsljj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/guwhnuvwl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gfhvvqhgx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gtskkqizm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.zdbjq.cn/Article/details/gexprftsf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.fehbvm.com/Article/details/gxcahbmnf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.hesvh.cn/Article/details/gdxclgpgv.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.zdbjq.cn/Article/details/ghjuvwcqf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.zdbjq.cn/Article/details/gzljpdutq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gxjyzgmlx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gymqnnzgf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/ggefpvayz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.zdbjq.cn/Article/details/glohbshca.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.zdbjq.cn/Article/details/gziyqxqcu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fehbvm.com/Article/details/grvemyoln.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/ggnxqplsd.sHtML

[F04] 追加写入文件
来源：http://m.share.hesvh.cn/Article/details/gmfymlhis.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/gsumzqyux.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.zdbjq.cn/Article/details/gvyexcvuj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gemnqzhab.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/ggqcqkbkd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.zdbjq.cn/Article/details/gchheypvq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fehbvm.com/Article/details/gouroylrp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.hesvh.cn/Article/details/gbilbnbrw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/gjnibaduy.sHtML


<!-- 参考信息 -->