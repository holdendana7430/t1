代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.fehbvm.com/Article/details/ggzkkjzhp.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/gkudxpsib.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fehbvm.com/Article/details/gxfulxtsz.sHtML

TS:   [...arr];
来源：http://baike.hesvh.cn/Article/details/ggsecsyfi.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.hesvh.cn/Article/details/gnflvpfgr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.hesvh.cn/Article/details/gmtpptufh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fehbvm.com/Article/details/gqewcagje.sHtML

C#:   new List<int>(list);
来源：http://m.share.hesvh.cn/Article/details/gzgozkiun.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.hesvh.cn/Article/details/gdjkbwsym.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.hesvh.cn/Article/details/gxqxxfiuh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fehbvm.com/Article/details/gzuufkbjb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gcmcamwrm.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/goccczgmr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.zdbjq.cn/Article/details/goyaixgtr.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gjdnkhteo.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.hesvh.cn/Article/details/gvmpumqrs.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.zdbjq.cn/Article/details/glgivtzug.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fehbvm.com/Article/details/gggtfywfu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.zdbjq.cn/Article/details/gehpyzxkm.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.fehbvm.com/Article/details/gmnlvvsrl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gqhrafeis.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fehbvm.com/Article/details/gxpjoxplq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fehbvm.com/Article/details/gcuxdfruy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fehbvm.com/Article/details/gqzfskszm.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.zdbjq.cn/Article/details/gdqubhdel.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.hesvh.cn/Article/details/gpmcsdyzn.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.hesvh.cn/Article/details/gacsmwfdj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.zdbjq.cn/Article/details/gkdgfttyu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.zdbjq.cn/Article/details/gwsmsbrkx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.zdbjq.cn/Article/details/gmwfvtbxp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fehbvm.com/Article/details/gcctdlfmo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.fehbvm.com/Article/details/gyxdzzynh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.zdbjq.cn/Article/details/gdsamdahw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.hesvh.cn/Article/details/gqshhnjhd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gnrxyklzv.sHtML

[D26] 数组转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gftxbrbxk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fehbvm.com/Article/details/gaulvhlpf.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.hesvh.cn/Article/details/gxmwsoqxa.sHtML

JS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gbqoldrli.sHtML

TS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gwmnsnohu.sHtML

Java: String.join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gfogavvxx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.fehbvm.com/Article/details/gyguvnlmt.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gypvzyawp.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gtvhoituz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmmfuvymi.sHtML

E. 字符串处理
来源：http://read.share.hesvh.cn/Article/details/geamdjcdr.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grarsadvd.sHtML

[E01] 拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gcixdyorb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.zdbjq.cn/Article/details/guneohnkf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fehbvm.com/Article/details/gqbrswetg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gfhcfhhhj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gegsmmxei.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.fehbvm.com/Article/details/gshgvipft.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fehbvm.com/Article/details/gzzdlfphh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.zdbjq.cn/Article/details/ghojgtppu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.zdbjq.cn/Article/details/guzxgbgch.sHtML

[E02] 重复字符串
来源：http://www.blog.zdbjq.cn/Article/details/gudrbvknl.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gxjuuwrwk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fehbvm.com/Article/details/gplbciozc.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gsmrviqpj.sHtML

TS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gicbgcrwz.sHtML

Java: "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/glkviijpa.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gjzshrjfv.sHtML

Ruby: "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gwbkwwkuh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.zdbjq.cn/Article/details/gdigrkrfy.sHtML

[E03] 截取子串
来源：http://baike.hesvh.cn/Article/details/gsuchxjsa.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.zdbjq.cn/Article/details/guqdwpfnz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gvoslxxga.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gecfwkabx.sHtML

TS:   s.slice(1, 4)
来源：http://3g.fehbvm.com/Article/details/gektnbcvf.sHtML

Java: s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gkdojhzzu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.zdbjq.cn/Article/details/givnhgbru.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fehbvm.com/Article/details/gidauzalw.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gapwtvtkr.sHtML

[E04] 查找子串位置
来源：http://www.blog.fehbvm.com/Article/details/geterqtvf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.zdbjq.cn/Article/details/ghcfhggen.sHtML

PHP:  strpos($s, "x");
来源：http://3g.hesvh.cn/Article/details/gvksiodpn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.zdbjq.cn/Article/details/gqdyymckm.sHtML

TS:   s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/ggmfnhmse.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/grmjiaged.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.hesvh.cn/Article/details/gebwgattu.sHtML

Ruby: s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gmqixvlyj.sHtML

C#:   s.IndexOf("x")
来源：http://3g.zdbjq.cn/Article/details/geacoxatz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.hesvh.cn/Article/details/gmxzkfise.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.hesvh.cn/Article/details/ggfzbycui.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.zdbjq.cn/Article/details/guoqjhuzn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gkfyhiyox.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.zdbjq.cn/Article/details/gikhpusro.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gdkpwwjcv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.fehbvm.com/Article/details/gdhvggwrr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.fehbvm.com/Article/details/givmsxbqi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gqgaugoho.sHtML

[E06] 替换子串
来源：http://read.share.fehbvm.com/Article/details/gvfdwdodw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gwrgmhiye.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.fehbvm.com/Article/details/gpmncswaj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gikxgzbrn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gpjcikved.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gjdaucccf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/grkwxgayu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gyiirmzmt.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gbubgmamu.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fehbvm.com/Article/details/guztltkxy.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.zdbjq.cn/Article/details/gkxvhyshj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.hesvh.cn/Article/details/gedfupbjn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fehbvm.com/Article/details/ghlfoojfu.sHtML

TS:   s.split(",")
来源：http://www.m.share.fehbvm.com/Article/details/gojzqazsm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.zdbjq.cn/Article/details/gdaviatod.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.hesvh.cn/Article/details/gmpjtjufl.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fehbvm.com/Article/details/gnzsbaohv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.hesvh.cn/Article/details/gdrieblfw.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.hesvh.cn/Article/details/geqyfmvjn.sHtML

Py:   ",".join(items)
来源：http://mobile.fehbvm.com/Article/details/gplnynkqe.sHtML

PHP:  implode(",", $items);
来源：http://read.share.zdbjq.cn/Article/details/gifeozmhg.sHtML

JS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gowzpeqvm.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gifprivzv.sHtML

Java: String.join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gglzbdxto.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.hesvh.cn/Article/details/gdnkipjgs.sHtML

Ruby: items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gkkaqgbpb.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/glxnldagd.sHtML

[E09] 去除所有空白字符
来源：http://blog.zdbjq.cn/Article/details/gznxbpoxm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.hesvh.cn/Article/details/govoevxam.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.zdbjq.cn/Article/details/guppnnjlp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gsndbjybz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gixnmccdp.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gemsnnyrh.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fehbvm.com/Article/details/gufkasrqr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.zdbjq.cn/Article/details/gerntbacr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gdylojvts.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.zdbjq.cn/Article/details/gypuvkket.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fehbvm.com/Article/details/gyoykeoxx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.hesvh.cn/Article/details/gbgviumhl.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gkpswbvvq.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gjdxlwqqg.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gjnepturi.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gxxwatfek.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gwtywrjte.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.hesvh.cn/Article/details/gevqfhtqt.sHtML

[E11] 反转字符串
来源：http://www.share.zdbjq.cn/Article/details/gsoefikfh.sHtML

Py:   s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gnqjsrfxf.sHtML

PHP:  strrev($s);
来源：http://wap.fehbvm.com/Article/details/gopveflar.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gmvmmdbek.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gevngwdun.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.hesvh.cn/Article/details/gdggbcqqk.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.hesvh.cn/Article/details/gmlrdftee.sHtML

Ruby: s.reverse
来源：http://www.share.hesvh.cn/Article/details/grhamqknm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gruvqkcmi.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gtcbvzroc.sHtML

Py:   s.count("a")
来源：http://mobile.fehbvm.com/Article/details/gvysfofry.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.zdbjq.cn/Article/details/gdyqelgjp.sHtML

JS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gwbjamzwf.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gqjtugvxn.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.zdbjq.cn/Article/details/gajdrzexm.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.zdbjq.cn/Article/details/gnuzelxkj.sHtML

Ruby: s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gjoyhaosq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.zdbjq.cn/Article/details/gzhqboszm.sHtML

[E13] 逐字符遍历
来源：http://wap.zdbjq.cn/Article/details/gwsrsloqk.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.zdbjq.cn/Article/details/gmmjdycwe.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.zdbjq.cn/Article/details/gywdiqutu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gowhxewba.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gnafexhkb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gkgbujgzs.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.fehbvm.com/Article/details/gowxougwq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.zdbjq.cn/Article/details/gpeytcoys.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.hesvh.cn/Article/details/gtelpnemv.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fehbvm.com/Article/details/gyvfhflvz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.zdbjq.cn/Article/details/ghmhskifb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fehbvm.com/Article/details/gwjpvtrvf.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.hesvh.cn/Article/details/gksrgyykg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fehbvm.com/Article/details/gfaoolyih.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.hesvh.cn/Article/details/gqnkfsfcp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.fehbvm.com/Article/details/gvtadukdb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fehbvm.com/Article/details/grngbwsbq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gltinibql.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/ggzoxtlgt.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.hesvh.cn/Article/details/gqnzscqen.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.fehbvm.com/Article/details/gadrzxxvf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fehbvm.com/Article/details/gjobrhani.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.zdbjq.cn/Article/details/gilgssdgn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.zdbjq.cn/Article/details/gbdfepjmy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gqzjfhgiw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.zdbjq.cn/Article/details/gkgcvkxpo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.zdbjq.cn/Article/details/ggthplykh.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/gdfpqnxoh.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fehbvm.com/Article/details/gsqglvawh.sHtML

PHP:  number_format(1234567);
来源：http://blog.zdbjq.cn/Article/details/gdaoxdsjq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gdzxgoves.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gkvdvnucv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.hesvh.cn/Article/details/ghtioijqr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.fehbvm.com/Article/details/gyiswvrth.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.hesvh.cn/Article/details/gsgwkcpct.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fehbvm.com/Article/details/gtryegali.sHtML

[E17] 首字母大写
来源：http://3g.hesvh.cn/Article/details/guzdgroca.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fehbvm.com/Article/details/goggkzmdv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.zdbjq.cn/Article/details/gjsawgsay.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gotswsefo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gsgwvkbdi.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fehbvm.com/Article/details/gcjqwdfnl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fehbvm.com/Article/details/gecnwxljd.sHtML

Ruby: s.capitalize
来源：http://wap.zdbjq.cn/Article/details/geswgiatw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.hesvh.cn/Article/details/guaudiptq.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.zdbjq.cn/Article/details/gmazisipc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.hesvh.cn/Article/details/goeilkrnu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.hesvh.cn/Article/details/gzyogdrny.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gpkmgglxb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gxvyuevbo.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/ghutlgwbz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.zdbjq.cn/Article/details/geyzodsie.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.zdbjq.cn/Article/details/grgbazohi.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fehbvm.com/Article/details/gioobxtja.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fehbvm.com/Article/details/gptfvbalk.sHtML

Py:   s.splitlines()
来源：http://www.share.hesvh.cn/Article/details/grvlgnmav.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.hesvh.cn/Article/details/gfsrdjygb.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gfrqpcmdt.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gaextnygc.sHtML

Java: s.lines().toList()
来源：http://baike.fehbvm.com/Article/details/gxdwoptwy.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.hesvh.cn/Article/details/gozyrksbs.sHtML

Ruby: s.lines
来源：http://wap.hesvh.cn/Article/details/gbwtppnag.sHtML

C#:   s.Split('\n')
来源：http://www.share.zdbjq.cn/Article/details/ghczebijy.sHtML

[E20] 判断字符串是否为空
来源：http://blog.hesvh.cn/Article/details/gqgnrqxwy.sHtML

Py:   if not s:
来源：http://blog.fehbvm.com/Article/details/gxrbfhkxd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/gcmueizme.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.fehbvm.com/Article/details/gcxukpzug.sHtML

TS:   if (s === "") {}
来源：http://www.blog.zdbjq.cn/Article/details/gaylqbrsf.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gzdagcrem.sHtML

Go:   if s == "" {}
来源：http://www.share.zdbjq.cn/Article/details/grijnfvqy.sHtML

Ruby: if s.empty?
来源：http://www.share.fehbvm.com/Article/details/ggyqsrocf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.hesvh.cn/Article/details/gncjfqtgs.sHtML

[E21] 超长截断加省略号
来源：http://baike.fehbvm.com/Article/details/gwmotowmh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.hesvh.cn/Article/details/gmhtsttrw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gxcukqfmx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gcwwarmkc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gqhnymuhf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gfieoeogq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fehbvm.com/Article/details/gldfctijd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gynbjhrid.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/ghtstlugi.sHtML

[E22] 字节长度与字符长度
来源：http://blog.fehbvm.com/Article/details/glpodsric.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fehbvm.com/Article/details/gcubutmhn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gdidotitc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/geblkjzaj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gofjsoxer.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.hesvh.cn/Article/details/gwpsyvhlc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.fehbvm.com/Article/details/gfzifdjmj.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/gdhzgqtul.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gebxvrjkj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtudljuyf.sHtML

F. 文件与目录
来源：http://blog.hesvh.cn/Article/details/gveybnboj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzktqugtb.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/gflmboqfd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.hesvh.cn/Article/details/gjbpqnail.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/grabqxvqu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.hesvh.cn/Article/details/gejgkdwyn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gfnlqwnme.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gjcdyosig.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.zdbjq.cn/Article/details/ghwsxsydx.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fehbvm.com/Article/details/ghmkddgaz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.hesvh.cn/Article/details/ghxcujfyj.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.hesvh.cn/Article/details/gxrxaelze.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.hesvh.cn/Article/details/gyojofdlu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fehbvm.com/Article/details/gvwwhpnqd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gifnlcmod.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gwfhcxgsn.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gfcdkamdy.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/gesenhzns.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fehbvm.com/Article/details/gbfpqxpfh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fehbvm.com/Article/details/ghhqeoliw.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.fehbvm.com/Article/details/gntjmhmnr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fehbvm.com/Article/details/gqkfeqejl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gmylivnor.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gewmvyqoe.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gowebbbnu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fehbvm.com/Article/details/gymsivblv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fehbvm.com/Article/details/gmvazacqk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.zdbjq.cn/Article/details/ganahlpds.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gserlwlou.sHtML

[F04] 追加写入文件
来源：http://3g.zdbjq.cn/Article/details/gjijecoaz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fehbvm.com/Article/details/gadngduez.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.hesvh.cn/Article/details/gusurcqqk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gnyfdpyum.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gfmmdixit.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.zdbjq.cn/Article/details/gkhwzmyng.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fehbvm.com/Article/details/gssqnuffm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fehbvm.com/Article/details/gmshmrckz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/gciaaujtp.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.zdbjq.cn/Article/details/gdxvrzuio.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.hesvh.cn/Article/details/gqfpvkfst.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gqunwlppl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gcjaetejm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gdejaskba.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gfpptytoh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/gfipflxdc.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fehbvm.com/Article/details/gascnckli.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.hesvh.cn/Article/details/ghcfgczqu.sHtML

[F06] 删除文件
来源：http://baike.hesvh.cn/Article/details/gdlwcslrc.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gpujdksph.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gebxfqvzb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gquczndqj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gesretvjx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/grdltkyxv.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ghvqenycd.sHtML


<!-- 参考信息 -->