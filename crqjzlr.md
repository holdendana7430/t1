代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gsfxrzlvg.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gdfmhcsrp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fehbvm.com/Article/details/gkoyuftzg.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fehbvm.com/Article/details/gomcyszle.sHtML

Ruby: arr.tally
来源：http://baike.hesvh.cn/Article/details/gzxdbhbtf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.zdbjq.cn/Article/details/gfqnjuubo.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fehbvm.com/Article/details/gvupjtjvh.sHtML

Py:   x in arr
来源：http://m.share.hesvh.cn/Article/details/gocvhcsgt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.hesvh.cn/Article/details/gjbdarxaq.sHtML

JS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gfzlintsa.sHtML

TS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/giqkbcnoc.sHtML

Java: list.contains(x)
来源：http://blog.zdbjq.cn/Article/details/gqpwcwhnu.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gyobuszgc.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fehbvm.com/Article/details/gmtjijqcb.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gokiaimyw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fehbvm.com/Article/details/gfjgkdwbw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gpbgbyeoo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fehbvm.com/Article/details/gzgpwszwx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.hesvh.cn/Article/details/gpvufvbsu.sHtML

TS:   [...arr];
来源：http://baike.fehbvm.com/Article/details/gfusjpvpx.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gehzbqztl.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.hesvh.cn/Article/details/ggezvoqco.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.zdbjq.cn/Article/details/gremwrhgf.sHtML

C#:   new List<int>(list);
来源：http://3g.zdbjq.cn/Article/details/ggooxxzan.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.zdbjq.cn/Article/details/gjlsdyjvq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fehbvm.com/Article/details/gsdvderoc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.hesvh.cn/Article/details/gwvyyhfcc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gbgkywdzh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/guejaxjay.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.fehbvm.com/Article/details/gahcjhnih.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/glblzdcqo.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.hesvh.cn/Article/details/gewpjwltb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.hesvh.cn/Article/details/gvatvoint.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.zdbjq.cn/Article/details/gclmqsafn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.hesvh.cn/Article/details/gjwewympa.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.zdbjq.cn/Article/details/gtzdmthus.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.hesvh.cn/Article/details/gmyuclnvn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gghhngqxf.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.zdbjq.cn/Article/details/godgfublc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.zdbjq.cn/Article/details/gybbamadu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fehbvm.com/Article/details/gihtszpcg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fehbvm.com/Article/details/gxguprzvn.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.hesvh.cn/Article/details/gsoamtpjl.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.zdbjq.cn/Article/details/gmfiunett.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.zdbjq.cn/Article/details/gpuudliie.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.zdbjq.cn/Article/details/gmjdrrlfo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.fehbvm.com/Article/details/gmnhkltse.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.fehbvm.com/Article/details/ggjcbfvld.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fehbvm.com/Article/details/gzbdscddq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.hesvh.cn/Article/details/gpjutpgak.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/gfrpldwda.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/gnsuzyvwf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.zdbjq.cn/Article/details/gwlmqoidx.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gyzgqcwfp.sHtML

JS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gxodnvwdt.sHtML

TS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gapahvokw.sHtML

Java: String.join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/giuxopitb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gjdlpwvjx.sHtML

Ruby: arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gquqisbpm.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gkmgwdvfk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grjvfcdud.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/gturvwiof.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwtlpwvmm.sHtML

[E01] 拼接字符串
来源：http://m.share.hesvh.cn/Article/details/glpmxtxow.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.hesvh.cn/Article/details/gnietfvcf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.zdbjq.cn/Article/details/ghfcykniu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/guqojljfl.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/gqpofaibs.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fehbvm.com/Article/details/gcetvvuji.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fehbvm.com/Article/details/gqdeucbxg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.zdbjq.cn/Article/details/ghvrzppwq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gwmvxpbdi.sHtML

[E02] 重复字符串
来源：http://wap.fehbvm.com/Article/details/gcxmxqvii.sHtML

Py:   "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gvpxmxkee.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/gpvgkggpe.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/geiufhizk.sHtML

TS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gajpulhqk.sHtML

Java: "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/ggiordgta.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.zdbjq.cn/Article/details/gxkewzxsg.sHtML

Ruby: "ab" * 3
来源：http://3g.hesvh.cn/Article/details/gvworgbsk.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.hesvh.cn/Article/details/gawvthrxa.sHtML

[E03] 截取子串
来源：http://wap.hesvh.cn/Article/details/ggvftsayj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.hesvh.cn/Article/details/gpkvcmthx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/guflkwxyy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gzjhacqen.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gpzopaykd.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gsstzwmxb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.hesvh.cn/Article/details/giakbxwww.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.hesvh.cn/Article/details/gqijjottm.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.hesvh.cn/Article/details/gdvgysgjv.sHtML

[E04] 查找子串位置
来源：http://www.m.share.hesvh.cn/Article/details/gjyqimmai.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gmlivgltm.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.hesvh.cn/Article/details/gthyafjfb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.hesvh.cn/Article/details/gzemlxwmk.sHtML

TS:   s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/grlwjbnvr.sHtML

Java: s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gnwwbcwql.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.hesvh.cn/Article/details/gaytorbdb.sHtML

Ruby: s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gypicfqzy.sHtML

C#:   s.IndexOf("x")
来源：http://baike.fehbvm.com/Article/details/gmcjvvmqz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.hesvh.cn/Article/details/giqogwopq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.fehbvm.com/Article/details/guuermkff.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.hesvh.cn/Article/details/guvwpejrw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gjetmzjhz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fehbvm.com/Article/details/gdtjtaras.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gqjvwkbiw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.hesvh.cn/Article/details/grlfxeffr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.hesvh.cn/Article/details/gleyjynhc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.hesvh.cn/Article/details/getaitwct.sHtML

[E06] 替换子串
来源：http://www.m.share.zdbjq.cn/Article/details/gtozfvjjm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gheaslbjl.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.zdbjq.cn/Article/details/gsfkscbuw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gqptvprsa.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gpcggupns.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gjgldvtki.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gibisywgr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gqophdlqn.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.hesvh.cn/Article/details/guqujxrxe.sHtML

[E07] 按分隔符拆分
来源：http://mobile.hesvh.cn/Article/details/gmzyxhhnc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.zdbjq.cn/Article/details/gscsfoptz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.zdbjq.cn/Article/details/giwpqvacn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.hesvh.cn/Article/details/gkryrvaha.sHtML

TS:   s.split(",")
来源：http://m.share.zdbjq.cn/Article/details/gibgwuyjp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fehbvm.com/Article/details/geuyimqbm.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/gonzfzddz.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.zdbjq.cn/Article/details/gsufvapaa.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.hesvh.cn/Article/details/gnzqaksvc.sHtML

[E08] 数组按分隔符合并
来源：http://baike.hesvh.cn/Article/details/gtqxjoodm.sHtML

Py:   ",".join(items)
来源：http://www.blog.fehbvm.com/Article/details/gqjizgwkk.sHtML

PHP:  implode(",", $items);
来源：http://mobile.zdbjq.cn/Article/details/gofnwpnlo.sHtML

JS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gereoqaml.sHtML

TS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gwsumrdhu.sHtML

Java: String.join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gsenfkllc.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.zdbjq.cn/Article/details/gfzzmsfjz.sHtML

Ruby: items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gwkkmogmi.sHtML

C#:   string.Join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gbsurlyus.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.hesvh.cn/Article/details/gyjffhsvv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fehbvm.com/Article/details/gqzhzqpvm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gujdjbvrh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/giindzxwf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gmryfdmzs.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gqhxprwvh.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.zdbjq.cn/Article/details/gxbnorvfl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.fehbvm.com/Article/details/ghnrkqfbe.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gynurzndd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.hesvh.cn/Article/details/gblnjzizt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gsyvxyoxy.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fehbvm.com/Article/details/ggmtkboyy.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gzmxpfocn.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gmapttkep.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gabnwxcnu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gjmzzfgxg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gezpyqnae.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fehbvm.com/Article/details/gjxhkpvta.sHtML

[E11] 反转字符串
来源：http://baike.fehbvm.com/Article/details/gfsbellcl.sHtML

Py:   s[::-1]
来源：http://3g.hesvh.cn/Article/details/gumavaxpz.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gjyylyhya.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gtusmkjsa.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gywzcmvos.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/gobydruxn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.fehbvm.com/Article/details/gpsjupail.sHtML

Ruby: s.reverse
来源：http://wap.hesvh.cn/Article/details/goucmoipa.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gamxuefjx.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.zdbjq.cn/Article/details/gtdqhsmff.sHtML

Py:   s.count("a")
来源：http://3g.fehbvm.com/Article/details/gfcfeplwd.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.hesvh.cn/Article/details/gjgimpqyk.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/ghbuggamf.sHtML

TS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gtvpdsrut.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.zdbjq.cn/Article/details/ghqmdfvsa.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fehbvm.com/Article/details/gestiktov.sHtML

Ruby: s.count("a")
来源：http://3g.hesvh.cn/Article/details/gjeckvnrj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.hesvh.cn/Article/details/gebdjhahs.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/gtbtqbqje.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.fehbvm.com/Article/details/gocdctfse.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.zdbjq.cn/Article/details/gllmwwbea.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gmuqvgyye.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gomuaayms.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gknuoequs.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/gdwriysbi.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.zdbjq.cn/Article/details/gmouexosa.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.hesvh.cn/Article/details/gyyhwiafj.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fehbvm.com/Article/details/grulhyaic.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.hesvh.cn/Article/details/gbbnwbrfd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.hesvh.cn/Article/details/gekpeafig.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.hesvh.cn/Article/details/gmqownwyf.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.hesvh.cn/Article/details/gtkbztvuu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gmhnkegmc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.zdbjq.cn/Article/details/givgyroel.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.zdbjq.cn/Article/details/gjyyswzxw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gomwioxin.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.zdbjq.cn/Article/details/gjhyniphp.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.zdbjq.cn/Article/details/gvzxxdhif.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.hesvh.cn/Article/details/gobevptpj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.hesvh.cn/Article/details/gpyyopdfv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.hesvh.cn/Article/details/ghnnvwlrs.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.hesvh.cn/Article/details/gxovqxbom.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gwfzsoomv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.zdbjq.cn/Article/details/gnxdiueyn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.hesvh.cn/Article/details/gagbxwtlt.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/gzsifbaos.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fehbvm.com/Article/details/ggloelsmi.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fehbvm.com/Article/details/ghfglosao.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gcxipvwuh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/ggsoaukmw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gzvbpukcn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.zdbjq.cn/Article/details/gtzvgshkv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.fehbvm.com/Article/details/gatlszaem.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.hesvh.cn/Article/details/gokmcqosy.sHtML

[E17] 首字母大写
来源：http://m.share.fehbvm.com/Article/details/gossrhloh.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.hesvh.cn/Article/details/gstxquqwf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.hesvh.cn/Article/details/grnqypifk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gwrkvyrva.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gevpowymc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.hesvh.cn/Article/details/gelwttknf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.hesvh.cn/Article/details/gooaudlqm.sHtML

Ruby: s.capitalize
来源：http://www.share.fehbvm.com/Article/details/ggdmcmieu.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fehbvm.com/Article/details/gjxqcebje.sHtML

[E18] 模板占位符替换
来源：http://m.share.zdbjq.cn/Article/details/giuthnysm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.fehbvm.com/Article/details/glleyuptp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/ghriqheph.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/ginwtccln.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gvtbvsbkj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gsstpywij.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gcmmgrwnt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fehbvm.com/Article/details/gwjqldawi.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.hesvh.cn/Article/details/gbikmoufe.sHtML

[E19] 多行文本按行拆分
来源：http://baike.hesvh.cn/Article/details/gnwbmgbcf.sHtML

Py:   s.splitlines()
来源：http://m.share.zdbjq.cn/Article/details/geevwjavv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gafshuexn.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/genvlldxw.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gxsnesdtb.sHtML

Java: s.lines().toList()
来源：http://m.share.fehbvm.com/Article/details/gwctwgsrb.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fehbvm.com/Article/details/gowznvmdu.sHtML

Ruby: s.lines
来源：http://read.share.zdbjq.cn/Article/details/gfiyznrwv.sHtML

C#:   s.Split('\n')
来源：http://baike.hesvh.cn/Article/details/getukuttm.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.fehbvm.com/Article/details/gwbcqqsnj.sHtML

Py:   if not s:
来源：http://baike.zdbjq.cn/Article/details/gtkbyvvsy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.hesvh.cn/Article/details/gubgsbkic.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.hesvh.cn/Article/details/guhzcioaf.sHtML

TS:   if (s === "") {}
来源：http://read.share.fehbvm.com/Article/details/gkpztymfc.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gawtvhziv.sHtML

Go:   if s == "" {}
来源：http://mobile.fehbvm.com/Article/details/gqxotqzmi.sHtML

Ruby: if s.empty?
来源：http://m.share.hesvh.cn/Article/details/gsdoxjtiq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.hesvh.cn/Article/details/gnpmgyumi.sHtML

[E21] 超长截断加省略号
来源：http://read.share.hesvh.cn/Article/details/gkyffrbfp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.zdbjq.cn/Article/details/gfdtxqzvg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gprmezewz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gfcowmzqq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/grlmvqaph.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gfliuwebz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.zdbjq.cn/Article/details/gkqjdhjcw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/ghcldnelk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gulynzevh.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.zdbjq.cn/Article/details/gqgpmakmv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.zdbjq.cn/Article/details/gpsvbpvug.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gzkubnttu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gcajnoxde.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/giyrqulck.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.zdbjq.cn/Article/details/galmsnprb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fehbvm.com/Article/details/gjswoccvc.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gmhmnpkzf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fehbvm.com/Article/details/gbvwqkzzs.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gligwmodl.sHtML

F. 文件与目录
来源：http://3g.fehbvm.com/Article/details/gmlufqqyw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/giaffmatn.sHtML

[F01] 读取整个文件
来源：http://baike.fehbvm.com/Article/details/gmnbtvlyo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.zdbjq.cn/Article/details/goxbcouef.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fehbvm.com/Article/details/gudaeugra.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.hesvh.cn/Article/details/gtyqsplhx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.hesvh.cn/Article/details/gcqxdtgwz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gfschzyoz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.zdbjq.cn/Article/details/ghqkfsmxz.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gbmcvvvyz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.hesvh.cn/Article/details/guaferuuy.sHtML

[F02] 逐行读取文件
来源：http://wap.hesvh.cn/Article/details/graraywec.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.zdbjq.cn/Article/details/gabjtcgkb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fehbvm.com/Article/details/gbfbfgogc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gwythrozq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gsxkryyvi.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gzbeyfduc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.zdbjq.cn/Article/details/gpnszmduh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.fehbvm.com/Article/details/gpleuqelj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.zdbjq.cn/Article/details/gdfjkfeid.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fehbvm.com/Article/details/gnlawhukx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fehbvm.com/Article/details/ghutujitw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/goraoiqsg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gcnjfwxgi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gtpgcdhju.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.hesvh.cn/Article/details/gabzyxyud.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.zdbjq.cn/Article/details/gqhoaxrjj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.zdbjq.cn/Article/details/gcpoqcxwa.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gryzstchx.sHtML

[F04] 追加写入文件
来源：http://mobile.hesvh.cn/Article/details/gqzgbgmde.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gjlfbnzqx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fehbvm.com/Article/details/gbytjddoj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gumaxmazt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gbvobghoi.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.hesvh.cn/Article/details/gzeekvwcf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.hesvh.cn/Article/details/gzcqmmayx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.hesvh.cn/Article/details/gzzadbxof.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fehbvm.com/Article/details/gvrvztknf.sHtML


<!-- 参考信息 -->