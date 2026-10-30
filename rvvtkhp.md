代发 wailian999

Ruby: arr.tally
来源：http://www.share.zdbjq.cn/Article/details/gcskpxqyl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.zdbjq.cn/Article/details/gxyjkeqew.sHtML

[D21] 判断是否包含某元素
来源：http://wap.zdbjq.cn/Article/details/gttlybbyw.sHtML

Py:   x in arr
来源：http://read.share.fehbvm.com/Article/details/gjbwgrmph.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.fehbvm.com/Article/details/gxfrksdfm.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gtqlwzeom.sHtML

TS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gpjiyuxlm.sHtML

Java: list.contains(x)
来源：http://m.share.zdbjq.cn/Article/details/ghrkvlddt.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gtxaijlkx.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/gdlqejxci.sHtML

C#:   list.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gcofsmryk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.fehbvm.com/Article/details/ggllsgcxz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fehbvm.com/Article/details/gbtrtzgmm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/ggwjfqnsi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.zdbjq.cn/Article/details/gddijwntx.sHtML

TS:   [...arr];
来源：http://m.share.fehbvm.com/Article/details/gprehfxqs.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fehbvm.com/Article/details/gwvkivhiq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gwmwqzwpn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fehbvm.com/Article/details/ghalamoro.sHtML

C#:   new List<int>(list);
来源：http://m.share.hesvh.cn/Article/details/gxkwjcymq.sHtML

[D23] reduce 累积计算
来源：http://m.share.hesvh.cn/Article/details/gmwkddwlm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.hesvh.cn/Article/details/gjnoundsv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.hesvh.cn/Article/details/gedumukfk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gtanygpli.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/glvymalpg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.hesvh.cn/Article/details/gympjkvei.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/goyslnhwb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fehbvm.com/Article/details/gjqmyttrn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.hesvh.cn/Article/details/govichjht.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.hesvh.cn/Article/details/glettxmom.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.hesvh.cn/Article/details/gsjfkcxlg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.hesvh.cn/Article/details/gzjhwueai.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gsurxrbet.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fehbvm.com/Article/details/gboyborzz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.hesvh.cn/Article/details/gcumunixj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.fehbvm.com/Article/details/gwzgxpkln.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fehbvm.com/Article/details/gwfxliica.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.zdbjq.cn/Article/details/gppeybivm.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fehbvm.com/Article/details/gqaerudnt.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fehbvm.com/Article/details/gsxhhecav.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.zdbjq.cn/Article/details/goefvmkta.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fehbvm.com/Article/details/gobpmlegy.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.hesvh.cn/Article/details/gqqwloxyq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.hesvh.cn/Article/details/gxeyvfbdy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.zdbjq.cn/Article/details/gaonjsxfn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.fehbvm.com/Article/details/gyuiepavm.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.hesvh.cn/Article/details/gsirznvou.sHtML

[D26] 数组转字符串
来源：http://mobile.hesvh.cn/Article/details/genvmwrfa.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.fehbvm.com/Article/details/gjuxmkfjl.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.hesvh.cn/Article/details/geqohftlp.sHtML

JS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gphscrpkt.sHtML

TS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/ggqwgpdqb.sHtML

Java: String.join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gxbqxmlin.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.hesvh.cn/Article/details/gonycmhma.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gxjasofzh.sHtML

C#:   string.Join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gjwowykrl.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvmvjeeci.sHtML

E. 字符串处理
来源：http://3g.fehbvm.com/Article/details/ggqdqoaeb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghtimbqfv.sHtML

[E01] 拼接字符串
来源：http://blog.fehbvm.com/Article/details/gekknvjlx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/gdormnuky.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.zdbjq.cn/Article/details/guykcfnua.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gshzumfws.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gshkzxqjy.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.zdbjq.cn/Article/details/gqjdwmlge.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fehbvm.com/Article/details/gvonsndmx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.zdbjq.cn/Article/details/gwbbtoawj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gbptqokki.sHtML

[E02] 重复字符串
来源：http://baike.zdbjq.cn/Article/details/gruyrlrpq.sHtML

Py:   "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/grnmgwcrg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.zdbjq.cn/Article/details/gwcfsfgow.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gaewaypnp.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gjebofswa.sHtML

Java: "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gaqzxnntj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fehbvm.com/Article/details/gmvqyzxay.sHtML

Ruby: "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gqdzmwjgb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.zdbjq.cn/Article/details/gkbpvnvsj.sHtML

[E03] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gglbuvxpu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fehbvm.com/Article/details/ggxuhwtbu.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/ghcipgaeg.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/geukuhvxo.sHtML

TS:   s.slice(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gwprzjekg.sHtML

Java: s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/ghzwozbrc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gikesouzs.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.zdbjq.cn/Article/details/gkwollgar.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fehbvm.com/Article/details/gwibxragb.sHtML

[E04] 查找子串位置
来源：http://mobile.hesvh.cn/Article/details/gudyhzcbm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/ganfxqoym.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.zdbjq.cn/Article/details/gbnbwnzxw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fehbvm.com/Article/details/glhhqwpwy.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/guoziugtb.sHtML

Java: s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gnhxfchsy.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.zdbjq.cn/Article/details/ghikehmez.sHtML

Ruby: s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gkhzkcrcq.sHtML

C#:   s.IndexOf("x")
来源：http://wap.hesvh.cn/Article/details/gslorkgkr.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.zdbjq.cn/Article/details/glegbgzhc.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.zdbjq.cn/Article/details/gesjcwvmh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.hesvh.cn/Article/details/gsofgiapx.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/glnccolbn.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fehbvm.com/Article/details/gprtwnpkd.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gacisonar.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fehbvm.com/Article/details/grjdpjvty.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.zdbjq.cn/Article/details/gwznouicp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/ghxzodgmq.sHtML

[E06] 替换子串
来源：http://www.m.share.fehbvm.com/Article/details/gzbycdhrj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gcxnljsrn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.hesvh.cn/Article/details/gpnzprfmi.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gmzukmrvt.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gmhwchnrj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gksqfoohn.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/geelxqqgt.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fehbvm.com/Article/details/gqttpmpbp.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.hesvh.cn/Article/details/gyafnwrhd.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.zdbjq.cn/Article/details/gjlwjyiqr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fehbvm.com/Article/details/gggcljabt.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gntrwdbzt.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.hesvh.cn/Article/details/gdvaewngg.sHtML

TS:   s.split(",")
来源：http://wap.zdbjq.cn/Article/details/gongrldlq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.zdbjq.cn/Article/details/ginwvwonz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.fehbvm.com/Article/details/gaqkfjwhc.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.hesvh.cn/Article/details/ggmtsisdr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/ggqqtliyy.sHtML

[E08] 数组按分隔符合并
来源：http://3g.zdbjq.cn/Article/details/gekuwgwci.sHtML

Py:   ",".join(items)
来源：http://www.m.share.zdbjq.cn/Article/details/goojsiybc.sHtML

PHP:  implode(",", $items);
来源：http://m.share.hesvh.cn/Article/details/gklghkurk.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gwxhkuvvi.sHtML

TS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gbfvlwxlb.sHtML

Java: String.join(",", items)
来源：http://wap.hesvh.cn/Article/details/gzqryhhny.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.hesvh.cn/Article/details/gyrktqvlz.sHtML

Ruby: items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gblxtuuiq.sHtML

C#:   string.Join(",", items)
来源：http://blog.hesvh.cn/Article/details/gpqzllbfw.sHtML

[E09] 去除所有空白字符
来源：http://m.share.zdbjq.cn/Article/details/gdixsahmb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.hesvh.cn/Article/details/ghqcxxpor.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gydxzpydd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gyzucgexb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/glxgpjots.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gwzoswbbu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.hesvh.cn/Article/details/gmffgewgd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.hesvh.cn/Article/details/gjlhlzuqn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.hesvh.cn/Article/details/ghiskrnhv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.zdbjq.cn/Article/details/gfrajdgio.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gvmzqzika.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fehbvm.com/Article/details/gcncbkvhu.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/geabmdtmw.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gbrkmmlmo.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gpvuroufj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gboadoroy.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/ggcfdoogz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.hesvh.cn/Article/details/gydeqmomq.sHtML

[E11] 反转字符串
来源：http://mobile.hesvh.cn/Article/details/glgwvtrhs.sHtML

Py:   s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gtagqvohs.sHtML

PHP:  strrev($s);
来源：http://baike.hesvh.cn/Article/details/gftrhywse.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gothhftpq.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/glieoxolj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.zdbjq.cn/Article/details/gzqglblam.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fehbvm.com/Article/details/gnwexzwfl.sHtML

Ruby: s.reverse
来源：http://blog.fehbvm.com/Article/details/gvdmzncdx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gacnpoaia.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gkwlymedb.sHtML

Py:   s.count("a")
来源：http://blog.hesvh.cn/Article/details/gjtifnhmu.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.zdbjq.cn/Article/details/gcsngplrf.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gghvfgtpy.sHtML

TS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/grjcnpxog.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.zdbjq.cn/Article/details/gtxslmcnt.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fehbvm.com/Article/details/gepefxcmu.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gtxnfkdrj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/gzcayhocs.sHtML

[E13] 逐字符遍历
来源：http://www.share.fehbvm.com/Article/details/gzaukudrf.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.zdbjq.cn/Article/details/gsgtssttf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fehbvm.com/Article/details/gxxocetzt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gqwymtsyr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gbvqytrrn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.hesvh.cn/Article/details/gzpyoilqy.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.fehbvm.com/Article/details/gymfwqdgi.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fehbvm.com/Article/details/gcwiebqno.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gsaujhzdg.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fehbvm.com/Article/details/gtshmojjk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.zdbjq.cn/Article/details/gmrtpttqz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fehbvm.com/Article/details/gjixrdblw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.fehbvm.com/Article/details/gfbsdbdec.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fehbvm.com/Article/details/gawwobinx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fehbvm.com/Article/details/gkdlqnmug.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.hesvh.cn/Article/details/gdvshonnt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.zdbjq.cn/Article/details/gfhahocwk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.zdbjq.cn/Article/details/gozysprpz.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.zdbjq.cn/Article/details/gticmogrb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gmmsiqamv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gpklzqqmz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.fehbvm.com/Article/details/gatjdfnqv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gseiqkbfs.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.zdbjq.cn/Article/details/golbpsobd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.hesvh.cn/Article/details/giymtfqee.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.zdbjq.cn/Article/details/gnrtvowro.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.zdbjq.cn/Article/details/gisyizssl.sHtML

[E16] 数字千分位
来源：http://baike.fehbvm.com/Article/details/gchbwddig.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.zdbjq.cn/Article/details/gtzskacdt.sHtML

PHP:  number_format(1234567);
来源：http://mobile.fehbvm.com/Article/details/gdiatafqe.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gkyacaaae.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/glbznhocc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.zdbjq.cn/Article/details/guesdtrsj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fehbvm.com/Article/details/gdpxihydu.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.zdbjq.cn/Article/details/gfphoiigz.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.zdbjq.cn/Article/details/gohjkdmrq.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/guyvhjypo.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.zdbjq.cn/Article/details/gycjfqheo.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.fehbvm.com/Article/details/gtkpomvye.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gqfvccxbo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gdhfypqxy.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fehbvm.com/Article/details/gslgbcveu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gttlgdziu.sHtML

Ruby: s.capitalize
来源：http://mobile.hesvh.cn/Article/details/gwklihkov.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.zdbjq.cn/Article/details/ghddmapbq.sHtML

[E18] 模板占位符替换
来源：http://wap.zdbjq.cn/Article/details/gxqsmwgxs.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.fehbvm.com/Article/details/ghaobdegp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.fehbvm.com/Article/details/gwzrdoiiu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gipnzourq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gjhshetap.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gkfiqlwmb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gxatzlfjv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.hesvh.cn/Article/details/gswcmhdzr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.hesvh.cn/Article/details/gfxlkmknb.sHtML

[E19] 多行文本按行拆分
来源：http://baike.hesvh.cn/Article/details/gaofwnhjc.sHtML

Py:   s.splitlines()
来源：http://baike.zdbjq.cn/Article/details/ghnkyqpys.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.hesvh.cn/Article/details/gifgqwsel.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/ggervzwrg.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/ghiaxzohv.sHtML

Java: s.lines().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gecazqjqr.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fehbvm.com/Article/details/gtaacdmmm.sHtML

Ruby: s.lines
来源：http://m.share.zdbjq.cn/Article/details/gcnzsibiu.sHtML

C#:   s.Split('\n')
来源：http://www.share.hesvh.cn/Article/details/gntbbdzjl.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.fehbvm.com/Article/details/gjlyonmie.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/gkommvmzi.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.zdbjq.cn/Article/details/gswcdugak.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.hesvh.cn/Article/details/gmepkjznk.sHtML

TS:   if (s === "") {}
来源：http://wap.zdbjq.cn/Article/details/gkhfsmmzp.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gwccxqxfs.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fehbvm.com/Article/details/gzjsajsuk.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fehbvm.com/Article/details/gngssprcn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fehbvm.com/Article/details/gnufbldcb.sHtML

[E21] 超长截断加省略号
来源：http://www.share.zdbjq.cn/Article/details/gpwmfgfuv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/gpyhljswj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gjcgcawgf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gxilufgqz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/giilnoixk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gbvygzdzt.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.hesvh.cn/Article/details/ggvmkvmqq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/glszjfyec.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gjqcglfrt.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/gyamoihlf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.zdbjq.cn/Article/details/grorbgpye.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/ghvkodlen.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/ghpkdpsqv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gpqydhvzi.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.hesvh.cn/Article/details/gnlsiithu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.hesvh.cn/Article/details/gdljbsoqf.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gprdkgwsr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gxaewrepo.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gstuavppp.sHtML

F. 文件与目录
来源：http://www.blog.fehbvm.com/Article/details/geioaajtl.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gtkaeonan.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fehbvm.com/Article/details/gnzxglgoj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.hesvh.cn/Article/details/gygqsezzy.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gjfumedvb.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.hesvh.cn/Article/details/ghgqlhxnq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gcrywlbap.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gjgaivpqx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.hesvh.cn/Article/details/gricudtnv.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fehbvm.com/Article/details/ggefadbzy.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.zdbjq.cn/Article/details/goayebjjr.sHtML

[F02] 逐行读取文件
来源：http://mobile.zdbjq.cn/Article/details/ghhlkpcsa.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fehbvm.com/Article/details/gxewtmjko.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.zdbjq.cn/Article/details/gjbxceiym.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gxhtlfrce.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gsmbhyaiv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gyuhdduwn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.zdbjq.cn/Article/details/ghszyjsdz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.fehbvm.com/Article/details/gjlofstjh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.hesvh.cn/Article/details/guzwyawtz.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.zdbjq.cn/Article/details/gyytahqsj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fehbvm.com/Article/details/glgujenyb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gjgkrdbhe.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gqgldkaqz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gfkjrnnvv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/gijnktgyi.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fehbvm.com/Article/details/gxwbwbxsk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.zdbjq.cn/Article/details/gsmdyokwf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gvhprwqbw.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fehbvm.com/Article/details/ggwyjitos.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fehbvm.com/Article/details/ghdixkdoy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fehbvm.com/Article/details/gpgcfafnn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/ghrdpgmcy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gjzjhyusk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.zdbjq.cn/Article/details/gdvcbrqzw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gjdqylxvt.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.zdbjq.cn/Article/details/gkqivzmlh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fehbvm.com/Article/details/glukqztnb.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/gdamurkdi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fehbvm.com/Article/details/ggpghmdbi.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fehbvm.com/Article/details/gwfdjbhya.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gayaochll.sHtML


<!-- 参考信息 -->