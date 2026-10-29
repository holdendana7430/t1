代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gazdalrvv.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gyebfyfsm.sHtML

C#:   list.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gzzkpynra.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.hesvh.cn/Article/details/glkjzsgkd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.hesvh.cn/Article/details/gumlciivr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fehbvm.com/Article/details/ggjnvdtnw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.hesvh.cn/Article/details/gblztusjq.sHtML

TS:   [...arr];
来源：http://3g.hesvh.cn/Article/details/gdcnohccl.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gxyzpilbr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.hesvh.cn/Article/details/goiixbvkx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.zdbjq.cn/Article/details/glewmiwxy.sHtML

C#:   new List<int>(list);
来源：http://mobile.zdbjq.cn/Article/details/gguttoefx.sHtML

[D23] reduce 累积计算
来源：http://blog.fehbvm.com/Article/details/gwodmwgxr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/gkucrmflb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fehbvm.com/Article/details/gwtxfxtgi.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gnwexncyc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gmujhxrrd.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fehbvm.com/Article/details/gnmlvamph.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gexgwoxmu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.zdbjq.cn/Article/details/gnclmybxp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.zdbjq.cn/Article/details/gctddnvyh.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fehbvm.com/Article/details/gtzgancdr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fehbvm.com/Article/details/gikbzeknl.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.hesvh.cn/Article/details/gbmcnelao.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fehbvm.com/Article/details/gtszjpowa.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gsdbpkbwr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fehbvm.com/Article/details/gmlosdynx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.hesvh.cn/Article/details/gnygzbdqq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.zdbjq.cn/Article/details/galhsbtcy.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.zdbjq.cn/Article/details/gkjbatxju.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.hesvh.cn/Article/details/gnmycovne.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fehbvm.com/Article/details/guiqwcjbb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.hesvh.cn/Article/details/ghluyjcue.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.hesvh.cn/Article/details/gzhxvjqiz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.hesvh.cn/Article/details/gysolejak.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gkegmahlf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.fehbvm.com/Article/details/gwwexmwev.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.hesvh.cn/Article/details/gpjnkiyfy.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.hesvh.cn/Article/details/gmzhmcnqj.sHtML

[D26] 数组转字符串
来源：http://www.share.hesvh.cn/Article/details/gpcnrzvqn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.hesvh.cn/Article/details/gbaiogfnx.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gbfwqvpeb.sHtML

JS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gjhbuhgmm.sHtML

TS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gfyvajlrf.sHtML

Java: String.join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gdtequwkf.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.zdbjq.cn/Article/details/geqrpbibp.sHtML

Ruby: arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gmzpvhrwv.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gtnhyuwsj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gujktglmn.sHtML

E. 字符串处理
来源：http://www.share.zdbjq.cn/Article/details/gtddpkwnr.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnbrzmhjd.sHtML

[E01] 拼接字符串
来源：http://wap.hesvh.cn/Article/details/gugisayit.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.hesvh.cn/Article/details/ghhpjxkra.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.hesvh.cn/Article/details/guhpcdvei.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gjheyqlur.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/grfbzshfa.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fehbvm.com/Article/details/gjdjycgra.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.hesvh.cn/Article/details/gdyncpgoe.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.hesvh.cn/Article/details/glbgthtxr.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gsccycrjq.sHtML

[E02] 重复字符串
来源：http://blog.fehbvm.com/Article/details/gkvcrixcm.sHtML

Py:   "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gkzkpwyib.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fehbvm.com/Article/details/gfraukztp.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/ggjdyspfz.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gpixhxecr.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gklvluvhl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.hesvh.cn/Article/details/gbttlmmzd.sHtML

Ruby: "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gjqbimqxc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.hesvh.cn/Article/details/gbdmlnzgm.sHtML

[E03] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/godlzxhkw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/gzwveznkd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gestlyasv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/geddgggee.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gyerxpeng.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/ghwtgeblo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.zdbjq.cn/Article/details/gdceprsff.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.zdbjq.cn/Article/details/gayityqtg.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.hesvh.cn/Article/details/gptudntxq.sHtML

[E04] 查找子串位置
来源：http://wap.hesvh.cn/Article/details/grppumzcg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fehbvm.com/Article/details/gpogayfjz.sHtML

PHP:  strpos($s, "x");
来源：http://3g.hesvh.cn/Article/details/gzmmiyvod.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.zdbjq.cn/Article/details/gxjtefuiv.sHtML

TS:   s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gvesaoboc.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/girxelfzh.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.zdbjq.cn/Article/details/gmmvicdmz.sHtML

Ruby: s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gozvjmbjo.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gviipherf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.zdbjq.cn/Article/details/gnvdzzktt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.fehbvm.com/Article/details/ggturjqgw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.hesvh.cn/Article/details/gzlotofoi.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gedbnevym.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fehbvm.com/Article/details/giuffpnit.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gothkakmw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.hesvh.cn/Article/details/guetmwpli.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fehbvm.com/Article/details/gskskjtqd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gyygdusxt.sHtML

[E06] 替换子串
来源：http://mobile.zdbjq.cn/Article/details/gohyasqin.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/grcoqraxo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fehbvm.com/Article/details/gfermizlt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gjtjtpmix.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gfwsfakrl.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gcpipjxkq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gcztnruuh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gbvqvmkuo.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gogbjwuzc.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fehbvm.com/Article/details/gihgffxqv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.hesvh.cn/Article/details/gizumagcr.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gjyzotqcc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fehbvm.com/Article/details/gjbnvpgty.sHtML

TS:   s.split(",")
来源：http://www.share.hesvh.cn/Article/details/glzrqomob.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.hesvh.cn/Article/details/gnlcxvdqn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fehbvm.com/Article/details/gacehotqm.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.hesvh.cn/Article/details/grnszzegg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.fehbvm.com/Article/details/gbtewwbok.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.hesvh.cn/Article/details/gzpqbvcas.sHtML

Py:   ",".join(items)
来源：http://3g.fehbvm.com/Article/details/gjlxkynav.sHtML

PHP:  implode(",", $items);
来源：http://m.share.zdbjq.cn/Article/details/gszjzaywr.sHtML

JS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/givlbnuih.sHtML

TS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/glwkyjahv.sHtML

Java: String.join(",", items)
来源：http://wap.fehbvm.com/Article/details/ggtrdstzl.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fehbvm.com/Article/details/gpzpagkbc.sHtML

Ruby: items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gxmeokayc.sHtML

C#:   string.Join(",", items)
来源：http://mobile.hesvh.cn/Article/details/ggnvcudek.sHtML

[E09] 去除所有空白字符
来源：http://baike.hesvh.cn/Article/details/gzywplugm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.zdbjq.cn/Article/details/gbtoqywju.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.zdbjq.cn/Article/details/gudxscxle.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gbkuyylep.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/ghnxlamnl.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gpwsmnofl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.zdbjq.cn/Article/details/gobbseywi.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fehbvm.com/Article/details/gdycprqbn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gmsxuqwmt.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.fehbvm.com/Article/details/gioeswulq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gpfeeohii.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.hesvh.cn/Article/details/gdhtfpwcs.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gijevmxop.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gzcohwvxq.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/grbtehmsx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gyfgmmazn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gnrravwsj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fehbvm.com/Article/details/gambyskhz.sHtML

[E11] 反转字符串
来源：http://3g.fehbvm.com/Article/details/ggnydozjn.sHtML

Py:   s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gaokupgnh.sHtML

PHP:  strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gcbtclxmc.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/guskxapzp.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gyyksgksw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fehbvm.com/Article/details/gonootavs.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fehbvm.com/Article/details/gcxtpouxr.sHtML

Ruby: s.reverse
来源：http://mobile.hesvh.cn/Article/details/ggckkzznh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gwlkezgpl.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.zdbjq.cn/Article/details/gzzsjpydt.sHtML

Py:   s.count("a")
来源：http://wap.fehbvm.com/Article/details/gvxgfknlo.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.zdbjq.cn/Article/details/gvkgydmxq.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gwtgabbxo.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gjcpheqtg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fehbvm.com/Article/details/gcjvxjmev.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.fehbvm.com/Article/details/gfhntqozc.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/ghmrztujq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fehbvm.com/Article/details/gdzqwobpp.sHtML

[E13] 逐字符遍历
来源：http://wap.hesvh.cn/Article/details/gxlczduez.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.hesvh.cn/Article/details/guhmukijh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.zdbjq.cn/Article/details/gznvgetza.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gckpdmixb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gzgpxuwsb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fehbvm.com/Article/details/gdbyvszbd.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.hesvh.cn/Article/details/gioxwvtts.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.hesvh.cn/Article/details/gvpgtfdbr.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.zdbjq.cn/Article/details/gqxnarosf.sHtML

[E14] URL 编码与 Base64
来源：http://wap.zdbjq.cn/Article/details/gyacvdzqy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.hesvh.cn/Article/details/gekocenoi.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.fehbvm.com/Article/details/gwlulmvae.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.fehbvm.com/Article/details/gbivkvgbs.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.hesvh.cn/Article/details/gyxqsgibc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fehbvm.com/Article/details/godnfhyxg.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fehbvm.com/Article/details/giziifbav.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fehbvm.com/Article/details/gbadnpegm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fehbvm.com/Article/details/gufaottdp.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.zdbjq.cn/Article/details/gbjvisgpm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.fehbvm.com/Article/details/gylqwyabo.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.hesvh.cn/Article/details/gcjyajmhy.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.zdbjq.cn/Article/details/gznygksiu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.hesvh.cn/Article/details/gggjklsfw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.hesvh.cn/Article/details/ghhvanblz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.zdbjq.cn/Article/details/gwrsgcrrw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.zdbjq.cn/Article/details/gxzkdbdri.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.zdbjq.cn/Article/details/ghpencavn.sHtML

[E16] 数字千分位
来源：http://www.share.fehbvm.com/Article/details/gutdresse.sHtML

Py:   f"{1234567:,}"
来源：http://wap.zdbjq.cn/Article/details/gvtnapygy.sHtML

PHP:  number_format(1234567);
来源：http://wap.hesvh.cn/Article/details/guuyspqnr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gyeelxpnj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gpiicznmq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.hesvh.cn/Article/details/gvnqfmagt.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.hesvh.cn/Article/details/grjbtbqdx.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.zdbjq.cn/Article/details/ggzozrnci.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fehbvm.com/Article/details/gleizcdwl.sHtML

[E17] 首字母大写
来源：http://m.share.fehbvm.com/Article/details/gsjpzyloh.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.hesvh.cn/Article/details/gvusxeoxn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.hesvh.cn/Article/details/gdgssbrus.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gsjgioycu.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gqphwxxdy.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.zdbjq.cn/Article/details/gidfqzbtt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gnqltigdl.sHtML

Ruby: s.capitalize
来源：http://m.share.fehbvm.com/Article/details/grpidyddk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.zdbjq.cn/Article/details/geimglhzh.sHtML

[E18] 模板占位符替换
来源：http://3g.hesvh.cn/Article/details/gvtfaqojg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.hesvh.cn/Article/details/gswlzrtcc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.fehbvm.com/Article/details/gffhemwwg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gfkssulrf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gfdjxpttm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gchbycomh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gdrcgxyef.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.hesvh.cn/Article/details/gqawqqxbs.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.hesvh.cn/Article/details/grkcmaflo.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.hesvh.cn/Article/details/gdyrortlg.sHtML

Py:   s.splitlines()
来源：http://blog.hesvh.cn/Article/details/gjaajsssf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.zdbjq.cn/Article/details/gkfiipamc.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gycsrasmb.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gwvjarzwq.sHtML

Java: s.lines().toList()
来源：http://blog.hesvh.cn/Article/details/gfrsgfxda.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.zdbjq.cn/Article/details/gycwqizhu.sHtML

Ruby: s.lines
来源：http://3g.fehbvm.com/Article/details/grdagzbaa.sHtML

C#:   s.Split('\n')
来源：http://baike.fehbvm.com/Article/details/gklbjambh.sHtML

[E20] 判断字符串是否为空
来源：http://wap.hesvh.cn/Article/details/grloptesy.sHtML

Py:   if not s:
来源：http://blog.hesvh.cn/Article/details/gznpuswbi.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.zdbjq.cn/Article/details/gwqifsnpr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fehbvm.com/Article/details/gnzidjmac.sHtML

TS:   if (s === "") {}
来源：http://3g.fehbvm.com/Article/details/grtzoaopj.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/ghvnmszgi.sHtML

Go:   if s == "" {}
来源：http://3g.fehbvm.com/Article/details/gdjfyvkdy.sHtML

Ruby: if s.empty?
来源：http://read.share.hesvh.cn/Article/details/gknywiegq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.zdbjq.cn/Article/details/ggthccjkc.sHtML

[E21] 超长截断加省略号
来源：http://3g.zdbjq.cn/Article/details/gubqvmgga.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fehbvm.com/Article/details/grxadnalu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gmfyyhfbl.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gnztgnmmj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gfbuvqqbg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/ghzoyaglm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.zdbjq.cn/Article/details/goesuzqjr.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gtzlyzuuv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gosmiiepa.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.zdbjq.cn/Article/details/gjxjiyweq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.zdbjq.cn/Article/details/gygfezvvz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gctpkxkeo.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gctzakolv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gyzjnbmfg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gzlmzkatu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.fehbvm.com/Article/details/gqjdgnpoq.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/gzoqusibj.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gmltyenvx.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkgdefchl.sHtML

F. 文件与目录
来源：http://mobile.hesvh.cn/Article/details/gonspxrnp.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggyvaiiqj.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fehbvm.com/Article/details/gdyejmqtu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.zdbjq.cn/Article/details/gkzyaannm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gdlcsgjrc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.hesvh.cn/Article/details/gxrvpfgwm.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.hesvh.cn/Article/details/ggthgcnmh.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gnuogtohu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.hesvh.cn/Article/details/ghprhrhjy.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gtmytguks.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.hesvh.cn/Article/details/gyfzvvfmn.sHtML

[F02] 逐行读取文件
来源：http://m.share.fehbvm.com/Article/details/gmesdvfpr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.hesvh.cn/Article/details/gfhpzsqjp.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/gunmmvisb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gyvcawcec.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gwxcxgucl.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/griolaupv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fehbvm.com/Article/details/gopwxxhqd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fehbvm.com/Article/details/gwwmaajeu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.hesvh.cn/Article/details/grzypnwgu.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.hesvh.cn/Article/details/gqtzqgfsb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fehbvm.com/Article/details/gabegdcns.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/ghcghsfbr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/giqelafse.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gbyqwtrhp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fehbvm.com/Article/details/gatbuesrd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.zdbjq.cn/Article/details/gbskzaacn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.hesvh.cn/Article/details/gosdlvuyf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gsoyrsqwj.sHtML

[F04] 追加写入文件
来源：http://www.blog.zdbjq.cn/Article/details/gffmfetyq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gjoykbikx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.zdbjq.cn/Article/details/gjpuyuque.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gtivmpcag.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gcelmbwqg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fehbvm.com/Article/details/gwezcpfdt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/gdhssbtxs.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.zdbjq.cn/Article/details/gxpulqpnx.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.zdbjq.cn/Article/details/gzacpaqkk.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.fehbvm.com/Article/details/gcaawmjgy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fehbvm.com/Article/details/gvjbszonw.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gyqfuvahy.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gvvdhjqqu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gtihzjhze.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gnaujutvb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/gncvxesmn.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gcvahfexa.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gpjfaeesh.sHtML

[F06] 删除文件
来源：http://www.blog.zdbjq.cn/Article/details/gcwuxvlnl.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gfcbrttnx.sHtML

PHP:  unlink("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gpgvfhiyk.sHtML


<!-- 参考信息 -->