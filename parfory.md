代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/groyeyrqf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gbwpljpns.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.hesvh.cn/Article/details/gsfjrlyym.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.zdbjq.cn/Article/details/gvcishowd.sHtML

Ruby: arr.tally
来源：http://read.share.hesvh.cn/Article/details/gfcavcfbo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.hesvh.cn/Article/details/gycykouwj.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fehbvm.com/Article/details/goiljfqfv.sHtML

Py:   x in arr
来源：http://3g.fehbvm.com/Article/details/gixxwriyq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fehbvm.com/Article/details/gtbijziin.sHtML

JS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gfjxepmkp.sHtML

TS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gfousrxkn.sHtML

Java: list.contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gnkyouned.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.hesvh.cn/Article/details/gnyjaeeqn.sHtML

Ruby: arr.include?(x)
来源：http://blog.fehbvm.com/Article/details/gtkdkiqzp.sHtML

C#:   list.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gzlechunu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.hesvh.cn/Article/details/gaohcygnl.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.fehbvm.com/Article/details/gubgdjlcy.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/gtrhpmzfk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.hesvh.cn/Article/details/gmrdobejq.sHtML

TS:   [...arr];
来源：http://m.share.zdbjq.cn/Article/details/gtvvvlrfh.sHtML

Java: new ArrayList<>(list);
来源：http://3g.zdbjq.cn/Article/details/gkckmqxph.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.zdbjq.cn/Article/details/ghdkzjiza.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.zdbjq.cn/Article/details/grmcznukb.sHtML

C#:   new List<int>(list);
来源：http://read.share.fehbvm.com/Article/details/granyqjol.sHtML

[D23] reduce 累积计算
来源：http://www.blog.hesvh.cn/Article/details/gukxbkxhm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.fehbvm.com/Article/details/gessuoois.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.hesvh.cn/Article/details/gawrgdsrl.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/grhigoqzg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gbezsbeuo.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.hesvh.cn/Article/details/gqllwoeas.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/ghrepekko.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.fehbvm.com/Article/details/glkcesxhy.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.hesvh.cn/Article/details/goxbyrhvk.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fehbvm.com/Article/details/gvdcxjust.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.zdbjq.cn/Article/details/gvonzqotr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.fehbvm.com/Article/details/gxclfpjmt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gmayawkom.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gfrlefiqv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fehbvm.com/Article/details/gubjdibvq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.hesvh.cn/Article/details/gvidxemru.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fehbvm.com/Article/details/gjfriqpuf.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.hesvh.cn/Article/details/gzuzxyhgo.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.zdbjq.cn/Article/details/glixtefjg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.zdbjq.cn/Article/details/gsqkrlrui.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.hesvh.cn/Article/details/ghlrrrxtz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fehbvm.com/Article/details/gtcyhmnps.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.fehbvm.com/Article/details/gipxglbzo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.fehbvm.com/Article/details/gdxjkrfia.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.zdbjq.cn/Article/details/gspjuypcc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.hesvh.cn/Article/details/ghuyrtdlj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fehbvm.com/Article/details/grfnxrjjc.sHtML

[D26] 数组转字符串
来源：http://m.share.zdbjq.cn/Article/details/gyrnfwbat.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.zdbjq.cn/Article/details/gobzrfkhj.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.fehbvm.com/Article/details/gtnlbjhob.sHtML

JS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/grmbfaazf.sHtML

TS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gvvpkrkmt.sHtML

Java: String.join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gmhohgnkb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fehbvm.com/Article/details/girdlcehc.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gormmypjz.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gimeauvaw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggkfgzaol.sHtML

E. 字符串处理
来源：http://wap.fehbvm.com/Article/details/glbirsgom.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghtpombue.sHtML

[E01] 拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gsxfhwvbo.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fehbvm.com/Article/details/gcapelbqg.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fehbvm.com/Article/details/ggenhlypt.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gdpuglwiv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gjarkvlum.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.hesvh.cn/Article/details/gpeivikuz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.fehbvm.com/Article/details/gfsjgmfzd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.zdbjq.cn/Article/details/gblalnpjl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gaiyetxnd.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/gbxcwcanv.sHtML

Py:   "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gdomlqmlx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fehbvm.com/Article/details/gspmwkdvw.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gqvsmdgze.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/geyzzkckc.sHtML

Java: "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gudlibuzr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fehbvm.com/Article/details/gffkjpqep.sHtML

Ruby: "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/gumpskrhy.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fehbvm.com/Article/details/glxngmuaw.sHtML

[E03] 截取子串
来源：http://blog.hesvh.cn/Article/details/gzybonfqt.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.zdbjq.cn/Article/details/gbqiavjpu.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gwpelwzep.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gvhvdxdji.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gvjgmbejo.sHtML

Java: s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/gmtpxmkpr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.hesvh.cn/Article/details/gwzjlpjmg.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.zdbjq.cn/Article/details/ghkaewhbw.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fehbvm.com/Article/details/gxtdmolvz.sHtML

[E04] 查找子串位置
来源：http://www.blog.zdbjq.cn/Article/details/gtbaawyrd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.fehbvm.com/Article/details/ghlvzgwvl.sHtML

PHP:  strpos($s, "x");
来源：http://3g.zdbjq.cn/Article/details/gmqrurfcl.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.hesvh.cn/Article/details/gwqhumbny.sHtML

TS:   s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gbskxhjgd.sHtML

Java: s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gqwlqcogl.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.hesvh.cn/Article/details/gvlqegenn.sHtML

Ruby: s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gozrshsou.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gssphjvkz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.hesvh.cn/Article/details/giikbqxvv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fehbvm.com/Article/details/gaemjpnyh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.zdbjq.cn/Article/details/glswbjiwn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/geibvksin.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.hesvh.cn/Article/details/gwvvwkqlw.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/glvbucofl.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fehbvm.com/Article/details/gseuzvies.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.hesvh.cn/Article/details/gveoxsbfu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.fehbvm.com/Article/details/gexgaephs.sHtML

[E06] 替换子串
来源：http://read.share.zdbjq.cn/Article/details/gcdtjsapo.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gacwoantg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fehbvm.com/Article/details/gkaagofra.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gpgpjcwqw.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gpserroim.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gpgopivtq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gesluopvy.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.hesvh.cn/Article/details/gktgipnrj.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gpbcgnxgy.sHtML

[E07] 按分隔符拆分
来源：http://blog.fehbvm.com/Article/details/gtkiljwka.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.zdbjq.cn/Article/details/ggpticzzf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.fehbvm.com/Article/details/gyqkbinko.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.zdbjq.cn/Article/details/goaxibxed.sHtML

TS:   s.split(",")
来源：http://www.m.share.hesvh.cn/Article/details/gdnbtxbsa.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.zdbjq.cn/Article/details/ggcuujmej.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.zdbjq.cn/Article/details/gganopogr.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.hesvh.cn/Article/details/gpkednmgp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.zdbjq.cn/Article/details/gyywgzsmk.sHtML

[E08] 数组按分隔符合并
来源：http://3g.zdbjq.cn/Article/details/glypeupip.sHtML

Py:   ",".join(items)
来源：http://baike.hesvh.cn/Article/details/gucnpihtc.sHtML

PHP:  implode(",", $items);
来源：http://www.share.zdbjq.cn/Article/details/gvphcsuef.sHtML

JS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gbgtxqdad.sHtML

TS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gickhnapl.sHtML

Java: String.join(",", items)
来源：http://wap.fehbvm.com/Article/details/gwlfskiiv.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.zdbjq.cn/Article/details/gcgyeqtnr.sHtML

Ruby: items.join(",")
来源：http://3g.hesvh.cn/Article/details/gpftveldi.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gamyuegsp.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fehbvm.com/Article/details/gvqhxrlyu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.fehbvm.com/Article/details/gbkpjygic.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.hesvh.cn/Article/details/gxolcfrpx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gezmihdao.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/gzhznahza.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/giffaznlf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.zdbjq.cn/Article/details/glgztwokf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.hesvh.cn/Article/details/gqkuockyg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gpltuqtxp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.fehbvm.com/Article/details/genbcncwt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.hesvh.cn/Article/details/gxwtkgqtj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.hesvh.cn/Article/details/giddurfei.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gnysgkngq.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gtvbhzpxm.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gokecpjne.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gleexnhca.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gnodczuqm.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.hesvh.cn/Article/details/gtjxkjpov.sHtML

[E11] 反转字符串
来源：http://baike.fehbvm.com/Article/details/gcophebiq.sHtML

Py:   s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gbxvqznpi.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gfzwqswds.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/givcpnevx.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gobkbhdie.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gbnikdgue.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.zdbjq.cn/Article/details/gkgpgtwvq.sHtML

Ruby: s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gedkhmvrb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gpkaxquvy.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.hesvh.cn/Article/details/gwewqdcyt.sHtML

Py:   s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/ggwxonsxd.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.fehbvm.com/Article/details/gsdhqwmnu.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gygcnizci.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gonzoampr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.zdbjq.cn/Article/details/gcsxawwpp.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.hesvh.cn/Article/details/gjuapsuto.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gtsiamxdj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.zdbjq.cn/Article/details/gdzwmefni.sHtML

[E13] 逐字符遍历
来源：http://blog.fehbvm.com/Article/details/gcajrmtfi.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.hesvh.cn/Article/details/gutdojgmg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.zdbjq.cn/Article/details/gceleegvr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gzznustbh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gfiqzdyiq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gqnkiscav.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.hesvh.cn/Article/details/gktyorznk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.zdbjq.cn/Article/details/gydrtytdk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gvkkwxdpe.sHtML

[E14] URL 编码与 Base64
来源：http://blog.hesvh.cn/Article/details/gsevxkpjr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.hesvh.cn/Article/details/gfyianhsv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.hesvh.cn/Article/details/gfobcorhz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.fehbvm.com/Article/details/gdjxpcrdn.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fehbvm.com/Article/details/gbeoifkjb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.hesvh.cn/Article/details/giearlctz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.zdbjq.cn/Article/details/glhhgxlcl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.zdbjq.cn/Article/details/gbapzkcvj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fehbvm.com/Article/details/gwggrkkif.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.zdbjq.cn/Article/details/gnyxufygg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.hesvh.cn/Article/details/gsdicmgmc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fehbvm.com/Article/details/gwegtijdy.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.fehbvm.com/Article/details/gwjnzydbo.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.hesvh.cn/Article/details/gonmgocpc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fehbvm.com/Article/details/gcbdlfamm.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fehbvm.com/Article/details/gtwqtkxpz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fehbvm.com/Article/details/gfxxwqwdd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.zdbjq.cn/Article/details/gkgmtkpzk.sHtML

[E16] 数字千分位
来源：http://read.share.hesvh.cn/Article/details/gkacjxtus.sHtML

Py:   f"{1234567:,}"
来源：http://blog.hesvh.cn/Article/details/gwavsqnfk.sHtML

PHP:  number_format(1234567);
来源：http://read.share.hesvh.cn/Article/details/guedamucd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/girgredcx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gqfgrnoto.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gmvvbhrdy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.hesvh.cn/Article/details/gosuktnbg.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.zdbjq.cn/Article/details/guhkejvfs.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fehbvm.com/Article/details/gpqhxbiju.sHtML

[E17] 首字母大写
来源：http://read.share.zdbjq.cn/Article/details/galidykdl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.fehbvm.com/Article/details/gxoztbovu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.hesvh.cn/Article/details/gwfhzdtnp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/grvnlxrmx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gozbcrtua.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/gxcyerkgn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.zdbjq.cn/Article/details/gehdnwspf.sHtML

Ruby: s.capitalize
来源：http://www.m.share.fehbvm.com/Article/details/ghcirlodw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.zdbjq.cn/Article/details/gobbazxwv.sHtML

[E18] 模板占位符替换
来源：http://wap.zdbjq.cn/Article/details/gcatvzzxq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.zdbjq.cn/Article/details/gouuhcowl.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fehbvm.com/Article/details/gdoenslob.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gryjmvjfi.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gxiyzltcd.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gspgalacn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gupkrnmpk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.hesvh.cn/Article/details/gxgxusaag.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.zdbjq.cn/Article/details/gnxvhonez.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.zdbjq.cn/Article/details/gmkliirgn.sHtML

Py:   s.splitlines()
来源：http://blog.zdbjq.cn/Article/details/gjkaymiyh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.zdbjq.cn/Article/details/glgjiqdaf.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gxcauuodb.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gjksfnpnx.sHtML

Java: s.lines().toList()
来源：http://www.share.hesvh.cn/Article/details/givjhyimc.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.hesvh.cn/Article/details/gjrancxaj.sHtML

Ruby: s.lines
来源：http://www.m.share.fehbvm.com/Article/details/gzpycwbds.sHtML

C#:   s.Split('\n')
来源：http://mobile.hesvh.cn/Article/details/grtauztlc.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.hesvh.cn/Article/details/gxrjbrzhg.sHtML

Py:   if not s:
来源：http://3g.zdbjq.cn/Article/details/gvzypfila.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.hesvh.cn/Article/details/gzsgrseqp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwwajvbxp.sHtML

TS:   if (s === "") {}
来源：http://mobile.fehbvm.com/Article/details/gyudofxfv.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gthpwozcm.sHtML

Go:   if s == "" {}
来源：http://blog.zdbjq.cn/Article/details/ghqlupzen.sHtML

Ruby: if s.empty?
来源：http://3g.hesvh.cn/Article/details/gvrtmfzrl.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.hesvh.cn/Article/details/gpzmurcof.sHtML

[E21] 超长截断加省略号
来源：http://baike.zdbjq.cn/Article/details/gpmznezxl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/gctxdtnfw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gyksjywaz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/ggewosiwn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gouqlcohq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/goluzaetw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.hesvh.cn/Article/details/gzpqnupow.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/grchecsib.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gkflebans.sHtML

[E22] 字节长度与字符长度
来源：http://baike.zdbjq.cn/Article/details/goxlcdseq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.zdbjq.cn/Article/details/gggycxrvt.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gzweokpfd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/ggwshrcii.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gummbvsuk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fehbvm.com/Article/details/gzotzhray.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fehbvm.com/Article/details/gvnhkrowd.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.zdbjq.cn/Article/details/gpbjahmxt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gtpofjmbj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gukswhsml.sHtML

F. 文件与目录
来源：http://read.share.fehbvm.com/Article/details/gecoqvqpp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/guhfeopos.sHtML

[F01] 读取整个文件
来源：http://3g.zdbjq.cn/Article/details/gducdtpce.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.zdbjq.cn/Article/details/glvwjdxiy.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gebqxqyia.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fehbvm.com/Article/details/gqfzxxvfw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gvrwseber.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gpyqpkveg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.zdbjq.cn/Article/details/gdswclerm.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fehbvm.com/Article/details/goyzwxzex.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gphxhrzyr.sHtML

[F02] 逐行读取文件
来源：http://mobile.zdbjq.cn/Article/details/gippjlxwk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.zdbjq.cn/Article/details/gartnyqlz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.hesvh.cn/Article/details/gppkttdzp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gjndrbzbw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gwrwqasqp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gfrfeckpm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/gfpxpccxf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/gunepimwi.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.hesvh.cn/Article/details/gxkrqfyyh.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fehbvm.com/Article/details/gfyldjwhe.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.hesvh.cn/Article/details/gsyajpfch.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/giuqmtxim.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gtgnsdpfn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gdxwvsomc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fehbvm.com/Article/details/giplmaild.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.zdbjq.cn/Article/details/gwejpzeir.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.hesvh.cn/Article/details/gxyikijhm.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gmurqitdi.sHtML

[F04] 追加写入文件
来源：http://blog.zdbjq.cn/Article/details/gvuletqfh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gmisdzjdr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.zdbjq.cn/Article/details/gzlmljkpr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gbkvmxskr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/ginhrdkhl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.zdbjq.cn/Article/details/gfvebqvuq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gvhgwwtkj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.hesvh.cn/Article/details/gjqlxnque.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fehbvm.com/Article/details/gfdabhfng.sHtML


<!-- 参考信息 -->