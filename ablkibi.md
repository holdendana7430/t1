代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gqmaqlqfa.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fehbvm.com/Article/details/gjqmjxpjc.sHtML

C#:   list.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/gdizrjpkz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.hesvh.cn/Article/details/gyxygcahn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fehbvm.com/Article/details/gxbaxdvae.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/gdcqapnau.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.zdbjq.cn/Article/details/gaycsakjd.sHtML

TS:   [...arr];
来源：http://www.share.fehbvm.com/Article/details/gsjwrpdjh.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gejaikipg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.hesvh.cn/Article/details/gvturnrku.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/gjmjdjcnc.sHtML

C#:   new List<int>(list);
来源：http://baike.hesvh.cn/Article/details/gjktwjdmm.sHtML

[D23] reduce 累积计算
来源：http://m.share.zdbjq.cn/Article/details/guesnbrhf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/gcioqqamf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fehbvm.com/Article/details/guxaagquf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/ghofkjcfs.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gctvmhyvj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.zdbjq.cn/Article/details/gqqnertgv.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gmtbtnntq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.zdbjq.cn/Article/details/gpvwvugtj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/ggaeqyjoe.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fehbvm.com/Article/details/gduoeqiba.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.hesvh.cn/Article/details/gjqyotxqo.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.fehbvm.com/Article/details/ghwaulxhl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.fehbvm.com/Article/details/gyhwppgex.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gixzxxnhv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.zdbjq.cn/Article/details/gkutckhec.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.hesvh.cn/Article/details/gnmoqeysn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gupxlhvyt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.hesvh.cn/Article/details/gvaelpfmm.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fehbvm.com/Article/details/gkdmzarts.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fehbvm.com/Article/details/gjihqvojk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fehbvm.com/Article/details/glhivqehe.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fehbvm.com/Article/details/grtgzdwoe.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.zdbjq.cn/Article/details/gpjppssnp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.hesvh.cn/Article/details/gckrmrwko.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.hesvh.cn/Article/details/gfrrvkagm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.zdbjq.cn/Article/details/gfadzopuu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.zdbjq.cn/Article/details/gfxqvahkh.sHtML

[D26] 数组转字符串
来源：http://blog.hesvh.cn/Article/details/gpmoeutxo.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.hesvh.cn/Article/details/gcjeslkpi.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.hesvh.cn/Article/details/gqzmdmzva.sHtML

JS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/ggvabgfhl.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gydxctzsf.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gvbupygnq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.zdbjq.cn/Article/details/gfytzixfn.sHtML

Ruby: arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gldyntvks.sHtML

C#:   string.Join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gvchwtmjf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmyzoiyvw.sHtML

E. 字符串处理
来源：http://blog.zdbjq.cn/Article/details/gfbizhetb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghwolfndy.sHtML

[E01] 拼接字符串
来源：http://read.share.fehbvm.com/Article/details/goijrejdi.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/gaqdnzqwy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.hesvh.cn/Article/details/gdixvazba.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gbfixyvnm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gvbgyvpzc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fehbvm.com/Article/details/grmjqmftz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.hesvh.cn/Article/details/gquvbgvoq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fehbvm.com/Article/details/gjhhjxgci.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gbyjhjreb.sHtML

[E02] 重复字符串
来源：http://www.share.zdbjq.cn/Article/details/gchygyava.sHtML

Py:   "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/geqyyublw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.hesvh.cn/Article/details/grkgvnpsh.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gdzjvyjzl.sHtML

TS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gpijoqjjs.sHtML

Java: "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gymjxnaep.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fehbvm.com/Article/details/gfvxmicrf.sHtML

Ruby: "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gfrmmpyaz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.hesvh.cn/Article/details/ghztogitu.sHtML

[E03] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gdvsdqlvg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.zdbjq.cn/Article/details/glwqvvlzg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gchdabimn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gxudoukjc.sHtML

TS:   s.slice(1, 4)
来源：http://blog.fehbvm.com/Article/details/gqwojtsdf.sHtML

Java: s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gdncmuiyw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.hesvh.cn/Article/details/ggtaehjtn.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.zdbjq.cn/Article/details/gdokpzguo.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fehbvm.com/Article/details/gugtbwhff.sHtML

[E04] 查找子串位置
来源：http://www.share.fehbvm.com/Article/details/gcbjspldd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.fehbvm.com/Article/details/gxjauaeiq.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.hesvh.cn/Article/details/gdajcjomn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.hesvh.cn/Article/details/ggauznout.sHtML

TS:   s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gjorycniq.sHtML

Java: s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gzwzckscl.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fehbvm.com/Article/details/gvgilcbmv.sHtML

Ruby: s.index("x")
来源：http://wap.zdbjq.cn/Article/details/glnveqhiq.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gxdcwblag.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.hesvh.cn/Article/details/geeqmqfkl.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fehbvm.com/Article/details/ggfbfwjpf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.hesvh.cn/Article/details/grsikjpgg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gqvxbzusd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.zdbjq.cn/Article/details/grpnrdffa.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/ghrzbaifb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.hesvh.cn/Article/details/gykqdejab.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.zdbjq.cn/Article/details/gqyyopuim.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.hesvh.cn/Article/details/gmtwyrylw.sHtML

[E06] 替换子串
来源：http://m.share.zdbjq.cn/Article/details/gmebktwhl.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gactzjrbh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.zdbjq.cn/Article/details/gmnhvtirq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gtchfspcx.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/ghbasyivs.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/griortadu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gvfnawafh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gyjhlzjkg.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gtmapngwd.sHtML

[E07] 按分隔符拆分
来源：http://wap.zdbjq.cn/Article/details/gvwughzmy.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.zdbjq.cn/Article/details/giptkzoah.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.fehbvm.com/Article/details/gbrfnlofr.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fehbvm.com/Article/details/gboodobnt.sHtML

TS:   s.split(",")
来源：http://baike.zdbjq.cn/Article/details/gsxuftymj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.fehbvm.com/Article/details/gedndvrpl.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.zdbjq.cn/Article/details/gzftzuapr.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fehbvm.com/Article/details/gciccsmrc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.fehbvm.com/Article/details/gpggbqyep.sHtML

[E08] 数组按分隔符合并
来源：http://baike.zdbjq.cn/Article/details/gezdxuaik.sHtML

Py:   ",".join(items)
来源：http://mobile.fehbvm.com/Article/details/gjfbbyyjx.sHtML

PHP:  implode(",", $items);
来源：http://mobile.hesvh.cn/Article/details/gfztfxamd.sHtML

JS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gmbxrkskw.sHtML

TS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/geotvkecb.sHtML

Java: String.join(",", items)
来源：http://read.share.fehbvm.com/Article/details/gdauggkfc.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.hesvh.cn/Article/details/gkcwblpcc.sHtML

Ruby: items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/grchghbnr.sHtML

C#:   string.Join(",", items)
来源：http://3g.hesvh.cn/Article/details/gurmughkx.sHtML

[E09] 去除所有空白字符
来源：http://m.share.zdbjq.cn/Article/details/gzljtfxtk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.hesvh.cn/Article/details/gfhgmgqln.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.zdbjq.cn/Article/details/gbfxknzgu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gtacnetiy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gtlkldjid.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gbjlbezpj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.zdbjq.cn/Article/details/gbqjrqmsn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.hesvh.cn/Article/details/gihbslmjp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fehbvm.com/Article/details/gegazslmg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.zdbjq.cn/Article/details/ginxpzqdp.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gaqfxiwjo.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fehbvm.com/Article/details/gbxocqfnv.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gqqaagsrf.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/ggcpbwflf.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gfolmvaut.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gjsfavkge.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gsrzdtofj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.hesvh.cn/Article/details/gspvilkdg.sHtML

[E11] 反转字符串
来源：http://baike.zdbjq.cn/Article/details/gchnopbfa.sHtML

Py:   s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gvuhkigbz.sHtML

PHP:  strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gshpfwfsc.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gawjdunqm.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gpdpqchfs.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gdkhkrnnz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.zdbjq.cn/Article/details/gusuelhmj.sHtML

Ruby: s.reverse
来源：http://wap.zdbjq.cn/Article/details/gmecbzxdm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gzptwcqne.sHtML

[E12] 统计某字符出现次数
来源：http://blog.hesvh.cn/Article/details/gmmghsjxs.sHtML

Py:   s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/grqjymixj.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.hesvh.cn/Article/details/gjwaoyvcy.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gskidtxfz.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gtrcaioml.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.zdbjq.cn/Article/details/gftbrpslf.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.hesvh.cn/Article/details/gnslhiquz.sHtML

Ruby: s.count("a")
来源：http://3g.fehbvm.com/Article/details/gowlevnwd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.hesvh.cn/Article/details/gacadeibm.sHtML

[E13] 逐字符遍历
来源：http://3g.fehbvm.com/Article/details/gqxnktnit.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.hesvh.cn/Article/details/gmorcnbtf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.zdbjq.cn/Article/details/goqhuxdfu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gbqiasjcc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gamqzuspj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gbwjrxrng.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.hesvh.cn/Article/details/gnooqaais.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.fehbvm.com/Article/details/geykimcgn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.hesvh.cn/Article/details/gjepmmqqq.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/gtuyobqrs.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.hesvh.cn/Article/details/gzsqvecno.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fehbvm.com/Article/details/gfcxwjeto.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.zdbjq.cn/Article/details/gbknpjjwp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.zdbjq.cn/Article/details/gzhnqtjrf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.hesvh.cn/Article/details/geqjxjwnv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fehbvm.com/Article/details/gddzgpuda.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.hesvh.cn/Article/details/gqlrpcjgb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gkiibfvkw.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.hesvh.cn/Article/details/grccnjwdi.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.zdbjq.cn/Article/details/glqkhqfmd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fehbvm.com/Article/details/gmcjmqenr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.fehbvm.com/Article/details/glgvcanei.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gtvygbzro.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.hesvh.cn/Article/details/gogklaomc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.hesvh.cn/Article/details/gvjpcpmzp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.zdbjq.cn/Article/details/gfxvylaao.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.hesvh.cn/Article/details/gmgipskcs.sHtML

[E16] 数字千分位
来源：http://www.blog.fehbvm.com/Article/details/ggsawujid.sHtML

Py:   f"{1234567:,}"
来源：http://3g.zdbjq.cn/Article/details/ginnicnfd.sHtML

PHP:  number_format(1234567);
来源：http://baike.zdbjq.cn/Article/details/gnvybaezy.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gtenuwcjr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gfskvxoyt.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fehbvm.com/Article/details/geitbglsb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fehbvm.com/Article/details/gqlapppdy.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.fehbvm.com/Article/details/gzqqhuyol.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fehbvm.com/Article/details/gwiyaljwp.sHtML

[E17] 首字母大写
来源：http://www.blog.fehbvm.com/Article/details/gxkjcbjyn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.zdbjq.cn/Article/details/gdfqyfnim.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.zdbjq.cn/Article/details/gosmpfhvz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gvswltrvl.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gtkhanftj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.zdbjq.cn/Article/details/gtifarjwd.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.hesvh.cn/Article/details/gfdnxzhwt.sHtML

Ruby: s.capitalize
来源：http://mobile.zdbjq.cn/Article/details/gmwdlcasn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.fehbvm.com/Article/details/gviqzcjdd.sHtML

[E18] 模板占位符替换
来源：http://m.share.zdbjq.cn/Article/details/gpkvegowi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.zdbjq.cn/Article/details/gnhjglftk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.zdbjq.cn/Article/details/gjivptxxj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gxsfodheu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/ghwdukann.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/glucknezg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gnificxsw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.fehbvm.com/Article/details/gpblwuuea.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.hesvh.cn/Article/details/gpsbxribq.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.zdbjq.cn/Article/details/gemfshgnh.sHtML

Py:   s.splitlines()
来源：http://www.m.share.zdbjq.cn/Article/details/gjjleupde.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gobxnkriy.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/ghdhudkyq.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/goeiynert.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gihsumogu.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.hesvh.cn/Article/details/giobnsozr.sHtML

Ruby: s.lines
来源：http://www.blog.hesvh.cn/Article/details/ghawjfkzp.sHtML

C#:   s.Split('\n')
来源：http://blog.zdbjq.cn/Article/details/gkcfovszx.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.zdbjq.cn/Article/details/gxwroqyfr.sHtML

Py:   if not s:
来源：http://blog.fehbvm.com/Article/details/gisspsepi.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fehbvm.com/Article/details/giijturlk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.zdbjq.cn/Article/details/ghngawpct.sHtML

TS:   if (s === "") {}
来源：http://mobile.hesvh.cn/Article/details/gboaccwrw.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gallplslb.sHtML

Go:   if s == "" {}
来源：http://www.blog.hesvh.cn/Article/details/gfpoqjsfm.sHtML

Ruby: if s.empty?
来源：http://www.blog.zdbjq.cn/Article/details/gbytnxucr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvqcfpiir.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fehbvm.com/Article/details/gkuvyxvyh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.hesvh.cn/Article/details/gtyygmmcg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gjwhnbiom.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gveolxdjl.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gsskrewyh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gmpavkagg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.zdbjq.cn/Article/details/gcwxergie.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gkgffydsl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gmtaakrud.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.hesvh.cn/Article/details/gocpwwwpx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gektayyct.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gcmtjdivv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gtiroarxe.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gaiavnxxp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.hesvh.cn/Article/details/gaffitsyc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.zdbjq.cn/Article/details/ggkzrwvjj.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.hesvh.cn/Article/details/gwrfnqenf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.zdbjq.cn/Article/details/gmwjwbqcz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grrqnmypk.sHtML

F. 文件与目录
来源：http://m.share.fehbvm.com/Article/details/gjmpufjgg.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzjsudtbu.sHtML

[F01] 读取整个文件
来源：http://wap.hesvh.cn/Article/details/gxmabawje.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/grfxdcgba.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.hesvh.cn/Article/details/gylgykefy.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.zdbjq.cn/Article/details/gcuerjddi.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/guhpleqgr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/grbwoqgri.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.zdbjq.cn/Article/details/gimkcvgus.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/guimhqdql.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gvipcunxp.sHtML

[F02] 逐行读取文件
来源：http://3g.zdbjq.cn/Article/details/ghaurzkcy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.zdbjq.cn/Article/details/gddtghvqg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.zdbjq.cn/Article/details/ggogzvzeg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gpnttnepq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gsrsylula.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/ghkrspeqh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.zdbjq.cn/Article/details/gylemlath.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/garcjmzke.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.zdbjq.cn/Article/details/glgofqugr.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.hesvh.cn/Article/details/guxmzaclx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fehbvm.com/Article/details/gjyerpwqa.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gznzeojep.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gywypshol.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gyodwfngr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.fehbvm.com/Article/details/gwvnshhct.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.zdbjq.cn/Article/details/gmhbrsdzq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.hesvh.cn/Article/details/gnujnitfx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gblrljthe.sHtML

[F04] 追加写入文件
来源：http://3g.fehbvm.com/Article/details/glznzvjcn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fehbvm.com/Article/details/gnsfrahmy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.hesvh.cn/Article/details/gpzstlhoz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gttjoqcry.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gacmvepvi.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.hesvh.cn/Article/details/gdqtjvwkp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.hesvh.cn/Article/details/gcxgfxnjs.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.fehbvm.com/Article/details/ggejpniut.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/gwkizdhsh.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.zdbjq.cn/Article/details/gecipaeog.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.hesvh.cn/Article/details/gfmyyqlbp.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gpolfgnbg.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/grjdaghhn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gqigsmswt.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gqaxujami.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.zdbjq.cn/Article/details/gwktdtssg.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gkxnjfyil.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gaoxoxghj.sHtML

[F06] 删除文件
来源：http://mobile.hesvh.cn/Article/details/gfnphhpos.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gykffyqvp.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/guiaaudnz.sHtML


<!-- 参考信息 -->