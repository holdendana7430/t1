代发 wailian999

Ruby: arr.tally
来源：http://wap.fehbvm.com/Article/details/gfnquaavg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.hesvh.cn/Article/details/gjtkjrasa.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.hesvh.cn/Article/details/gqtmuwasx.sHtML

Py:   x in arr
来源：http://wap.hesvh.cn/Article/details/guvyoioee.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fehbvm.com/Article/details/gjaapyjdt.sHtML

JS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gtcejetbn.sHtML

TS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gpizviuvu.sHtML

Java: list.contains(x)
来源：http://3g.zdbjq.cn/Article/details/gkblqwyhx.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.hesvh.cn/Article/details/gdgemedaz.sHtML

Ruby: arr.include?(x)
来源：http://blog.zdbjq.cn/Article/details/gmtedjxkd.sHtML

C#:   list.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gfxhgvpbk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fehbvm.com/Article/details/gposucogq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/gtqlvqtvv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.hesvh.cn/Article/details/grgseurnd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.zdbjq.cn/Article/details/gjltlujea.sHtML

TS:   [...arr];
来源：http://read.share.fehbvm.com/Article/details/gmdaokkgp.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.hesvh.cn/Article/details/gmnmhbgxz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fehbvm.com/Article/details/gqswauwuw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fehbvm.com/Article/details/gqthbqexe.sHtML

C#:   new List<int>(list);
来源：http://m.share.fehbvm.com/Article/details/gigprntsp.sHtML

[D23] reduce 累积计算
来源：http://wap.hesvh.cn/Article/details/grdfaovfg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fehbvm.com/Article/details/gvuxzaugj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fehbvm.com/Article/details/goerwxunx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gracfvtjr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gicqlrzfn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fehbvm.com/Article/details/gfeldismr.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gfpehshlz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.zdbjq.cn/Article/details/gzpoikclc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.fehbvm.com/Article/details/grjixwydw.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.hesvh.cn/Article/details/gohutoqcd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.zdbjq.cn/Article/details/gvffaqdja.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gyeolioma.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fehbvm.com/Article/details/gqczbsiax.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gocdopirg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.hesvh.cn/Article/details/ghverbvgv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.zdbjq.cn/Article/details/gshurqnan.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.hesvh.cn/Article/details/gmycccdno.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.hesvh.cn/Article/details/gcaupxqfd.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.hesvh.cn/Article/details/gwskwjzxg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.hesvh.cn/Article/details/gsudpqopm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gbuokjceq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.hesvh.cn/Article/details/gbsakwwkr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.zdbjq.cn/Article/details/gftlbztas.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.fehbvm.com/Article/details/gbcnwsqmq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.hesvh.cn/Article/details/gqarlkqzy.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.hesvh.cn/Article/details/grqqaygzn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.zdbjq.cn/Article/details/gkpvfgiui.sHtML

[D26] 数组转字符串
来源：http://baike.zdbjq.cn/Article/details/gkgavnkjy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gvrvecjau.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.zdbjq.cn/Article/details/gzehhloej.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gdrausejv.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gfjcpnywn.sHtML

Java: String.join(", ", list)
来源：http://3g.fehbvm.com/Article/details/ggfrtdddu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.hesvh.cn/Article/details/gohyrhpfm.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gtpvvneqg.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gssqlfowj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gsytjrlum.sHtML

E. 字符串处理
来源：http://read.share.fehbvm.com/Article/details/guxzulpmy.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gneganqol.sHtML

[E01] 拼接字符串
来源：http://blog.fehbvm.com/Article/details/gifvwdrqj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.fehbvm.com/Article/details/gmbjtkffu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.zdbjq.cn/Article/details/gsutxbnqf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gkllgxyqg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gikapmjwv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fehbvm.com/Article/details/gbtzpjuel.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.hesvh.cn/Article/details/gacbmxvyq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.zdbjq.cn/Article/details/glukhbasz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gytamzofa.sHtML

[E02] 重复字符串
来源：http://wap.hesvh.cn/Article/details/gzsdvgbhu.sHtML

Py:   "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/goskoxagx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.hesvh.cn/Article/details/ghqqyzjrq.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/ghktzuzwn.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gqtphlgms.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gibrpjfdc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.zdbjq.cn/Article/details/gycineecd.sHtML

Ruby: "ab" * 3
来源：http://3g.hesvh.cn/Article/details/gpecedveb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.fehbvm.com/Article/details/grznpulbd.sHtML

[E03] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gqwdchpkp.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.hesvh.cn/Article/details/gnjpffneo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gtbqqtqms.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gwtvcydql.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gzvjppgsr.sHtML

Java: s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/glzplcplo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.hesvh.cn/Article/details/gxvrqyngs.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.hesvh.cn/Article/details/gcriylcsk.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.hesvh.cn/Article/details/gsnosonkj.sHtML

[E04] 查找子串位置
来源：http://m.share.zdbjq.cn/Article/details/gdbknumld.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/gfhalthvx.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fehbvm.com/Article/details/gzlctmlyp.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.hesvh.cn/Article/details/gzkaygffg.sHtML

TS:   s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/gymqubjgo.sHtML

Java: s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gqsktzxnx.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.zdbjq.cn/Article/details/gmdurkcty.sHtML

Ruby: s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gozxtmopt.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gjjwzxlom.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.hesvh.cn/Article/details/gcrquodwy.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.hesvh.cn/Article/details/glubvlbtx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.hesvh.cn/Article/details/gynqntucs.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gheclbxpo.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.zdbjq.cn/Article/details/gizdmzcsi.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gqkqjtgqa.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fehbvm.com/Article/details/gbskcnqgc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.hesvh.cn/Article/details/gwbqhkjez.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gmiidhkyg.sHtML

[E06] 替换子串
来源：http://www.m.share.fehbvm.com/Article/details/gouqbfnnk.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/grfjijztu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.hesvh.cn/Article/details/gkbuiqaqn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gmnhlzqco.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gkpzaegvh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/grnnvxrlt.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gpaxwkcka.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.fehbvm.com/Article/details/ghlxluicw.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.hesvh.cn/Article/details/gdpaknecl.sHtML

[E07] 按分隔符拆分
来源：http://blog.fehbvm.com/Article/details/gyxojtjoq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fehbvm.com/Article/details/guylkrwkj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.fehbvm.com/Article/details/gdfnmzjjh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fehbvm.com/Article/details/gwpapezqj.sHtML

TS:   s.split(",")
来源：http://mobile.zdbjq.cn/Article/details/gliugcgmd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.fehbvm.com/Article/details/gtkptawvh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.zdbjq.cn/Article/details/gwwurpjkb.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.hesvh.cn/Article/details/gnegxufjf.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.fehbvm.com/Article/details/grrlpenwv.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.zdbjq.cn/Article/details/ghdqhpacw.sHtML

Py:   ",".join(items)
来源：http://wap.hesvh.cn/Article/details/gyovecxfy.sHtML

PHP:  implode(",", $items);
来源：http://blog.hesvh.cn/Article/details/gdfyidfmy.sHtML

JS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gryssatly.sHtML

TS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gjunthijg.sHtML

Java: String.join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gyndvlqfo.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.hesvh.cn/Article/details/gbkcnpznu.sHtML

Ruby: items.join(",")
来源：http://baike.fehbvm.com/Article/details/gzowmluaz.sHtML

C#:   string.Join(",", items)
来源：http://wap.fehbvm.com/Article/details/gneqajdme.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.zdbjq.cn/Article/details/gfkbcirow.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.zdbjq.cn/Article/details/gczwqwndp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.fehbvm.com/Article/details/ghjkmjwfr.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gmzpvjmkz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gdqpjghgg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gkcboyyho.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.hesvh.cn/Article/details/gfclysxru.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.hesvh.cn/Article/details/gcifajbrh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.fehbvm.com/Article/details/ggidikjkw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.fehbvm.com/Article/details/gucfssvdd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.hesvh.cn/Article/details/gajoratyd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.zdbjq.cn/Article/details/gygbykqng.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gpswuplhn.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/ghpmdichl.sHtML

Java: String.format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/genlmcxin.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gusuhmihm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/grnqhzjgj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fehbvm.com/Article/details/gsgdzxeww.sHtML

[E11] 反转字符串
来源：http://blog.hesvh.cn/Article/details/gkkceewyh.sHtML

Py:   s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gjblrzcmu.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/ggmjgrlxa.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gwqwobjme.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gqmokagaj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gkvsmfkny.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fehbvm.com/Article/details/gqostxxxn.sHtML

Ruby: s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gewtynkpm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gwdjtuzis.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.zdbjq.cn/Article/details/gfdiwomcx.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gbocjszwq.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.hesvh.cn/Article/details/gfrhboorz.sHtML

JS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gilojopbt.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gpxjfwhwh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fehbvm.com/Article/details/gsukjmjwx.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.hesvh.cn/Article/details/gpvinugrn.sHtML

Ruby: s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gjtdsbeea.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fehbvm.com/Article/details/gwxefeogc.sHtML

[E13] 逐字符遍历
来源：http://www.share.fehbvm.com/Article/details/gsvucinnm.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.fehbvm.com/Article/details/gsljnwmfp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.hesvh.cn/Article/details/gacwcduws.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gbwezcesi.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/guahhwbqe.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.zdbjq.cn/Article/details/gdxcjbnwa.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.fehbvm.com/Article/details/guwmuwtge.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fehbvm.com/Article/details/glsvhcwyc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.hesvh.cn/Article/details/gvosunskf.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fehbvm.com/Article/details/gzbovfgwm.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.zdbjq.cn/Article/details/gsmtumsqh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fehbvm.com/Article/details/gxtvxlops.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.zdbjq.cn/Article/details/gapmwdqun.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.zdbjq.cn/Article/details/gcdobxbpo.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.hesvh.cn/Article/details/gxgpwiedl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.hesvh.cn/Article/details/gblpsqgzq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fehbvm.com/Article/details/gzinshskp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.hesvh.cn/Article/details/givqzydir.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/gmplfaoey.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.zdbjq.cn/Article/details/gsvwqqmjw.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gcbfvqdpc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.hesvh.cn/Article/details/gblnlrzei.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.zdbjq.cn/Article/details/gdotwhevv.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.hesvh.cn/Article/details/gqmhqvyjb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fehbvm.com/Article/details/gsegugkvx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.hesvh.cn/Article/details/gzeelrwff.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.hesvh.cn/Article/details/gkdzgtznl.sHtML

[E16] 数字千分位
来源：http://3g.hesvh.cn/Article/details/gxqbsqogs.sHtML

Py:   f"{1234567:,}"
来源：http://blog.fehbvm.com/Article/details/gwntqgsch.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fehbvm.com/Article/details/grpyovdyr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gwfiicked.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gzmyxxema.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gnxhphcev.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.zdbjq.cn/Article/details/gjohjmlmg.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.hesvh.cn/Article/details/gkbrvfmwd.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.zdbjq.cn/Article/details/gvebyhjld.sHtML

[E17] 首字母大写
来源：http://mobile.zdbjq.cn/Article/details/gzzsvhhuq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.hesvh.cn/Article/details/gjcpcobor.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.fehbvm.com/Article/details/gaucmovvk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/giskinbvq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gmkjaagos.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fehbvm.com/Article/details/glkkbybzy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.zdbjq.cn/Article/details/gomfxbvga.sHtML

Ruby: s.capitalize
来源：http://www.share.hesvh.cn/Article/details/gcpfwldvu.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.hesvh.cn/Article/details/gxtkuijfc.sHtML

[E18] 模板占位符替换
来源：http://www.blog.hesvh.cn/Article/details/ggqcyroyq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.zdbjq.cn/Article/details/gevozwonj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fehbvm.com/Article/details/gbsrundyz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gncofwztv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/ghscebxdb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gyifpwvir.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gxvljnycj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.hesvh.cn/Article/details/gbjcqxzpv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.fehbvm.com/Article/details/ggszbhzgj.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/gehxgqnpo.sHtML

Py:   s.splitlines()
来源：http://m.share.zdbjq.cn/Article/details/gyabjaaey.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fehbvm.com/Article/details/giuikmaem.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gjufobobv.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gggeqwmga.sHtML

Java: s.lines().toList()
来源：http://3g.zdbjq.cn/Article/details/gytplpwcz.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.zdbjq.cn/Article/details/glqiqkabj.sHtML

Ruby: s.lines
来源：http://mobile.fehbvm.com/Article/details/guoawrxvl.sHtML

C#:   s.Split('\n')
来源：http://www.blog.hesvh.cn/Article/details/gnknjkkjt.sHtML

[E20] 判断字符串是否为空
来源：http://3g.zdbjq.cn/Article/details/gkpplvqls.sHtML

Py:   if not s:
来源：http://www.share.hesvh.cn/Article/details/ggqrskvum.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/gbvhjqqfb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.hesvh.cn/Article/details/grhzoxinn.sHtML

TS:   if (s === "") {}
来源：http://3g.hesvh.cn/Article/details/gcopdmfss.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gpbwtswhq.sHtML

Go:   if s == "" {}
来源：http://www.m.share.zdbjq.cn/Article/details/gujhuramt.sHtML

Ruby: if s.empty?
来源：http://m.share.zdbjq.cn/Article/details/gbydifyqu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.hesvh.cn/Article/details/grcvzzdqe.sHtML

[E21] 超长截断加省略号
来源：http://wap.zdbjq.cn/Article/details/gubfifyho.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fehbvm.com/Article/details/gcimoesqd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gvmrvrary.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gdwgcxjwo.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gigfracwt.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gsszfonkd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.hesvh.cn/Article/details/gsalvdoqs.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gqqckhkha.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gchnhpijm.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fehbvm.com/Article/details/ghdcmwpof.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.zdbjq.cn/Article/details/gjjprtiet.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/glfwqggpr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gdqorswbv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gutyndpre.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.fehbvm.com/Article/details/gcivvzinw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.fehbvm.com/Article/details/gnfxxsunt.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gpaptilyt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.hesvh.cn/Article/details/gvxlcvfto.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxjyntqiw.sHtML

F. 文件与目录
来源：http://www.share.zdbjq.cn/Article/details/gnejymrlt.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqwqkdrnt.sHtML

[F01] 读取整个文件
来源：http://blog.fehbvm.com/Article/details/gjrusakij.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.zdbjq.cn/Article/details/gxijdtush.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gopgfqaah.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.zdbjq.cn/Article/details/gxgyqshjn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fehbvm.com/Article/details/gehjtpmfr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gucolqjrn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.zdbjq.cn/Article/details/gunvjfdrb.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gwxtstcno.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.fehbvm.com/Article/details/gtzwqfetv.sHtML

[F02] 逐行读取文件
来源：http://mobile.hesvh.cn/Article/details/gjnigsthv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.hesvh.cn/Article/details/gfoxdttbv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzswwensf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/glfwznnfd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gfgciyqgu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/ggojrtxif.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.hesvh.cn/Article/details/gmqywgmzi.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.fehbvm.com/Article/details/gkjtcrrny.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fehbvm.com/Article/details/ghfqmnccs.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.hesvh.cn/Article/details/gmsgiepvi.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.zdbjq.cn/Article/details/gtxdjvwuq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/glddvaria.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gnizhgokd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gjwgqhnki.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fehbvm.com/Article/details/ghadkyfyn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.zdbjq.cn/Article/details/gvffrcuib.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.hesvh.cn/Article/details/gyuoluavh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gueaotqbo.sHtML

[F04] 追加写入文件
来源：http://baike.hesvh.cn/Article/details/glxknunae.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/gmryjragx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fehbvm.com/Article/details/gvoqihkko.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gcrokywcr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gezxwfihk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.zdbjq.cn/Article/details/gsowavhxm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fehbvm.com/Article/details/grkrtjpsp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/galqfwkyb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.hesvh.cn/Article/details/gponcfscp.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.hesvh.cn/Article/details/gxcjbhjxj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fehbvm.com/Article/details/ggeqwzshc.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/gfpqvsezx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gtzuvwlzh.sHtML


<!-- 参考信息 -->