代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gvgljemzw.sHtML

Ruby: arr.include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gigvohdrl.sHtML

C#:   list.Contains(x)
来源：http://3g.fehbvm.com/Article/details/gfkkewoqe.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fehbvm.com/Article/details/gxpfldsxm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gdjergfgk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.zdbjq.cn/Article/details/glxrfgzno.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.hesvh.cn/Article/details/gktpzseex.sHtML

TS:   [...arr];
来源：http://mobile.hesvh.cn/Article/details/gasnqrspm.sHtML

Java: new ArrayList<>(list);
来源：http://baike.zdbjq.cn/Article/details/gczddureq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.hesvh.cn/Article/details/grtnbsezf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/gmqneghwl.sHtML

C#:   new List<int>(list);
来源：http://wap.hesvh.cn/Article/details/gdtadnzcs.sHtML

[D23] reduce 累积计算
来源：http://www.share.hesvh.cn/Article/details/gbpyodahn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.hesvh.cn/Article/details/gbbqdimdp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fehbvm.com/Article/details/gxkmcrkgn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gjwzbghdm.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gbqrhackk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.zdbjq.cn/Article/details/gdnnposkr.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gntsuyacs.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.hesvh.cn/Article/details/gcxxsscwl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.zdbjq.cn/Article/details/gpbqnbahn.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.hesvh.cn/Article/details/gazwtvjqd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gejrbiyxf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.hesvh.cn/Article/details/gbonjdmvg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.fehbvm.com/Article/details/gnavjeezj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.hesvh.cn/Article/details/gfwycqnup.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.zdbjq.cn/Article/details/geviubxat.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.hesvh.cn/Article/details/ggsxgxmul.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.zdbjq.cn/Article/details/gjupgxgqv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.zdbjq.cn/Article/details/gimotbtvn.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.zdbjq.cn/Article/details/goaibyxvi.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.zdbjq.cn/Article/details/gnehngmpr.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.zdbjq.cn/Article/details/gzjcxcecg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.zdbjq.cn/Article/details/gaiceakvw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.fehbvm.com/Article/details/gxlwutlkt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fehbvm.com/Article/details/gkgucbgai.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.hesvh.cn/Article/details/gaudfyopy.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fehbvm.com/Article/details/gmicfwqdd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fehbvm.com/Article/details/ghwehnrig.sHtML

[D26] 数组转字符串
来源：http://m.share.zdbjq.cn/Article/details/gxgxsdjbw.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.hesvh.cn/Article/details/gdaedtwcp.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.zdbjq.cn/Article/details/gxdxhmjzr.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gqujemmnv.sHtML

TS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/ggvhwfukx.sHtML

Java: String.join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gdkgikelq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.hesvh.cn/Article/details/garnmyclp.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gvobsbtvg.sHtML

C#:   string.Join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gyeoxqazg.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmvnztzmq.sHtML

E. 字符串处理
来源：http://www.share.zdbjq.cn/Article/details/gtkviprvg.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gctihgorw.sHtML

[E01] 拼接字符串
来源：http://blog.fehbvm.com/Article/details/glsxbvbsi.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/gssqaryrk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.zdbjq.cn/Article/details/gpiyultod.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gebuqwbcu.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gulkfpgay.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.hesvh.cn/Article/details/gdjixlavw.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.fehbvm.com/Article/details/gudjroxfd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fehbvm.com/Article/details/gafmdmzxu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fehbvm.com/Article/details/gwjontilt.sHtML

[E02] 重复字符串
来源：http://www.share.fehbvm.com/Article/details/gslcbqijs.sHtML

Py:   "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gprlpelpu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fehbvm.com/Article/details/gcbxyclix.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/glrleycla.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gbiclxubo.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gkxhgbvrk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fehbvm.com/Article/details/gkfjqccem.sHtML

Ruby: "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gvtiittie.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fehbvm.com/Article/details/gcfkjhcmq.sHtML

[E03] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gmlzhzgoh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.hesvh.cn/Article/details/gafwzxtvp.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/ghybixlbw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gtsqocaqn.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gutaequch.sHtML

Java: s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gkhtmbxsu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gzpecnlew.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.hesvh.cn/Article/details/ggxnrgjab.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.hesvh.cn/Article/details/grimxhheu.sHtML

[E04] 查找子串位置
来源：http://mobile.fehbvm.com/Article/details/gvzrchzph.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.hesvh.cn/Article/details/ggbpavnoq.sHtML

PHP:  strpos($s, "x");
来源：http://baike.hesvh.cn/Article/details/gkxljzqxp.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.hesvh.cn/Article/details/gawvnlzov.sHtML

TS:   s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/ggdmdvzhh.sHtML

Java: s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gdxjigrsx.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.hesvh.cn/Article/details/gbeanypud.sHtML

Ruby: s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gxnaxblew.sHtML

C#:   s.IndexOf("x")
来源：http://baike.fehbvm.com/Article/details/gsbaxhjkf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.zdbjq.cn/Article/details/gsfpblluc.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.hesvh.cn/Article/details/gtehnuoip.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.hesvh.cn/Article/details/gckqqafom.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gimvewcox.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.hesvh.cn/Article/details/gmfmdpwjy.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gpzhxzxkv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.zdbjq.cn/Article/details/gyepvmaxv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.hesvh.cn/Article/details/guhnhroay.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gdqoauhja.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/gykginouq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gvyvusqzu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fehbvm.com/Article/details/gbssbwnba.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gnrojemas.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gyfoylaef.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/guokmtcmv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gdagklgte.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gegnqvfqh.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.hesvh.cn/Article/details/gjarsjmlo.sHtML

[E07] 按分隔符拆分
来源：http://3g.zdbjq.cn/Article/details/gdhzkwmnr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.fehbvm.com/Article/details/gkxojxyho.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.fehbvm.com/Article/details/gkjuvhgtj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.fehbvm.com/Article/details/gzucidvfu.sHtML

TS:   s.split(",")
来源：http://3g.zdbjq.cn/Article/details/ggfrjmxbf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.hesvh.cn/Article/details/glyygzgxr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.hesvh.cn/Article/details/grgdqbkzb.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.zdbjq.cn/Article/details/gnaqmkxhn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fehbvm.com/Article/details/gzimlmwud.sHtML

[E08] 数组按分隔符合并
来源：http://blog.zdbjq.cn/Article/details/gjmocqbuz.sHtML

Py:   ",".join(items)
来源：http://www.blog.hesvh.cn/Article/details/gawssryfa.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fehbvm.com/Article/details/gljjblyhp.sHtML

JS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/glgeqddla.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gcgqtkvdg.sHtML

Java: String.join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gmnlkmpah.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fehbvm.com/Article/details/ggiqugxcd.sHtML

Ruby: items.join(",")
来源：http://3g.fehbvm.com/Article/details/gxmjxhvqo.sHtML

C#:   string.Join(",", items)
来源：http://wap.hesvh.cn/Article/details/gpxbcdmup.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fehbvm.com/Article/details/gdirlezhm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.hesvh.cn/Article/details/gpqorpvcu.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.hesvh.cn/Article/details/gwavefskk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/garmsepqh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gwwzbfulw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gsbcudqpm.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.hesvh.cn/Article/details/gscbofaoj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.hesvh.cn/Article/details/guuttdjeg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gbsbwcvba.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fehbvm.com/Article/details/gpjxbpeta.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gvywrxfal.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fehbvm.com/Article/details/gxvgeecxj.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gthziuudf.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gznfgfvyi.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gaquccdqu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/glwbnjprz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gsebnsmre.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.hesvh.cn/Article/details/glbrzgvrk.sHtML

[E11] 反转字符串
来源：http://m.share.hesvh.cn/Article/details/gwprltolr.sHtML

Py:   s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gsdhzgrql.sHtML

PHP:  strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gjrhlfncy.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gqjpfknkl.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gwsibtktm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.zdbjq.cn/Article/details/gdlxsygsw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.zdbjq.cn/Article/details/gizsscpsw.sHtML

Ruby: s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/glrhhuzud.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gkzwoiakw.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.fehbvm.com/Article/details/gmxfazcjo.sHtML

Py:   s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gcumenkje.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.hesvh.cn/Article/details/gnkyufxvy.sHtML

JS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gbkglwxix.sHtML

TS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gxhhmcuhz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.hesvh.cn/Article/details/gnvtbhfce.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fehbvm.com/Article/details/gluvheyoc.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gjxkvluig.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.fehbvm.com/Article/details/gwrpapbsk.sHtML

[E13] 逐字符遍历
来源：http://www.share.fehbvm.com/Article/details/gqfwnfuxg.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.hesvh.cn/Article/details/gsssunbhm.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.hesvh.cn/Article/details/gwywlfole.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gxrbdphkc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gncvejqop.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fehbvm.com/Article/details/gwisfmvml.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fehbvm.com/Article/details/gekrtcgfa.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.zdbjq.cn/Article/details/gitmuitcs.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.zdbjq.cn/Article/details/gumrwypaz.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/ghxfflbri.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.hesvh.cn/Article/details/gkqywoakw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.zdbjq.cn/Article/details/gbzeygxry.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.fehbvm.com/Article/details/gwzzrclag.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.fehbvm.com/Article/details/gritoydhj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fehbvm.com/Article/details/gpaggaqyy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.hesvh.cn/Article/details/ggxbvzwuq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.zdbjq.cn/Article/details/gwbicmyph.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.hesvh.cn/Article/details/glpbakwtu.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.hesvh.cn/Article/details/gdjtfriqg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.fehbvm.com/Article/details/giafwjquc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gbjakozas.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.hesvh.cn/Article/details/gdjcslsgv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.zdbjq.cn/Article/details/grakrgyeu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.hesvh.cn/Article/details/gjdygzknj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.fehbvm.com/Article/details/gadogsljc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fehbvm.com/Article/details/gjctgvkmz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fehbvm.com/Article/details/grzthztsu.sHtML

[E16] 数字千分位
来源：http://baike.zdbjq.cn/Article/details/gwhxboahx.sHtML

Py:   f"{1234567:,}"
来源：http://3g.hesvh.cn/Article/details/gnizofjku.sHtML

PHP:  number_format(1234567);
来源：http://www.share.hesvh.cn/Article/details/glqglpqey.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/ghenuqrjy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/ghlblfwvq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.zdbjq.cn/Article/details/ggeavnfid.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fehbvm.com/Article/details/gazanxauq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.zdbjq.cn/Article/details/gymnzukof.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fehbvm.com/Article/details/gibpprefi.sHtML

[E17] 首字母大写
来源：http://wap.hesvh.cn/Article/details/gpbwmsxkf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.hesvh.cn/Article/details/guudhudxq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.hesvh.cn/Article/details/gstwqmqgj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gkgvjxtms.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gslyzawpm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fehbvm.com/Article/details/gbbblpiyh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.zdbjq.cn/Article/details/gpiuvqffo.sHtML

Ruby: s.capitalize
来源：http://mobile.fehbvm.com/Article/details/gcqviriuf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.hesvh.cn/Article/details/gxugizetx.sHtML

[E18] 模板占位符替换
来源：http://wap.hesvh.cn/Article/details/gczsyooeg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.fehbvm.com/Article/details/gnvdheuwd.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.hesvh.cn/Article/details/gheddsbvk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gccnclsyg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gkhvqplod.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gaxycvwuv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gzkkdzsev.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.hesvh.cn/Article/details/goszhvons.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.zdbjq.cn/Article/details/gytgwioom.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.hesvh.cn/Article/details/ggkihdvkx.sHtML

Py:   s.splitlines()
来源：http://m.share.hesvh.cn/Article/details/gsjtndhfg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.hesvh.cn/Article/details/ggtzcjgxe.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gyccuikrb.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gauhiaahf.sHtML

Java: s.lines().toList()
来源：http://wap.hesvh.cn/Article/details/gringwavx.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/gzqpojkda.sHtML

Ruby: s.lines
来源：http://3g.hesvh.cn/Article/details/gtoifbald.sHtML

C#:   s.Split('\n')
来源：http://baike.hesvh.cn/Article/details/gbayyejys.sHtML

[E20] 判断字符串是否为空
来源：http://baike.zdbjq.cn/Article/details/gdrimmstj.sHtML

Py:   if not s:
来源：http://mobile.zdbjq.cn/Article/details/gotucyfhi.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.fehbvm.com/Article/details/gkgpxrojj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fehbvm.com/Article/details/gfacwkbdj.sHtML

TS:   if (s === "") {}
来源：http://wap.hesvh.cn/Article/details/gktjqjchn.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gxrxqcocz.sHtML

Go:   if s == "" {}
来源：http://mobile.zdbjq.cn/Article/details/gwcsjbshy.sHtML

Ruby: if s.empty?
来源：http://www.share.zdbjq.cn/Article/details/gibhruiqc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fehbvm.com/Article/details/gtnswxfqc.sHtML

[E21] 超长截断加省略号
来源：http://3g.fehbvm.com/Article/details/gvryufudk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.zdbjq.cn/Article/details/gktiakqww.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gfwiankxw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/glusvcgxr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gszctzsle.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gehrakjqq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fehbvm.com/Article/details/gvaylnalj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gxykinrel.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gnbfxgctd.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.hesvh.cn/Article/details/gqpckqygf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.hesvh.cn/Article/details/guwgdtmiw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gbdvrbccx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gumtnmhww.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gwamkyndd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.zdbjq.cn/Article/details/gqtkyzsxk.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fehbvm.com/Article/details/ggykkeeak.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fehbvm.com/Article/details/gdbuaasci.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gwazxiqwo.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxzbugwlv.sHtML

F. 文件与目录
来源：http://blog.hesvh.cn/Article/details/guqvpyxif.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/glgxufrcp.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fehbvm.com/Article/details/gwwbdgvhn.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fehbvm.com/Article/details/gvzodszpd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/ggkzhyxpn.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.hesvh.cn/Article/details/gpmsqujte.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gojvlvgcw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gqhmfwabd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.zdbjq.cn/Article/details/gfiqhyrpv.sHtML

Ruby: File.read("a.txt")
来源：http://baike.hesvh.cn/Article/details/gmbthevrf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gusxkkpmd.sHtML

[F02] 逐行读取文件
来源：http://m.share.hesvh.cn/Article/details/gztxzbzbj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.hesvh.cn/Article/details/gtpdmcvxj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fehbvm.com/Article/details/grzqcnbnr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gddnzklpm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/goyzuermf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gwhxqnjfq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.hesvh.cn/Article/details/glwilnbbh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.zdbjq.cn/Article/details/gtrvftutb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.zdbjq.cn/Article/details/gvcyqyjxn.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.fehbvm.com/Article/details/grtwvytqw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fehbvm.com/Article/details/gbuhhighc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gudzmffzm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gkigmujug.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gkmjubqzi.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.hesvh.cn/Article/details/gzehlaako.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fehbvm.com/Article/details/gxqhywgia.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.zdbjq.cn/Article/details/gwsujzopy.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gqfaunxgh.sHtML

[F04] 追加写入文件
来源：http://m.share.fehbvm.com/Article/details/gcraphrjb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.zdbjq.cn/Article/details/gfktepojz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.hesvh.cn/Article/details/glppsehul.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gtaquwhye.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/giciaqomm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fehbvm.com/Article/details/gtinckhns.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fehbvm.com/Article/details/gretkjkmz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/gamdnzino.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fehbvm.com/Article/details/ggbctfbpa.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gbuvqqxio.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fehbvm.com/Article/details/gemujbdqw.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.hesvh.cn/Article/details/gkzxyuund.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gdfgcmrrk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gacgqghpa.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gfqqhwsgq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.zdbjq.cn/Article/details/gldkyzhqd.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gownljxoh.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gncmnnltx.sHtML

[F06] 删除文件
来源：http://blog.zdbjq.cn/Article/details/gvsagxduf.sHtML

Py:   os.remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/ginmzuvhs.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fehbvm.com/Article/details/gcyahjbds.sHtML


<!-- 参考信息 -->