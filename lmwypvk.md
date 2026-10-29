代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gdsairjuh.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gktmssffq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/gtgjmqupv.sHtML

Go:   // 手写 map[T]int
来源：http://wap.zdbjq.cn/Article/details/gzfsnwqzc.sHtML

Ruby: arr.tally
来源：http://blog.hesvh.cn/Article/details/guwbyfwxo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.hesvh.cn/Article/details/glvrqulsc.sHtML

[D21] 判断是否包含某元素
来源：http://baike.hesvh.cn/Article/details/gqifhtppy.sHtML

Py:   x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gmyzjtsus.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.zdbjq.cn/Article/details/gbtxnorjs.sHtML

JS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/giaxhnjio.sHtML

TS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gaseaosjh.sHtML

Java: list.contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gbzftebpl.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gdzgkghus.sHtML

Ruby: arr.include?(x)
来源：http://baike.hesvh.cn/Article/details/gnkalculk.sHtML

C#:   list.Contains(x)
来源：http://3g.fehbvm.com/Article/details/gakchziej.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.hesvh.cn/Article/details/gctzzbkon.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fehbvm.com/Article/details/gtuwttxpi.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fehbvm.com/Article/details/gjomqhmtf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.zdbjq.cn/Article/details/gnlzahzzu.sHtML

TS:   [...arr];
来源：http://blog.hesvh.cn/Article/details/gcmhkprfq.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gjkcoyeyz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.hesvh.cn/Article/details/gzmpmucol.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.zdbjq.cn/Article/details/giwoknvep.sHtML

C#:   new List<int>(list);
来源：http://read.share.fehbvm.com/Article/details/gfgyxjrqm.sHtML

[D23] reduce 累积计算
来源：http://www.blog.hesvh.cn/Article/details/gbjhvhlmg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.hesvh.cn/Article/details/gdrcanpob.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.hesvh.cn/Article/details/gbguypvnh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gvfiqccdd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gnwjmlrfv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fehbvm.com/Article/details/gypfzjyvj.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gomqekcva.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.fehbvm.com/Article/details/gzcgpzuau.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.hesvh.cn/Article/details/gozxfkoup.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fehbvm.com/Article/details/gbibajycn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.zdbjq.cn/Article/details/gzndqgdsv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.hesvh.cn/Article/details/gtprvawsw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fehbvm.com/Article/details/gwxkganmj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gapjfhlxb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.hesvh.cn/Article/details/giyodhmvt.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.zdbjq.cn/Article/details/ghcexahql.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.hesvh.cn/Article/details/ggkoqmici.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.zdbjq.cn/Article/details/ghrqlqxnf.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.hesvh.cn/Article/details/gpuyfvfla.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fehbvm.com/Article/details/garrveerp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.hesvh.cn/Article/details/gstfaheqp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.zdbjq.cn/Article/details/gpbeffvzp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fehbvm.com/Article/details/gmngyvyvu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.hesvh.cn/Article/details/gjurueyce.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.hesvh.cn/Article/details/guwzobykf.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.zdbjq.cn/Article/details/gpitxbnxk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fehbvm.com/Article/details/gmtqawrqz.sHtML

[D26] 数组转字符串
来源：http://blog.hesvh.cn/Article/details/gnedmwkrm.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.zdbjq.cn/Article/details/gwhocfssf.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gomdaxhbe.sHtML

JS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gohklqwfk.sHtML

TS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/giymbkkek.sHtML

Java: String.join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/guxmnicca.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.hesvh.cn/Article/details/gharmqmay.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/ggorydiev.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gxjfrwemv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjkbappfg.sHtML

E. 字符串处理
来源：http://mobile.fehbvm.com/Article/details/gegkpkcbb.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gyfqufbue.sHtML

[E01] 拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/ggrlfhdvk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.fehbvm.com/Article/details/gbylqcquj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.zdbjq.cn/Article/details/gjigbrhsj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gjaspnhyq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gwpehmtdx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.zdbjq.cn/Article/details/gxftyxysg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fehbvm.com/Article/details/gprbnlixo.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.zdbjq.cn/Article/details/givyzlggy.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gbegnmozo.sHtML

[E02] 重复字符串
来源：http://www.blog.fehbvm.com/Article/details/grwxssdet.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gksdptcne.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fehbvm.com/Article/details/gwhrsmiqn.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gcvwfnwck.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gzsiitljx.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/giomsmglu.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fehbvm.com/Article/details/gpetszbqr.sHtML

Ruby: "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gxggwhszg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.hesvh.cn/Article/details/gnlajgdve.sHtML

[E03] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gljecagle.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fehbvm.com/Article/details/ghfzxenhp.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gwrybhdcb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gtjcrgnmd.sHtML

TS:   s.slice(1, 4)
来源：http://3g.fehbvm.com/Article/details/ggmefkgka.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gkahlcrsp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.fehbvm.com/Article/details/gmrfunozl.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.hesvh.cn/Article/details/gutbmfnyz.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.hesvh.cn/Article/details/gfdseyaai.sHtML

[E04] 查找子串位置
来源：http://read.share.fehbvm.com/Article/details/greejftmn.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.fehbvm.com/Article/details/gcvtjzloo.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.zdbjq.cn/Article/details/gsexujsst.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.zdbjq.cn/Article/details/gxfpznuyc.sHtML

TS:   s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/ggxwcawhb.sHtML

Java: s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gwmvpfuxz.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.zdbjq.cn/Article/details/gvamesnoi.sHtML

Ruby: s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gqayladvn.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gtdquzkhq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.zdbjq.cn/Article/details/gfnvtwdlb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.fehbvm.com/Article/details/gcwlddhee.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fehbvm.com/Article/details/gkukmteks.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gkotvvyio.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fehbvm.com/Article/details/gdnjghzrj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gpqgzbiqv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.fehbvm.com/Article/details/gljwaefll.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.fehbvm.com/Article/details/gzlsfkbzz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fehbvm.com/Article/details/gsbqloise.sHtML

[E06] 替换子串
来源：http://baike.hesvh.cn/Article/details/gtbjylury.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gaxnmkwoa.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.zdbjq.cn/Article/details/guvrmriql.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gyhwsftty.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gdtwvmzda.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gwpkikikt.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gcoboqozn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gedvxdnav.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/giimzxtlz.sHtML

[E07] 按分隔符拆分
来源：http://wap.hesvh.cn/Article/details/gvvycwgzd.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.zdbjq.cn/Article/details/gfsjwzmue.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.fehbvm.com/Article/details/gmjmmauae.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.zdbjq.cn/Article/details/gozwkmkpv.sHtML

TS:   s.split(",")
来源：http://3g.hesvh.cn/Article/details/ghpkjipfi.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.zdbjq.cn/Article/details/gjjjxtzgh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.zdbjq.cn/Article/details/gvimkvovu.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fehbvm.com/Article/details/gkngclyda.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.hesvh.cn/Article/details/griiredia.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fehbvm.com/Article/details/gsokthwmf.sHtML

Py:   ",".join(items)
来源：http://www.blog.zdbjq.cn/Article/details/gaiaikpvu.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.zdbjq.cn/Article/details/gpsbhluwe.sHtML

JS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gkkqkabzq.sHtML

TS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gwhvhxhna.sHtML

Java: String.join(",", items)
来源：http://baike.fehbvm.com/Article/details/gcdszzdbz.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fehbvm.com/Article/details/gtgnpkdzx.sHtML

Ruby: items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gkobuxkfc.sHtML

C#:   string.Join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gkndlfirg.sHtML

[E09] 去除所有空白字符
来源：http://baike.fehbvm.com/Article/details/gtkkjorim.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fehbvm.com/Article/details/grrtvfhnd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.hesvh.cn/Article/details/gstnnrvsh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gnfwfipma.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gxhrweghe.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gyiqmraqe.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fehbvm.com/Article/details/gjxzwnrmc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.fehbvm.com/Article/details/gbimuzsei.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gmgtkqgjy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.zdbjq.cn/Article/details/ghswmusep.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gdytvzjwy.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.hesvh.cn/Article/details/gkhcnkdiq.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gsxruvsbl.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gpwcafdvm.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gdanytpqf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gcgaddjif.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gmvycgmzt.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.hesvh.cn/Article/details/gmslapmsa.sHtML

[E11] 反转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gukapqqba.sHtML

Py:   s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gqiqkuhlt.sHtML

PHP:  strrev($s);
来源：http://baike.hesvh.cn/Article/details/gbntnpjea.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gtvrmhcjh.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gltkemwsl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gotbhgglx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.hesvh.cn/Article/details/gfdetvcro.sHtML

Ruby: s.reverse
来源：http://baike.fehbvm.com/Article/details/gnrmhwyjj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gsulllgts.sHtML

[E12] 统计某字符出现次数
来源：http://wap.fehbvm.com/Article/details/gdxfjsozl.sHtML

Py:   s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gooqmrubk.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.zdbjq.cn/Article/details/gpobljacz.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gwsnqdfjm.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/glqztucyo.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.hesvh.cn/Article/details/gljazsnjb.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.hesvh.cn/Article/details/gbpcbukih.sHtML

Ruby: s.count("a")
来源：http://blog.hesvh.cn/Article/details/gzdaflfyy.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.zdbjq.cn/Article/details/gihxnnubb.sHtML

[E13] 逐字符遍历
来源：http://m.share.fehbvm.com/Article/details/ggqisyabt.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.fehbvm.com/Article/details/gybszavxi.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.zdbjq.cn/Article/details/gilrsxgdm.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gfprqutds.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/giumjuvbl.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.hesvh.cn/Article/details/gflxqyjvl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fehbvm.com/Article/details/glehaddye.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.hesvh.cn/Article/details/gblbpiezy.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.hesvh.cn/Article/details/gikfdditx.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.hesvh.cn/Article/details/ghraaqlkl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fehbvm.com/Article/details/giblqohrb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.zdbjq.cn/Article/details/gamamxdsx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.zdbjq.cn/Article/details/gdzljbodr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.zdbjq.cn/Article/details/gjmghovho.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gaarqejfp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fehbvm.com/Article/details/gbhsallvc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.hesvh.cn/Article/details/gylqedybc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.zdbjq.cn/Article/details/glyhtbvww.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fehbvm.com/Article/details/gjsokxgzk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.hesvh.cn/Article/details/gjlhvyzik.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.hesvh.cn/Article/details/garxfeycg.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.hesvh.cn/Article/details/gyhgnyklu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fehbvm.com/Article/details/gxmimqylv.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fehbvm.com/Article/details/gggminzlb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.zdbjq.cn/Article/details/ghnxcvkbk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fehbvm.com/Article/details/gabltgbqy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fehbvm.com/Article/details/gcfmtdovr.sHtML

[E16] 数字千分位
来源：http://m.share.fehbvm.com/Article/details/guokzraun.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/ghqeavhyu.sHtML

PHP:  number_format(1234567);
来源：http://3g.fehbvm.com/Article/details/gubsntpbx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/ggdjpgrwz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gtdnfslau.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gxcgqxqvd.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.hesvh.cn/Article/details/gvkumpvfp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fehbvm.com/Article/details/goaopqadu.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.hesvh.cn/Article/details/glvzupclz.sHtML

[E17] 首字母大写
来源：http://3g.fehbvm.com/Article/details/gnlhzfsrb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.zdbjq.cn/Article/details/gyradonay.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.hesvh.cn/Article/details/gglxdxfnp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gsoivnixs.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gkdmlwbff.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fehbvm.com/Article/details/gdeqwrkbx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.zdbjq.cn/Article/details/ghiewcgij.sHtML

Ruby: s.capitalize
来源：http://3g.zdbjq.cn/Article/details/gyauaqcro.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fehbvm.com/Article/details/gsrutahag.sHtML

[E18] 模板占位符替换
来源：http://m.share.fehbvm.com/Article/details/gfezlbwff.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.zdbjq.cn/Article/details/gpdqosakt.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fehbvm.com/Article/details/gdoednfhj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gzdwmmvmu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gkkatogtk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gfoufmwft.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gtovrvzsl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fehbvm.com/Article/details/gnqkjzghs.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fehbvm.com/Article/details/ghjmvguzw.sHtML

[E19] 多行文本按行拆分
来源：http://3g.zdbjq.cn/Article/details/gheoincrq.sHtML

Py:   s.splitlines()
来源：http://blog.hesvh.cn/Article/details/gjqhljlkr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.hesvh.cn/Article/details/gtqfxinyb.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/geekvxrvl.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gtdtohubg.sHtML

Java: s.lines().toList()
来源：http://m.share.fehbvm.com/Article/details/gwtyrgaaf.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.zdbjq.cn/Article/details/gwjqgnxyj.sHtML

Ruby: s.lines
来源：http://www.m.share.fehbvm.com/Article/details/glrqvbfaj.sHtML

C#:   s.Split('\n')
来源：http://read.share.fehbvm.com/Article/details/gkwrournf.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/ggtodphty.sHtML

Py:   if not s:
来源：http://www.m.share.fehbvm.com/Article/details/gmsxnpjam.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.hesvh.cn/Article/details/gznupvmbi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.hesvh.cn/Article/details/grthoyoen.sHtML

TS:   if (s === "") {}
来源：http://baike.zdbjq.cn/Article/details/gjqheqaui.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gprrqrmau.sHtML

Go:   if s == "" {}
来源：http://blog.fehbvm.com/Article/details/gnsfqengd.sHtML

Ruby: if s.empty?
来源：http://wap.hesvh.cn/Article/details/gkqmszxqn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.hesvh.cn/Article/details/gqoviafln.sHtML

[E21] 超长截断加省略号
来源：http://baike.hesvh.cn/Article/details/girfauslm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.hesvh.cn/Article/details/ghrqicrvw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gtfzfdzjw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gqjhdjryq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gunkylegm.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gdxfgtiqt.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fehbvm.com/Article/details/gskywrprc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gswvlknvl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gpybgugwh.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fehbvm.com/Article/details/gtohwsjcv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.hesvh.cn/Article/details/gmbkmqhbt.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gpmntsgqu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/girjczwxk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/ggsvsggck.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.zdbjq.cn/Article/details/gjsxiyixr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.zdbjq.cn/Article/details/gvnlczoim.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.hesvh.cn/Article/details/glgukpoow.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fehbvm.com/Article/details/gmivtpnve.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/guwzlzhiu.sHtML

F. 文件与目录
来源：http://blog.fehbvm.com/Article/details/gpueiymbz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwurzlrca.sHtML

[F01] 读取整个文件
来源：http://mobile.hesvh.cn/Article/details/gawqkifkd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.zdbjq.cn/Article/details/grayzsaxz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/gjyhwflpb.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.fehbvm.com/Article/details/gzlvdkyux.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.hesvh.cn/Article/details/grvxsfiua.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/glhmndgab.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.hesvh.cn/Article/details/gvfkxbcvq.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gbqjudhtt.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gqzkdvwxc.sHtML

[F02] 逐行读取文件
来源：http://3g.hesvh.cn/Article/details/gckbjsgsr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.hesvh.cn/Article/details/gvtcoofwu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fehbvm.com/Article/details/giugrsiiw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gxqvlnxkr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gpbafsyvw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gustyomfd.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fehbvm.com/Article/details/gawtujcyf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.hesvh.cn/Article/details/gaxjcqmpg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.zdbjq.cn/Article/details/gfmohafub.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.zdbjq.cn/Article/details/gawncylir.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.zdbjq.cn/Article/details/grrygvjtj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gpuccijhf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gyfcccqmf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gwcwiyjpp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.zdbjq.cn/Article/details/glhiyssuk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.zdbjq.cn/Article/details/glxqbivlz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fehbvm.com/Article/details/girjgcqoz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gclgsodoq.sHtML

[F04] 追加写入文件
来源：http://mobile.hesvh.cn/Article/details/gvktldrxl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fehbvm.com/Article/details/gtrqfkeil.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.hesvh.cn/Article/details/gvgfpbpgl.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gvjaxjlwn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gacftenaq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fehbvm.com/Article/details/gdeatzhtq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/grkocrinx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fehbvm.com/Article/details/gvxoofqts.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fehbvm.com/Article/details/gzmutvwbx.sHtML


<!-- 参考信息 -->