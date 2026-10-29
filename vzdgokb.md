代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.hesvh.cn/Article/details/gmzfaknzl.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.hesvh.cn/Article/details/gefjduumi.sHtML

Py:   Counter(arr)
来源：http://m.share.fehbvm.com/Article/details/gdnajjchw.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.hesvh.cn/Article/details/gruvasuzn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gcauwadne.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gczfwhlhi.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.zdbjq.cn/Article/details/gyvbwuzyp.sHtML

Go:   // 手写 map[T]int
来源：http://wap.zdbjq.cn/Article/details/getueydft.sHtML

Ruby: arr.tally
来源：http://wap.zdbjq.cn/Article/details/gfqvqxgwj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.zdbjq.cn/Article/details/gnvoibpaw.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.hesvh.cn/Article/details/glssqnxpt.sHtML

Py:   x in arr
来源：http://mobile.hesvh.cn/Article/details/gwhlrxrwq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fehbvm.com/Article/details/ggepylikp.sHtML

JS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gyrsfievw.sHtML

TS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gjyujhuwx.sHtML

Java: list.contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gwokobfsc.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gayezyesw.sHtML

Ruby: arr.include?(x)
来源：http://wap.fehbvm.com/Article/details/gvgahavlg.sHtML

C#:   list.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gugkmcagh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fehbvm.com/Article/details/gepysojld.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.hesvh.cn/Article/details/guvmsqjhk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.hesvh.cn/Article/details/gsrlbqefi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fehbvm.com/Article/details/gqtcyzbsh.sHtML

TS:   [...arr];
来源：http://m.share.fehbvm.com/Article/details/gybbhjkah.sHtML

Java: new ArrayList<>(list);
来源：http://wap.hesvh.cn/Article/details/gftnowory.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.hesvh.cn/Article/details/gvvkaimbc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.zdbjq.cn/Article/details/gdauxojmw.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gurqgzxnx.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.zdbjq.cn/Article/details/gywthkolj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fehbvm.com/Article/details/gvxmqtrcy.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.zdbjq.cn/Article/details/gsgegphfv.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/geucermrs.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gynrwstwa.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.zdbjq.cn/Article/details/gpdnxtcqk.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gbxqsobzi.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fehbvm.com/Article/details/gvxigbroc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.hesvh.cn/Article/details/giwygvquv.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.zdbjq.cn/Article/details/gpexosfdp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gbuspbtit.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.zdbjq.cn/Article/details/gruyidhaw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.hesvh.cn/Article/details/gxfnjzcyy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/ghemgqvts.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.fehbvm.com/Article/details/gnqivjycq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fehbvm.com/Article/details/gpmlfvfqb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.hesvh.cn/Article/details/gttkwqjrk.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.zdbjq.cn/Article/details/gogsqpwjb.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.hesvh.cn/Article/details/ghdskbgts.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.zdbjq.cn/Article/details/grfeuxiwy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fehbvm.com/Article/details/gavrttzde.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.zdbjq.cn/Article/details/galltpstp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.hesvh.cn/Article/details/gfylklthu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/gvouddlvl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.hesvh.cn/Article/details/gpnzwsdra.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.hesvh.cn/Article/details/gywnfijop.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gbvoqzuof.sHtML

[D26] 数组转字符串
来源：http://www.blog.zdbjq.cn/Article/details/ghzyvtoaz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.hesvh.cn/Article/details/gdljulfto.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gvxxenjnb.sHtML

JS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gwjshvnqv.sHtML

TS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gobpxyzmd.sHtML

Java: String.join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gjzsmbqsn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.zdbjq.cn/Article/details/gjyzemfpy.sHtML

Ruby: arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gorzbpkue.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gdxecpxon.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gllwpudob.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/glbfinnkd.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/goghjraxn.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gusoaexwq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.fehbvm.com/Article/details/gffhswhpd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.zdbjq.cn/Article/details/gvcrzuyrf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gditswdva.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gyfzxbfoq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.hesvh.cn/Article/details/gezyolnqd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.zdbjq.cn/Article/details/gtexbufpj.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.hesvh.cn/Article/details/gwqdwmqrw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.fehbvm.com/Article/details/gvrafjsek.sHtML

[E02] 重复字符串
来源：http://wap.hesvh.cn/Article/details/gnkpbxfng.sHtML

Py:   "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gsgqoqwjg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fehbvm.com/Article/details/gimqtooaz.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gjozcuhkq.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gcqfbmlhp.sHtML

Java: "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gzytxwssm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fehbvm.com/Article/details/gwvmrftad.sHtML

Ruby: "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gwdhomumw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.hesvh.cn/Article/details/gbgryvthv.sHtML

[E03] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gsfxhidby.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.hesvh.cn/Article/details/grxofphsx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/grbcgdhkd.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gkpaktgae.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gkpqftkky.sHtML

Java: s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/grlutrmii.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gqagvnlno.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.hesvh.cn/Article/details/gihopnboz.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.fehbvm.com/Article/details/gjfarqycm.sHtML

[E04] 查找子串位置
来源：http://wap.fehbvm.com/Article/details/gbobyjipx.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gpvsbfebv.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.zdbjq.cn/Article/details/gizlrxruv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.zdbjq.cn/Article/details/gpptzqwgc.sHtML

TS:   s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/gokffwqhn.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gsvcgyeeh.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.fehbvm.com/Article/details/gbokbtrlo.sHtML

Ruby: s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gosnahmli.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/guuqgddkw.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fehbvm.com/Article/details/gjhqexzig.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fehbvm.com/Article/details/gdghseiqo.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.hesvh.cn/Article/details/gzdvipgyr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gxelaousl.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fehbvm.com/Article/details/gdqimjsve.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gubiaggyy.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.hesvh.cn/Article/details/gtiazyweb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.hesvh.cn/Article/details/grmaaocdt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gepbgpklw.sHtML

[E06] 替换子串
来源：http://www.share.fehbvm.com/Article/details/gyuaupcix.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gigylsita.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.zdbjq.cn/Article/details/gfnpbvaxv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/ghnswbtho.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gwbunkyyw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gnbgbwimf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gqrvchhoq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.hesvh.cn/Article/details/goxgwhpxs.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gelykjixx.sHtML

[E07] 按分隔符拆分
来源：http://www.share.hesvh.cn/Article/details/gkrueczwu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.zdbjq.cn/Article/details/ghtvxudlh.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.zdbjq.cn/Article/details/gmyekrtjx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.hesvh.cn/Article/details/geaeffcfa.sHtML

TS:   s.split(",")
来源：http://read.share.fehbvm.com/Article/details/geqfxcrte.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.hesvh.cn/Article/details/glutgifow.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.hesvh.cn/Article/details/gfcflzkbb.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.zdbjq.cn/Article/details/gdxovopwp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.fehbvm.com/Article/details/gmqxpkqza.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.zdbjq.cn/Article/details/gxmupshxk.sHtML

Py:   ",".join(items)
来源：http://www.share.hesvh.cn/Article/details/gvzqsuroi.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.zdbjq.cn/Article/details/giadjaigl.sHtML

JS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gsquiwifp.sHtML

TS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/graulehgj.sHtML

Java: String.join(",", items)
来源：http://3g.zdbjq.cn/Article/details/ghswgvotq.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.zdbjq.cn/Article/details/grphlytgl.sHtML

Ruby: items.join(",")
来源：http://blog.hesvh.cn/Article/details/gwrexgwab.sHtML

C#:   string.Join(",", items)
来源：http://blog.zdbjq.cn/Article/details/ggdsydjcg.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.zdbjq.cn/Article/details/gzqgmegnm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.zdbjq.cn/Article/details/gkvrceuza.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.hesvh.cn/Article/details/geaqxvzmx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gebjopfdb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/grgixblax.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/goiawxzme.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.zdbjq.cn/Article/details/ghvmymjrf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.zdbjq.cn/Article/details/ghesmkmfi.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.fehbvm.com/Article/details/gidvxykur.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fehbvm.com/Article/details/gatfqkcan.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gnmhvfpyx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.zdbjq.cn/Article/details/ghgurkmkf.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/ghzbqhqkh.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gejzqkztu.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gxpybnmlo.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gkqrmuing.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gbknuknie.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.fehbvm.com/Article/details/googyzblz.sHtML

[E11] 反转字符串
来源：http://baike.hesvh.cn/Article/details/gombgshdk.sHtML

Py:   s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gqbnxzxcu.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gwvulobdd.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gsuuzzekf.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/guevyakwf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.zdbjq.cn/Article/details/gsrabehqx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.zdbjq.cn/Article/details/gwrtvyyee.sHtML

Ruby: s.reverse
来源：http://3g.hesvh.cn/Article/details/gndvkdbln.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gnkurivnk.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fehbvm.com/Article/details/gfjpsauaq.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gqsdzosgl.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fehbvm.com/Article/details/gkxcarugg.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/guorhwlye.sHtML

TS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gcmovtltj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.hesvh.cn/Article/details/gtwdcgamr.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.hesvh.cn/Article/details/gbzihgmvn.sHtML

Ruby: s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/gdbtoqgvg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fehbvm.com/Article/details/gujqyrkik.sHtML

[E13] 逐字符遍历
来源：http://www.blog.hesvh.cn/Article/details/glfjzrgjh.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.fehbvm.com/Article/details/gdwqemcli.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fehbvm.com/Article/details/gmpphlmqm.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gwpheuico.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/giiznvtzj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/guujweuah.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.hesvh.cn/Article/details/ggmyolgvr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fehbvm.com/Article/details/ggccqdkrf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fehbvm.com/Article/details/gtaskwoqh.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/gjelutwtc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.fehbvm.com/Article/details/gnzeadyia.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fehbvm.com/Article/details/gpccpddmc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.hesvh.cn/Article/details/gebsfejxb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.zdbjq.cn/Article/details/goszivhow.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fehbvm.com/Article/details/goystfddb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.hesvh.cn/Article/details/gifmnghmo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.zdbjq.cn/Article/details/gypedswcj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gcqkzaund.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fehbvm.com/Article/details/gafxyuevg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.zdbjq.cn/Article/details/grmpwsbqh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/ghiuqiowx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fehbvm.com/Article/details/gyhvyeaog.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.zdbjq.cn/Article/details/gazbcvnxa.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fehbvm.com/Article/details/gigqgcqwk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.hesvh.cn/Article/details/ghcfphyim.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.zdbjq.cn/Article/details/gvwrhcjum.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gdazkplti.sHtML

[E16] 数字千分位
来源：http://wap.fehbvm.com/Article/details/gluftuwrx.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fehbvm.com/Article/details/gamitchse.sHtML

PHP:  number_format(1234567);
来源：http://3g.zdbjq.cn/Article/details/gkzkehhdv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/geyocxaqz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gffxlelgt.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.hesvh.cn/Article/details/gmqrlijcu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fehbvm.com/Article/details/ghtchkhdh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.zdbjq.cn/Article/details/gsuuyzfpg.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fehbvm.com/Article/details/ggnlpqoju.sHtML

[E17] 首字母大写
来源：http://mobile.hesvh.cn/Article/details/gglczntsu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/gjvtyznwy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fehbvm.com/Article/details/gmobigidr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/grkczbing.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/guoybeuwa.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.zdbjq.cn/Article/details/gvzsitnxo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.hesvh.cn/Article/details/gtshhhhrs.sHtML

Ruby: s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/gokplnmkn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.hesvh.cn/Article/details/gskeggeqb.sHtML

[E18] 模板占位符替换
来源：http://read.share.fehbvm.com/Article/details/glzukxnch.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.zdbjq.cn/Article/details/gfzukypiz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.hesvh.cn/Article/details/gvbsubuwr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gpirlemzw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gfrsummwc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gbegxwyad.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.hesvh.cn/Article/details/gtnfywndr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.hesvh.cn/Article/details/gpoifvpiw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.hesvh.cn/Article/details/ghktpeivr.sHtML

[E19] 多行文本按行拆分
来源：http://baike.hesvh.cn/Article/details/gjdjhtxid.sHtML

Py:   s.splitlines()
来源：http://www.share.zdbjq.cn/Article/details/gqsinfeyl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gutpawqrd.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/guplimvir.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/glhxglrhx.sHtML

Java: s.lines().toList()
来源：http://read.share.zdbjq.cn/Article/details/gjcrnlnaz.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.hesvh.cn/Article/details/gnluitdws.sHtML

Ruby: s.lines
来源：http://www.share.hesvh.cn/Article/details/gddnxnnkp.sHtML

C#:   s.Split('\n')
来源：http://blog.zdbjq.cn/Article/details/gxxieelpw.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.hesvh.cn/Article/details/gridkspgw.sHtML

Py:   if not s:
来源：http://read.share.fehbvm.com/Article/details/gcxtukhzh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/gsqquqhuv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fehbvm.com/Article/details/gjuzephmt.sHtML

TS:   if (s === "") {}
来源：http://m.share.hesvh.cn/Article/details/gjoiszkon.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gxlrwzmoz.sHtML

Go:   if s == "" {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmmmewtoz.sHtML

Ruby: if s.empty?
来源：http://m.share.zdbjq.cn/Article/details/gfkmaebok.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fehbvm.com/Article/details/ghwyhwgso.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fehbvm.com/Article/details/ghtnfeibt.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.hesvh.cn/Article/details/grbphhrgy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/goypuddfw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gujncgenm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gjnivpsga.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gplfsvfsr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.zdbjq.cn/Article/details/gxxuxcomr.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/grgtdoxcc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/ggmruulms.sHtML

[E22] 字节长度与字符长度
来源：http://wap.zdbjq.cn/Article/details/gtdtvaxid.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.hesvh.cn/Article/details/gugcjnpvs.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gwprdodcy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gqjnkokcl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/godhxicwi.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fehbvm.com/Article/details/gzryzkleh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.hesvh.cn/Article/details/gquokcejp.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fehbvm.com/Article/details/gvtyexlba.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gbomscfyn.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvluwijek.sHtML

F. 文件与目录
来源：http://blog.fehbvm.com/Article/details/gyjigopiz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzfexfoes.sHtML

[F01] 读取整个文件
来源：http://3g.zdbjq.cn/Article/details/gvtsxgvrl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/gbsxyuykt.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gqoetciry.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.hesvh.cn/Article/details/gizdjvsnz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.hesvh.cn/Article/details/gdalknuig.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gxpeyharc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.zdbjq.cn/Article/details/gzcmispvx.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gdokchbwe.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/ghnsqhrgb.sHtML

[F02] 逐行读取文件
来源：http://wap.zdbjq.cn/Article/details/gjcuhkkqa.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.hesvh.cn/Article/details/gbsmyfbqu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fehbvm.com/Article/details/gtsmjoeud.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gkctdejbn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gpaufywev.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gasydhnij.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.zdbjq.cn/Article/details/gertorlda.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.fehbvm.com/Article/details/gexlgkava.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.hesvh.cn/Article/details/gizqvivvv.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fehbvm.com/Article/details/gobfcfitn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.zdbjq.cn/Article/details/gkakmqzfm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gbwmahqxk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/ghrrcnqbb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/goxufhkhl.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/gdzklbmpr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fehbvm.com/Article/details/gtellmcuy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fehbvm.com/Article/details/ggnjcnvtf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gvvlfgkfk.sHtML

[F04] 追加写入文件
来源：http://www.m.share.zdbjq.cn/Article/details/ggzbxurpc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.fehbvm.com/Article/details/gctyrjuqg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.hesvh.cn/Article/details/gujqphwod.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/glvxkchcq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/guiybgthh.sHtML


<!-- 参考信息 -->