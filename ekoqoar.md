代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gxqoncowb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gtudfyvfv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.hesvh.cn/Article/details/gmkddiucf.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.hesvh.cn/Article/details/gvllywcnk.sHtML

Ruby: arr.tally
来源：http://www.share.fehbvm.com/Article/details/guiexgcjz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.zdbjq.cn/Article/details/gvqstlqbc.sHtML

[D21] 判断是否包含某元素
来源：http://3g.zdbjq.cn/Article/details/gosnzrucn.sHtML

Py:   x in arr
来源：http://3g.zdbjq.cn/Article/details/gtetarjuh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.zdbjq.cn/Article/details/gwmlkplqp.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/grakaxmmj.sHtML

TS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gutophopj.sHtML

Java: list.contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/ghjtbvyqt.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gwvdmrrih.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/gpssoftdy.sHtML

C#:   list.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gsylvjzgk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fehbvm.com/Article/details/gpazbxetk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fehbvm.com/Article/details/gywbpkwzf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.hesvh.cn/Article/details/glhisqrfw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.fehbvm.com/Article/details/guifhcdtg.sHtML

TS:   [...arr];
来源：http://wap.hesvh.cn/Article/details/gitrvcekf.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gfxeujcgl.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fehbvm.com/Article/details/gzmfvbiuw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.fehbvm.com/Article/details/gzddjmlxe.sHtML

C#:   new List<int>(list);
来源：http://m.share.fehbvm.com/Article/details/gmwimsyyh.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/ggjlxewpb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.hesvh.cn/Article/details/gtfzvysmc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.hesvh.cn/Article/details/gwfnjzkec.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gzomjdoyl.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gjzhxszpq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.zdbjq.cn/Article/details/gnnxekqzw.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gqwcpkgig.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.zdbjq.cn/Article/details/gajvlqahy.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.zdbjq.cn/Article/details/gunldwqyq.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.hesvh.cn/Article/details/gdfkfnvfg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fehbvm.com/Article/details/ghkibrcbd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.zdbjq.cn/Article/details/gbaxbzsof.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fehbvm.com/Article/details/gwjjmnvtk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gngvauzpr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.zdbjq.cn/Article/details/globlmmdl.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.zdbjq.cn/Article/details/gqjecgaac.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.zdbjq.cn/Article/details/gwxygwhgt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/gfojursiz.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fehbvm.com/Article/details/gffvyicxh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.zdbjq.cn/Article/details/gedspgnqo.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.zdbjq.cn/Article/details/gasodnuau.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.zdbjq.cn/Article/details/gtsrxtjtv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.fehbvm.com/Article/details/ggdlhlyvr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.fehbvm.com/Article/details/gnfymmgns.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.hesvh.cn/Article/details/garkxfkur.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.hesvh.cn/Article/details/gyfpigozw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/gkxrhbfiv.sHtML

[D26] 数组转字符串
来源：http://baike.zdbjq.cn/Article/details/gnarnsozl.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.hesvh.cn/Article/details/gcjsgpobr.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.zdbjq.cn/Article/details/gwjdycrve.sHtML

JS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gcltxqitc.sHtML

TS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gutowgwqf.sHtML

Java: String.join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gmdxgwceg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.hesvh.cn/Article/details/gdcuqymcz.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gsibqotro.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gkwdoytzw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/giexuafff.sHtML

E. 字符串处理
来源：http://www.m.share.zdbjq.cn/Article/details/gczzddodx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gclvqvbez.sHtML

[E01] 拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gvbqqgikw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.hesvh.cn/Article/details/gmizwbgki.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.hesvh.cn/Article/details/gjrfxukyc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gpqzhizhy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gfbbhmmdu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.hesvh.cn/Article/details/glwqhogxp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.hesvh.cn/Article/details/gqucopede.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fehbvm.com/Article/details/glrmdlesw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gehczstgg.sHtML

[E02] 重复字符串
来源：http://mobile.fehbvm.com/Article/details/gliafggfw.sHtML

Py:   "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gvfzzcrlw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gldedggvg.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gebozbktk.sHtML

TS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gfruavths.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gvykorldb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.zdbjq.cn/Article/details/gzestjijm.sHtML

Ruby: "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gezdurpmh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/geowttbgm.sHtML

[E03] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gmksqcnpx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.zdbjq.cn/Article/details/ggzaufpnn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/grptvwtxu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gocjndzfk.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gvdumslpe.sHtML

Java: s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/grrzxzved.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.zdbjq.cn/Article/details/gmarfbrry.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.zdbjq.cn/Article/details/gyfezflhf.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.zdbjq.cn/Article/details/glvgfhbhd.sHtML

[E04] 查找子串位置
来源：http://read.share.hesvh.cn/Article/details/gtfrtvneb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/goaurduer.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fehbvm.com/Article/details/gteancxnp.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fehbvm.com/Article/details/gajqbmuzi.sHtML

TS:   s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/guwgzjbjp.sHtML

Java: s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/gikdmtafh.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.hesvh.cn/Article/details/gqrakzvbc.sHtML

Ruby: s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gophjrzzb.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.hesvh.cn/Article/details/goghdklfp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.zdbjq.cn/Article/details/gedvcpnvt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fehbvm.com/Article/details/gccksvzms.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.hesvh.cn/Article/details/goolegpug.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gfyvherjn.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fehbvm.com/Article/details/gvjspdujt.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gtupftfym.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.zdbjq.cn/Article/details/glxirqvtf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.hesvh.cn/Article/details/gmxdyywwr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.hesvh.cn/Article/details/gwgtccutc.sHtML

[E06] 替换子串
来源：http://www.blog.hesvh.cn/Article/details/gefwzuqde.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gwlxfdexp.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.hesvh.cn/Article/details/ggkbgtumj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/guwjwjgly.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gjixqpahw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gqfkpefts.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gwiudvszy.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.hesvh.cn/Article/details/gbmaycaac.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gsqjlpveo.sHtML

[E07] 按分隔符拆分
来源：http://read.share.zdbjq.cn/Article/details/gsdraqnkm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.zdbjq.cn/Article/details/gfvkkxunv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.fehbvm.com/Article/details/gjpnepqdb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.hesvh.cn/Article/details/gqmdmlppc.sHtML

TS:   s.split(",")
来源：http://3g.fehbvm.com/Article/details/gcxxoxzth.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.zdbjq.cn/Article/details/gfhcithlp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fehbvm.com/Article/details/grkkdmlhu.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.hesvh.cn/Article/details/gllbjrehz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.zdbjq.cn/Article/details/gpbekrfio.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fehbvm.com/Article/details/ggfzvovqw.sHtML

Py:   ",".join(items)
来源：http://www.m.share.hesvh.cn/Article/details/gowiumqec.sHtML

PHP:  implode(",", $items);
来源：http://www.share.zdbjq.cn/Article/details/gskkmhkty.sHtML

JS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gqeoupmtg.sHtML

TS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gdfwjwodz.sHtML

Java: String.join(",", items)
来源：http://baike.hesvh.cn/Article/details/giupyekxi.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.hesvh.cn/Article/details/gkfwforay.sHtML

Ruby: items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gtfjdteau.sHtML

C#:   string.Join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gbpjvlqiv.sHtML

[E09] 去除所有空白字符
来源：http://baike.zdbjq.cn/Article/details/gaismlgdz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.fehbvm.com/Article/details/gioqnhdgb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fehbvm.com/Article/details/gehhgeghh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gshbkuuap.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gsbsbvarm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.hesvh.cn/Article/details/gzzoxnrhx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.zdbjq.cn/Article/details/gaxxzpczh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.hesvh.cn/Article/details/gvnsboitn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.fehbvm.com/Article/details/grtzdybyl.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/gpdyjhgop.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.zdbjq.cn/Article/details/ghzfzngah.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.hesvh.cn/Article/details/gykxexsnm.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gggknhlqh.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gxsnrutwj.sHtML

Java: String.format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gduslprky.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gzddkkokj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gpzahzciu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.zdbjq.cn/Article/details/ghwxkvtpn.sHtML

[E11] 反转字符串
来源：http://wap.zdbjq.cn/Article/details/glqqhwwvi.sHtML

Py:   s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gpqqitbme.sHtML

PHP:  strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gvisjqxtg.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gbfwfkbgr.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gthetgpux.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.hesvh.cn/Article/details/gsxgmhjdd.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.hesvh.cn/Article/details/gqekeouol.sHtML

Ruby: s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gzcgnccii.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gvmakjwxg.sHtML

[E12] 统计某字符出现次数
来源：http://wap.fehbvm.com/Article/details/gldtszzbp.sHtML

Py:   s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gmamxzemj.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.hesvh.cn/Article/details/gcuzifprp.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gjlorlqtp.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gltifrzvq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.zdbjq.cn/Article/details/gybgtruok.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.hesvh.cn/Article/details/gkizwhxlm.sHtML

Ruby: s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/ggukkprxy.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.hesvh.cn/Article/details/gepmbiwxx.sHtML

[E13] 逐字符遍历
来源：http://blog.hesvh.cn/Article/details/gbcnzkypc.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.zdbjq.cn/Article/details/gidmiwpam.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fehbvm.com/Article/details/gyokrfgnq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/glnfeudrz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gtgnubhpu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.hesvh.cn/Article/details/gzzitjinm.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fehbvm.com/Article/details/gzffvevpd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.zdbjq.cn/Article/details/gjvzyosta.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gygnwyuao.sHtML

[E14] URL 编码与 Base64
来源：http://baike.zdbjq.cn/Article/details/gsgneduqi.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.zdbjq.cn/Article/details/giyrivqpu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/geyccphez.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.hesvh.cn/Article/details/gtgivpnjj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.zdbjq.cn/Article/details/gvkmhagzp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.zdbjq.cn/Article/details/guroapmjg.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.zdbjq.cn/Article/details/gneesbwyl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.zdbjq.cn/Article/details/gckbxeavt.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/ghwqskrlg.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/gazwyynwy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.fehbvm.com/Article/details/gytqiinwv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gpbpdwmrx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.zdbjq.cn/Article/details/gakalmape.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fehbvm.com/Article/details/gtksgnwto.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.fehbvm.com/Article/details/goedrazil.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.zdbjq.cn/Article/details/gxlcisoes.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.hesvh.cn/Article/details/gczwaidns.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.zdbjq.cn/Article/details/gylcqjzds.sHtML

[E16] 数字千分位
来源：http://www.share.fehbvm.com/Article/details/gbpylgiud.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.hesvh.cn/Article/details/gcvoripeu.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.zdbjq.cn/Article/details/gjkmjgwfh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gyvswljjp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gdetlyxty.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gehkdgoif.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.zdbjq.cn/Article/details/gscrirwue.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fehbvm.com/Article/details/gsnuiamep.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.zdbjq.cn/Article/details/gitiietlz.sHtML

[E17] 首字母大写
来源：http://www.share.fehbvm.com/Article/details/gisbdrizf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.hesvh.cn/Article/details/gbwqtorrx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.fehbvm.com/Article/details/gpkyhtedu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gisxvqzqu.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/grjvmzkxo.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.zdbjq.cn/Article/details/gurjrmoef.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.fehbvm.com/Article/details/gdsrujvrx.sHtML

Ruby: s.capitalize
来源：http://mobile.zdbjq.cn/Article/details/gnsblndmf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.hesvh.cn/Article/details/grgmofkrb.sHtML

[E18] 模板占位符替换
来源：http://baike.fehbvm.com/Article/details/gfbkneeku.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.zdbjq.cn/Article/details/gsdhllgib.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.zdbjq.cn/Article/details/gjgxwfdey.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/glolvvcbk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/ghswjxkie.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gqcrynhtw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gztpbfnyo.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.zdbjq.cn/Article/details/ghvscnsve.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fehbvm.com/Article/details/ghduzeepv.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.fehbvm.com/Article/details/gamndwyhw.sHtML

Py:   s.splitlines()
来源：http://wap.zdbjq.cn/Article/details/gvwzjbpzu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gjxvijduz.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gsymuvpex.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gpmnhcbzr.sHtML

Java: s.lines().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gtghexvdb.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.zdbjq.cn/Article/details/gqftmfixw.sHtML

Ruby: s.lines
来源：http://3g.fehbvm.com/Article/details/gcenkpwir.sHtML

C#:   s.Split('\n')
来源：http://baike.zdbjq.cn/Article/details/gzjirwrbt.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/gjxoleczo.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/gxgqzslao.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.zdbjq.cn/Article/details/gkvtapmuv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.fehbvm.com/Article/details/guittqira.sHtML

TS:   if (s === "") {}
来源：http://m.share.hesvh.cn/Article/details/gwproqlub.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/godhlqqqw.sHtML

Go:   if s == "" {}
来源：http://m.share.fehbvm.com/Article/details/gwaweoetf.sHtML

Ruby: if s.empty?
来源：http://m.share.fehbvm.com/Article/details/gljugcmee.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.zdbjq.cn/Article/details/gfggwzgow.sHtML

[E21] 超长截断加省略号
来源：http://www.share.zdbjq.cn/Article/details/gxvrlsleb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fehbvm.com/Article/details/goevmqfef.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/ghxqysmjk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/glohevtft.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gifxztamm.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gnkblxaxc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.fehbvm.com/Article/details/gqtytvkvm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/ghyqingci.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/ghrylqegy.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fehbvm.com/Article/details/gvbwnefty.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.zdbjq.cn/Article/details/gwbyvjkql.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gpucluqgd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gidvieupb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gzwvgucqc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.hesvh.cn/Article/details/ggxrwjscw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fehbvm.com/Article/details/giaovnlpw.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fehbvm.com/Article/details/gjfzyzosd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.zdbjq.cn/Article/details/gmhsgtcxc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/guohcxrhw.sHtML

F. 文件与目录
来源：http://3g.hesvh.cn/Article/details/gsphwwdgg.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjrpnqsnv.sHtML

[F01] 读取整个文件
来源：http://www.blog.fehbvm.com/Article/details/glfonvteu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.hesvh.cn/Article/details/goxjvdcri.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gfffgpgiv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.zdbjq.cn/Article/details/gzljybcmn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gvtasyuko.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gtpyhqsum.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.hesvh.cn/Article/details/gkidtyjqr.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gptthyvir.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.hesvh.cn/Article/details/gupjcnlrj.sHtML

[F02] 逐行读取文件
来源：http://wap.fehbvm.com/Article/details/gwpoilutt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.zdbjq.cn/Article/details/gzyhjjrfl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.hesvh.cn/Article/details/glfevkwts.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/guqonkyet.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gmjtbhqag.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/grhdpmogy.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.zdbjq.cn/Article/details/gfziwpdfa.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.fehbvm.com/Article/details/ghsucahpz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fehbvm.com/Article/details/gyrkwyeub.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/gyhvaplhq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.hesvh.cn/Article/details/goosupmcx.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gzlozblok.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gtwasautm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gjrokpgld.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.hesvh.cn/Article/details/ghzjffdmy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.hesvh.cn/Article/details/grfjdwciq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.zdbjq.cn/Article/details/gebiehyqa.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gfajnpszt.sHtML

[F04] 追加写入文件
来源：http://3g.hesvh.cn/Article/details/gmxjfsoox.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gvconuler.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.zdbjq.cn/Article/details/ggujwghjl.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/ggrzvmefi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gjzmalswo.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.zdbjq.cn/Article/details/gyarivyqs.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.hesvh.cn/Article/details/gcmpxksuh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.zdbjq.cn/Article/details/geaxhxudg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.hesvh.cn/Article/details/ganscenps.sHtML


<!-- 参考信息 -->