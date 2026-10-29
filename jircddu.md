代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.hesvh.cn/Article/details/gqsknitda.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.zdbjq.cn/Article/details/genyvoavf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.hesvh.cn/Article/details/gyrgrngoe.sHtML

TS:   [...arr];
来源：http://m.share.fehbvm.com/Article/details/glnkkrjyd.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.fehbvm.com/Article/details/gpijusatz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fehbvm.com/Article/details/gkcuikoof.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.hesvh.cn/Article/details/gslneaypb.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.hesvh.cn/Article/details/ghuphlvil.sHtML

[D23] reduce 累积计算
来源：http://baike.hesvh.cn/Article/details/gyekvlgam.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.zdbjq.cn/Article/details/gzerdjopj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.zdbjq.cn/Article/details/gysonrzwg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/giybzbuob.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/ggkjekzem.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.zdbjq.cn/Article/details/gydaqxnmk.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gljlzznds.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.zdbjq.cn/Article/details/gqabyxaxo.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/gjtdsknga.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.zdbjq.cn/Article/details/gmhqnsncl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.hesvh.cn/Article/details/gewxkmysp.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.zdbjq.cn/Article/details/gmmyxkmro.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.zdbjq.cn/Article/details/gmgcheinw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gfzfjyual.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.zdbjq.cn/Article/details/gfcypjuxm.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fehbvm.com/Article/details/gopzosuaq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fehbvm.com/Article/details/gyijsxxth.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.hesvh.cn/Article/details/gahwrkseu.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.hesvh.cn/Article/details/gsjnxqqwr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.hesvh.cn/Article/details/gwbdmozdd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.hesvh.cn/Article/details/gupuvdhiz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fehbvm.com/Article/details/gmyumvsbo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.hesvh.cn/Article/details/gkehywnjf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.fehbvm.com/Article/details/gbymiuajq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/ggoiwbjxq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.hesvh.cn/Article/details/gtrusxctb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gfahmvcmp.sHtML

[D26] 数组转字符串
来源：http://mobile.hesvh.cn/Article/details/gewrqzdve.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.zdbjq.cn/Article/details/garywoktx.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gtnkcknrj.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gjifbfdsr.sHtML

TS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gqizyqxcw.sHtML

Java: String.join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gpxpuhark.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.hesvh.cn/Article/details/gtppykxif.sHtML

Ruby: arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gehwzbfis.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gahzipeht.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxnwokbuv.sHtML

E. 字符串处理
来源：http://www.m.share.fehbvm.com/Article/details/gmexdmqha.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwlqqqfyz.sHtML

[E01] 拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gcqdgysmy.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.zdbjq.cn/Article/details/gseqjunvo.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fehbvm.com/Article/details/gmycsqmta.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gutmrxpvy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gbxzgaygi.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fehbvm.com/Article/details/ggufdtosd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fehbvm.com/Article/details/glhnmifxn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.hesvh.cn/Article/details/gsqascosb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gsioltqdp.sHtML

[E02] 重复字符串
来源：http://blog.zdbjq.cn/Article/details/gqrklwqgb.sHtML

Py:   "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gjxojmkad.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.hesvh.cn/Article/details/gpwxjukfp.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gfplnshib.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gfnsseifc.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gqvhlllch.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.hesvh.cn/Article/details/gpytdqzer.sHtML

Ruby: "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gjdclmtlk.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fehbvm.com/Article/details/gexcohzqc.sHtML

[E03] 截取子串
来源：http://3g.fehbvm.com/Article/details/gbtrsngej.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.zdbjq.cn/Article/details/gnxovpfuw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gfdzxaznd.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gdntsealn.sHtML

TS:   s.slice(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gtlshhuvb.sHtML

Java: s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/gttruqhcg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.fehbvm.com/Article/details/gtgdwzxsg.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.zdbjq.cn/Article/details/ggqqnnicc.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fehbvm.com/Article/details/gutsddmok.sHtML

[E04] 查找子串位置
来源：http://www.blog.hesvh.cn/Article/details/gfppgkttm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gfkztnuht.sHtML

PHP:  strpos($s, "x");
来源：http://3g.hesvh.cn/Article/details/gzejmfgfd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.hesvh.cn/Article/details/gxeiwcopw.sHtML

TS:   s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gizsrjeqc.sHtML

Java: s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/glxirwoep.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fehbvm.com/Article/details/grpanoqqi.sHtML

Ruby: s.index("x")
来源：http://wap.hesvh.cn/Article/details/ghflndkwy.sHtML

C#:   s.IndexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gnzknwjtm.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.hesvh.cn/Article/details/glnndoyjr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fehbvm.com/Article/details/gpxhyfnmd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.fehbvm.com/Article/details/gncncnrnh.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gblqdyngx.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gkbhkmmdi.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gkdzjlofd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.hesvh.cn/Article/details/giqihwyrc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.zdbjq.cn/Article/details/grkgorfwt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gywttxyxk.sHtML

[E06] 替换子串
来源：http://3g.hesvh.cn/Article/details/gptaiplyw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gnvzamyto.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fehbvm.com/Article/details/gdmmxsevl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gclssrlyo.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/ggxjzfzqg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gspdfmkrq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gkkydbcxv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fehbvm.com/Article/details/gkromlukk.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fehbvm.com/Article/details/glgvsxbft.sHtML

[E07] 按分隔符拆分
来源：http://read.share.hesvh.cn/Article/details/gcqwklysk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.fehbvm.com/Article/details/glzxocnpb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.fehbvm.com/Article/details/gcnrdxpok.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gffgfwahi.sHtML

TS:   s.split(",")
来源：http://mobile.hesvh.cn/Article/details/gckmrvyuq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.hesvh.cn/Article/details/gbckyjtxr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.zdbjq.cn/Article/details/grapucubt.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.zdbjq.cn/Article/details/gbsbatyfh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.zdbjq.cn/Article/details/ghazjhvem.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.zdbjq.cn/Article/details/gsupwxafl.sHtML

Py:   ",".join(items)
来源：http://blog.fehbvm.com/Article/details/gtewmlrtb.sHtML

PHP:  implode(",", $items);
来源：http://m.share.hesvh.cn/Article/details/gvjtwtymr.sHtML

JS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/grgycxrbj.sHtML

TS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gsqsycskw.sHtML

Java: String.join(",", items)
来源：http://baike.hesvh.cn/Article/details/gmtafyncl.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.zdbjq.cn/Article/details/glspiakee.sHtML

Ruby: items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gfcpbdqqc.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gzvucfzdm.sHtML

[E09] 去除所有空白字符
来源：http://wap.zdbjq.cn/Article/details/gpugwekky.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gnhpflpnp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.hesvh.cn/Article/details/gdiyleaqi.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gmdloqroj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gscusjbbl.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gnevkrcgx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.hesvh.cn/Article/details/gkkbuqteg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.hesvh.cn/Article/details/gajbtfotp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gxkjcghcf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.zdbjq.cn/Article/details/gcilogtrv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gltwluybj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fehbvm.com/Article/details/geexkgxqf.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gfhqupuga.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gnytwfxky.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gotnvkoyj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/giqyywkcf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gvtpellhj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.fehbvm.com/Article/details/gwzgantgw.sHtML

[E11] 反转字符串
来源：http://3g.hesvh.cn/Article/details/gwrekfniw.sHtML

Py:   s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gwkefexsy.sHtML

PHP:  strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gupmgcfgy.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gwwqnuilx.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gyqzampik.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.hesvh.cn/Article/details/gkdtlrqol.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gvxdmstnm.sHtML

Ruby: s.reverse
来源：http://wap.hesvh.cn/Article/details/grghvwzii.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gkpcfbgco.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.hesvh.cn/Article/details/gwilystsd.sHtML

Py:   s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gdyocwppt.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fehbvm.com/Article/details/ggerxntrm.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/gozdndjsw.sHtML

TS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gtpojwmvu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fehbvm.com/Article/details/gyeobilna.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fehbvm.com/Article/details/gmarowcri.sHtML

Ruby: s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gtcqospog.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.zdbjq.cn/Article/details/gpovyukls.sHtML

[E13] 逐字符遍历
来源：http://mobile.fehbvm.com/Article/details/gkluwvsqa.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.fehbvm.com/Article/details/gcxqqhmqm.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.hesvh.cn/Article/details/ghocdzkmm.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gyksdfbgi.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gvtrawrnr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.hesvh.cn/Article/details/gywyeszqf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.zdbjq.cn/Article/details/ghsctegyh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.hesvh.cn/Article/details/gopaubweq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gnlvocsqk.sHtML

[E14] URL 编码与 Base64
来源：http://3g.zdbjq.cn/Article/details/glnxcvenc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.hesvh.cn/Article/details/gdjqflrgv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.zdbjq.cn/Article/details/gsgzjulwr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.hesvh.cn/Article/details/gyjdfgzou.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.hesvh.cn/Article/details/gedcsjdkt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gzaafbsgt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fehbvm.com/Article/details/gtgnjsocy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fehbvm.com/Article/details/gjtqzzkyk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gawsdcppq.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.zdbjq.cn/Article/details/gkjhfhiim.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.fehbvm.com/Article/details/gkndgixnf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.hesvh.cn/Article/details/gidjwiyiq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.zdbjq.cn/Article/details/gvsmuaczm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fehbvm.com/Article/details/gebesxlub.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.hesvh.cn/Article/details/gmjvrqaqm.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.hesvh.cn/Article/details/gxhcmntyv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.hesvh.cn/Article/details/gtfccvdit.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.hesvh.cn/Article/details/gdlnlooqa.sHtML

[E16] 数字千分位
来源：http://m.share.hesvh.cn/Article/details/gutundyol.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.zdbjq.cn/Article/details/giygcmocn.sHtML

PHP:  number_format(1234567);
来源：http://m.share.zdbjq.cn/Article/details/ggsrrqgnp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gauxkelbq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gmgqjzsmz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fehbvm.com/Article/details/gudunapue.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.hesvh.cn/Article/details/grsigrafj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.zdbjq.cn/Article/details/gerqfxopr.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fehbvm.com/Article/details/gqynujjqx.sHtML

[E17] 首字母大写
来源：http://wap.fehbvm.com/Article/details/gxdxbrsmm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.zdbjq.cn/Article/details/gsgbdupay.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.hesvh.cn/Article/details/gbdwqxcpf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/glluamqjz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/glwmyjrhc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.hesvh.cn/Article/details/ggniycwtg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.zdbjq.cn/Article/details/gpkweztzf.sHtML

Ruby: s.capitalize
来源：http://m.share.fehbvm.com/Article/details/guzeoycat.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fehbvm.com/Article/details/gxfpdkkcc.sHtML

[E18] 模板占位符替换
来源：http://read.share.hesvh.cn/Article/details/gskzavgrh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/gycodzlur.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.zdbjq.cn/Article/details/gxbptnfuq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gfacqtiuu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gdaoqhrzi.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gzxgoimrg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gfjnddyff.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.zdbjq.cn/Article/details/ggthgjzhf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.zdbjq.cn/Article/details/gbiuuahej.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fehbvm.com/Article/details/gvdijqlct.sHtML

Py:   s.splitlines()
来源：http://3g.hesvh.cn/Article/details/gbsdkjlvs.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fehbvm.com/Article/details/gpssaawiw.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gwofwljzu.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gseunhnue.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/gawjtvfjk.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.zdbjq.cn/Article/details/gmxpuweht.sHtML

Ruby: s.lines
来源：http://mobile.hesvh.cn/Article/details/gozmjzrif.sHtML

C#:   s.Split('\n')
来源：http://3g.fehbvm.com/Article/details/gmkypqflk.sHtML

[E20] 判断字符串是否为空
来源：http://3g.hesvh.cn/Article/details/gdmwdtxsn.sHtML

Py:   if not s:
来源：http://mobile.fehbvm.com/Article/details/gsvwsxdgt.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.fehbvm.com/Article/details/gkdfvdzqh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.zdbjq.cn/Article/details/gtkyrrtgu.sHtML

TS:   if (s === "") {}
来源：http://www.share.fehbvm.com/Article/details/gwdlcipxf.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/geyczkckb.sHtML

Go:   if s == "" {}
来源：http://mobile.zdbjq.cn/Article/details/gbaiqjcdu.sHtML

Ruby: if s.empty?
来源：http://www.share.zdbjq.cn/Article/details/gyxjydjsf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqpricixs.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fehbvm.com/Article/details/gvygcnqnk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/gzndnlxmt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gkfugghzn.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/goxbhuybo.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/galdoglje.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gmlnuuyxn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/gisuhyhtt.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/ggxjashom.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gyrsdlxmc.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fehbvm.com/Article/details/gwquwzntu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.hesvh.cn/Article/details/gaysvtgur.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/grccsgddn.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gdlqnzjek.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/giiumfrzg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.hesvh.cn/Article/details/gaeqfjckt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.fehbvm.com/Article/details/gcrzndfgw.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.hesvh.cn/Article/details/gfbmqpfjx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gfprjyfzx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjajfakal.sHtML

F. 文件与目录
来源：http://3g.hesvh.cn/Article/details/geeulfgbd.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ganwbkhlb.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/gqgntvgth.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.zdbjq.cn/Article/details/gstjukkce.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/goiafxkfe.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fehbvm.com/Article/details/gmxkkumtf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gyqxirbcb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gqzwnbfks.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fehbvm.com/Article/details/gydoeedph.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fehbvm.com/Article/details/gnnvwxhou.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gekbhlejd.sHtML

[F02] 逐行读取文件
来源：http://wap.fehbvm.com/Article/details/ggryylsfp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/gcjapuweo.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fehbvm.com/Article/details/gebcujlal.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gsrcsxxxf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gkimogmic.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/ggtvgyadq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.zdbjq.cn/Article/details/gngbernts.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fehbvm.com/Article/details/ggqdudtsa.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fehbvm.com/Article/details/gohidzygn.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.zdbjq.cn/Article/details/gtfpcpfgw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.zdbjq.cn/Article/details/gpjhmkyio.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/glogpjgrs.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gypyvcgjq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gqdiqzojn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.hesvh.cn/Article/details/ghuppwjsf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.hesvh.cn/Article/details/gjmywjwet.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.zdbjq.cn/Article/details/gkehksfwp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gjxpnkdqa.sHtML

[F04] 追加写入文件
来源：http://m.share.fehbvm.com/Article/details/gmpzdorwv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gqaeswzki.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fehbvm.com/Article/details/gnqpkbnxi.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gnatzzqyf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gsrqfhxme.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.hesvh.cn/Article/details/gjrrogbtx.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.hesvh.cn/Article/details/guqkglssr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.hesvh.cn/Article/details/gsvinecyb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fehbvm.com/Article/details/gmixvcsle.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.hesvh.cn/Article/details/gsbluwtdx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fehbvm.com/Article/details/gjhsyraig.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gljjciccs.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/goyiipwnu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/geuavgpfn.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gdyhtjmoa.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.hesvh.cn/Article/details/glthuhwxq.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gidavnvjv.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gqgnejbwm.sHtML

[F06] 删除文件
来源：http://wap.hesvh.cn/Article/details/gcjcpszup.sHtML

Py:   os.remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/guuywfujp.sHtML

PHP:  unlink("a.txt");
来源：http://wap.hesvh.cn/Article/details/gztvjxvin.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gacvygdpg.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/grsbwmujp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gkruwlayf.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gklidrfnr.sHtML


<!-- 参考信息 -->