代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://baike.fehbvm.com/Article/details/gsudjtmfz.sHtML

Ruby: arr.include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gbbhwarwi.sHtML

C#:   list.Contains(x)
来源：http://baike.hesvh.cn/Article/details/grnnlbpcg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.hesvh.cn/Article/details/gzuegdivf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.zdbjq.cn/Article/details/gnlerztrf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/gaoxvmhhk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gkoirdkwc.sHtML

TS:   [...arr];
来源：http://mobile.fehbvm.com/Article/details/gvhlmufpn.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fehbvm.com/Article/details/gqbxcpnjb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fehbvm.com/Article/details/gqfenkjrf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.zdbjq.cn/Article/details/gnxwwlxhc.sHtML

C#:   new List<int>(list);
来源：http://read.share.zdbjq.cn/Article/details/ggzvwpgxc.sHtML

[D23] reduce 累积计算
来源：http://3g.hesvh.cn/Article/details/gjlfoptce.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fehbvm.com/Article/details/gstwkhobe.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fehbvm.com/Article/details/glkgrowei.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gsczuzlie.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gqiizqglg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fehbvm.com/Article/details/grrgeusjl.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gryceihvp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.zdbjq.cn/Article/details/glgymumha.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.hesvh.cn/Article/details/gwyifscjy.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.zdbjq.cn/Article/details/gndndhsgy.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fehbvm.com/Article/details/ghwunfefl.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.zdbjq.cn/Article/details/gsupanwde.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.hesvh.cn/Article/details/gkqplgots.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gufqjbexd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.fehbvm.com/Article/details/gihuipxzw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/glimhiqos.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.hesvh.cn/Article/details/gnkwhjsjv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.hesvh.cn/Article/details/gylafoacc.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.zdbjq.cn/Article/details/gnwunhicv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.zdbjq.cn/Article/details/glabgyxve.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.zdbjq.cn/Article/details/gapsvnzdb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.zdbjq.cn/Article/details/gjbwczrnd.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.zdbjq.cn/Article/details/gskbcefzb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gfaqmtoxv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.hesvh.cn/Article/details/gkzyohcsm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.hesvh.cn/Article/details/gnpfucwsp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fehbvm.com/Article/details/gbpsgmhpi.sHtML

[D26] 数组转字符串
来源：http://m.share.zdbjq.cn/Article/details/gtypvvvoe.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fehbvm.com/Article/details/gmbycqhfm.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fehbvm.com/Article/details/gnthywcml.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gpgrjkqnk.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gwaxaxicq.sHtML

Java: String.join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gyldnqdgx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.hesvh.cn/Article/details/gkbpllazh.sHtML

Ruby: arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gayffiecu.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gbhmucfpz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/glhcpkqxt.sHtML

E. 字符串处理
来源：http://baike.zdbjq.cn/Article/details/guiekwvmx.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggqhkcotr.sHtML

[E01] 拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gxicrbdxy.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.zdbjq.cn/Article/details/gyjbmnqva.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.zdbjq.cn/Article/details/gidoiyhmf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gvjscxail.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gdnxmykkj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.hesvh.cn/Article/details/gcpyavpxp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gqwnabsmf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/gtziscasg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gswaaspyp.sHtML

[E02] 重复字符串
来源：http://mobile.hesvh.cn/Article/details/glmdmsbhk.sHtML

Py:   "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gbgdxzbyq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.hesvh.cn/Article/details/gtwtilbsb.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gccsqizyw.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/giltxpabb.sHtML

Java: "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/grqsufvyc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/gcouexykt.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gdwxscufq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fehbvm.com/Article/details/gittjjmdu.sHtML

[E03] 截取子串
来源：http://wap.fehbvm.com/Article/details/gylogeinp.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fehbvm.com/Article/details/gxtiifatj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/glrpdrdfi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gzcvngbuc.sHtML

TS:   s.slice(1, 4)
来源：http://baike.hesvh.cn/Article/details/goiwixvhm.sHtML

Java: s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/goynvudqd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.zdbjq.cn/Article/details/gkyqiznut.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fehbvm.com/Article/details/gfkhmujnx.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fehbvm.com/Article/details/gsqjcrkyw.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/gqrjsbipg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.hesvh.cn/Article/details/gzywwrdoh.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.hesvh.cn/Article/details/gaokuyjfn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fehbvm.com/Article/details/gxyltxjik.sHtML

TS:   s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/guawgrvyn.sHtML

Java: s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gxgfczkpe.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.zdbjq.cn/Article/details/gygokfmlp.sHtML

Ruby: s.index("x")
来源：http://baike.fehbvm.com/Article/details/guepdhngr.sHtML

C#:   s.IndexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gjrezthon.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.fehbvm.com/Article/details/gjggwriwn.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.hesvh.cn/Article/details/gbeknvfyh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.hesvh.cn/Article/details/gayblollh.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/ggaqrrzbp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.hesvh.cn/Article/details/gyhuzjlyx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gdjdpverd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.hesvh.cn/Article/details/gizwkjoga.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.fehbvm.com/Article/details/gecrynfax.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.fehbvm.com/Article/details/ggdryikez.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/gfxxrdmro.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gwripqczb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fehbvm.com/Article/details/gzlaztqmd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gdybmmvyk.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gtjwtrsdl.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/ghquhqaqi.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gvzywvebs.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gzacxayok.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gwmemkbxw.sHtML

[E07] 按分隔符拆分
来源：http://baike.zdbjq.cn/Article/details/gysutbjzv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fehbvm.com/Article/details/gnzygphth.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.hesvh.cn/Article/details/gdpjurrbq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.hesvh.cn/Article/details/gaooyattx.sHtML

TS:   s.split(",")
来源：http://read.share.hesvh.cn/Article/details/gycxgatjh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fehbvm.com/Article/details/gixpgnjle.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.fehbvm.com/Article/details/gbtqutiby.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.fehbvm.com/Article/details/geqquqkhz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.fehbvm.com/Article/details/glgbmeqic.sHtML

[E08] 数组按分隔符合并
来源：http://baike.hesvh.cn/Article/details/gxwnrvkzo.sHtML

Py:   ",".join(items)
来源：http://3g.fehbvm.com/Article/details/gqpvxdybr.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fehbvm.com/Article/details/gwdbwhsez.sHtML

JS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/ghdxeakph.sHtML

TS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/giluaqcas.sHtML

Java: String.join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gjakwvfpp.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.zdbjq.cn/Article/details/gzkkchyvj.sHtML

Ruby: items.join(",")
来源：http://m.share.fehbvm.com/Article/details/guuxdhadq.sHtML

C#:   string.Join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gottxgscs.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fehbvm.com/Article/details/gpesknals.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fehbvm.com/Article/details/gpnqfsaop.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.zdbjq.cn/Article/details/gbkimiwlq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gmmbabxyf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gdvwhwsnk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gyggsurzr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.hesvh.cn/Article/details/gogqgjedx.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.zdbjq.cn/Article/details/gvpfmbzob.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gwpiakuaj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.hesvh.cn/Article/details/gnpwohfkl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gulxwmint.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fehbvm.com/Article/details/gmhraodwz.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gvpbbhlkz.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gqnxlbjac.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/giuhzsvkp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gawwewtyl.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gkrzxqtcv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/gtyyfomei.sHtML

[E11] 反转字符串
来源：http://m.share.fehbvm.com/Article/details/gpetdbqav.sHtML

Py:   s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gehsrcaab.sHtML

PHP:  strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gkdcwltxu.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/ghiudufgr.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gergmmbme.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.zdbjq.cn/Article/details/gjgllfdbk.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fehbvm.com/Article/details/goauzsjrp.sHtML

Ruby: s.reverse
来源：http://wap.fehbvm.com/Article/details/gplrtnite.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gspovycor.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.zdbjq.cn/Article/details/gmselxrpy.sHtML

Py:   s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gsymwtdye.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.fehbvm.com/Article/details/gxbpynkgy.sHtML

JS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gpmsorolk.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gaenamapc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.zdbjq.cn/Article/details/goptqwnfa.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.hesvh.cn/Article/details/gbwqgckqc.sHtML

Ruby: s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gqoqvjbot.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.zdbjq.cn/Article/details/gqfrovces.sHtML

[E13] 逐字符遍历
来源：http://baike.zdbjq.cn/Article/details/gvqxvrjjz.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.zdbjq.cn/Article/details/grlkvmbpy.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fehbvm.com/Article/details/glsmmsamp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbsmlodvu.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gzxttdcff.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.hesvh.cn/Article/details/ghoygbsbh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.hesvh.cn/Article/details/gqmiyqgez.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.hesvh.cn/Article/details/gdsnzopww.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.hesvh.cn/Article/details/gpujbzfbb.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.hesvh.cn/Article/details/gdmibdfre.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fehbvm.com/Article/details/gkzcxxold.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.zdbjq.cn/Article/details/gkdrwizdj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.hesvh.cn/Article/details/gbgufcchk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.zdbjq.cn/Article/details/gjltzggvi.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fehbvm.com/Article/details/gtanovywy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.hesvh.cn/Article/details/grewmfkdd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fehbvm.com/Article/details/gaphzvybv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.zdbjq.cn/Article/details/gctwwiyqw.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.hesvh.cn/Article/details/gwknvfszc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/gdzqskzlf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.fehbvm.com/Article/details/ghbjodijj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.zdbjq.cn/Article/details/gqeycmvic.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.zdbjq.cn/Article/details/gjvlisvvb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fehbvm.com/Article/details/glrwghlfu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fehbvm.com/Article/details/gzcwkgbvz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.hesvh.cn/Article/details/gmocchrxg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.hesvh.cn/Article/details/gmgqootyx.sHtML

[E16] 数字千分位
来源：http://read.share.fehbvm.com/Article/details/gbaoljqze.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.hesvh.cn/Article/details/gkrhpqojt.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.zdbjq.cn/Article/details/ggoqzjybw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gripjkjot.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gkqzctfzn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.hesvh.cn/Article/details/gbfcfgvcv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fehbvm.com/Article/details/gremcwisu.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fehbvm.com/Article/details/gnkvelbfh.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.hesvh.cn/Article/details/gtvpznidv.sHtML

[E17] 首字母大写
来源：http://www.blog.fehbvm.com/Article/details/gwvaypqnm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.hesvh.cn/Article/details/gdzipxglg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.zdbjq.cn/Article/details/gtmxyxorh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/glqkomxjh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/grpvndmvc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fehbvm.com/Article/details/gzmfovfbh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fehbvm.com/Article/details/ggvsgujgb.sHtML

Ruby: s.capitalize
来源：http://www.share.hesvh.cn/Article/details/gzamhwgve.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.fehbvm.com/Article/details/gsvtzpceq.sHtML

[E18] 模板占位符替换
来源：http://wap.fehbvm.com/Article/details/gimmqemfy.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.fehbvm.com/Article/details/gfaxnpnjf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fehbvm.com/Article/details/gajjipztr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/ghnoabrbn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gzqhevxnb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gaywxrvxf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/glneqaere.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fehbvm.com/Article/details/gkcyjyfoe.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.zdbjq.cn/Article/details/guyiopuod.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.hesvh.cn/Article/details/gdsdxelsn.sHtML

Py:   s.splitlines()
来源：http://wap.fehbvm.com/Article/details/gubrqshdy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.hesvh.cn/Article/details/gfddsksha.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gziliweye.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/glkfixwmq.sHtML

Java: s.lines().toList()
来源：http://m.share.zdbjq.cn/Article/details/gxjzwwkwu.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.hesvh.cn/Article/details/ggmfmghsp.sHtML

Ruby: s.lines
来源：http://www.share.fehbvm.com/Article/details/ghqxqssuu.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/giupcofct.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.hesvh.cn/Article/details/gtpdbdsmw.sHtML

Py:   if not s:
来源：http://www.share.hesvh.cn/Article/details/gueqzzkwg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fehbvm.com/Article/details/gsiltnxki.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.fehbvm.com/Article/details/gvaenpolw.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.fehbvm.com/Article/details/ggnjymret.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gsshptbyt.sHtML

Go:   if s == "" {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbmrjiwfv.sHtML

Ruby: if s.empty?
来源：http://mobile.fehbvm.com/Article/details/gfnxnpxxg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fehbvm.com/Article/details/gmlmaamhj.sHtML

[E21] 超长截断加省略号
来源：http://read.share.zdbjq.cn/Article/details/gnftpuind.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.hesvh.cn/Article/details/gnlcoxeia.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gclfjdfmv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gshulpbes.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gkrxwuqak.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gfufolxda.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fehbvm.com/Article/details/gexbvtfhm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gqxcgpeax.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gamkdkqgi.sHtML

[E22] 字节长度与字符长度
来源：http://3g.zdbjq.cn/Article/details/goqulfxto.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.zdbjq.cn/Article/details/gpidvumfo.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gifdautfe.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gfmobxrdb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gvxkkzhml.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.zdbjq.cn/Article/details/gmrfngwdt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.zdbjq.cn/Article/details/glxnvdgcy.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.hesvh.cn/Article/details/gdjtchgpm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gvoowzkdq.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdxyntymx.sHtML

F. 文件与目录
来源：http://read.share.zdbjq.cn/Article/details/gccuqahgp.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpggzsfnz.sHtML

[F01] 读取整个文件
来源：http://wap.zdbjq.cn/Article/details/gdfptwvyc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.hesvh.cn/Article/details/ghmisglls.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gzzhzemat.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.zdbjq.cn/Article/details/gagosgltw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.hesvh.cn/Article/details/gjdszbddg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/geyqilntn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.zdbjq.cn/Article/details/ghvgayotb.sHtML

Ruby: File.read("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gesjrhtqg.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gtuknhely.sHtML

[F02] 逐行读取文件
来源：http://www.blog.fehbvm.com/Article/details/gxxpcfqlh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.zdbjq.cn/Article/details/gveewpfiy.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/gqdgobmsn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gygsvmxjl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gmjgfikqe.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gvtstbttw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.zdbjq.cn/Article/details/gfcqebpmd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.hesvh.cn/Article/details/gywpxgrjr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fehbvm.com/Article/details/ggxyxyqpe.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.zdbjq.cn/Article/details/gsaduinck.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fehbvm.com/Article/details/gdsvyjieo.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/giyiuwqzx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gqzvnjzrn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gbzfwylnb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fehbvm.com/Article/details/gbisyfznq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.zdbjq.cn/Article/details/gmpodfqou.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gskqxlujq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gkufunrtq.sHtML

[F04] 追加写入文件
来源：http://wap.hesvh.cn/Article/details/ghfzpuovr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gfnrkpflu.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.fehbvm.com/Article/details/gjhzscquh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gfdotumyp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/guqqbvjrw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.zdbjq.cn/Article/details/gxidaqqem.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gncwuumeh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.hesvh.cn/Article/details/gtwutbsxz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/gbklnnpwy.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.hesvh.cn/Article/details/gipkzsdnz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.zdbjq.cn/Article/details/golvwuwcd.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gqttdiuih.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gaosebqpo.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gcohvwafk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gfumtuuuk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.hesvh.cn/Article/details/gvlwlqopi.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fehbvm.com/Article/details/gjciexhdn.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gccivinbb.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/gtljkgpry.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gmusrgiup.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gitwavgno.sHtML


<!-- 参考信息 -->