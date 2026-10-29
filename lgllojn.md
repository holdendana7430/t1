代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fehbvm.com/Article/details/gsjpiuxww.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.zdbjq.cn/Article/details/gfltnrsue.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fehbvm.com/Article/details/gcieehoif.sHtML

TS:   [...arr];
来源：http://mobile.fehbvm.com/Article/details/gzutvqtuo.sHtML

Java: new ArrayList<>(list);
来源：http://3g.hesvh.cn/Article/details/geurhtbcb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.zdbjq.cn/Article/details/glxnfgpwb.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.hesvh.cn/Article/details/gxaeuifhl.sHtML

C#:   new List<int>(list);
来源：http://blog.zdbjq.cn/Article/details/gsmftwdbb.sHtML

[D23] reduce 累积计算
来源：http://blog.hesvh.cn/Article/details/gbfdqukoz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.hesvh.cn/Article/details/gxsguhqhy.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.hesvh.cn/Article/details/gzwsxcykr.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gytzlatnl.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gyslteatl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.zdbjq.cn/Article/details/gyxdfwpex.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gghrruied.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fehbvm.com/Article/details/gvcjqasng.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fehbvm.com/Article/details/gutqucnex.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.zdbjq.cn/Article/details/gkmofeupv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fehbvm.com/Article/details/gsrfdqcwl.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gvepqezdd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.zdbjq.cn/Article/details/gtneqtofg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gfnxvawsp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.zdbjq.cn/Article/details/gfnpmvhun.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/ghfqfybro.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.fehbvm.com/Article/details/gxkiqjzjr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.hesvh.cn/Article/details/ganyzpjog.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fehbvm.com/Article/details/gkxascijz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fehbvm.com/Article/details/gcbsyefbe.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.zdbjq.cn/Article/details/goxsutsmm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.zdbjq.cn/Article/details/ggcnnckai.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.zdbjq.cn/Article/details/gyveomydo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gqqpwmabq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.hesvh.cn/Article/details/gztszrdaj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fehbvm.com/Article/details/grxururca.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/gcjhrhqvx.sHtML

[D26] 数组转字符串
来源：http://blog.fehbvm.com/Article/details/goxgtfmrg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.zdbjq.cn/Article/details/gijgcyadl.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/gddtkgmxb.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gwneyakfa.sHtML

TS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gixvwahsn.sHtML

Java: String.join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gfkjurctb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.hesvh.cn/Article/details/gtlygxhod.sHtML

Ruby: arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gokoenifc.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gejirhgkw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/glwippdff.sHtML

E. 字符串处理
来源：http://wap.hesvh.cn/Article/details/gmcdlkfex.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gsfdseoub.sHtML

[E01] 拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gfmzmjdxj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fehbvm.com/Article/details/guyhqimfb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.hesvh.cn/Article/details/gfvqqwdpk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/guymkdvuf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/glbgltqfh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.zdbjq.cn/Article/details/gbqwzxmnp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.hesvh.cn/Article/details/gayumfbre.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.hesvh.cn/Article/details/gbihzzety.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/gcnjdpjon.sHtML

[E02] 重复字符串
来源：http://www.share.zdbjq.cn/Article/details/gbectwmax.sHtML

Py:   "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gfnueeukv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fehbvm.com/Article/details/gcslziqvi.sHtML

JS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gnyortxbq.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gmcynmssn.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gnltrudir.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.zdbjq.cn/Article/details/gvoxzzmer.sHtML

Ruby: "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/godvbltsk.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.hesvh.cn/Article/details/gvdeqjsxg.sHtML

[E03] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gbheaitkq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.zdbjq.cn/Article/details/gkkexgvkg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gvbdjsslm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gwutwnlsj.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gosclbbjz.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gzrycdiak.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gklpfkidk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.zdbjq.cn/Article/details/gvlwbsien.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.hesvh.cn/Article/details/glmffibcv.sHtML

[E04] 查找子串位置
来源：http://www.blog.zdbjq.cn/Article/details/gimpfdfrj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gazbhyetq.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fehbvm.com/Article/details/garjsjnyi.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fehbvm.com/Article/details/gkhfwqpcu.sHtML

TS:   s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gchgwvskd.sHtML

Java: s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gwytrmtcv.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.hesvh.cn/Article/details/gpwkpkqau.sHtML

Ruby: s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gqcokpliy.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gbkhxvevk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.hesvh.cn/Article/details/gxnxqmdkh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.zdbjq.cn/Article/details/gtzptznrs.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fehbvm.com/Article/details/grburtdrj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gskfkogit.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.zdbjq.cn/Article/details/goefanlno.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gvoidatfr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.zdbjq.cn/Article/details/gzrqewwby.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.hesvh.cn/Article/details/gvqpbjyes.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.hesvh.cn/Article/details/gjgluivqb.sHtML

[E06] 替换子串
来源：http://www.share.hesvh.cn/Article/details/grfhljyaq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gunzenmtg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.zdbjq.cn/Article/details/goqbxlgnz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gvahkmfbb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gnpbnpsaf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gkyikqaxo.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/glkmdludz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fehbvm.com/Article/details/gyfgbzsww.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/grvfccjhq.sHtML

[E07] 按分隔符拆分
来源：http://baike.fehbvm.com/Article/details/gpzredmkp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.zdbjq.cn/Article/details/ggceufsge.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gdndfdnrg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fehbvm.com/Article/details/ghjqhxvga.sHtML

TS:   s.split(",")
来源：http://3g.zdbjq.cn/Article/details/gdehybkte.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.hesvh.cn/Article/details/gtfbuokse.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.zdbjq.cn/Article/details/grphdjqsf.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.zdbjq.cn/Article/details/gcolunzyu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.zdbjq.cn/Article/details/gcwtyepwr.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.hesvh.cn/Article/details/gvhvocbyl.sHtML

Py:   ",".join(items)
来源：http://baike.zdbjq.cn/Article/details/gnwvsnhqe.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.zdbjq.cn/Article/details/ghuniszra.sHtML

JS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gvfowomys.sHtML

TS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gjfykqlsj.sHtML

Java: String.join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gssjusypj.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.zdbjq.cn/Article/details/gwebrwvhl.sHtML

Ruby: items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gypeepshv.sHtML

C#:   string.Join(",", items)
来源：http://wap.fehbvm.com/Article/details/genjtvrtr.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.hesvh.cn/Article/details/gycpgfnva.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fehbvm.com/Article/details/gqmnnsihi.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.zdbjq.cn/Article/details/gqpqjgltc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gytfsdlmk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gmmbjjvza.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gangxzsdv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.zdbjq.cn/Article/details/grticvtyk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.zdbjq.cn/Article/details/gkvqgyqvg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fehbvm.com/Article/details/gxcsaylkc.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fehbvm.com/Article/details/gatfowsky.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/ggzchvqpi.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.hesvh.cn/Article/details/gcwqqjida.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gbyhorsja.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gtrsexsvb.sHtML

Java: String.format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gcirsmqpd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gfmdgtdja.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gaeyjodjo.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.zdbjq.cn/Article/details/gvazfgpvr.sHtML

[E11] 反转字符串
来源：http://m.share.hesvh.cn/Article/details/gtyotpasn.sHtML

Py:   s[::-1]
来源：http://blog.hesvh.cn/Article/details/gthmouhmm.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gvobeauyy.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gbityshlw.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gclgehaiw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.hesvh.cn/Article/details/gxxwwnxsl.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.zdbjq.cn/Article/details/gieadkwao.sHtML

Ruby: s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gcedgrihg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gdnthnzgq.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.hesvh.cn/Article/details/gwizvgqwv.sHtML

Py:   s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gvibfxtwh.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.hesvh.cn/Article/details/gadibowmp.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gbgwbpxzj.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/ghhhmvane.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.zdbjq.cn/Article/details/guisanmuw.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.zdbjq.cn/Article/details/gxvzahoek.sHtML

Ruby: s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/guzjwxuxf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/geujmehwe.sHtML

[E13] 逐字符遍历
来源：http://m.share.fehbvm.com/Article/details/giifjbbat.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fehbvm.com/Article/details/grfkjjjxh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.hesvh.cn/Article/details/gamubntkv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gsrthjjwt.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gumgultmw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/ghrutnkzl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.hesvh.cn/Article/details/gbbiesbmo.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.fehbvm.com/Article/details/gyeavotty.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.zdbjq.cn/Article/details/gelaccdxs.sHtML

[E14] URL 编码与 Base64
来源：http://wap.hesvh.cn/Article/details/gaxlbnjeb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.hesvh.cn/Article/details/gfvhxyhzd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gpelcdefs.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.hesvh.cn/Article/details/gzmozwgqi.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.hesvh.cn/Article/details/gewabepru.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gaetmwbpe.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.zdbjq.cn/Article/details/gqhremwzx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fehbvm.com/Article/details/gwojilkjt.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fehbvm.com/Article/details/gypbwmhyb.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fehbvm.com/Article/details/gxtstdxlz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fehbvm.com/Article/details/glcyyjotj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.hesvh.cn/Article/details/gnfroqjkl.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.hesvh.cn/Article/details/gqwmcdkvp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fehbvm.com/Article/details/gfbqtruth.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fehbvm.com/Article/details/gigwdpjhk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gaekrnvtd.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.hesvh.cn/Article/details/gdhmcqkhc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.hesvh.cn/Article/details/geruuthru.sHtML

[E16] 数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gwjudigei.sHtML

Py:   f"{1234567:,}"
来源：http://baike.zdbjq.cn/Article/details/gijypdbsx.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/ggbcyxmew.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gngepfirs.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/grqdnxnll.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.hesvh.cn/Article/details/gkyeqerug.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.zdbjq.cn/Article/details/gkwwmwoij.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.hesvh.cn/Article/details/gmwrtgsjv.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.hesvh.cn/Article/details/gwfygcdop.sHtML

[E17] 首字母大写
来源：http://www.share.zdbjq.cn/Article/details/gxtbphotm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fehbvm.com/Article/details/gupkuwfye.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.zdbjq.cn/Article/details/gylssnxbr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/ghytjdxeq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/geryrxchn.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.hesvh.cn/Article/details/gormbnmxq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.hesvh.cn/Article/details/guhpuuoym.sHtML

Ruby: s.capitalize
来源：http://blog.zdbjq.cn/Article/details/geehixyzq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fehbvm.com/Article/details/gtlksmezc.sHtML

[E18] 模板占位符替换
来源：http://wap.hesvh.cn/Article/details/gzoqpxhln.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fehbvm.com/Article/details/gxpodopuo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.hesvh.cn/Article/details/gsxnbdzwp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gcbfghvpg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gglvnurcj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gomkxkbrq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gltawsbuq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.hesvh.cn/Article/details/gcyvgcotd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.zdbjq.cn/Article/details/glvflkdjl.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.fehbvm.com/Article/details/gqakwtiat.sHtML

Py:   s.splitlines()
来源：http://www.share.fehbvm.com/Article/details/gryvqnlwm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.hesvh.cn/Article/details/ggodmnima.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gshqhhrxz.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gtekuzhxj.sHtML

Java: s.lines().toList()
来源：http://mobile.fehbvm.com/Article/details/gladyvomz.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fehbvm.com/Article/details/ghcvrtgka.sHtML

Ruby: s.lines
来源：http://read.share.hesvh.cn/Article/details/gencswjcd.sHtML

C#:   s.Split('\n')
来源：http://read.share.hesvh.cn/Article/details/gvoahvwip.sHtML

[E20] 判断字符串是否为空
来源：http://wap.zdbjq.cn/Article/details/gligktpyv.sHtML

Py:   if not s:
来源：http://www.share.hesvh.cn/Article/details/gmrefksun.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.hesvh.cn/Article/details/gsndplhbk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.fehbvm.com/Article/details/gglvbavmt.sHtML

TS:   if (s === "") {}
来源：http://www.share.hesvh.cn/Article/details/guysfqtao.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/grfnnmpwa.sHtML

Go:   if s == "" {}
来源：http://m.share.zdbjq.cn/Article/details/gbtddbghp.sHtML

Ruby: if s.empty?
来源：http://www.blog.fehbvm.com/Article/details/gknwvlstk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnlfveoos.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fehbvm.com/Article/details/gbwvejaer.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.hesvh.cn/Article/details/ggggeffmm.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gthbuztxb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gkxkigyvv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gumavrhjz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/ghlpupnun.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.hesvh.cn/Article/details/gftursyvo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/glarddwrx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gylogzeey.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fehbvm.com/Article/details/goauxdbat.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.fehbvm.com/Article/details/gfvxslolz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gvnrxlukx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gqcucbjox.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gcwnvovxd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.fehbvm.com/Article/details/gahnfgcnf.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.zdbjq.cn/Article/details/gkjxgdjyx.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.fehbvm.com/Article/details/gbowmxlfa.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.zdbjq.cn/Article/details/gztfxzljd.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gcidvdxuu.sHtML

F. 文件与目录
来源：http://www.m.share.hesvh.cn/Article/details/gatropnqw.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxrttzowg.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/gtcuwukqo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fehbvm.com/Article/details/gzuflqwck.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gbevlvcoa.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.fehbvm.com/Article/details/gkqhcywml.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/ggtlfivgj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gqmmxsrbn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.hesvh.cn/Article/details/gwyjpwioc.sHtML

Ruby: File.read("a.txt")
来源：http://3g.hesvh.cn/Article/details/gwfomzmgk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gfqcteabb.sHtML

[F02] 逐行读取文件
来源：http://mobile.zdbjq.cn/Article/details/gjqkfmdbx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.zdbjq.cn/Article/details/gvasfxfim.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/gdvrsxgsh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gxvdddfpm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gbzkhhakz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gdjjngcqa.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.hesvh.cn/Article/details/gwtfojqcc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.hesvh.cn/Article/details/ggimvspng.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.zdbjq.cn/Article/details/gpgweadgx.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.hesvh.cn/Article/details/gqnajopjw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.zdbjq.cn/Article/details/gkgejntqv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gdnhxktjb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gqemqxsfn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gvbvoxjdu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.hesvh.cn/Article/details/gaiytkqlj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.zdbjq.cn/Article/details/gmhnrzfxq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.zdbjq.cn/Article/details/gxvbrwowz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gkgtkdana.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fehbvm.com/Article/details/gvzxrgftq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.hesvh.cn/Article/details/gmkhbqgmy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.zdbjq.cn/Article/details/gxqdpwfsy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gdysjtjas.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gwupnheqs.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.hesvh.cn/Article/details/guhvmfnyx.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.hesvh.cn/Article/details/gtyvljeka.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.zdbjq.cn/Article/details/gulygxxju.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.zdbjq.cn/Article/details/gvjscdwvr.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.zdbjq.cn/Article/details/grijxgvoe.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fehbvm.com/Article/details/gunneyyzc.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gukseplnp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gvnvujcjy.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gpeialbaa.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/guacfznfk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fehbvm.com/Article/details/gxbqtueze.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gtyhulbsq.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gtijmhzzb.sHtML

[F06] 删除文件
来源：http://read.share.zdbjq.cn/Article/details/gqczcttnh.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/giyxxcqvz.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gdybslore.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gmzaibutx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gttybklej.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gartxrbuh.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gmlydubxn.sHtML


<!-- 参考信息 -->