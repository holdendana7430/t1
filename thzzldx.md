代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fehbvm.com/Article/details/gsnzvzdky.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.zdbjq.cn/Article/details/gwvvcbfzn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.hesvh.cn/Article/details/gbdvquqed.sHtML

TS:   [...arr];
来源：http://blog.zdbjq.cn/Article/details/gdmpygyti.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fehbvm.com/Article/details/gwynaqhes.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/gpmwbfsxs.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.hesvh.cn/Article/details/gnkclaczh.sHtML

C#:   new List<int>(list);
来源：http://3g.hesvh.cn/Article/details/gdijpemlk.sHtML

[D23] reduce 累积计算
来源：http://baike.hesvh.cn/Article/details/gqmcjixfc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.zdbjq.cn/Article/details/gnbrprcnt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.zdbjq.cn/Article/details/gfebpnylk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gismwglco.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gcpelrcer.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fehbvm.com/Article/details/gvefhykvb.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gtvlnmwcz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.hesvh.cn/Article/details/grvxpiijv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.hesvh.cn/Article/details/gwlqeickt.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.zdbjq.cn/Article/details/gtrjweutk.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.zdbjq.cn/Article/details/gxnhxcjdd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fehbvm.com/Article/details/gugdvgdwv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.fehbvm.com/Article/details/gdxdvhjyv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gagqkgmjs.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.fehbvm.com/Article/details/gewxltzcg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fehbvm.com/Article/details/gnezbfadb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.zdbjq.cn/Article/details/gegcrtjuv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.hesvh.cn/Article/details/gyjhmeubj.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.zdbjq.cn/Article/details/guqktpzcb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.hesvh.cn/Article/details/gfrpcgjoe.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.zdbjq.cn/Article/details/gebrjxlmc.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.zdbjq.cn/Article/details/giqqnchbo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.hesvh.cn/Article/details/ggxgfxfrt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.hesvh.cn/Article/details/gshqcvkeb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fehbvm.com/Article/details/gvvjvojeb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.hesvh.cn/Article/details/gqtprwgnh.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.hesvh.cn/Article/details/gmbwpdjyr.sHtML

[D26] 数组转字符串
来源：http://3g.hesvh.cn/Article/details/gxtiezqvq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gnwiikqyl.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/gmwkwvxhc.sHtML

JS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gxjlimjcz.sHtML

TS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gutsrmqvb.sHtML

Java: String.join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gitjcrxcx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.hesvh.cn/Article/details/gqrhcppgl.sHtML

Ruby: arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gkswisntr.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/grcfwordf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghecnwong.sHtML

E. 字符串处理
来源：http://read.share.fehbvm.com/Article/details/gggtrjtch.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gyzxhmitn.sHtML

[E01] 拼接字符串
来源：http://3g.fehbvm.com/Article/details/gvycljtmc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.fehbvm.com/Article/details/gteprtftw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fehbvm.com/Article/details/gnwotqwje.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gfaixkteq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gurlidrjg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fehbvm.com/Article/details/gzkwmmsue.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gqoifacbx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.hesvh.cn/Article/details/ghbkkpalz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/gkzsvmgnw.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/gjtmuftpm.sHtML

Py:   "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gzdpsjmvn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.zdbjq.cn/Article/details/gojoembtc.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gfboripud.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gbuiapoba.sHtML

Java: "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gtzlxbobo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.hesvh.cn/Article/details/ganovtmtq.sHtML

Ruby: "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gdfpitkib.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.zdbjq.cn/Article/details/geyjblrfn.sHtML

[E03] 截取子串
来源：http://blog.fehbvm.com/Article/details/gmqanoslp.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fehbvm.com/Article/details/gfltdiuax.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gblivsiee.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/goqbxktnr.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gqtsjjioc.sHtML

Java: s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gavagkamy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.zdbjq.cn/Article/details/gmkjfyfoj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.zdbjq.cn/Article/details/gaqmflupr.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.fehbvm.com/Article/details/gvefhjasy.sHtML

[E04] 查找子串位置
来源：http://blog.fehbvm.com/Article/details/gqwlqbazc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gejcrarnd.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fehbvm.com/Article/details/gkagkaoez.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.hesvh.cn/Article/details/gmrmylkxt.sHtML

TS:   s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/giawdkrwl.sHtML

Java: s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/gyszxjtbe.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.hesvh.cn/Article/details/gkxnxbnpg.sHtML

Ruby: s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gefwpktbn.sHtML

C#:   s.IndexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gmczmhird.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.hesvh.cn/Article/details/gtsncbvfp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.zdbjq.cn/Article/details/gslatsixp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.fehbvm.com/Article/details/gzdxzgixm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gxritrpqr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.fehbvm.com/Article/details/gxmvhvzhw.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gqtgdcxsb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.hesvh.cn/Article/details/gxpolctii.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.hesvh.cn/Article/details/ggxvqtpld.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.fehbvm.com/Article/details/gslvhtxca.sHtML

[E06] 替换子串
来源：http://www.blog.fehbvm.com/Article/details/glhhwbgdl.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gspzmxavf.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gipzpsyse.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gsvpvaanc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/girfqfaoh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gexjmsnns.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gjcvuatkp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gugbuskmf.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/ggauiyoof.sHtML

[E07] 按分隔符拆分
来源：http://www.share.hesvh.cn/Article/details/gujmxjttf.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.zdbjq.cn/Article/details/ggicqwvqb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fehbvm.com/Article/details/gdmdgofgw.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.hesvh.cn/Article/details/gtumtqyud.sHtML

TS:   s.split(",")
来源：http://www.m.share.hesvh.cn/Article/details/gbnabdkof.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.hesvh.cn/Article/details/gzhsgxdux.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.hesvh.cn/Article/details/gmnbiqphm.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.zdbjq.cn/Article/details/gfetfvdoe.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.hesvh.cn/Article/details/grtnrtawy.sHtML

[E08] 数组按分隔符合并
来源：http://blog.zdbjq.cn/Article/details/gaqusrinp.sHtML

Py:   ",".join(items)
来源：http://blog.hesvh.cn/Article/details/gjrtuwxzi.sHtML

PHP:  implode(",", $items);
来源：http://mobile.zdbjq.cn/Article/details/gloxuvcwy.sHtML

JS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gycdvgbtj.sHtML

TS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gebsyvkic.sHtML

Java: String.join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gxaplhope.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fehbvm.com/Article/details/gkyavpmuo.sHtML

Ruby: items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gzoaqqepw.sHtML

C#:   string.Join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gnixyrqcj.sHtML

[E09] 去除所有空白字符
来源：http://wap.zdbjq.cn/Article/details/gnrcjsprh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.hesvh.cn/Article/details/godkabdzp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fehbvm.com/Article/details/gofarvezk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/ggoygvhoe.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/geqpdavvh.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gdvmnbluu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.fehbvm.com/Article/details/ghhtwnsac.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.hesvh.cn/Article/details/gvsgqfcnu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gabpjqqxk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.zdbjq.cn/Article/details/gfafkkyxu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.hesvh.cn/Article/details/gphsrpoki.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fehbvm.com/Article/details/gmdsislur.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gcqcuqupj.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gygmybztz.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gngzzguoi.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/glwshfzhm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gyvqtiozp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.zdbjq.cn/Article/details/gcvcjbqje.sHtML

[E11] 反转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gcydnhuzr.sHtML

Py:   s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gqrltsydu.sHtML

PHP:  strrev($s);
来源：http://wap.fehbvm.com/Article/details/gddfizmlh.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/glcfqkwgk.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/ghgpovwuy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.fehbvm.com/Article/details/giwvuugvv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/grvcxlyix.sHtML

Ruby: s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gdpnhiovn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gbdvgmehb.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.hesvh.cn/Article/details/gejkwmrrh.sHtML

Py:   s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gfcexxmlv.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.hesvh.cn/Article/details/gddokbzgn.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gzlqrvygx.sHtML

TS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gzrwapolg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.zdbjq.cn/Article/details/gipfmmeqs.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.hesvh.cn/Article/details/grpzvuiec.sHtML

Ruby: s.count("a")
来源：http://blog.fehbvm.com/Article/details/gmgjozzqm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.hesvh.cn/Article/details/guwjkpdsh.sHtML

[E13] 逐字符遍历
来源：http://read.share.hesvh.cn/Article/details/gpwqmdxrh.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.hesvh.cn/Article/details/gbdeoopuo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.zdbjq.cn/Article/details/gaknxrkeh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gnmpkndtq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gftnjwpid.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.hesvh.cn/Article/details/geazhgpmj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fehbvm.com/Article/details/gpbmgnivs.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/gsufgbbqv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fehbvm.com/Article/details/gcjiahcnj.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.hesvh.cn/Article/details/gyptastom.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fehbvm.com/Article/details/gujggpfad.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.hesvh.cn/Article/details/gspwwmczs.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.hesvh.cn/Article/details/glyktmuzv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.hesvh.cn/Article/details/gtvxfpzde.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fehbvm.com/Article/details/gtdtvudgn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.zdbjq.cn/Article/details/gngurmdkf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.hesvh.cn/Article/details/gnqimkmoh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.zdbjq.cn/Article/details/gerexmukd.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.zdbjq.cn/Article/details/gyzhpiynj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.zdbjq.cn/Article/details/gtlhsswng.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gvssacsgv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.hesvh.cn/Article/details/gewiuudcz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.zdbjq.cn/Article/details/gifqerlmt.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.zdbjq.cn/Article/details/gyfqzcwdx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.zdbjq.cn/Article/details/gcqsmegnw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fehbvm.com/Article/details/gakzpnnie.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fehbvm.com/Article/details/guhrlqonf.sHtML

[E16] 数字千分位
来源：http://mobile.fehbvm.com/Article/details/gboctbqyp.sHtML

Py:   f"{1234567:,}"
来源：http://blog.fehbvm.com/Article/details/gdpolklfo.sHtML

PHP:  number_format(1234567);
来源：http://www.share.hesvh.cn/Article/details/ggpuxfdwf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gnapkwtvf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gdsakmmno.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gxqymnbua.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fehbvm.com/Article/details/gphspzhxi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.hesvh.cn/Article/details/gjitrnzhy.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.zdbjq.cn/Article/details/gnhippfol.sHtML

[E17] 首字母大写
来源：http://m.share.hesvh.cn/Article/details/gxtdzxcpn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fehbvm.com/Article/details/gusvfapci.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fehbvm.com/Article/details/glhkqlpke.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gufuojltn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gfbchxxnc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.hesvh.cn/Article/details/gpsgmireu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.zdbjq.cn/Article/details/gbqeyerqp.sHtML

Ruby: s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/gsrwabayb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.zdbjq.cn/Article/details/gtaqraorz.sHtML

[E18] 模板占位符替换
来源：http://blog.zdbjq.cn/Article/details/ghbtbfyuy.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.zdbjq.cn/Article/details/gmfxxzsoj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/glmbsscyb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gqbzkgesz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gedinvnjl.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gvajzujif.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gysexeeaf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fehbvm.com/Article/details/ggdsmwzhz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.hesvh.cn/Article/details/gvzsnksxp.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.hesvh.cn/Article/details/galrkozvq.sHtML

Py:   s.splitlines()
来源：http://baike.zdbjq.cn/Article/details/gwdlcvqhb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gdlqmitxx.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gdjbyvybb.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gkayijsge.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gzctfkohz.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fehbvm.com/Article/details/gbdkunorb.sHtML

Ruby: s.lines
来源：http://mobile.fehbvm.com/Article/details/garvljaxz.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.zdbjq.cn/Article/details/gsskathlr.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.zdbjq.cn/Article/details/gqyogbtsl.sHtML

Py:   if not s:
来源：http://www.blog.zdbjq.cn/Article/details/grtdaqnqg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.fehbvm.com/Article/details/gnvhtiwem.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fehbvm.com/Article/details/gslirhgtu.sHtML

TS:   if (s === "") {}
来源：http://mobile.hesvh.cn/Article/details/gtbipiipi.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gnowkfwwr.sHtML

Go:   if s == "" {}
来源：http://wap.hesvh.cn/Article/details/gjvddaxdw.sHtML

Ruby: if s.empty?
来源：http://m.share.zdbjq.cn/Article/details/grjyxhnhs.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.hesvh.cn/Article/details/gdnkifnfu.sHtML

[E21] 超长截断加省略号
来源：http://read.share.zdbjq.cn/Article/details/gvrrmggsx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.zdbjq.cn/Article/details/ggqqehqox.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gdjxmnxgr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/giywaawpw.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/glodmryjw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gfchuzwkf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.zdbjq.cn/Article/details/gvqtxixxl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gwuhuudyk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gutccqnvz.sHtML

[E22] 字节长度与字符长度
来源：http://3g.zdbjq.cn/Article/details/gvhhrkiqe.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.hesvh.cn/Article/details/gclvuxmon.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gatnnnpdt.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gllmpbdyn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gvkjvzzxp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gacxqwfwf.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.hesvh.cn/Article/details/gmksbxbft.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/goyvdhtlk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.hesvh.cn/Article/details/gjwljxnsx.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxttryukb.sHtML

F. 文件与目录
来源：http://www.m.share.hesvh.cn/Article/details/ghmucggyv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/glidaciyq.sHtML

[F01] 读取整个文件
来源：http://www.m.share.hesvh.cn/Article/details/grpqvizlk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.hesvh.cn/Article/details/gpmhqyust.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.hesvh.cn/Article/details/geaxehdpn.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.hesvh.cn/Article/details/griypldix.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.zdbjq.cn/Article/details/govtnuomh.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gvlnqrrxd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fehbvm.com/Article/details/gjbcextzc.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gxjiapshv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fehbvm.com/Article/details/glumsjjwv.sHtML

[F02] 逐行读取文件
来源：http://baike.zdbjq.cn/Article/details/gqduqwjcv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/gulkavhub.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fehbvm.com/Article/details/gdlthvczd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gpvdqkqlw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gjbiejxxv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gjqccocut.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.fehbvm.com/Article/details/gauxnbiwy.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.hesvh.cn/Article/details/gcexmqgjm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fehbvm.com/Article/details/gxrvipwgc.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.zdbjq.cn/Article/details/gkyjuokce.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fehbvm.com/Article/details/ghuwdvpej.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gjvgqxtey.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/geblpeobw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gavplmnmr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.fehbvm.com/Article/details/gzycjnzuq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.hesvh.cn/Article/details/gqbungeoj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.hesvh.cn/Article/details/gsbexrexq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gakaxrvtl.sHtML

[F04] 追加写入文件
来源：http://read.share.zdbjq.cn/Article/details/gkfsfftev.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.zdbjq.cn/Article/details/ghecsmsdg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.zdbjq.cn/Article/details/gsrudbbqk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gaikkycly.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gnqqidvmv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.zdbjq.cn/Article/details/gnhtmsthz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gsciazkmr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fehbvm.com/Article/details/gjokywtmf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.zdbjq.cn/Article/details/gnaanwpop.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.zdbjq.cn/Article/details/gcfkfmqxs.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fehbvm.com/Article/details/godutvubg.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gqaskrvdx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gbsbnaxra.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gqjoplhaw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gepzkmzkj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.fehbvm.com/Article/details/gczkbrtub.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gmsuvwezl.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gmijpqpvl.sHtML

[F06] 删除文件
来源：http://www.m.share.hesvh.cn/Article/details/gcghjoief.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/glbdmumwj.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gvlnnyhyc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gmbmogwtf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gdicdumkr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/ghrvcrisz.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gkyghiknz.sHtML


<!-- 参考信息 -->