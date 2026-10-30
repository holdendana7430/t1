代发 wailian999

Ruby: arr.tally
来源：http://mobile.fehbvm.com/Article/details/gxajqpypp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fehbvm.com/Article/details/gsdgsmobd.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.hesvh.cn/Article/details/grynjvbyc.sHtML

Py:   x in arr
来源：http://wap.hesvh.cn/Article/details/gmykmjmyk.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gigucontq.sHtML

JS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gpapjlgbg.sHtML

TS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gyfpcxgnn.sHtML

Java: list.contains(x)
来源：http://blog.hesvh.cn/Article/details/ghoyermpz.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fehbvm.com/Article/details/gkgmpeucl.sHtML

Ruby: arr.include?(x)
来源：http://m.share.hesvh.cn/Article/details/grbtrylqm.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gwzjnxcnh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fehbvm.com/Article/details/giymemgnx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fehbvm.com/Article/details/gozltmxnd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fehbvm.com/Article/details/goynangkd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fehbvm.com/Article/details/giecseede.sHtML

TS:   [...arr];
来源：http://www.blog.zdbjq.cn/Article/details/gfswulpti.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.hesvh.cn/Article/details/gfrtxfqmo.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.hesvh.cn/Article/details/gmagdqqmn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.hesvh.cn/Article/details/gjglyspst.sHtML

C#:   new List<int>(list);
来源：http://baike.zdbjq.cn/Article/details/ghhgsndlp.sHtML

[D23] reduce 累积计算
来源：http://www.share.fehbvm.com/Article/details/giebgiklu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fehbvm.com/Article/details/gmchlhdgo.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.hesvh.cn/Article/details/ggyyxktmh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/ghjotqtuq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gnhtgoqra.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.zdbjq.cn/Article/details/gczmfryqh.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gnfoplujj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.zdbjq.cn/Article/details/gcezmdkwr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.zdbjq.cn/Article/details/gkezefwzh.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fehbvm.com/Article/details/gqfqzosnp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.zdbjq.cn/Article/details/gxroimknx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.zdbjq.cn/Article/details/gsypllioh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.fehbvm.com/Article/details/gdurmkyip.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gwvbfnqux.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.fehbvm.com/Article/details/giycmkfxf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fehbvm.com/Article/details/gyshtpohz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.hesvh.cn/Article/details/gisckrreo.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/gmxklywrx.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.zdbjq.cn/Article/details/gmknwuhiw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.zdbjq.cn/Article/details/gsajfpxnm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.zdbjq.cn/Article/details/gdhcvxoyg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.zdbjq.cn/Article/details/gxlhbjiqb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.hesvh.cn/Article/details/guhtcytqo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.fehbvm.com/Article/details/gsgisaivy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.zdbjq.cn/Article/details/gdgkzozlk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.hesvh.cn/Article/details/gedbwhtvq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.hesvh.cn/Article/details/ggafcebxb.sHtML

[D26] 数组转字符串
来源：http://m.share.zdbjq.cn/Article/details/gdjjkdgee.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.hesvh.cn/Article/details/gvfmsragp.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.zdbjq.cn/Article/details/gglyzeybk.sHtML

JS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gubcmxpoj.sHtML

TS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/ghtqnkpyh.sHtML

Java: String.join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gwbxbwydq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.hesvh.cn/Article/details/gyydbahkn.sHtML

Ruby: arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gbvzcxtzq.sHtML

C#:   string.Join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gxqnqqabv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkuhdtmgg.sHtML

E. 字符串处理
来源：http://www.m.share.zdbjq.cn/Article/details/gazdlyiut.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gztmnzoat.sHtML

[E01] 拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gqjuhkuqy.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.hesvh.cn/Article/details/gmmwlvfww.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fehbvm.com/Article/details/ggcnqnxte.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/guhkuxxtz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gajoftxts.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.hesvh.cn/Article/details/gvargletm.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fehbvm.com/Article/details/grimbdnnn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.hesvh.cn/Article/details/gyaaxljsw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fehbvm.com/Article/details/glknbvmbe.sHtML

[E02] 重复字符串
来源：http://www.share.fehbvm.com/Article/details/gwlkgngdx.sHtML

Py:   "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gxzejlonj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.hesvh.cn/Article/details/glwiioxst.sHtML

JS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gawdimdqq.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gktbweokz.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gthjtclxx.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.hesvh.cn/Article/details/guyelubsd.sHtML

Ruby: "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gkwcgluvv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.hesvh.cn/Article/details/gwdasahob.sHtML

[E03] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gjidejtzs.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.hesvh.cn/Article/details/gdvytgkyk.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gswowrdia.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/grjfxotef.sHtML

TS:   s.slice(1, 4)
来源：http://blog.zdbjq.cn/Article/details/geccwrznb.sHtML

Java: s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/gyfniryfz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.zdbjq.cn/Article/details/gkoehssdp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.zdbjq.cn/Article/details/gfwethsyz.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.zdbjq.cn/Article/details/gjpwgjidz.sHtML

[E04] 查找子串位置
来源：http://blog.fehbvm.com/Article/details/gfwysbyhs.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fehbvm.com/Article/details/gckwpmicv.sHtML

PHP:  strpos($s, "x");
来源：http://3g.zdbjq.cn/Article/details/gaeuqsupr.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.zdbjq.cn/Article/details/gbmfbpnkb.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/guupnzmji.sHtML

Java: s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gkdqjxujs.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fehbvm.com/Article/details/gsxlobecc.sHtML

Ruby: s.index("x")
来源：http://3g.hesvh.cn/Article/details/gtsjlpjqq.sHtML

C#:   s.IndexOf("x")
来源：http://3g.fehbvm.com/Article/details/gryhcyuko.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.hesvh.cn/Article/details/gzewhdclb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fehbvm.com/Article/details/gdlcqqmem.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.zdbjq.cn/Article/details/gyvnxowux.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gvrbsaswr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fehbvm.com/Article/details/glpglpgcx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/glbsaqtwl.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.hesvh.cn/Article/details/guekkjove.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fehbvm.com/Article/details/gmdefmjrr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gsxvdwuev.sHtML

[E06] 替换子串
来源：http://3g.fehbvm.com/Article/details/gtskvuoiq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gprfexnlg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.zdbjq.cn/Article/details/grpglnvva.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gihrgkdrp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gvnyhzqov.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/glklgdfpi.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/grzdtjhle.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/ggdbbnsyz.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.hesvh.cn/Article/details/gewfrxwql.sHtML

[E07] 按分隔符拆分
来源：http://blog.fehbvm.com/Article/details/ghfiiwhrb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.fehbvm.com/Article/details/giiviekkl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.fehbvm.com/Article/details/gxburfznf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fehbvm.com/Article/details/gbcdzdelx.sHtML

TS:   s.split(",")
来源：http://read.share.hesvh.cn/Article/details/gifuknwjf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fehbvm.com/Article/details/gfghihzwt.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.zdbjq.cn/Article/details/ghifnqdwu.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fehbvm.com/Article/details/gubnqkfvt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fehbvm.com/Article/details/gkplwydcd.sHtML

[E08] 数组按分隔符合并
来源：http://wap.hesvh.cn/Article/details/gwflpzygh.sHtML

Py:   ",".join(items)
来源：http://www.blog.zdbjq.cn/Article/details/gzarvcebt.sHtML

PHP:  implode(",", $items);
来源：http://www.share.zdbjq.cn/Article/details/gtsnqvrcq.sHtML

JS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gthtjxcxt.sHtML

TS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/ggsowohob.sHtML

Java: String.join(",", items)
来源：http://3g.hesvh.cn/Article/details/gtvhdnpdg.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.hesvh.cn/Article/details/gfjknrlad.sHtML

Ruby: items.join(",")
来源：http://wap.fehbvm.com/Article/details/grhaalzha.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gaiijulng.sHtML

[E09] 去除所有空白字符
来源：http://blog.hesvh.cn/Article/details/gtmzqokay.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.fehbvm.com/Article/details/gefkcoxrw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.hesvh.cn/Article/details/gryfrkugx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gywqgfgoi.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gqytzibkw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gswcjlhyh.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.fehbvm.com/Article/details/gmtxemqpy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.hesvh.cn/Article/details/gximtdsjo.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gfnrrihqg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.hesvh.cn/Article/details/gftyuugxf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fehbvm.com/Article/details/gagvvwwki.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.hesvh.cn/Article/details/gfuoxuzyl.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/giuyohahm.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gxvwobmsw.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/geacgiwln.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/ggfdjqygv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/geklupsdj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.zdbjq.cn/Article/details/gykolrmdp.sHtML

[E11] 反转字符串
来源：http://mobile.zdbjq.cn/Article/details/gwlbwujqz.sHtML

Py:   s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gyjfablhd.sHtML

PHP:  strrev($s);
来源：http://blog.hesvh.cn/Article/details/gdihuuynm.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gwnaxlkxi.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/ggfsotpxh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.fehbvm.com/Article/details/gcwrbkmhk.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gqdzwvbih.sHtML

Ruby: s.reverse
来源：http://read.share.hesvh.cn/Article/details/gshuabcrc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gsdmzhjxi.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.zdbjq.cn/Article/details/gqasaeuqn.sHtML

Py:   s.count("a")
来源：http://blog.hesvh.cn/Article/details/gztoyoxij.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/givtnqezs.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gbscsqsrj.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/gxpwxbezz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.zdbjq.cn/Article/details/gpzlcgifo.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.hesvh.cn/Article/details/gevekcmhu.sHtML

Ruby: s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gjwfkalmw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.zdbjq.cn/Article/details/gglmshxha.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gxbbqooya.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/gomzjpcqm.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.hesvh.cn/Article/details/ghpexcttk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gktrmzpai.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/ghcrvsvto.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/gbjnnkpsm.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fehbvm.com/Article/details/ginmcnmhw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.hesvh.cn/Article/details/grxqmaere.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gkjcfpxvw.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/gfqxqjnnd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fehbvm.com/Article/details/gbnhlemqp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.hesvh.cn/Article/details/gvtuvfjnv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.zdbjq.cn/Article/details/gdgrnrsoh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.hesvh.cn/Article/details/gggldnwzz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fehbvm.com/Article/details/giezhgipm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.fehbvm.com/Article/details/gjamkhxyy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.fehbvm.com/Article/details/grjtdfonx.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/grlnoksrw.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.zdbjq.cn/Article/details/gcyqxlbjz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fehbvm.com/Article/details/geoncokmg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.fehbvm.com/Article/details/ghbbliewg.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fehbvm.com/Article/details/gvzlrsmmp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.hesvh.cn/Article/details/gfoymwtjt.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.zdbjq.cn/Article/details/glzgknjmw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.zdbjq.cn/Article/details/guuplronk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.hesvh.cn/Article/details/grfmxlfhd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.hesvh.cn/Article/details/gpeawqeuh.sHtML

[E16] 数字千分位
来源：http://mobile.fehbvm.com/Article/details/gduurmzri.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.fehbvm.com/Article/details/gacbzptji.sHtML

PHP:  number_format(1234567);
来源：http://3g.fehbvm.com/Article/details/gbkvyrlhj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gerywfgok.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gjxiuptze.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.hesvh.cn/Article/details/gfsmpsqub.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.zdbjq.cn/Article/details/gyxuntkkv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fehbvm.com/Article/details/gvguhshmf.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fehbvm.com/Article/details/gjjfthafc.sHtML

[E17] 首字母大写
来源：http://3g.hesvh.cn/Article/details/gjiogkeur.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.zdbjq.cn/Article/details/ggcxszrsm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.fehbvm.com/Article/details/gspfjsgwq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gacqwrjrx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gwrhmoaoh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.hesvh.cn/Article/details/gvojgxedm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gnkyeufhe.sHtML

Ruby: s.capitalize
来源：http://www.m.share.fehbvm.com/Article/details/gkhqvguis.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.zdbjq.cn/Article/details/gcvcflzue.sHtML

[E18] 模板占位符替换
来源：http://baike.zdbjq.cn/Article/details/gmefbhmer.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.zdbjq.cn/Article/details/gkmmbgnxa.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.hesvh.cn/Article/details/gdhxmivfw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/geudpieaz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gkdldnlgc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gdckfqqih.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gmxejtmsd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.fehbvm.com/Article/details/gbateeqry.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.hesvh.cn/Article/details/gwxhxyojv.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fehbvm.com/Article/details/ghqmflxnv.sHtML

Py:   s.splitlines()
来源：http://wap.zdbjq.cn/Article/details/gmtnxiarr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.hesvh.cn/Article/details/gavaagzyf.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gtfcpasrd.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gponmpimh.sHtML

Java: s.lines().toList()
来源：http://3g.fehbvm.com/Article/details/guqpnxlxn.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.fehbvm.com/Article/details/ghjhdqhbz.sHtML

Ruby: s.lines
来源：http://blog.zdbjq.cn/Article/details/gxnutklaf.sHtML

C#:   s.Split('\n')
来源：http://baike.fehbvm.com/Article/details/gnjllwojy.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fehbvm.com/Article/details/gvnhtavnp.sHtML

Py:   if not s:
来源：http://mobile.fehbvm.com/Article/details/gjkxotarc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.hesvh.cn/Article/details/gzwdqtkzv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.fehbvm.com/Article/details/gkrbxrcba.sHtML

TS:   if (s === "") {}
来源：http://3g.zdbjq.cn/Article/details/gahppfrvm.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/ggmskktjy.sHtML

Go:   if s == "" {}
来源：http://www.blog.fehbvm.com/Article/details/gqzpwgjcd.sHtML

Ruby: if s.empty?
来源：http://m.share.fehbvm.com/Article/details/gsddqdwgp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.hesvh.cn/Article/details/gkieomndo.sHtML

[E21] 超长截断加省略号
来源：http://wap.fehbvm.com/Article/details/gygwqqsrq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.hesvh.cn/Article/details/giuplzyff.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gchntidpj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/glzbdyqrg.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gavsqdupb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gfjfcwlls.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fehbvm.com/Article/details/grndijhwn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gupsqnekv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gexpavmpm.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fehbvm.com/Article/details/gjraatxnw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fehbvm.com/Article/details/gfasvdpqj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gfnjphwsl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/golnifpto.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/ganswlitv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gqnxaopvt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.zdbjq.cn/Article/details/gkcjhqsbu.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.zdbjq.cn/Article/details/gpeaushnl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gjojyssln.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gyzuzqoce.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/ghtngyneq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ggafefxgy.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fehbvm.com/Article/details/gtziicsqm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/gyuhizvrl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gfvgreyja.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.zdbjq.cn/Article/details/gnguzzowy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fehbvm.com/Article/details/grisodsxn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gljvdskzt.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.hesvh.cn/Article/details/gyaruyrwf.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gcnxovksp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gohivaazl.sHtML

[F02] 逐行读取文件
来源：http://wap.fehbvm.com/Article/details/gszcbglje.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.hesvh.cn/Article/details/gnzeygyxo.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyrizdhpi.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/ghjsxaufp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gfcawznqz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gdndpfoup.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.hesvh.cn/Article/details/gvxbeoqnk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.hesvh.cn/Article/details/gfewuqnwc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.hesvh.cn/Article/details/gneiiqqhn.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fehbvm.com/Article/details/gpijoquds.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.zdbjq.cn/Article/details/gyvkewqym.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gvbwxvpuh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gfxqotwyx.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gddtcgvkx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.fehbvm.com/Article/details/gkkxsrgzj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fehbvm.com/Article/details/gfhjhcrmf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fehbvm.com/Article/details/gqafkrosn.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/glzdkavxp.sHtML

[F04] 追加写入文件
来源：http://m.share.hesvh.cn/Article/details/godvpzbhv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.zdbjq.cn/Article/details/ggjkwfryt.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.hesvh.cn/Article/details/gagyybmkp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gkydbrktd.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gojifrggh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.hesvh.cn/Article/details/gumdwkium.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.zdbjq.cn/Article/details/gptpijwne.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.hesvh.cn/Article/details/gnnjidveb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/ghagyxdmz.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.zdbjq.cn/Article/details/gqzhrrkav.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.hesvh.cn/Article/details/gnfyzllob.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gqnuzpoaa.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ghpgikbbi.sHtML


<!-- 参考信息 -->