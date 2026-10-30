代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gyfsmsbmm.sHtML

Ruby: arr.include?(x)
来源：http://blog.hesvh.cn/Article/details/ggobbvgte.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gbuajgesx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fehbvm.com/Article/details/gqqugqnzn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.zdbjq.cn/Article/details/gfrournfe.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.zdbjq.cn/Article/details/gpinbjjly.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fehbvm.com/Article/details/gijvlpnno.sHtML

TS:   [...arr];
来源：http://wap.hesvh.cn/Article/details/gxqovxhcc.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.zdbjq.cn/Article/details/gohheqird.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gqrgfznhh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fehbvm.com/Article/details/gltvdeabs.sHtML

C#:   new List<int>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gbeidmqbe.sHtML

[D23] reduce 累积计算
来源：http://mobile.hesvh.cn/Article/details/gdzmclprd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fehbvm.com/Article/details/grdudqdxf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gjatrresm.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gxotagrdf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/guiluqseo.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fehbvm.com/Article/details/gzygogaxb.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gzptybyaw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fehbvm.com/Article/details/gxultelcj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fehbvm.com/Article/details/gsdunxkrr.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.hesvh.cn/Article/details/gqfigqqce.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.hesvh.cn/Article/details/gecjtsarv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fehbvm.com/Article/details/gelwufeyz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.zdbjq.cn/Article/details/gxnlbifrz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.hesvh.cn/Article/details/gfljeppqd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.zdbjq.cn/Article/details/garrgpwnk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.hesvh.cn/Article/details/gsfvhflrj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gykzxmavj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fehbvm.com/Article/details/gofgspoto.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.zdbjq.cn/Article/details/gtvhtjxko.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fehbvm.com/Article/details/glyshgoxl.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.hesvh.cn/Article/details/gkccsqkim.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/gnrtziylu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fehbvm.com/Article/details/gnuhbftvx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/ggwvadmgw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fehbvm.com/Article/details/gkdsouyzi.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gvzbwdngn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.zdbjq.cn/Article/details/gfwqnvmda.sHtML

[D26] 数组转字符串
来源：http://wap.fehbvm.com/Article/details/gawwilnxi.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.zdbjq.cn/Article/details/gygdkjiks.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fehbvm.com/Article/details/ggxbwyxme.sHtML

JS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gvsplbvwj.sHtML

TS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gnogjqehb.sHtML

Java: String.join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gfbysbakv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.zdbjq.cn/Article/details/ggjrnriso.sHtML

Ruby: arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/ghmlpbfxr.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gmwhulhfo.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/goofdogct.sHtML

E. 字符串处理
来源：http://wap.fehbvm.com/Article/details/gowpawjau.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gordmgjkl.sHtML

[E01] 拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gjchecngm.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/gnlgmrepa.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fehbvm.com/Article/details/gqeaxhzww.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/gfrzwstxf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gnsebjodf.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.zdbjq.cn/Article/details/giekjulve.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.hesvh.cn/Article/details/gcjcmzhyp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.hesvh.cn/Article/details/gjechyghc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gyiwonjoa.sHtML

[E02] 重复字符串
来源：http://3g.fehbvm.com/Article/details/gghyokurg.sHtML

Py:   "ab" * 3
来源：http://baike.hesvh.cn/Article/details/grqnkyere.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.zdbjq.cn/Article/details/gaabtuwzc.sHtML

JS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gmdaztlck.sHtML

TS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gklpoqqkj.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gvafjxfxw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.hesvh.cn/Article/details/gqjqzfntg.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/gubzgundt.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fehbvm.com/Article/details/gujwssupd.sHtML

[E03] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gyydwhivw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fehbvm.com/Article/details/gifmwjrom.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/ggtwhumlp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gxtsljmgb.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gzxctihuf.sHtML

Java: s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gynrrbnzp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gmufnignv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fehbvm.com/Article/details/gwqspeghv.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fehbvm.com/Article/details/glkpvppbi.sHtML

[E04] 查找子串位置
来源：http://blog.fehbvm.com/Article/details/gdlxcmwmo.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gfdcycbak.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.hesvh.cn/Article/details/gblcmejhv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.zdbjq.cn/Article/details/gsriwbheh.sHtML

TS:   s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gvnakokcz.sHtML

Java: s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gmsohrzdb.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.fehbvm.com/Article/details/gaocfovuq.sHtML

Ruby: s.index("x")
来源：http://blog.zdbjq.cn/Article/details/ghtdfzesm.sHtML

C#:   s.IndexOf("x")
来源：http://baike.zdbjq.cn/Article/details/glbkmonat.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.zdbjq.cn/Article/details/gyqkqctkw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.hesvh.cn/Article/details/gfvhouzvg.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.fehbvm.com/Article/details/gvxaxahje.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gdiawppuw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fehbvm.com/Article/details/ghfjkayoj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gtafbjtfl.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/gkojlfamb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.zdbjq.cn/Article/details/gyfmdhwog.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gjzqanfgb.sHtML

[E06] 替换子串
来源：http://www.m.share.fehbvm.com/Article/details/gpuyhuyfd.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/geycvuclb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.zdbjq.cn/Article/details/gelrrfaww.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gvnbyemdm.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gqqqnuajh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/ghabyjboy.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gzwgjgboo.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.hesvh.cn/Article/details/gbqktnnkq.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gvrgchnid.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fehbvm.com/Article/details/geuezyqvm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fehbvm.com/Article/details/gblyljkmx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gtevdnngm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.zdbjq.cn/Article/details/gixrzwskt.sHtML

TS:   s.split(",")
来源：http://baike.zdbjq.cn/Article/details/gckrxlvbf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.zdbjq.cn/Article/details/gmddziljx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.fehbvm.com/Article/details/gfhmzxtxd.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.fehbvm.com/Article/details/gtlywzuzt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.hesvh.cn/Article/details/gulzrbemt.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fehbvm.com/Article/details/gnadmfnvi.sHtML

Py:   ",".join(items)
来源：http://m.share.hesvh.cn/Article/details/guybjyctx.sHtML

PHP:  implode(",", $items);
来源：http://blog.zdbjq.cn/Article/details/gqsdyglhl.sHtML

JS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gkbxrolbi.sHtML

TS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gprzxcnqk.sHtML

Java: String.join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/grnjpyntp.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.zdbjq.cn/Article/details/gvwuxqtdt.sHtML

Ruby: items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gvjtjaetb.sHtML

C#:   string.Join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gptgrvyng.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.zdbjq.cn/Article/details/gcacfohtz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.zdbjq.cn/Article/details/gsalmunnm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.zdbjq.cn/Article/details/gddqcbzum.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/grhqpubnx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/gmigbbvsd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gpcsvobgx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fehbvm.com/Article/details/gfqhigqhn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.hesvh.cn/Article/details/glvswidem.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.fehbvm.com/Article/details/guagbjcdf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.hesvh.cn/Article/details/gfaazngqb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.hesvh.cn/Article/details/gehyzqrne.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.zdbjq.cn/Article/details/gzquccdih.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gczhscdgs.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gwqwsxniv.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gdlxamcpp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gnruvwhdd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gtvugqucg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.zdbjq.cn/Article/details/gaufbmfjm.sHtML

[E11] 反转字符串
来源：http://3g.zdbjq.cn/Article/details/gbgxcqlir.sHtML

Py:   s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gzxtajbab.sHtML

PHP:  strrev($s);
来源：http://baike.hesvh.cn/Article/details/gzrmvqmuu.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gkitxkcbv.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gxeuuowpr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.hesvh.cn/Article/details/gohqluasa.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gesbeamuy.sHtML

Ruby: s.reverse
来源：http://mobile.hesvh.cn/Article/details/galnuyxlo.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gypzwjmic.sHtML

[E12] 统计某字符出现次数
来源：http://3g.zdbjq.cn/Article/details/gldwufjfd.sHtML

Py:   s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gedtpbecz.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.zdbjq.cn/Article/details/gbnhsjsqn.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gyocytzso.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/ggsdhvszy.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.fehbvm.com/Article/details/gjksmfzzr.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.zdbjq.cn/Article/details/gzsdxcvlv.sHtML

Ruby: s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gfhplhngs.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.zdbjq.cn/Article/details/gmhqxnyrj.sHtML

[E13] 逐字符遍历
来源：http://www.share.zdbjq.cn/Article/details/gzirlfpfp.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fehbvm.com/Article/details/gzgvdurzv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.hesvh.cn/Article/details/gypnkhrzz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gicfvufvl.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gypnmupfr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gnxqpppja.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.zdbjq.cn/Article/details/gkhhufvxi.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.zdbjq.cn/Article/details/gxznbqlpe.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fehbvm.com/Article/details/gxvmtjxme.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.hesvh.cn/Article/details/gxafehoxi.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.hesvh.cn/Article/details/gywuhyads.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.zdbjq.cn/Article/details/goorjckzl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.fehbvm.com/Article/details/gfedxnazi.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gmyhuzato.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fehbvm.com/Article/details/gwobhgeda.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fehbvm.com/Article/details/ghmxpbtvq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fehbvm.com/Article/details/goeljbxtg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fehbvm.com/Article/details/gkdbxtdox.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fehbvm.com/Article/details/gskwzushw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gmjfzkkeh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.fehbvm.com/Article/details/gxpoadpgb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.hesvh.cn/Article/details/gfhgqvmfk.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.zdbjq.cn/Article/details/gewptlfze.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.zdbjq.cn/Article/details/gbjqfguhb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.zdbjq.cn/Article/details/gygghgcnb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fehbvm.com/Article/details/gglkmcryp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.zdbjq.cn/Article/details/grdeelgif.sHtML

[E16] 数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gliiyohut.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fehbvm.com/Article/details/gaxnfijmu.sHtML

PHP:  number_format(1234567);
来源：http://www.share.zdbjq.cn/Article/details/gvumacvml.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gmfsxjtdu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gofokgiky.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gpayaypid.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.zdbjq.cn/Article/details/gulnnzmop.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.hesvh.cn/Article/details/gyahfsagt.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.hesvh.cn/Article/details/gcufpfqjg.sHtML

[E17] 首字母大写
来源：http://www.m.share.fehbvm.com/Article/details/gecghadlr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.hesvh.cn/Article/details/gvqmrnxms.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.hesvh.cn/Article/details/goenusysj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/ggjnlvylt.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/galrjtyaz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fehbvm.com/Article/details/gvjhrdhoy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.hesvh.cn/Article/details/gtudzixqx.sHtML

Ruby: s.capitalize
来源：http://baike.fehbvm.com/Article/details/gsxvbtulf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fehbvm.com/Article/details/gxxysvxru.sHtML

[E18] 模板占位符替换
来源：http://read.share.hesvh.cn/Article/details/gtxqkbxzx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.zdbjq.cn/Article/details/gnnzgsyrb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.zdbjq.cn/Article/details/gfjkobbvc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gscolgyqt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gtpqnsxnc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gnvbdsoaq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gmhbilyxj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.fehbvm.com/Article/details/gqasgwypd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fehbvm.com/Article/details/gedjceqdk.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fehbvm.com/Article/details/glttjgdts.sHtML

Py:   s.splitlines()
来源：http://baike.zdbjq.cn/Article/details/gtfwgxape.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.hesvh.cn/Article/details/ghsjitfnh.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gcoywiobp.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gvuujxrke.sHtML

Java: s.lines().toList()
来源：http://wap.hesvh.cn/Article/details/gxdkgroti.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.hesvh.cn/Article/details/gtohhyzfl.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/gwhmkzcdd.sHtML

C#:   s.Split('\n')
来源：http://blog.hesvh.cn/Article/details/gbqlppthn.sHtML

[E20] 判断字符串是否为空
来源：http://baike.zdbjq.cn/Article/details/gmxbvrtwu.sHtML

Py:   if not s:
来源：http://baike.hesvh.cn/Article/details/gyclamyhj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.zdbjq.cn/Article/details/gclzcijrq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.fehbvm.com/Article/details/gxtatmbej.sHtML

TS:   if (s === "") {}
来源：http://www.share.fehbvm.com/Article/details/gapbdjxrp.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/grjdaumhb.sHtML

Go:   if s == "" {}
来源：http://mobile.fehbvm.com/Article/details/gsyosqsnp.sHtML

Ruby: if s.empty?
来源：http://mobile.fehbvm.com/Article/details/gjhgneinx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkbjyhxzy.sHtML

[E21] 超长截断加省略号
来源：http://blog.hesvh.cn/Article/details/gkdbtzeba.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fehbvm.com/Article/details/gcujyxhbi.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gawydnqov.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gjnszdfjs.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gkghqadww.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gauvdvwgr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.hesvh.cn/Article/details/gdxiuektx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gdwmdfkba.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gxslamtkp.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fehbvm.com/Article/details/gxyusgbra.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.zdbjq.cn/Article/details/gwingbzda.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gwajscjdw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gaqnrpatw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gjzyudazy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.hesvh.cn/Article/details/gchnnkkre.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.zdbjq.cn/Article/details/gmxklynsb.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fehbvm.com/Article/details/gcymqyzpd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gxasbxfud.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmealvbkx.sHtML

F. 文件与目录
来源：http://blog.hesvh.cn/Article/details/gobhjzeyt.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gccugjceh.sHtML

[F01] 读取整个文件
来源：http://m.share.fehbvm.com/Article/details/gtshgrpgh.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.fehbvm.com/Article/details/ggtedtwtu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/ghsqngkte.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.zdbjq.cn/Article/details/gxzgecpzv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/grjnhfvhk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gtbvryfjt.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.zdbjq.cn/Article/details/gpoykjuau.sHtML

Ruby: File.read("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gxdqmqygq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/grgtlmhrh.sHtML

[F02] 逐行读取文件
来源：http://www.share.fehbvm.com/Article/details/gnqtsbmkd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fehbvm.com/Article/details/gpcusescs.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.zdbjq.cn/Article/details/grkqrvfya.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/giwsocjug.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gsrmmbfnf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gxmkxotlj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.hesvh.cn/Article/details/gdhdworzd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.hesvh.cn/Article/details/gqzgxdlvg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.fehbvm.com/Article/details/geidgrzsc.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.hesvh.cn/Article/details/gydybwfik.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fehbvm.com/Article/details/gsfklfaad.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gqtfdimix.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gdmflaqem.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/greaselbx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.zdbjq.cn/Article/details/glwgyyyti.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.zdbjq.cn/Article/details/gmnbnafgx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gmaktiqjl.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gduijwbed.sHtML

[F04] 追加写入文件
来源：http://3g.fehbvm.com/Article/details/gpdpzzksi.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fehbvm.com/Article/details/grcpzypbw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fehbvm.com/Article/details/gitwaygjm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gjqenwqwe.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gkbqblqbo.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.zdbjq.cn/Article/details/gyjrshrip.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.zdbjq.cn/Article/details/gimsvoftp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.fehbvm.com/Article/details/gfnkyxnlu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fehbvm.com/Article/details/gbgtxwiii.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fehbvm.com/Article/details/ggbaulkpt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/gtathzqra.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/genhkvwky.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/grmyhndrk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/grrfdzqzn.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gkbebywco.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.zdbjq.cn/Article/details/gojzsjnjw.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gvienpacr.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gtqsjegzq.sHtML

[F06] 删除文件
来源：http://mobile.fehbvm.com/Article/details/goaiwxujc.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/ggrovouas.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fehbvm.com/Article/details/gmnowsrvr.sHtML


<!-- 参考信息 -->