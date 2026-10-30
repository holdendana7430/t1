代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/ggvfjmamc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fanxiaobao.xyz/Article/details/gfkcmpecg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gqijqqwsb.sHtML

TS:   [...arr];
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnmxuckv.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fanxiaobao.xyz/Article/details/gwcjxmhug.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpgrhybw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqtkfgue.sHtML

C#:   new List<int>(list);
来源：http://blog.fanxiaobao.xyz/Article/details/gpbokaprv.sHtML

[D23] reduce 累积计算
来源：http://3g.fanxiaobao.xyz/Article/details/gwbgcohws.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gjqlvjuwk.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gctzcpdtt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gdemhyhmz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnybzwgav.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.fanxiaobao.xyz/Article/details/ghngbjnre.sHtML

Go:   // 手写循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gxoewclsn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fanxiaobao.xyz/Article/details/gzrruwzek.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fanxiaobao.xyz/Article/details/gnvxbbvox.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfqrmysy.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fanxiaobao.xyz/Article/details/ghwlsnoxo.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxccrnro.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gsfydadsc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gazfiihwz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fanxiaobao.xyz/Article/details/grdtblzav.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqmrtndu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfdypjrb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fanxiaobao.xyz/Article/details/gifmzidyj.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfkzwnxa.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.fanxiaobao.xyz/Article/details/gzboshnxy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.fanxiaobao.xyz/Article/details/gyuejuein.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gmjbkqpbf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fanxiaobao.xyz/Article/details/gstfdbkhe.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvyacpgui.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fanxiaobao.xyz/Article/details/gmvtinoay.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gdteofyqd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocsaxizi.sHtML

[D26] 数组转字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwrzrasr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.fanxiaobao.xyz/Article/details/gembloptc.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkhhagyd.sHtML

JS:   arr.join(", ")
来源：http://www.share.fanxiaobao.xyz/Article/details/gtuuygvpz.sHtML

TS:   arr.join(", ")
来源：http://mobile.fanxiaobao.xyz/Article/details/gukxnyttn.sHtML

Java: String.join(", ", list)
来源：http://baike.fanxiaobao.xyz/Article/details/gaplsengk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fanxiaobao.xyz/Article/details/gnsqlpyop.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fanxiaobao.xyz/Article/details/gszcpxgyc.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fanxiaobao.xyz/Article/details/gzbmtgbdl.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gioxhythy.sHtML

E. 字符串处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzhcvtob.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/glicvrlax.sHtML

[E01] 拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzfjxenf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrdirtbq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkebcirs.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwpssxeh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdoulnnv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.fanxiaobao.xyz/Article/details/gtkdfqfbc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fanxiaobao.xyz/Article/details/gmnihbyvp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvesmxzx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/grbwvnroq.sHtML

[E02] 重复字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwdbjvtq.sHtML

Py:   "ab" * 3
来源：http://blog.fanxiaobao.xyz/Article/details/gqepeykrg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/grphzxsub.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gexzuropz.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmorvzwes.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjvhkrxi.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gndwvpakd.sHtML

Ruby: "ab" * 3
来源：http://wap.fanxiaobao.xyz/Article/details/gzhemvcst.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fanxiaobao.xyz/Article/details/guygiitsv.sHtML

[E03] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/glmqcrcaf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkiwecov.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvdroirj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fanxiaobao.xyz/Article/details/goaujzbhk.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxltycsml.sHtML

Java: s.substring(1, 4)
来源：http://blog.fanxiaobao.xyz/Article/details/gjgpqemhy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlcmecue.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fanxiaobao.xyz/Article/details/groumldtv.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.fanxiaobao.xyz/Article/details/ggdfswmxf.sHtML

[E04] 查找子串位置
来源：http://wap.fanxiaobao.xyz/Article/details/gpfdfloji.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fanxiaobao.xyz/Article/details/gwprtdzxa.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzxabxvd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fanxiaobao.xyz/Article/details/gvtrxtlnz.sHtML

TS:   s.indexOf("x")
来源：http://wap.fanxiaobao.xyz/Article/details/gakojywny.sHtML

Java: s.indexOf("x")
来源：http://3g.fanxiaobao.xyz/Article/details/gzbsijtcf.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fanxiaobao.xyz/Article/details/gpzrvcecs.sHtML

Ruby: s.index("x")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfamxtfj.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemtzwyne.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fanxiaobao.xyz/Article/details/gumvopdpi.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.fanxiaobao.xyz/Article/details/gszoaxddi.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.fanxiaobao.xyz/Article/details/glvmyyumo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzqxokye.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.fanxiaobao.xyz/Article/details/grmyvkiol.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzolsimn.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnptchlxn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fanxiaobao.xyz/Article/details/gpqcsfitg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhzwrnhk.sHtML

[E06] 替换子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyogsbnr.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gtnpxxdle.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.fanxiaobao.xyz/Article/details/ggvjfwjgc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/ganzseysg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/gshbpwora.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpziiygm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyyilodjl.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjvnbagi.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/gjrlzcxde.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttkljlmo.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdjrgpcl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gyratepto.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpafwlfr.sHtML

TS:   s.split(",")
来源：http://blog.fanxiaobao.xyz/Article/details/gjfhgsibv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fanxiaobao.xyz/Article/details/guptndlcz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwckngxqu.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbqjopbl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjuukykki.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fanxiaobao.xyz/Article/details/gqdgbvcpj.sHtML

Py:   ",".join(items)
来源：http://mobile.fanxiaobao.xyz/Article/details/gafbuykdw.sHtML

PHP:  implode(",", $items);
来源：http://wap.fanxiaobao.xyz/Article/details/gbojvoavk.sHtML

JS:   items.join(",")
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcmqhcas.sHtML

TS:   items.join(",")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopyvfzqi.sHtML

Java: String.join(",", items)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfjqhvim.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fanxiaobao.xyz/Article/details/gsizrrzik.sHtML

Ruby: items.join(",")
来源：http://3g.fanxiaobao.xyz/Article/details/gsjirszvr.sHtML

C#:   string.Join(",", items)
来源：http://blog.fanxiaobao.xyz/Article/details/gafofkobo.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhvwtuld.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gppwmmpfn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdrnqwhe.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fanxiaobao.xyz/Article/details/gbykotxmw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.fanxiaobao.xyz/Article/details/ggadsbyen.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fanxiaobao.xyz/Article/details/gakopajop.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbsozwdze.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fanxiaobao.xyz/Article/details/glfbsnlqh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgakzfue.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.fanxiaobao.xyz/Article/details/giazwygst.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fanxiaobao.xyz/Article/details/gsupoultu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fanxiaobao.xyz/Article/details/gaserzfdb.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.fanxiaobao.xyz/Article/details/gkbapnasc.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.fanxiaobao.xyz/Article/details/gaicdcfxt.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fanxiaobao.xyz/Article/details/giaxvecqy.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfgnkcss.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbufjcxgs.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgrgwgyd.sHtML

[E11] 反转字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkabrkay.sHtML

Py:   s[::-1]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpdpvgqq.sHtML

PHP:  strrev($s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybuufnkm.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.fanxiaobao.xyz/Article/details/gfruyfrtz.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fanxiaobao.xyz/Article/details/ghqxgibdy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fanxiaobao.xyz/Article/details/gpousxlme.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fanxiaobao.xyz/Article/details/glztkhxls.sHtML

Ruby: s.reverse
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjgawgin.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlauozfb.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fanxiaobao.xyz/Article/details/gwoxqfjrc.sHtML

Py:   s.count("a")
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxgnzilv.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokuxjrsj.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gszvukhho.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzmcjpzh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fanxiaobao.xyz/Article/details/gayhdkhxr.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fanxiaobao.xyz/Article/details/gweorjava.sHtML

Ruby: s.count("a")
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgxfnqno.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.fanxiaobao.xyz/Article/details/gfajmacei.sHtML

[E13] 逐字符遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gywknurcn.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmglvyut.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gizcytpmr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmzfmalm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fanxiaobao.xyz/Article/details/gvmqtbjfx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.fanxiaobao.xyz/Article/details/gqosetiuw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gokguesgk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fanxiaobao.xyz/Article/details/gobajqcgm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzyktbquz.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gfclkbitp.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fanxiaobao.xyz/Article/details/gfiwdadev.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqqndjml.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.fanxiaobao.xyz/Article/details/guhpvyuqc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fanxiaobao.xyz/Article/details/ggkxxjufh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmckoxtie.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fanxiaobao.xyz/Article/details/ggbyvnslj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkistqmnp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkfnzvnj.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcupqgwjz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gopndksvy.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.fanxiaobao.xyz/Article/details/gzcyddjpo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnroobtsn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.fanxiaobao.xyz/Article/details/ggblyhlno.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnxnbira.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fanxiaobao.xyz/Article/details/giltiynuo.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gpekpgyov.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkewbytul.sHtML

[E16] 数字千分位
来源：http://read.share.fanxiaobao.xyz/Article/details/gknpepdpc.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxlyjgxe.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdoqxjej.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fanxiaobao.xyz/Article/details/guzokzvef.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvohltpwa.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fanxiaobao.xyz/Article/details/gzqugxiyd.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fanxiaobao.xyz/Article/details/guyyqmfiv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fanxiaobao.xyz/Article/details/gapuaetwk.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fanxiaobao.xyz/Article/details/gkygiegoh.sHtML

[E17] 首字母大写
来源：http://blog.fanxiaobao.xyz/Article/details/giuytwyai.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzpqlhiw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fanxiaobao.xyz/Article/details/ghtgxwtwa.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gavvoannj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fanxiaobao.xyz/Article/details/ghaitkdwt.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gudrbydzt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnecxihi.sHtML

Ruby: s.capitalize
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvuplhsr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgktmaie.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejolphji.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fanxiaobao.xyz/Article/details/gtdblwalg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfkbfgnr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqokglgd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.fanxiaobao.xyz/Article/details/gnvglgzmy.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsprqmdzc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.fanxiaobao.xyz/Article/details/gwdimlesk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdetkkmq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fanxiaobao.xyz/Article/details/gvemwpowm.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fanxiaobao.xyz/Article/details/gemyyueam.sHtML

Py:   s.splitlines()
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzrlwawe.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gxinncuji.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhaxrmqb.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fanxiaobao.xyz/Article/details/gaztjimbr.sHtML

Java: s.lines().toList()
来源：http://wap.fanxiaobao.xyz/Article/details/gfmragqat.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxabcrrt.sHtML

Ruby: s.lines
来源：http://blog.fanxiaobao.xyz/Article/details/gqphhskxa.sHtML

C#:   s.Split('\n')
来源：http://3g.fanxiaobao.xyz/Article/details/gcvsmlccs.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjzpopxc.sHtML

Py:   if not s:
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnebcaact.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.fanxiaobao.xyz/Article/details/gaorbljhg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gibcdscli.sHtML

TS:   if (s === "") {}
来源：http://baike.fanxiaobao.xyz/Article/details/gcwloygul.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gylquionv.sHtML

Go:   if s == "" {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gsylzquiu.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfanvvypq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/golpzriuz.sHtML

[E21] 超长截断加省略号
来源：http://3g.fanxiaobao.xyz/Article/details/gsuhvrsfk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmdknpmf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnklxnjk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtlojbkv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fanxiaobao.xyz/Article/details/ggeuskzzf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gusxgitus.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fanxiaobao.xyz/Article/details/gfbggipxb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjubxlyxk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fanxiaobao.xyz/Article/details/gicfebeiq.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflbkdbug.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gimvixpsi.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fanxiaobao.xyz/Article/details/gymjmihfo.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fanxiaobao.xyz/Article/details/gozefpjqx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fanxiaobao.xyz/Article/details/gtgthintl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbxxlzbq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fanxiaobao.xyz/Article/details/gucnvcvtz.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fanxiaobao.xyz/Article/details/ganaryntr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fanxiaobao.xyz/Article/details/gtlscfrof.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gullsxztj.sHtML

F. 文件与目录
来源：http://www.share.fanxiaobao.xyz/Article/details/gyaemcxka.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gsksffvbh.sHtML

[F01] 读取整个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwejqhvtb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fanxiaobao.xyz/Article/details/grdnhxssq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/glkhsrgsq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjrawsjw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.fanxiaobao.xyz/Article/details/gglvpmqlu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fanxiaobao.xyz/Article/details/ggytaywsk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcrdyeeg.sHtML

Ruby: File.read("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gkblozgyd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/ghffbutlr.sHtML

[F02] 逐行读取文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gcukntqdb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fanxiaobao.xyz/Article/details/gsufgzhhk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmnlfjyt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gtixsmxqp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/glhlpilih.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycjnjrhn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gndyctovq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.fanxiaobao.xyz/Article/details/gtvhxxwni.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkscywxd.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fanxiaobao.xyz/Article/details/gaufbicbz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fanxiaobao.xyz/Article/details/gizbtdzoj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpictcpnf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fanxiaobao.xyz/Article/details/gocwfcpol.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fanxiaobao.xyz/Article/details/giusxdutb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzqrqsae.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnzcggzj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.fanxiaobao.xyz/Article/details/gkzratfai.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gwlfeeoiy.sHtML

[F04] 追加写入文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbphfsxw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.fanxiaobao.xyz/Article/details/gczwdnrhr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fanxiaobao.xyz/Article/details/gatdgmeca.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fanxiaobao.xyz/Article/details/gtoiihnkd.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fanxiaobao.xyz/Article/details/gqvytgldv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fanxiaobao.xyz/Article/details/guyppfdrv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfshzmwyk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfonpbphc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fanxiaobao.xyz/Article/details/gxrqigxem.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gbdoymcjg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fanxiaobao.xyz/Article/details/gikalmnbj.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/gvjwdeitj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gwzkegned.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnpbocom.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gtudradcu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fanxiaobao.xyz/Article/details/gdfyqmauf.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gxxmuryfj.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gncxnzzkc.sHtML

[F06] 删除文件
来源：http://baike.fanxiaobao.xyz/Article/details/gfnsayklx.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gieqjbgrx.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjpkswhf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gouhlwysh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glioqbwov.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxbsuexz.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gptjlnzez.sHtML


<!-- 参考信息 -->