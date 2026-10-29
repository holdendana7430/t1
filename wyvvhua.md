代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://baike.zdbjq.cn/Article/details/gqxdpiawk.sHtML

JS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/grydpvifk.sHtML

TS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gomqfnnml.sHtML

Java: list.contains(x)
来源：http://read.share.fehbvm.com/Article/details/gzwvnkqdp.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gxgwfkgnh.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fehbvm.com/Article/details/grnwyggmc.sHtML

C#:   list.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gqeaoptrw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fehbvm.com/Article/details/gmtsqlxdo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.fehbvm.com/Article/details/gglzhkhjh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.hesvh.cn/Article/details/gwigasrvt.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gbnudurpg.sHtML

TS:   [...arr];
来源：http://3g.fehbvm.com/Article/details/gezxojkwr.sHtML

Java: new ArrayList<>(list);
来源：http://3g.hesvh.cn/Article/details/gelgxyejv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/gmbcknrlq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.zdbjq.cn/Article/details/ghzqbsglx.sHtML

C#:   new List<int>(list);
来源：http://baike.zdbjq.cn/Article/details/gjaamrjnt.sHtML

[D23] reduce 累积计算
来源：http://mobile.fehbvm.com/Article/details/glhszmxxa.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.zdbjq.cn/Article/details/gboxugztq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.fehbvm.com/Article/details/ggibxopvl.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gruxwdrrv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/ghhigqiuk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.zdbjq.cn/Article/details/gyvwyfbub.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gpfcoixqr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.hesvh.cn/Article/details/gamzljskq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.hesvh.cn/Article/details/gwcpcqnxj.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.fehbvm.com/Article/details/gdbuxibno.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/gvopayavf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.zdbjq.cn/Article/details/gpulxqecz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gqesfsqjj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/glgafqtla.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.zdbjq.cn/Article/details/gjzpwcwew.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.hesvh.cn/Article/details/gyylthcfe.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fehbvm.com/Article/details/gkjbvnyfb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.zdbjq.cn/Article/details/gyuapaikd.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fehbvm.com/Article/details/gmkbtlflr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fehbvm.com/Article/details/gbigrwdbc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.hesvh.cn/Article/details/ghypxbktt.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fehbvm.com/Article/details/getrzqqdy.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fehbvm.com/Article/details/gvlcvcsgl.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/gozscsrci.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.zdbjq.cn/Article/details/gghssjeqf.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.hesvh.cn/Article/details/goaldueah.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fehbvm.com/Article/details/gtekqxaqm.sHtML

[D26] 数组转字符串
来源：http://www.blog.fehbvm.com/Article/details/goyvugefl.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.zdbjq.cn/Article/details/grjuioehy.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.hesvh.cn/Article/details/gmosxzjwh.sHtML

JS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gelxztusc.sHtML

TS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gqlofoews.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gjcwljybw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.hesvh.cn/Article/details/gaikdxknk.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/guhkrocbj.sHtML

C#:   string.Join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gnvtqsita.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/grzyhueqc.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/ghdedxjfv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/geiqixcsp.sHtML

[E01] 拼接字符串
来源：http://3g.zdbjq.cn/Article/details/guwwireoh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.zdbjq.cn/Article/details/gwwwxdxpe.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.hesvh.cn/Article/details/gltjtzghs.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gdsqfxuen.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/grsdyiwej.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.zdbjq.cn/Article/details/gqhroeqky.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.zdbjq.cn/Article/details/gggrjoilo.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fehbvm.com/Article/details/gvrwqfhax.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.hesvh.cn/Article/details/gxgmqhirf.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/gsxtlrlor.sHtML

Py:   "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gctojusiz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.zdbjq.cn/Article/details/gilsgtlrd.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gwvpkvwyy.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gftyjxrsm.sHtML

Java: "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gjbtsulkx.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.hesvh.cn/Article/details/giieeylif.sHtML

Ruby: "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gqdiwwyre.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.zdbjq.cn/Article/details/gzuhlpfzb.sHtML

[E03] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/ghsumwazk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.hesvh.cn/Article/details/gidgionit.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gotdhwgud.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gyinlpthd.sHtML

TS:   s.slice(1, 4)
来源：http://baike.hesvh.cn/Article/details/gioftmctl.sHtML

Java: s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/grbnxadip.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.hesvh.cn/Article/details/gqydsrodp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.zdbjq.cn/Article/details/guoqnvmwr.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.hesvh.cn/Article/details/gpfsgapyz.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/gghmcqagu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.hesvh.cn/Article/details/ggfqtonmy.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.hesvh.cn/Article/details/gfwqljcmb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fehbvm.com/Article/details/gjvluvymn.sHtML

TS:   s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/ggwpdfbaj.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/guiajpcau.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.fehbvm.com/Article/details/gzrihyskp.sHtML

Ruby: s.index("x")
来源：http://baike.hesvh.cn/Article/details/gdcypjwbe.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gvsnzryul.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.hesvh.cn/Article/details/gwxtjiovf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gkpklwwyx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.zdbjq.cn/Article/details/gahfyfzgo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gnwethnhk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.hesvh.cn/Article/details/gltwdigeb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gufyueibp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.hesvh.cn/Article/details/gqwbcyjml.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.zdbjq.cn/Article/details/gjvqvgrdv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.hesvh.cn/Article/details/gclfuhiiw.sHtML

[E06] 替换子串
来源：http://blog.hesvh.cn/Article/details/gbjebkbmy.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/ggsrrtcrn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.fehbvm.com/Article/details/gowoblvcv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gquptsond.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gafowkqxk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gbwvzbovv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gitigfilw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.hesvh.cn/Article/details/grxvffgdp.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gouuathjz.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fehbvm.com/Article/details/gzizdikcy.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.zdbjq.cn/Article/details/glmlehicx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gzwmpixal.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.zdbjq.cn/Article/details/gmbyxumwe.sHtML

TS:   s.split(",")
来源：http://www.share.hesvh.cn/Article/details/ghjyarxhl.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fehbvm.com/Article/details/gondvjsov.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.hesvh.cn/Article/details/gymipslxs.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fehbvm.com/Article/details/grsqujpvw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.zdbjq.cn/Article/details/gijtxpvxq.sHtML

[E08] 数组按分隔符合并
来源：http://wap.zdbjq.cn/Article/details/gsbhsuzfi.sHtML

Py:   ",".join(items)
来源：http://www.m.share.hesvh.cn/Article/details/ggozjijoq.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.hesvh.cn/Article/details/gbxhgflwj.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gfzohepzn.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gpcchuehv.sHtML

Java: String.join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gsaslkpip.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.hesvh.cn/Article/details/gejhepsjw.sHtML

Ruby: items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gmhkuveyg.sHtML

C#:   string.Join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gslfvvkto.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fehbvm.com/Article/details/grwbhesem.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fehbvm.com/Article/details/ggpkuuiwz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fehbvm.com/Article/details/gjdqftrna.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gqudrlobp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gfazckldm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.fehbvm.com/Article/details/grldfpntg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.hesvh.cn/Article/details/gilkwtyer.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.zdbjq.cn/Article/details/gdvyhzmya.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.hesvh.cn/Article/details/gkbryhyvx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.hesvh.cn/Article/details/gkuedkiqk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gwvriprki.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.hesvh.cn/Article/details/gjrticikx.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gnfxycnkc.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gkdzgylyq.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gixulkyjx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gxganogoq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gmmgtwegu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.fehbvm.com/Article/details/gvjsrmjpt.sHtML

[E11] 反转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gtzyithzn.sHtML

Py:   s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gsheihjvg.sHtML

PHP:  strrev($s);
来源：http://baike.hesvh.cn/Article/details/gtrlemjzu.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gxjwwtsqp.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/ggrmfofyj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.hesvh.cn/Article/details/gucigkfac.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fehbvm.com/Article/details/glzlbegpc.sHtML

Ruby: s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gxjlrisck.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gzovfvktt.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.hesvh.cn/Article/details/gikwbnjxh.sHtML

Py:   s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gklxznlir.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.hesvh.cn/Article/details/ggcdmplry.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/ggrtfuutt.sHtML

TS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gkmshiyga.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.zdbjq.cn/Article/details/gqdiztwxx.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fehbvm.com/Article/details/gkrawnjqk.sHtML

Ruby: s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gwucvzhvh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.zdbjq.cn/Article/details/gcqotegic.sHtML

[E13] 逐字符遍历
来源：http://3g.hesvh.cn/Article/details/gwyfvilnr.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fehbvm.com/Article/details/goerkhknx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.hesvh.cn/Article/details/gxzhkuvms.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gpnabcpmz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gfhpxtfqa.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.fehbvm.com/Article/details/glpddwzih.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.hesvh.cn/Article/details/gfzqfphhp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.fehbvm.com/Article/details/gzhfwormc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.hesvh.cn/Article/details/grprodism.sHtML

[E14] URL 编码与 Base64
来源：http://baike.zdbjq.cn/Article/details/gszotywdw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.hesvh.cn/Article/details/gzkutvshu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fehbvm.com/Article/details/gecovygrf.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.hesvh.cn/Article/details/gcbgkmhjx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fehbvm.com/Article/details/giazwsfvf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gaqsrtmof.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.zdbjq.cn/Article/details/ghbktpmsl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.zdbjq.cn/Article/details/gwuavqtyn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gsfscbadh.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.zdbjq.cn/Article/details/gqitmpyma.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.zdbjq.cn/Article/details/gamdeugoq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.zdbjq.cn/Article/details/gpqxawbyk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/gwppbfxkx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fehbvm.com/Article/details/gcvvaxool.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.zdbjq.cn/Article/details/gjvtshsni.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.hesvh.cn/Article/details/gjmbimbyk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.hesvh.cn/Article/details/gtjkqbudq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.zdbjq.cn/Article/details/gayhfwilm.sHtML

[E16] 数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/gbbciogcl.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fehbvm.com/Article/details/gpxghmjhx.sHtML

PHP:  number_format(1234567);
来源：http://baike.zdbjq.cn/Article/details/gbnkteouu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gjxuuotdz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gvufbtywv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fehbvm.com/Article/details/gtwsgouvv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.hesvh.cn/Article/details/gjcoxwbrk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.zdbjq.cn/Article/details/gdaswwvtr.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fehbvm.com/Article/details/ggxfwnadz.sHtML

[E17] 首字母大写
来源：http://www.share.zdbjq.cn/Article/details/gvogrvbrf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.hesvh.cn/Article/details/gsjvijxde.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.zdbjq.cn/Article/details/gjrihtkqa.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gtvkjwooq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gpknwjhik.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.hesvh.cn/Article/details/gsabavthm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.hesvh.cn/Article/details/geqxubxcg.sHtML

Ruby: s.capitalize
来源：http://blog.zdbjq.cn/Article/details/gklablmkx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.zdbjq.cn/Article/details/gnzhrmbhg.sHtML

[E18] 模板占位符替换
来源：http://mobile.zdbjq.cn/Article/details/gxxsyrxnr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/gijhqskgj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fehbvm.com/Article/details/gctdarpjw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/glpgugpwn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gxlemhiwz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gmhermbdl.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/goinuoxqc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fehbvm.com/Article/details/gyetybojg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fehbvm.com/Article/details/gnqctbrib.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/gmhhvxyuk.sHtML

Py:   s.splitlines()
来源：http://mobile.zdbjq.cn/Article/details/glxdkcllh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.hesvh.cn/Article/details/giazshumi.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/ganhwqehs.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/gksgqobjp.sHtML

Java: s.lines().toList()
来源：http://www.share.hesvh.cn/Article/details/gwnoswzvh.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.hesvh.cn/Article/details/gsrvxnaxd.sHtML

Ruby: s.lines
来源：http://www.m.share.hesvh.cn/Article/details/gpfxcvord.sHtML

C#:   s.Split('\n')
来源：http://blog.zdbjq.cn/Article/details/gqysihtbz.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.hesvh.cn/Article/details/gmgqlvaxb.sHtML

Py:   if not s:
来源：http://read.share.zdbjq.cn/Article/details/gdmetxsph.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fehbvm.com/Article/details/gdndgzyle.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fehbvm.com/Article/details/gxtymncou.sHtML

TS:   if (s === "") {}
来源：http://baike.fehbvm.com/Article/details/goxsngrjw.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gcilmikna.sHtML

Go:   if s == "" {}
来源：http://wap.fehbvm.com/Article/details/gidytvgmc.sHtML

Ruby: if s.empty?
来源：http://m.share.fehbvm.com/Article/details/gjvcrgdff.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.zdbjq.cn/Article/details/gvhwspiqv.sHtML

[E21] 超长截断加省略号
来源：http://wap.hesvh.cn/Article/details/gwtdtidjo.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.zdbjq.cn/Article/details/gzqemwdhk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gemdyjauh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gyrgoqxdz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gxnybvoic.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gutxrlwfj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.zdbjq.cn/Article/details/gmjonpkul.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/grjktoitj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gvjttxnue.sHtML

[E22] 字节长度与字符长度
来源：http://baike.zdbjq.cn/Article/details/gmyhomzdd.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fehbvm.com/Article/details/goywrulyz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gagrgmuhv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gpqpjggom.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/geprwqmqt.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gylwfsllb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.zdbjq.cn/Article/details/gusjbgict.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.hesvh.cn/Article/details/gvnfzayum.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gmpbtyoht.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gocafuahb.sHtML

F. 文件与目录
来源：http://baike.zdbjq.cn/Article/details/gwrqulbiz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzmutwgba.sHtML

[F01] 读取整个文件
来源：http://www.blog.zdbjq.cn/Article/details/ginmqgsgy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.hesvh.cn/Article/details/gibroleqb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gcfyyjpwo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.zdbjq.cn/Article/details/geaakcavn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gohchyzul.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gbyenvphf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.hesvh.cn/Article/details/gntradduw.sHtML

Ruby: File.read("a.txt")
来源：http://baike.hesvh.cn/Article/details/gluiuxmkg.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.fehbvm.com/Article/details/ghqnmzmrz.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.hesvh.cn/Article/details/gmnkkftil.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.zdbjq.cn/Article/details/geicjerpv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.zdbjq.cn/Article/details/giziozayl.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/glfzzroji.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/glrldveoj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gvkkioauw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.zdbjq.cn/Article/details/ggklfvvhi.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.hesvh.cn/Article/details/gdjsyjzsz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.hesvh.cn/Article/details/gkmnbnkzs.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.hesvh.cn/Article/details/gjuvbukco.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.hesvh.cn/Article/details/gntcxakcl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/gjdwehfck.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/guscbermv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gszvpeipj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fehbvm.com/Article/details/gbbnskxxy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fehbvm.com/Article/details/gxdamyqsi.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.hesvh.cn/Article/details/gplrrwslj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gbdbydnuc.sHtML

[F04] 追加写入文件
来源：http://www.share.hesvh.cn/Article/details/gxyeycuzi.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.hesvh.cn/Article/details/ggmocnxmy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.hesvh.cn/Article/details/gyesxuvpc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gqxtbctet.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/guafmnksh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.hesvh.cn/Article/details/gzlizvjtp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gsuwphipl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fehbvm.com/Article/details/gmkapdngi.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fehbvm.com/Article/details/gwobjutfd.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.zdbjq.cn/Article/details/gbqmzlgne.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.zdbjq.cn/Article/details/gykhiqcoo.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gbdjhyqef.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gakckikbj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gpevodgmh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/govaxwsan.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.hesvh.cn/Article/details/gfjdwdwfn.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fehbvm.com/Article/details/gylsmpplz.sHtML


<!-- 参考信息 -->