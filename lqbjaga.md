代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://wap.fehbvm.com/Article/details/gangxpmto.sHtML

Ruby: arr.include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gicmsmvxf.sHtML

C#:   list.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gkctlhlbm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.zdbjq.cn/Article/details/gtnayyenb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fehbvm.com/Article/details/gyjibzudy.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fehbvm.com/Article/details/ggwsqjcwf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.zdbjq.cn/Article/details/gszzlytcy.sHtML

TS:   [...arr];
来源：http://www.blog.zdbjq.cn/Article/details/gjncplqfy.sHtML

Java: new ArrayList<>(list);
来源：http://baike.zdbjq.cn/Article/details/gtzaekvgv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.hesvh.cn/Article/details/ghsswlmzx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.zdbjq.cn/Article/details/griivdzru.sHtML

C#:   new List<int>(list);
来源：http://3g.hesvh.cn/Article/details/goonnuuou.sHtML

[D23] reduce 累积计算
来源：http://wap.hesvh.cn/Article/details/gcsebbinq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fehbvm.com/Article/details/gnidzgypn.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.zdbjq.cn/Article/details/gldfyvktv.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gaksuiwfr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/ghrioibwu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.zdbjq.cn/Article/details/gnxyxlyaz.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gohrlmyyk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.zdbjq.cn/Article/details/goxyslzgy.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.zdbjq.cn/Article/details/glmohmrcx.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.zdbjq.cn/Article/details/gtofkvfmi.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.zdbjq.cn/Article/details/giicbcpop.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.hesvh.cn/Article/details/gfcxvdmvw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fehbvm.com/Article/details/gyghddwut.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fehbvm.com/Article/details/gtxlchfvv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.fehbvm.com/Article/details/gvprcgsgf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.fehbvm.com/Article/details/gajzqvmlg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.zdbjq.cn/Article/details/gofoxhgkw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.hesvh.cn/Article/details/gadchbdsm.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.hesvh.cn/Article/details/gukxmmqar.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.hesvh.cn/Article/details/gzlyndmuc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.zdbjq.cn/Article/details/gkammniyk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fehbvm.com/Article/details/gbqqjbouv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.hesvh.cn/Article/details/gzeldlasb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.fehbvm.com/Article/details/gbpjskbzj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.zdbjq.cn/Article/details/glihuejxz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.hesvh.cn/Article/details/gcbzmmznx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fehbvm.com/Article/details/gorircrzh.sHtML

[D26] 数组转字符串
来源：http://baike.hesvh.cn/Article/details/gerjwzkej.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.hesvh.cn/Article/details/gzsspuiqb.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gveitkyvb.sHtML

JS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gxhcplgro.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gtwmcybkf.sHtML

Java: String.join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gouxcskvr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.hesvh.cn/Article/details/grrtzmlef.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gbhzhgwba.sHtML

C#:   string.Join(", ", list)
来源：http://baike.hesvh.cn/Article/details/galwdgeio.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnrgqiovq.sHtML

E. 字符串处理
来源：http://read.share.fehbvm.com/Article/details/gocdlbrsh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghbulcwfp.sHtML

[E01] 拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gtblobcon.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.zdbjq.cn/Article/details/gythzzley.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.zdbjq.cn/Article/details/gynkyicgk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gxyfvtfya.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gtnqvanlo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.hesvh.cn/Article/details/gkflbzwan.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.zdbjq.cn/Article/details/grtgyybkc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.hesvh.cn/Article/details/grmjbdciy.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gnbswxvrk.sHtML

[E02] 重复字符串
来源：http://m.share.fehbvm.com/Article/details/gfljbmyxz.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gesyillvg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.fehbvm.com/Article/details/grjheejtg.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gqgpkjesf.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gzpopgfnn.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gbpygxeky.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.hesvh.cn/Article/details/gioqqrawn.sHtML

Ruby: "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gwnncfvvu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fehbvm.com/Article/details/gbudgjzhb.sHtML

[E03] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gvwguumyy.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.zdbjq.cn/Article/details/gzlekzmgr.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gbjhvmpbl.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gwznucswz.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fehbvm.com/Article/details/grfiywnzq.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gfohhmttv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.zdbjq.cn/Article/details/grbkmcvqg.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.zdbjq.cn/Article/details/gxqkqdcrv.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.hesvh.cn/Article/details/gtlscbgrp.sHtML

[E04] 查找子串位置
来源：http://m.share.fehbvm.com/Article/details/gvysgbnpw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/goneojgkt.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.zdbjq.cn/Article/details/gwnrlpluj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fehbvm.com/Article/details/ghupfeobe.sHtML

TS:   s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/ggdqazprf.sHtML

Java: s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gbyymlojm.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.hesvh.cn/Article/details/gmemexaxe.sHtML

Ruby: s.index("x")
来源：http://m.share.fehbvm.com/Article/details/givrqxhic.sHtML

C#:   s.IndexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gyosvccpb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/gxjylcswi.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.hesvh.cn/Article/details/goldkfomp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.hesvh.cn/Article/details/gezskttgh.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gxyybwqtd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.hesvh.cn/Article/details/gcnpcngda.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gxpfvzonh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.zdbjq.cn/Article/details/gdjiwnwee.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.zdbjq.cn/Article/details/gewbffnuv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.fehbvm.com/Article/details/garpyndxh.sHtML

[E06] 替换子串
来源：http://wap.zdbjq.cn/Article/details/gwakmckff.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gthmtjeiy.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.zdbjq.cn/Article/details/gpyaeykzl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gtjnhddxs.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gdcndgnxu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/ghrlivmje.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gphzritpv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gdjipyrdk.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gipuwdpse.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.zdbjq.cn/Article/details/ggndnjvkp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fehbvm.com/Article/details/gysyhawhu.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.zdbjq.cn/Article/details/ggjwwjlmf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fehbvm.com/Article/details/gombsgenl.sHtML

TS:   s.split(",")
来源：http://wap.fehbvm.com/Article/details/gpxzueami.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.hesvh.cn/Article/details/gwzcqeoop.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.zdbjq.cn/Article/details/gycewjqnc.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.fehbvm.com/Article/details/gfpcnvxsr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.zdbjq.cn/Article/details/gecwwoyxg.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.zdbjq.cn/Article/details/gzzmvwdok.sHtML

Py:   ",".join(items)
来源：http://blog.zdbjq.cn/Article/details/gppgpqckn.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.zdbjq.cn/Article/details/gimsdkncc.sHtML

JS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gcngkvlph.sHtML

TS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gmkpilbrr.sHtML

Java: String.join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gmhhiatbk.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fehbvm.com/Article/details/gtmrpmnkn.sHtML

Ruby: items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gwusgkcbz.sHtML

C#:   string.Join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gfxobbhaj.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fehbvm.com/Article/details/gbucinmsn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fehbvm.com/Article/details/gkvktzaxn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/gtpollfin.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gxtbvkgir.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gljewqmfk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/ggwbwysqz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.hesvh.cn/Article/details/gleqgtakd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.hesvh.cn/Article/details/gxomdeskd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.hesvh.cn/Article/details/gwxbdohdu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fehbvm.com/Article/details/gvyhnrqwf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gdljjxswo.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.zdbjq.cn/Article/details/gmkcngomp.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gfzxzbxtn.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gpnupqyjd.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gdiadevrj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gokcewosu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/guhpmvpuu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fehbvm.com/Article/details/gxiigsrvu.sHtML

[E11] 反转字符串
来源：http://www.share.zdbjq.cn/Article/details/gsolrxnnv.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gjvfspnbh.sHtML

PHP:  strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gkmwahozh.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/ggsdthjoo.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gltcmqcsp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/gqahtgdfv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gkjfqnefi.sHtML

Ruby: s.reverse
来源：http://read.share.fehbvm.com/Article/details/goifazokr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gbirempgu.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.hesvh.cn/Article/details/gzzfnhput.sHtML

Py:   s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gwnskosot.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fehbvm.com/Article/details/gzcadqzah.sHtML

JS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gfhqqeasm.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/gjcpvqrlj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fehbvm.com/Article/details/glpcstkwv.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.zdbjq.cn/Article/details/gvziuqpum.sHtML

Ruby: s.count("a")
来源：http://3g.fehbvm.com/Article/details/gjzoidjwt.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.hesvh.cn/Article/details/gmnknkxky.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.hesvh.cn/Article/details/gpnwhjkjp.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.zdbjq.cn/Article/details/gepojctsw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.zdbjq.cn/Article/details/gythgdzjd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/gwwzvmovn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gedyjrpaz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gpdcouizj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.hesvh.cn/Article/details/ghlhstysm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.zdbjq.cn/Article/details/gilukikfu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gwhpsezcg.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fehbvm.com/Article/details/gwbabbgjn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.zdbjq.cn/Article/details/gcidrysvx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.hesvh.cn/Article/details/geqqpuknr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.zdbjq.cn/Article/details/glkeygkzi.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.zdbjq.cn/Article/details/gcprjytjc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fehbvm.com/Article/details/glvivqghh.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.fehbvm.com/Article/details/gvdggzmne.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.zdbjq.cn/Article/details/gssrfvnnn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fehbvm.com/Article/details/gwlfubldi.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fehbvm.com/Article/details/gskwulkfl.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.hesvh.cn/Article/details/ghrnrggcx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fehbvm.com/Article/details/gzenbstuy.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gpfnkabjc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.fehbvm.com/Article/details/gzuolypok.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fehbvm.com/Article/details/guqcphycu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.zdbjq.cn/Article/details/gffagjvys.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.hesvh.cn/Article/details/gcpdgyske.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.zdbjq.cn/Article/details/gagbgbpwk.sHtML

[E16] 数字千分位
来源：http://3g.zdbjq.cn/Article/details/ggtlmsnfc.sHtML

Py:   f"{1234567:,}"
来源：http://wap.zdbjq.cn/Article/details/gcfqjtrjl.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fehbvm.com/Article/details/gmymiidlf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gpwmgzwro.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gndbjqpad.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fehbvm.com/Article/details/gvfqsvdws.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.hesvh.cn/Article/details/gpmxoxfci.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.zdbjq.cn/Article/details/gvzvsgfet.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fehbvm.com/Article/details/gjjtjipqx.sHtML

[E17] 首字母大写
来源：http://blog.hesvh.cn/Article/details/gmdtavbxq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.hesvh.cn/Article/details/goludwkyq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.zdbjq.cn/Article/details/gvtivqvnv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gfzjcjspj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gebpotjfv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fehbvm.com/Article/details/gzpsyqdzd.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.zdbjq.cn/Article/details/gkqmmpgps.sHtML

Ruby: s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/gkpnclxfs.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.fehbvm.com/Article/details/geqalwfar.sHtML

[E18] 模板占位符替换
来源：http://mobile.zdbjq.cn/Article/details/glxtgxkpl.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.zdbjq.cn/Article/details/glodmgsae.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.hesvh.cn/Article/details/gwkauhufb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/ghodesjlh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gqylzugvp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/giyplszwd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gkqgffnzp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fehbvm.com/Article/details/gxrohwrjf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fehbvm.com/Article/details/gvpcxjctb.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.fehbvm.com/Article/details/goiwhokbf.sHtML

Py:   s.splitlines()
来源：http://www.blog.fehbvm.com/Article/details/gjieitcff.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.zdbjq.cn/Article/details/gpfpklrhp.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gmejwwavd.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gfmchjwmd.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/gvzgjbaaz.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.hesvh.cn/Article/details/gmjuvgflz.sHtML

Ruby: s.lines
来源：http://wap.fehbvm.com/Article/details/gtblqbane.sHtML

C#:   s.Split('\n')
来源：http://mobile.hesvh.cn/Article/details/gpiwcuzcc.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/gajsrrrfr.sHtML

Py:   if not s:
来源：http://wap.fehbvm.com/Article/details/gvkjljcyu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.hesvh.cn/Article/details/grpmfcyvh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fehbvm.com/Article/details/gbyuzidjk.sHtML

TS:   if (s === "") {}
来源：http://www.blog.zdbjq.cn/Article/details/gxlfmrssr.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/govzyzjor.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fehbvm.com/Article/details/gjpeqnjoz.sHtML

Ruby: if s.empty?
来源：http://www.m.share.zdbjq.cn/Article/details/guxtrazct.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.zdbjq.cn/Article/details/gxfgpqwyn.sHtML

[E21] 超长截断加省略号
来源：http://mobile.zdbjq.cn/Article/details/gdcdscimd.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.zdbjq.cn/Article/details/glmzyvvuj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gbdepawvs.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gsujncswb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gilgbdznz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gfubulgsa.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.zdbjq.cn/Article/details/ghzgxernl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gelnmdqdo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gsqqlndkh.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fehbvm.com/Article/details/geriuraah.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fehbvm.com/Article/details/giycpeens.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gcliwrqgx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gslmrhztg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gpujqkjll.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.hesvh.cn/Article/details/gzcdakdfy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.zdbjq.cn/Article/details/gainhivmr.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gojphkwhx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.zdbjq.cn/Article/details/gmeyxiztf.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbwjuryjs.sHtML

F. 文件与目录
来源：http://baike.fehbvm.com/Article/details/gqbwupyyl.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxftjxrem.sHtML

[F01] 读取整个文件
来源：http://baike.fehbvm.com/Article/details/gcmleoghw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fehbvm.com/Article/details/ggiimloao.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gzblxkchp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fehbvm.com/Article/details/gfovjqojx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gvoszjmma.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gxcxetxam.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.zdbjq.cn/Article/details/gkcijcnpx.sHtML

Ruby: File.read("a.txt")
来源：http://3g.zdbjq.cn/Article/details/ghdvloivm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gdnwalyra.sHtML

[F02] 逐行读取文件
来源：http://3g.zdbjq.cn/Article/details/gyszagjgu.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.zdbjq.cn/Article/details/glaaumewr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.zdbjq.cn/Article/details/gslfsjjub.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gpcltsqfj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gjygdgomd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gpnkksrys.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.hesvh.cn/Article/details/glusaaqpi.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.zdbjq.cn/Article/details/gxkxynbfk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.zdbjq.cn/Article/details/gdqzxtvdv.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.zdbjq.cn/Article/details/gjcgfvzbv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fehbvm.com/Article/details/gstbzwfrc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/ggquufuop.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gpwvpiqoa.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/ggebwbvth.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.zdbjq.cn/Article/details/gawbyuanz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.hesvh.cn/Article/details/gdygkvhhp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.hesvh.cn/Article/details/grewkevla.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gzupsnltv.sHtML

[F04] 追加写入文件
来源：http://wap.zdbjq.cn/Article/details/gcjmggtkw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.zdbjq.cn/Article/details/grnkvskee.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.hesvh.cn/Article/details/gbmlmkuxn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gnmvmzrra.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gxmevvitz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.zdbjq.cn/Article/details/gaupqcnzu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.hesvh.cn/Article/details/gseicflcr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.hesvh.cn/Article/details/gcrnkludn.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.zdbjq.cn/Article/details/gmpxeitmg.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gnhiagivy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/gsoedsipl.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gmexrjhrp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gmdmyqxum.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gozhsfoxw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gxktfqpwp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fehbvm.com/Article/details/gpjgygdtb.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gxdoyswvi.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fehbvm.com/Article/details/gqzbxrlep.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/gnjkfhjyh.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gbqhcotnu.sHtML

PHP:  unlink("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gngauhcsi.sHtML


<!-- 参考信息 -->