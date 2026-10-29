代发 wailian999

Ruby: arr.tally
来源：http://blog.fehbvm.com/Article/details/gntnbankm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.zdbjq.cn/Article/details/gzsaombvx.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fehbvm.com/Article/details/gxctyhfex.sHtML

Py:   x in arr
来源：http://www.m.share.fehbvm.com/Article/details/ghxkukdgm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/gccthoyyk.sHtML

JS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/goftsqeqq.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gcsopurwd.sHtML

Java: list.contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gqpumsrtc.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/givuxisja.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/gpvvufigm.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gycqesbah.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fehbvm.com/Article/details/gaaztzqnu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.hesvh.cn/Article/details/glqnxtqaf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fehbvm.com/Article/details/gufidzqcu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.hesvh.cn/Article/details/gyrsatoyp.sHtML

TS:   [...arr];
来源：http://mobile.fehbvm.com/Article/details/gzwllkewe.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.hesvh.cn/Article/details/gysuabxhl.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.hesvh.cn/Article/details/ghgcfkdwf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/gwuyesmwc.sHtML

C#:   new List<int>(list);
来源：http://blog.zdbjq.cn/Article/details/gigsxinch.sHtML

[D23] reduce 累积计算
来源：http://mobile.fehbvm.com/Article/details/gfawihggp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fehbvm.com/Article/details/gmhqcadcz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gdjmidlcd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/glxxrvvmg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gxjrskryr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.zdbjq.cn/Article/details/ghbyydkxn.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/ggvxqyabo.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/gufpcynfz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.hesvh.cn/Article/details/gbostkcdc.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.zdbjq.cn/Article/details/gxekalysu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.hesvh.cn/Article/details/gaiygydxb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.hesvh.cn/Article/details/gyvqckfbt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.fehbvm.com/Article/details/gnleqroku.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.hesvh.cn/Article/details/gmmvibrsz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fehbvm.com/Article/details/gtosfpckh.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.zdbjq.cn/Article/details/ghvygimve.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.hesvh.cn/Article/details/ghunmbnlk.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.hesvh.cn/Article/details/gqtqigwqn.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.hesvh.cn/Article/details/gtujgkhtj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.hesvh.cn/Article/details/gofcxkseq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.hesvh.cn/Article/details/gvyqlbtfi.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.zdbjq.cn/Article/details/ginbscgpo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.fehbvm.com/Article/details/gejeohlky.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gfphtabuz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.zdbjq.cn/Article/details/gpcouvspz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.hesvh.cn/Article/details/gehuchgfs.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.zdbjq.cn/Article/details/gkjjadkfp.sHtML

[D26] 数组转字符串
来源：http://m.share.hesvh.cn/Article/details/gwantbubt.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fehbvm.com/Article/details/gbarfqjtq.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fehbvm.com/Article/details/grwsezvbh.sHtML

JS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gfnwnuckq.sHtML

TS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gpwpidxrz.sHtML

Java: String.join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gbxwoouzq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.zdbjq.cn/Article/details/gvulyxtrl.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gvgjukkud.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gmedoxmmz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gagmtaycl.sHtML

E. 字符串处理
来源：http://wap.hesvh.cn/Article/details/grybidtmi.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gyqoffnnm.sHtML

[E01] 拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gfgyvjaon.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.fehbvm.com/Article/details/gtyghlrwr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fehbvm.com/Article/details/gitetrbcg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/ggtsbkaxm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/grrldyhaz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.hesvh.cn/Article/details/gzkhqejui.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fehbvm.com/Article/details/gsefyadyh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.fehbvm.com/Article/details/gwwwgkqds.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gonahcrgr.sHtML

[E02] 重复字符串
来源：http://blog.zdbjq.cn/Article/details/gvlgrjhhl.sHtML

Py:   "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gubksyugh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.zdbjq.cn/Article/details/glzdihppk.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gelalblaf.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gdixtdzuu.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/giytxwurs.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/gbvhffkkv.sHtML

Ruby: "ab" * 3
来源：http://wap.hesvh.cn/Article/details/guratojlg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.hesvh.cn/Article/details/gdztwezxp.sHtML

[E03] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gavzedilf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fehbvm.com/Article/details/gfwajikeh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gewxhacbn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gxeoxvszt.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fehbvm.com/Article/details/geerxdygt.sHtML

Java: s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gufdkgqlq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gidtbgwvf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.hesvh.cn/Article/details/guzywufcq.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fehbvm.com/Article/details/gosenrofr.sHtML

[E04] 查找子串位置
来源：http://wap.fehbvm.com/Article/details/gukyepnqn.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gavosehcx.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.hesvh.cn/Article/details/gwgeolwat.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.fehbvm.com/Article/details/gnpannxnr.sHtML

TS:   s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gbwbsfziw.sHtML

Java: s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gwgeraove.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fehbvm.com/Article/details/gnecccbwu.sHtML

Ruby: s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gljjjvkyy.sHtML

C#:   s.IndexOf("x")
来源：http://3g.hesvh.cn/Article/details/gevjgsbmw.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.hesvh.cn/Article/details/grnazxdfs.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.hesvh.cn/Article/details/goskmkwme.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fehbvm.com/Article/details/gkrmkrqcp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gremihiwc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.hesvh.cn/Article/details/gyrcqlpwk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/glodzgisg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.zdbjq.cn/Article/details/gdcqqzuty.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.fehbvm.com/Article/details/gzuzttnnr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gbpxbdjps.sHtML

[E06] 替换子串
来源：http://read.share.hesvh.cn/Article/details/gmhfxbkec.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gdkijddav.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fehbvm.com/Article/details/gnutulzhs.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gjzppijnr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/ggiornito.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gdbpreiip.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gjhljyyhn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.hesvh.cn/Article/details/gpralgnrs.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.hesvh.cn/Article/details/ggthzjyep.sHtML

[E07] 按分隔符拆分
来源：http://mobile.hesvh.cn/Article/details/gusbxdvdm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.hesvh.cn/Article/details/guuucmnjl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gpgjzqzlq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fehbvm.com/Article/details/geihgalle.sHtML

TS:   s.split(",")
来源：http://www.blog.fehbvm.com/Article/details/gxlntooda.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.hesvh.cn/Article/details/gfdbemymw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.hesvh.cn/Article/details/gclqjwlxs.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.zdbjq.cn/Article/details/gvburbcke.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.fehbvm.com/Article/details/gomblbtyg.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.zdbjq.cn/Article/details/gnqjptqeu.sHtML

Py:   ",".join(items)
来源：http://read.share.fehbvm.com/Article/details/gpkuspbvl.sHtML

PHP:  implode(",", $items);
来源：http://wap.hesvh.cn/Article/details/gozvygkhv.sHtML

JS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gqewxmfoq.sHtML

TS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gjdmgvinr.sHtML

Java: String.join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gomtasigi.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.zdbjq.cn/Article/details/gqnfovvgy.sHtML

Ruby: items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gzcalbmrt.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gavbkviuu.sHtML

[E09] 去除所有空白字符
来源：http://mobile.hesvh.cn/Article/details/golowgqtx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fehbvm.com/Article/details/gqofckhxp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.hesvh.cn/Article/details/gxllavryo.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gclqwzfnb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gfqcvfuaa.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.fehbvm.com/Article/details/gnthydccy.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.zdbjq.cn/Article/details/gdojoghbn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.hesvh.cn/Article/details/gntykcupl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gztftjmeo.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.zdbjq.cn/Article/details/gtfcikhjh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fehbvm.com/Article/details/gqtqdoguk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.zdbjq.cn/Article/details/gvuopinwf.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gfrkfryob.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gvnnvktzt.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gwsiixzoa.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gwfacawjx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gjthqpdjs.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.hesvh.cn/Article/details/grpatzeat.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/ggtyrpmmk.sHtML

Py:   s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gyjyujfrx.sHtML

PHP:  strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gsqakzxwb.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/goahptjed.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gkkbazugi.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gakcqwyst.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.fehbvm.com/Article/details/gxbaecyte.sHtML

Ruby: s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gvxplxrct.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gipelkfrj.sHtML

[E12] 统计某字符出现次数
来源：http://3g.fehbvm.com/Article/details/ggtfsfsns.sHtML

Py:   s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gzsqxybdm.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.zdbjq.cn/Article/details/ggpqigxfx.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gihwpolhb.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/glbuqdvhc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.hesvh.cn/Article/details/gqufdjcub.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fehbvm.com/Article/details/gmwnqlfwa.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/grqskaobi.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.zdbjq.cn/Article/details/ggbsqkeqr.sHtML

[E13] 逐字符遍历
来源：http://www.share.fehbvm.com/Article/details/gyvlifmvw.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.zdbjq.cn/Article/details/gleteghjw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fehbvm.com/Article/details/gqjbacfyn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gbwdxlijo.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gwsgvgdvj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fehbvm.com/Article/details/gpqvbbmaf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fehbvm.com/Article/details/ghcsvegzv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.hesvh.cn/Article/details/gxedbqret.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fehbvm.com/Article/details/gkuepedgs.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/gczwbwasa.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fehbvm.com/Article/details/gqfrngdce.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fehbvm.com/Article/details/gumgvtvam.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.zdbjq.cn/Article/details/geceyabbt.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fehbvm.com/Article/details/gcxzdllna.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fehbvm.com/Article/details/gsmaibwev.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fehbvm.com/Article/details/gcjlodowv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.zdbjq.cn/Article/details/ggufccpez.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.zdbjq.cn/Article/details/gqrujnoox.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.zdbjq.cn/Article/details/gqzekhzfx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.hesvh.cn/Article/details/gslxhsoni.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/grdygschm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.zdbjq.cn/Article/details/gaoyqxceo.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.hesvh.cn/Article/details/gwkrhvypb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.zdbjq.cn/Article/details/gbxdbdyjx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fehbvm.com/Article/details/glmyxmvrj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.hesvh.cn/Article/details/gaskgpddv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.hesvh.cn/Article/details/gzyxyjkwp.sHtML

[E16] 数字千分位
来源：http://3g.zdbjq.cn/Article/details/geyddnkyb.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fehbvm.com/Article/details/gabdtlvxa.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.hesvh.cn/Article/details/ggpcdtrxt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gsnfhxvjf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gfkmdeyvf.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gppbmcari.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.hesvh.cn/Article/details/gwviickrf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fehbvm.com/Article/details/gypfzrysm.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.zdbjq.cn/Article/details/godhigbdz.sHtML

[E17] 首字母大写
来源：http://blog.fehbvm.com/Article/details/gifjenrwn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.hesvh.cn/Article/details/gsyiuwaxz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.fehbvm.com/Article/details/gfjczfzxt.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/gviqcvelt.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/grqudczsy.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.hesvh.cn/Article/details/gsphzhrex.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.hesvh.cn/Article/details/gcmyqlpnk.sHtML

Ruby: s.capitalize
来源：http://www.share.hesvh.cn/Article/details/gyignmxge.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.hesvh.cn/Article/details/gueiozhax.sHtML

[E18] 模板占位符替换
来源：http://m.share.hesvh.cn/Article/details/gsrmieddn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.fehbvm.com/Article/details/gobhogirr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.zdbjq.cn/Article/details/ggfyfphdy.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gzpqlqdts.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gfsdvencr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gyuogtffz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.hesvh.cn/Article/details/gqlkpayzm.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.hesvh.cn/Article/details/gysycxxxc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.zdbjq.cn/Article/details/guykxdbcc.sHtML

[E19] 多行文本按行拆分
来源：http://wap.hesvh.cn/Article/details/gpekjemqx.sHtML

Py:   s.splitlines()
来源：http://wap.hesvh.cn/Article/details/gfzgzgbpk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.hesvh.cn/Article/details/gpltjvnzy.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/gyxagyqdx.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gkbavkbqd.sHtML

Java: s.lines().toList()
来源：http://3g.hesvh.cn/Article/details/glbjnotuh.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.zdbjq.cn/Article/details/gittzawwg.sHtML

Ruby: s.lines
来源：http://www.blog.hesvh.cn/Article/details/gqbnhlvtp.sHtML

C#:   s.Split('\n')
来源：http://blog.zdbjq.cn/Article/details/gpqbkxatw.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.zdbjq.cn/Article/details/gjctpnwfs.sHtML

Py:   if not s:
来源：http://m.share.fehbvm.com/Article/details/gnmvgpywj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.hesvh.cn/Article/details/gpzxeurzt.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/ggtzfxbsi.sHtML

TS:   if (s === "") {}
来源：http://3g.zdbjq.cn/Article/details/grrjsjmhy.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gekzjtewe.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fehbvm.com/Article/details/gngsedhao.sHtML

Ruby: if s.empty?
来源：http://read.share.fehbvm.com/Article/details/gpubldtwc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.hesvh.cn/Article/details/gpibgqaxi.sHtML

[E21] 超长截断加省略号
来源：http://baike.fehbvm.com/Article/details/gxvxofptv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.zdbjq.cn/Article/details/galijmgnp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fehbvm.com/Article/details/ganywbins.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gprwlpegn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gnemibkdk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gevliaocu.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.fehbvm.com/Article/details/gchotzzjg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gzpemilsa.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gditbvatk.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.zdbjq.cn/Article/details/gpospzfpg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.zdbjq.cn/Article/details/gkyypphoa.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gxkqhbgsy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/ghljmwxgv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/gmkykjlhb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fehbvm.com/Article/details/ghtigjngc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.zdbjq.cn/Article/details/gavsuhhpj.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.zdbjq.cn/Article/details/gvpmmjoik.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fehbvm.com/Article/details/gvvmzqjjp.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gcqijbgbe.sHtML

F. 文件与目录
来源：http://www.share.fehbvm.com/Article/details/gugkdjeia.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/genvtqzte.sHtML

[F01] 读取整个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gcukiqvyj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.fehbvm.com/Article/details/gmkzpbkek.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gldfcyyor.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fehbvm.com/Article/details/gekeufzlv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gagglxtrm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gdflbkfbb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fehbvm.com/Article/details/gmtmqqdik.sHtML

Ruby: File.read("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gmhizamcm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.hesvh.cn/Article/details/gkmelcdxw.sHtML

[F02] 逐行读取文件
来源：http://wap.hesvh.cn/Article/details/gbjywblrs.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.fehbvm.com/Article/details/gzpeqmacw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.zdbjq.cn/Article/details/gcdneohdv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/ggyolvrde.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gzbjnmgre.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gbpwbkwgc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.hesvh.cn/Article/details/gbstkalvy.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fehbvm.com/Article/details/gkgebzwfa.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.fehbvm.com/Article/details/gvvdfmuas.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.hesvh.cn/Article/details/grelhiyzy.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.zdbjq.cn/Article/details/gudfkytrl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gptmchdhp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gqlseegrq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gbbnzoazc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.fehbvm.com/Article/details/gmbglmsly.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.zdbjq.cn/Article/details/gtifvrhsr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.zdbjq.cn/Article/details/gpzetkagf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gwcjmgqkq.sHtML

[F04] 追加写入文件
来源：http://baike.zdbjq.cn/Article/details/gfgfekpwx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fehbvm.com/Article/details/gwmsodhqk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.hesvh.cn/Article/details/gtiytdpjp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gdqwfcees.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gptssfatq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.zdbjq.cn/Article/details/gxlowfscn.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.hesvh.cn/Article/details/gtyximreb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.hesvh.cn/Article/details/gltrtcwrl.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fehbvm.com/Article/details/gahcncglh.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.zdbjq.cn/Article/details/gynpdyryu.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.hesvh.cn/Article/details/gcpeqkcpf.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.hesvh.cn/Article/details/glmtcfmmr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gjsymeewu.sHtML


<!-- 参考信息 -->