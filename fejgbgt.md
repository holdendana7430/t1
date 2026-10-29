代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gfmbrqtsb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/gamkokchb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.zdbjq.cn/Article/details/gczwxaisq.sHtML

Go:   // 手写 map[T]int
来源：http://baike.hesvh.cn/Article/details/gfuarypuu.sHtML

Ruby: arr.tally
来源：http://blog.hesvh.cn/Article/details/ggjzsnknl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.hesvh.cn/Article/details/gqdvmahkb.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fehbvm.com/Article/details/gyjiqgaey.sHtML

Py:   x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gealzramm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.zdbjq.cn/Article/details/gcdnutukj.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/ghucrhbwb.sHtML

TS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gcqglcdzt.sHtML

Java: list.contains(x)
来源：http://mobile.fehbvm.com/Article/details/gipwhmfdn.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fehbvm.com/Article/details/gunajqajp.sHtML

Ruby: arr.include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gpmiypnox.sHtML

C#:   list.Contains(x)
来源：http://3g.fehbvm.com/Article/details/gmesqhslk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.hesvh.cn/Article/details/gypvhotmt.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.fehbvm.com/Article/details/gbgupsgwe.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fehbvm.com/Article/details/gxrecxocp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gwehzvxmp.sHtML

TS:   [...arr];
来源：http://wap.zdbjq.cn/Article/details/gezsnrifn.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.fehbvm.com/Article/details/gcbdowudg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.hesvh.cn/Article/details/gspozceku.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.zdbjq.cn/Article/details/geqcnsklm.sHtML

C#:   new List<int>(list);
来源：http://www.share.zdbjq.cn/Article/details/gnnoohlwq.sHtML

[D23] reduce 累积计算
来源：http://wap.fehbvm.com/Article/details/gotxlidnj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.hesvh.cn/Article/details/gicuxcbfz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.hesvh.cn/Article/details/gwoemzhyd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gufaldrcz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gtwzhoaov.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.zdbjq.cn/Article/details/gwjxvqbch.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gnezqhgcj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.zdbjq.cn/Article/details/gmxdoiwhc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fehbvm.com/Article/details/gauadlxjg.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.zdbjq.cn/Article/details/gyrlleoby.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.hesvh.cn/Article/details/gvbssjrji.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.zdbjq.cn/Article/details/ghihirmiq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.fehbvm.com/Article/details/gamkyxhnt.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gfnfjmffs.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.zdbjq.cn/Article/details/gblyzqzei.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.zdbjq.cn/Article/details/gahnpnofi.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.zdbjq.cn/Article/details/gvpsmqmpu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.hesvh.cn/Article/details/ghyslwkdj.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fehbvm.com/Article/details/gkurgieoz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fehbvm.com/Article/details/ggubnjotc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.hesvh.cn/Article/details/gmefnzwdh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fehbvm.com/Article/details/gswclrlrw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.zdbjq.cn/Article/details/gbblwzwdw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.hesvh.cn/Article/details/gdksstzep.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fehbvm.com/Article/details/gftgvznit.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fehbvm.com/Article/details/gnzzallbg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fehbvm.com/Article/details/gcwaylvmx.sHtML

[D26] 数组转字符串
来源：http://m.share.hesvh.cn/Article/details/gwqrkdtkg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.hesvh.cn/Article/details/gednneujo.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fehbvm.com/Article/details/gtxxbiovg.sHtML

JS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gvcsibmqf.sHtML

TS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gcizekfuu.sHtML

Java: String.join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gzqqijiyi.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.hesvh.cn/Article/details/gxfwaxizp.sHtML

Ruby: arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gwnxjiqdd.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/glhfsfjgg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gyqgobnua.sHtML

E. 字符串处理
来源：http://baike.zdbjq.cn/Article/details/gstlblgdj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gsmaaufel.sHtML

[E01] 拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gkayhhrin.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.fehbvm.com/Article/details/gquhjccat.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.zdbjq.cn/Article/details/gaiemybyp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gvnibwvrm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gbglhnwzh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.hesvh.cn/Article/details/gvgpashmu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fehbvm.com/Article/details/gbflajrfj.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fehbvm.com/Article/details/glrfbriim.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gqcwaweuo.sHtML

[E02] 重复字符串
来源：http://m.share.fehbvm.com/Article/details/gdhkpkmdb.sHtML

Py:   "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gvjvekhjq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.fehbvm.com/Article/details/gjdaahhdi.sHtML

JS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gdihydbnc.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gugieiyac.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gjqgwuaxn.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.zdbjq.cn/Article/details/glgtnrdlr.sHtML

Ruby: "ab" * 3
来源：http://baike.hesvh.cn/Article/details/glrfphbzl.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/gkectkvfu.sHtML

[E03] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gnybgpsfc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.hesvh.cn/Article/details/gbfzkeoof.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gsvjzoipd.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gwjuxkpvg.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gepinqwav.sHtML

Java: s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gzfuikzom.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.hesvh.cn/Article/details/glatgmvud.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.fehbvm.com/Article/details/gtclngqbi.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.zdbjq.cn/Article/details/gfvorbeyu.sHtML

[E04] 查找子串位置
来源：http://m.share.hesvh.cn/Article/details/glyjaahkv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gckwwwpgm.sHtML

PHP:  strpos($s, "x");
来源：http://3g.hesvh.cn/Article/details/ganmqglbq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fehbvm.com/Article/details/gumgmtdet.sHtML

TS:   s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gnxvuleip.sHtML

Java: s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/giyntevzi.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.hesvh.cn/Article/details/giufrgkzb.sHtML

Ruby: s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gfesqbaco.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gfiychuhv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.zdbjq.cn/Article/details/gdvizflym.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.fehbvm.com/Article/details/giydrqvdx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fehbvm.com/Article/details/gmgkljnag.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gxvcwvyai.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.hesvh.cn/Article/details/gpuietabi.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gbrgqndau.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fehbvm.com/Article/details/gkwwxdcik.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.zdbjq.cn/Article/details/gmodcwwpv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gxyvyitrz.sHtML

[E06] 替换子串
来源：http://www.m.share.fehbvm.com/Article/details/gfcswrooe.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gucajttfy.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.fehbvm.com/Article/details/gneuaqkvt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gfochydkl.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gvmfoiufg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gabqmgahk.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/glrseabni.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.hesvh.cn/Article/details/gtaqhwidu.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.hesvh.cn/Article/details/gevyrngog.sHtML

[E07] 按分隔符拆分
来源：http://mobile.fehbvm.com/Article/details/guxynutgg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.hesvh.cn/Article/details/gfvwjwfop.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.hesvh.cn/Article/details/gbbkgjumz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.hesvh.cn/Article/details/givhrxcsq.sHtML

TS:   s.split(",")
来源：http://blog.zdbjq.cn/Article/details/gwzrajgnr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.zdbjq.cn/Article/details/gmvedvtci.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.zdbjq.cn/Article/details/giglyvvkc.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.fehbvm.com/Article/details/geqiseyef.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.hesvh.cn/Article/details/gadhxrqqv.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fehbvm.com/Article/details/ggpokzaae.sHtML

Py:   ",".join(items)
来源：http://3g.fehbvm.com/Article/details/gvwjalruj.sHtML

PHP:  implode(",", $items);
来源：http://baike.zdbjq.cn/Article/details/gzjmkctzg.sHtML

JS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gdepnovge.sHtML

TS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gxplevryo.sHtML

Java: String.join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gkjsdbucj.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.zdbjq.cn/Article/details/ggynhzinq.sHtML

Ruby: items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/grxjqfzra.sHtML

C#:   string.Join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gehuyfwjr.sHtML

[E09] 去除所有空白字符
来源：http://read.share.hesvh.cn/Article/details/gnllaaeyy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.hesvh.cn/Article/details/gupmxdsln.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gtxvskbwe.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gzpxumycf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/ggdscpzqh.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.fehbvm.com/Article/details/gqgdsuggv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.hesvh.cn/Article/details/grovazjua.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.hesvh.cn/Article/details/gsddieksk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gapgaahcl.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.hesvh.cn/Article/details/germprqun.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gxsewybab.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.zdbjq.cn/Article/details/grrzxphhc.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gqjffefjd.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gzdwjibkz.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gtjhxbopp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/glbiaqtpr.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gymxqbxgv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.zdbjq.cn/Article/details/gwvtrefhy.sHtML

[E11] 反转字符串
来源：http://mobile.hesvh.cn/Article/details/gtrjfhmui.sHtML

Py:   s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gopdqkuum.sHtML

PHP:  strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gxbpqvikr.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gvipzezxw.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gnohlojuc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gryvzzqnc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fehbvm.com/Article/details/gkkvimhjh.sHtML

Ruby: s.reverse
来源：http://mobile.fehbvm.com/Article/details/gehyzkpyf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gcqxgtebi.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.hesvh.cn/Article/details/geghmsmgy.sHtML

Py:   s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gtqyzwahv.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.hesvh.cn/Article/details/gauokygcs.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gvkbvguqw.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/gtwyillim.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.fehbvm.com/Article/details/gippkpabf.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fehbvm.com/Article/details/gdoasrqbl.sHtML

Ruby: s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gagqufjsz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.fehbvm.com/Article/details/giklxhdpe.sHtML

[E13] 逐字符遍历
来源：http://blog.fehbvm.com/Article/details/gfhowibcc.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.zdbjq.cn/Article/details/gbrxeiozq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fehbvm.com/Article/details/ggewygfhy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/ggdpxtueo.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gzyyjmhtu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gldfnpxks.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.zdbjq.cn/Article/details/gdtkkqmdb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.zdbjq.cn/Article/details/gliexlypy.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gptyjwyta.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.fehbvm.com/Article/details/gflbjipud.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.zdbjq.cn/Article/details/ghjhrvbaa.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fehbvm.com/Article/details/gafafgjlw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.zdbjq.cn/Article/details/guovuptnk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.hesvh.cn/Article/details/gxgbtapmx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.fehbvm.com/Article/details/glubyfmks.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.zdbjq.cn/Article/details/gelodwmen.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.zdbjq.cn/Article/details/gxjhgbawg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.zdbjq.cn/Article/details/gourzmjeo.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.fehbvm.com/Article/details/gfzvthvfb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fehbvm.com/Article/details/gycqrheuv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.hesvh.cn/Article/details/gsragbamq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fehbvm.com/Article/details/gofoopjpl.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.fehbvm.com/Article/details/gqamwohis.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fehbvm.com/Article/details/grezzpztc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.hesvh.cn/Article/details/gglkgqgoi.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.hesvh.cn/Article/details/gjeejlpob.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.zdbjq.cn/Article/details/ghiuwilwj.sHtML

[E16] 数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gmkgzovnz.sHtML

Py:   f"{1234567:,}"
来源：http://3g.hesvh.cn/Article/details/gwlzhdolx.sHtML

PHP:  number_format(1234567);
来源：http://baike.zdbjq.cn/Article/details/goipxdscs.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gickbyvcb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gzizxjngk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gsybopwwm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fehbvm.com/Article/details/gfomfkckp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.hesvh.cn/Article/details/gvgcfpzlx.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.zdbjq.cn/Article/details/glyobeclo.sHtML

[E17] 首字母大写
来源：http://read.share.fehbvm.com/Article/details/gcfncdgyn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.hesvh.cn/Article/details/gwnezrmgr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.zdbjq.cn/Article/details/gswvodfqt.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gghpjhkcf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gcwmkokoj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fehbvm.com/Article/details/ghtapoyrx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gxkpigjvy.sHtML

Ruby: s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/gbkmscmbv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.hesvh.cn/Article/details/ghlwcwzjk.sHtML

[E18] 模板占位符替换
来源：http://baike.fehbvm.com/Article/details/galzcurum.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fehbvm.com/Article/details/gqffhxfzi.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.zdbjq.cn/Article/details/geianarko.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gmyknmqfm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gsipiwfkv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gdfihbtdd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.hesvh.cn/Article/details/gcxsvhyhb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.hesvh.cn/Article/details/gqbmbwycg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.zdbjq.cn/Article/details/gpkpzgomv.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fehbvm.com/Article/details/gcuqjgezy.sHtML

Py:   s.splitlines()
来源：http://m.share.zdbjq.cn/Article/details/gekyvmtlo.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.hesvh.cn/Article/details/gxdgdiycr.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gaqufcygj.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gtgzgsrvr.sHtML

Java: s.lines().toList()
来源：http://www.m.share.hesvh.cn/Article/details/glhculpqv.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fehbvm.com/Article/details/gpvjwrsdw.sHtML

Ruby: s.lines
来源：http://baike.hesvh.cn/Article/details/gdaqmmzmp.sHtML

C#:   s.Split('\n')
来源：http://read.share.zdbjq.cn/Article/details/gasbicwea.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.hesvh.cn/Article/details/gciyrqomq.sHtML

Py:   if not s:
来源：http://www.share.hesvh.cn/Article/details/gwuzspbwd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.fehbvm.com/Article/details/gccnlxnpc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fehbvm.com/Article/details/gugazkidl.sHtML

TS:   if (s === "") {}
来源：http://3g.zdbjq.cn/Article/details/gokuwbwny.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gwhgawgjo.sHtML

Go:   if s == "" {}
来源：http://baike.fehbvm.com/Article/details/gxjbhgumm.sHtML

Ruby: if s.empty?
来源：http://www.share.fehbvm.com/Article/details/gijnecnbe.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fehbvm.com/Article/details/gxprbkklb.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fehbvm.com/Article/details/gnhgrygxv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.hesvh.cn/Article/details/gxkxyxkpf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gqdumhmxh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gkaqdfwqe.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gltsjrdld.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gbdiankzp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fehbvm.com/Article/details/gjwylpoxh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gdddkvvdg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/glcafifwx.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fehbvm.com/Article/details/gsscyctgi.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.zdbjq.cn/Article/details/gptlqhuai.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gdizgxpkk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gwuarxybj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gmpchwtah.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fehbvm.com/Article/details/guyvebnzk.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.zdbjq.cn/Article/details/gnpzuwulw.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gpcdacxsn.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fehbvm.com/Article/details/gmdsprxxx.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gybthvvqo.sHtML

F. 文件与目录
来源：http://m.share.fehbvm.com/Article/details/gtmcqcldx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnstbfwsl.sHtML

[F01] 读取整个文件
来源：http://3g.zdbjq.cn/Article/details/ggajztdzc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.hesvh.cn/Article/details/gbkxjxecy.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gzccvwioa.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.hesvh.cn/Article/details/glzqxvaxk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gxuholsln.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gjvwmhdec.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.hesvh.cn/Article/details/gwegoxlot.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gjcauvcud.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gmjxkgomr.sHtML

[F02] 逐行读取文件
来源：http://wap.hesvh.cn/Article/details/gfssbnccc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.hesvh.cn/Article/details/glnjphszm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fehbvm.com/Article/details/gitcwjgid.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/ghclgvdac.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gcysbgfyn.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gcizoutdy.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.hesvh.cn/Article/details/ghdzrywhp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.zdbjq.cn/Article/details/gihitbiiv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fehbvm.com/Article/details/gzuothprf.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.hesvh.cn/Article/details/ggbzvqzir.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.hesvh.cn/Article/details/gqvdjekpc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gdomiqvdk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gahbrzxpp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gwdveprsv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.hesvh.cn/Article/details/gekwucudv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.hesvh.cn/Article/details/gidoxjsva.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.hesvh.cn/Article/details/garrcdfev.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gttynislc.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/gxqephhlk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.hesvh.cn/Article/details/ggyhnwkjf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.hesvh.cn/Article/details/ghdbifibo.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gnpvdmmck.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gncqbastp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.hesvh.cn/Article/details/gvxldjbfl.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.zdbjq.cn/Article/details/gqulmmyks.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.zdbjq.cn/Article/details/gskhhslfa.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/gmshpnlic.sHtML


<!-- 参考信息 -->