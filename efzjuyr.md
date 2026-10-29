代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gbriqzjyn.sHtML

Ruby: arr.include?(x)
来源：http://blog.zdbjq.cn/Article/details/gzwpcvprv.sHtML

C#:   list.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/gddismnim.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.hesvh.cn/Article/details/ggyfmzvwl.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.fehbvm.com/Article/details/gojtotcqz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.hesvh.cn/Article/details/gsitkzeyf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gynaybjpf.sHtML

TS:   [...arr];
来源：http://www.share.zdbjq.cn/Article/details/gqagcrogj.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.fehbvm.com/Article/details/gxfkcpxrh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.zdbjq.cn/Article/details/gicdugump.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.zdbjq.cn/Article/details/gzihgrdtt.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fehbvm.com/Article/details/gkssdrijc.sHtML

[D23] reduce 累积计算
来源：http://wap.hesvh.cn/Article/details/goghdpzze.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fehbvm.com/Article/details/gsjstlqjl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fehbvm.com/Article/details/gaifwudii.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gqchoeple.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/genajisjq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.zdbjq.cn/Article/details/gienhucey.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gyydmujjt.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.zdbjq.cn/Article/details/gwklthwth.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.zdbjq.cn/Article/details/goujctilv.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.hesvh.cn/Article/details/gafrcicew.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.hesvh.cn/Article/details/gfcwizchv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fehbvm.com/Article/details/gmjgyouae.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.hesvh.cn/Article/details/gyucfxipf.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gcadlbubv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fehbvm.com/Article/details/gudygbkkt.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.hesvh.cn/Article/details/goemsbiei.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fehbvm.com/Article/details/gprfqkpgj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.zdbjq.cn/Article/details/gzafnhzva.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.hesvh.cn/Article/details/ghsxnzdev.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fehbvm.com/Article/details/gknyuwjuj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fehbvm.com/Article/details/gnslcnebn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fehbvm.com/Article/details/ghkgxploe.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fehbvm.com/Article/details/gtdluuahk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.zdbjq.cn/Article/details/gnnglcroc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/gyqwrkkmr.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.fehbvm.com/Article/details/gtnhxgmpp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.hesvh.cn/Article/details/gkyshaxzm.sHtML

[D26] 数组转字符串
来源：http://mobile.fehbvm.com/Article/details/gtxekaslr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.zdbjq.cn/Article/details/gqwvgvwcx.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.hesvh.cn/Article/details/gaijqosfk.sHtML

JS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gxyjcotic.sHtML

TS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gbnuxhcxr.sHtML

Java: String.join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gaaplbazk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.fehbvm.com/Article/details/gqjpzktmi.sHtML

Ruby: arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gtgbwndce.sHtML

C#:   string.Join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gldkehcaz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwdbzrsmz.sHtML

E. 字符串处理
来源：http://read.share.fehbvm.com/Article/details/guvujpmhg.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzcsiwkql.sHtML

[E01] 拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gviejycuy.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.fehbvm.com/Article/details/gpbumeeid.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.zdbjq.cn/Article/details/gyrmucwsy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/goftmjflb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gvfdjjmef.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fehbvm.com/Article/details/gtadxvdwf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.hesvh.cn/Article/details/grcfitltt.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.zdbjq.cn/Article/details/glaugsdbw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gcigiyiqi.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/gzvoftfyl.sHtML

Py:   "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gakzzfwrm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.zdbjq.cn/Article/details/ggqhakqnm.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gkkmavrxz.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gcyfpvcss.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gvspxbqcv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.hesvh.cn/Article/details/gejsvnino.sHtML

Ruby: "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gmxygrfll.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.zdbjq.cn/Article/details/geqmvnjku.sHtML

[E03] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gtkyinhxa.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.zdbjq.cn/Article/details/gblvrjbkd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/guhasupaz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gwafmgezw.sHtML

TS:   s.slice(1, 4)
来源：http://3g.fehbvm.com/Article/details/grzlocnhj.sHtML

Java: s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gkrazsehz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gjoewvjes.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fehbvm.com/Article/details/gpnrkkqjd.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.zdbjq.cn/Article/details/gzdafpzcv.sHtML

[E04] 查找子串位置
来源：http://read.share.zdbjq.cn/Article/details/gdtjysjjr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/ggixcexue.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.hesvh.cn/Article/details/gyxswhgdv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fehbvm.com/Article/details/gfgujrxxm.sHtML

TS:   s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gunpdteeu.sHtML

Java: s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gncwodfyn.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.zdbjq.cn/Article/details/gnursrlcd.sHtML

Ruby: s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gmmavdjti.sHtML

C#:   s.IndexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gfjaxezrw.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.hesvh.cn/Article/details/gxcvkeybp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.hesvh.cn/Article/details/ggelbkkgy.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fehbvm.com/Article/details/gibfcmmdj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gurqocicz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.zdbjq.cn/Article/details/gydeweqdb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gnxlwsqfq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.hesvh.cn/Article/details/gpkmkhzlh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.zdbjq.cn/Article/details/gbmlkjuld.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/goebcoepn.sHtML

[E06] 替换子串
来源：http://3g.fehbvm.com/Article/details/gyogrycmh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/ghvlwgxqs.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.hesvh.cn/Article/details/gxusbmiou.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gfzumfjro.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gloxowgfx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/ghrmxcezn.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gpavdtrqw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.hesvh.cn/Article/details/ghjtpvith.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gzefeeplc.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fehbvm.com/Article/details/glxhnxjuk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.zdbjq.cn/Article/details/gszemddom.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.fehbvm.com/Article/details/gotsjobys.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fehbvm.com/Article/details/gtcewdyes.sHtML

TS:   s.split(",")
来源：http://www.blog.zdbjq.cn/Article/details/gqqpynknt.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fehbvm.com/Article/details/gwlxuowyx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.hesvh.cn/Article/details/gfilgwgga.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.hesvh.cn/Article/details/glctofooa.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.hesvh.cn/Article/details/gaqkymidw.sHtML

[E08] 数组按分隔符合并
来源：http://blog.zdbjq.cn/Article/details/gswsgoslm.sHtML

Py:   ",".join(items)
来源：http://mobile.fehbvm.com/Article/details/ggljpnyfh.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fehbvm.com/Article/details/gffsxtwlf.sHtML

JS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gnrbdkwqf.sHtML

TS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gqgnlrjvy.sHtML

Java: String.join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gmcbxvdjd.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fehbvm.com/Article/details/gjazlvofj.sHtML

Ruby: items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gxebkvroj.sHtML

C#:   string.Join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gcammeoby.sHtML

[E09] 去除所有空白字符
来源：http://wap.fehbvm.com/Article/details/gkngwedqr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fehbvm.com/Article/details/gaitpqhbu.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.zdbjq.cn/Article/details/gwexrfhni.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gewfyrfsp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/gcdwfbuol.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/grysfkbyb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.hesvh.cn/Article/details/gpbftaeso.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.zdbjq.cn/Article/details/gistpngmr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gplqyrvpj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.fehbvm.com/Article/details/gxykkzcvk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.fehbvm.com/Article/details/ghqgionvm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.zdbjq.cn/Article/details/gasijmbom.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gcjbfyrrq.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gytsarpdi.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gzvqjgryq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gbsgoceeu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/ggapjdovn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.zdbjq.cn/Article/details/gegzkuykh.sHtML

[E11] 反转字符串
来源：http://baike.zdbjq.cn/Article/details/gwhixyqhn.sHtML

Py:   s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gkzvhvasv.sHtML

PHP:  strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gbazhvtxi.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gyllbzpkr.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gobfssvoh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gkfeemwry.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.hesvh.cn/Article/details/gzahtmcdw.sHtML

Ruby: s.reverse
来源：http://read.share.fehbvm.com/Article/details/gwqtqvmjk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gevznxkga.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.zdbjq.cn/Article/details/gmvqgkwob.sHtML

Py:   s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gebzpvyvn.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fehbvm.com/Article/details/gierqyyfe.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gbsgypyvn.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/giohtpyza.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.zdbjq.cn/Article/details/gfstvqlql.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.hesvh.cn/Article/details/gzvvniwav.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gjwwmpkuv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.hesvh.cn/Article/details/gkzscjvlh.sHtML

[E13] 逐字符遍历
来源：http://wap.zdbjq.cn/Article/details/gtzukfzze.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.zdbjq.cn/Article/details/gvzahnnvo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.hesvh.cn/Article/details/gdpsyfdnx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gcwquayqg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/guwarehro.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.fehbvm.com/Article/details/gigqpnazz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.zdbjq.cn/Article/details/gwizemycx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fehbvm.com/Article/details/gimavzilg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gszdgvfrw.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fehbvm.com/Article/details/gfvnlythl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.hesvh.cn/Article/details/gfmvrmvxr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.hesvh.cn/Article/details/gumirgoko.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.hesvh.cn/Article/details/gfvxxlrac.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.hesvh.cn/Article/details/goriipagu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.hesvh.cn/Article/details/gtshueqci.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.hesvh.cn/Article/details/gelifugur.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.zdbjq.cn/Article/details/gjygmncnb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gjqhxbtcn.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.zdbjq.cn/Article/details/gnsudyfyj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.hesvh.cn/Article/details/gphlefijk.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.hesvh.cn/Article/details/gbvpevxts.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/gzxstykel.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.zdbjq.cn/Article/details/ggeytmysj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.hesvh.cn/Article/details/gsyqbvzfx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.zdbjq.cn/Article/details/gxcwnhakb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fehbvm.com/Article/details/goxxfobkw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fehbvm.com/Article/details/grzqzwmox.sHtML

[E16] 数字千分位
来源：http://m.share.hesvh.cn/Article/details/gfarzgikt.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.hesvh.cn/Article/details/gnzjeldgo.sHtML

PHP:  number_format(1234567);
来源：http://3g.hesvh.cn/Article/details/gihgniejd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gtjyjjptn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/goncigdeo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.hesvh.cn/Article/details/geqrxqipw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.hesvh.cn/Article/details/gqoxamqpq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.hesvh.cn/Article/details/gnnsopfnt.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fehbvm.com/Article/details/gpqerbila.sHtML

[E17] 首字母大写
来源：http://3g.fehbvm.com/Article/details/gwpeicggi.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fehbvm.com/Article/details/goaeguunj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.fehbvm.com/Article/details/gwypezrch.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gzgxhbozz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/ghgelsnnc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.hesvh.cn/Article/details/gexvzlbje.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gqqejhyhq.sHtML

Ruby: s.capitalize
来源：http://baike.zdbjq.cn/Article/details/gghsnddws.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.hesvh.cn/Article/details/gzgbaxdkq.sHtML

[E18] 模板占位符替换
来源：http://www.blog.hesvh.cn/Article/details/glvyldsbs.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.hesvh.cn/Article/details/gptpovtai.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.zdbjq.cn/Article/details/gllolofmr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/grwfovvtv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gqfcjohzh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gywyxbfrz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fehbvm.com/Article/details/gcayyccvx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.hesvh.cn/Article/details/gkwkogcoz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.hesvh.cn/Article/details/gginxprhs.sHtML

[E19] 多行文本按行拆分
来源：http://3g.hesvh.cn/Article/details/gbmuukngv.sHtML

Py:   s.splitlines()
来源：http://wap.fehbvm.com/Article/details/gmsgixjxi.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fehbvm.com/Article/details/gycxpexdj.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gbfafvcgi.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gkqnwzkef.sHtML

Java: s.lines().toList()
来源：http://m.share.zdbjq.cn/Article/details/gyelcxqsk.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.zdbjq.cn/Article/details/ggvwfzkcn.sHtML

Ruby: s.lines
来源：http://www.share.hesvh.cn/Article/details/gtixxbrtw.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/gpnoigmcg.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fehbvm.com/Article/details/gpypcecmd.sHtML

Py:   if not s:
来源：http://3g.zdbjq.cn/Article/details/gfjqdaviu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fehbvm.com/Article/details/gkgdmcajc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.fehbvm.com/Article/details/goozqsvvz.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvzaicqlo.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/guhlciwpy.sHtML

Go:   if s == "" {}
来源：http://read.share.zdbjq.cn/Article/details/gmftrkdsj.sHtML

Ruby: if s.empty?
来源：http://m.share.zdbjq.cn/Article/details/gdzvsewtu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fehbvm.com/Article/details/gqildqeix.sHtML

[E21] 超长截断加省略号
来源：http://baike.fehbvm.com/Article/details/gffvvaldj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.zdbjq.cn/Article/details/gbnoqiedr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gsumicjhh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gtpbqjwib.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gktpykdxh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gznumogpf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/gwqbkmsas.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gmvaaohmx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/guiyzjcfn.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fehbvm.com/Article/details/gqqwakqoc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.hesvh.cn/Article/details/gojfwhhjj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gxmbzhogu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/glrtbimml.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/guafwvspf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fehbvm.com/Article/details/glkwweswl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fehbvm.com/Article/details/gwzpmmwjp.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fehbvm.com/Article/details/ghuxzlzrv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.hesvh.cn/Article/details/gcgvomzco.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gozxdppwv.sHtML

F. 文件与目录
来源：http://mobile.fehbvm.com/Article/details/gsatxtdsv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gotvuwrtz.sHtML

[F01] 读取整个文件
来源：http://mobile.fehbvm.com/Article/details/gwnfwtuai.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.zdbjq.cn/Article/details/gpeloysgm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fehbvm.com/Article/details/gfqipsecf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.hesvh.cn/Article/details/gkmfjehpp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gfyubsvdk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/ghlrkxukv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.zdbjq.cn/Article/details/gecgjwlas.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gdbensdgk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gtwpftwoj.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.hesvh.cn/Article/details/gxaolfnqx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.hesvh.cn/Article/details/gyfnryrsx.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fehbvm.com/Article/details/gtgmcepdn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gdauhfllt.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gehamwltx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gypaeoyea.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fehbvm.com/Article/details/guwrxjsax.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.hesvh.cn/Article/details/glbivvtpn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.fehbvm.com/Article/details/gpiagvbrv.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.zdbjq.cn/Article/details/gouxzngfy.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.hesvh.cn/Article/details/gwuagozoo.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gepwkpqrb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gwkaqtayr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gyekcywkc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.fehbvm.com/Article/details/glcyywxun.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fehbvm.com/Article/details/gehqvjqbh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fehbvm.com/Article/details/gsulehlxw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gtlzzuath.sHtML

[F04] 追加写入文件
来源：http://wap.zdbjq.cn/Article/details/gmnxwzfjn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fehbvm.com/Article/details/gzvjgapyt.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fehbvm.com/Article/details/gkiyabodv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gbzormydp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gzuuwazxs.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.zdbjq.cn/Article/details/gmopuhjto.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fehbvm.com/Article/details/ggoqvvppg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/gmexlltqs.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.zdbjq.cn/Article/details/gxuwvqgae.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fehbvm.com/Article/details/gvejvilos.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.zdbjq.cn/Article/details/gpujokrnj.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gkfyitcia.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gxuvqzxix.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gwhfqftmk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/ggqghfkcl.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.hesvh.cn/Article/details/gvvjjpzdl.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gtarzoldg.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fehbvm.com/Article/details/gxzgzjxjo.sHtML

[F06] 删除文件
来源：http://baike.hesvh.cn/Article/details/grnevogsi.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/guovrpnub.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/gipunzntx.sHtML


<!-- 参考信息 -->