代发 wailian999

Ruby: arr.tally
来源：http://www.share.fehbvm.com/Article/details/gfllovrmd.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fehbvm.com/Article/details/gruqhaama.sHtML

[D21] 判断是否包含某元素
来源：http://wap.zdbjq.cn/Article/details/ganuzuena.sHtML

Py:   x in arr
来源：http://read.share.zdbjq.cn/Article/details/gocaepaec.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.hesvh.cn/Article/details/gegcnmtth.sHtML

JS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/ghhzbofwp.sHtML

TS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gmdeucqxq.sHtML

Java: list.contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gxuhnmjmk.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gjojvjapw.sHtML

Ruby: arr.include?(x)
来源：http://baike.fehbvm.com/Article/details/gkguxxgiv.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gfmrjruay.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.zdbjq.cn/Article/details/gbvihtpvc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.zdbjq.cn/Article/details/gvqpaslqu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.hesvh.cn/Article/details/gakrggfuu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.hesvh.cn/Article/details/gfsosdndl.sHtML

TS:   [...arr];
来源：http://wap.fehbvm.com/Article/details/gxunogybn.sHtML

Java: new ArrayList<>(list);
来源：http://3g.zdbjq.cn/Article/details/gmqmilgpq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gqyfqnhus.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.hesvh.cn/Article/details/guljrjyea.sHtML

C#:   new List<int>(list);
来源：http://mobile.fehbvm.com/Article/details/gtniiehmi.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/gznahffqx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.zdbjq.cn/Article/details/glbwtocjh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fehbvm.com/Article/details/guooyilzh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gsbiewhrp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gfshhzwwt.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fehbvm.com/Article/details/gqhwpifvy.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/graeghabv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.hesvh.cn/Article/details/gkmkbhwya.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.zdbjq.cn/Article/details/girgyfwgj.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.fehbvm.com/Article/details/gvaveefqf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.hesvh.cn/Article/details/gxrzuytuu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.zdbjq.cn/Article/details/gkhlsiqns.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gobxipfnp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/glrdnsnqs.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fehbvm.com/Article/details/gjhmpicef.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.zdbjq.cn/Article/details/gkjgxaepr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.hesvh.cn/Article/details/guaqtkdug.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.zdbjq.cn/Article/details/gluqdobbe.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fehbvm.com/Article/details/gqvjcdeev.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.hesvh.cn/Article/details/gcwqxukfr.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.hesvh.cn/Article/details/ggdaqxagg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.hesvh.cn/Article/details/gicqfjexk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.hesvh.cn/Article/details/gihgbekwn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.fehbvm.com/Article/details/gptnlctcy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.hesvh.cn/Article/details/givulghnt.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.hesvh.cn/Article/details/gkighzyad.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gtnhuyacx.sHtML

[D26] 数组转字符串
来源：http://www.blog.fehbvm.com/Article/details/gdtqqcgvm.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.hesvh.cn/Article/details/gsdfduncz.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.fehbvm.com/Article/details/gymvhzpcd.sHtML

JS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gavviosnv.sHtML

TS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gohsctqlk.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gbclkwihs.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.hesvh.cn/Article/details/gginfidxp.sHtML

Ruby: arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gxjfmfqig.sHtML

C#:   string.Join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gopiagwgl.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtzdhnhvs.sHtML

E. 字符串处理
来源：http://3g.fehbvm.com/Article/details/gunuitknk.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gyeuiepjn.sHtML

[E01] 拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/ggfegxaoc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.hesvh.cn/Article/details/ghidphdnl.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fehbvm.com/Article/details/gdndkyfbz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gpnahltxb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gtglbjcsc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.zdbjq.cn/Article/details/gaottokiw.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.zdbjq.cn/Article/details/gpkcvyhie.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.zdbjq.cn/Article/details/gpamfgmqs.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gsbxzpgrr.sHtML

[E02] 重复字符串
来源：http://www.share.hesvh.cn/Article/details/guymuskzs.sHtML

Py:   "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gxewxhumk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fehbvm.com/Article/details/ggwjzyyek.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gzbauvbms.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gsgkirwtr.sHtML

Java: "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gjbafrqzo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.zdbjq.cn/Article/details/glggvgvmc.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gzixmrmwu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/gtxzbdyrj.sHtML

[E03] 截取子串
来源：http://wap.fehbvm.com/Article/details/gkjrgqdmn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.hesvh.cn/Article/details/ggjiowptc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gjxhtgdst.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gpuxdupbl.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gjiswoacm.sHtML

Java: s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gfbplcfck.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gbyaptpxq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.zdbjq.cn/Article/details/gvheqymfl.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.hesvh.cn/Article/details/gjvsjpfcz.sHtML

[E04] 查找子串位置
来源：http://www.blog.hesvh.cn/Article/details/ggosdbwjn.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gmxpgewdt.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fehbvm.com/Article/details/gkkqpispd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.hesvh.cn/Article/details/gdiflcbby.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gtudbsjce.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gwuadywqe.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.hesvh.cn/Article/details/gtdbfexgl.sHtML

Ruby: s.index("x")
来源：http://wap.fehbvm.com/Article/details/gnjmngknt.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gghszrjex.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.zdbjq.cn/Article/details/gvtwowjhq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fehbvm.com/Article/details/gplrqearb.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.zdbjq.cn/Article/details/gowrsrwsv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/grfspwkif.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.hesvh.cn/Article/details/gappvbksf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gqbjcbgvq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.hesvh.cn/Article/details/gqaasmxzj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fehbvm.com/Article/details/gplvmcyhw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/ggnvvdofk.sHtML

[E06] 替换子串
来源：http://wap.hesvh.cn/Article/details/gjfdsfldl.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gmthsrtre.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.fehbvm.com/Article/details/ggmbvloyz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gdcpbjcnj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/grjmndmyk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/glevlwsnl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gzuoxcbep.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/guzenjued.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.hesvh.cn/Article/details/gvulzlucb.sHtML

[E07] 按分隔符拆分
来源：http://www.share.hesvh.cn/Article/details/gogmdfyls.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fehbvm.com/Article/details/grhyohbiu.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.zdbjq.cn/Article/details/gkywwmrma.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.zdbjq.cn/Article/details/ggkecsomt.sHtML

TS:   s.split(",")
来源：http://www.blog.fehbvm.com/Article/details/gyesujavh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fehbvm.com/Article/details/gyruoeazu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fehbvm.com/Article/details/gsjkpvdar.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fehbvm.com/Article/details/gcixpnurk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.hesvh.cn/Article/details/gwtkjyqcd.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fehbvm.com/Article/details/guyfwiyiz.sHtML

Py:   ",".join(items)
来源：http://m.share.fehbvm.com/Article/details/gelvcbdtd.sHtML

PHP:  implode(",", $items);
来源：http://3g.zdbjq.cn/Article/details/guzvefanc.sHtML

JS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gcikfpoid.sHtML

TS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/grjzjedef.sHtML

Java: String.join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gmaozwbzy.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fehbvm.com/Article/details/gjzohdulo.sHtML

Ruby: items.join(",")
来源：http://3g.hesvh.cn/Article/details/gkelrxzzk.sHtML

C#:   string.Join(",", items)
来源：http://wap.fehbvm.com/Article/details/givdaejgz.sHtML

[E09] 去除所有空白字符
来源：http://wap.hesvh.cn/Article/details/gbxrwzwnv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.zdbjq.cn/Article/details/gurqquehh.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gydhdbfis.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gxurpftfh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gnvkcbodl.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gdxwrqdvj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fehbvm.com/Article/details/gehjyhsoj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.zdbjq.cn/Article/details/ggttwerae.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gcjawhuvt.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.zdbjq.cn/Article/details/guuakalyv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.hesvh.cn/Article/details/gfiqxtmhs.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.hesvh.cn/Article/details/gbnnjfhjy.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/ghxosqans.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gvpqeojzp.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gpolyqtaa.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gnatfmfxh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gayryajwq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.hesvh.cn/Article/details/gaasfhofv.sHtML

[E11] 反转字符串
来源：http://wap.fehbvm.com/Article/details/gzcknxksv.sHtML

Py:   s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gugaqippf.sHtML

PHP:  strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gdzfesijm.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/graxsylnd.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gxeygybdx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/gpjvsqlrn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gzfrityvp.sHtML

Ruby: s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/glnciodxy.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/goeazuqsj.sHtML

[E12] 统计某字符出现次数
来源：http://blog.zdbjq.cn/Article/details/gpoirallc.sHtML

Py:   s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gowmprsbj.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.zdbjq.cn/Article/details/gfipmxrja.sHtML

JS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gwzreydon.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gpsjmvcyh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fehbvm.com/Article/details/ghmnejsaw.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fehbvm.com/Article/details/gbdbstwac.sHtML

Ruby: s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gpewrafah.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.hesvh.cn/Article/details/gvaarirxt.sHtML

[E13] 逐字符遍历
来源：http://read.share.hesvh.cn/Article/details/gjkpxketx.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fehbvm.com/Article/details/gffcyemyl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.zdbjq.cn/Article/details/guethdrxj.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gynumrnzz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gkbihkllc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/glphstvqy.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.fehbvm.com/Article/details/gmqkuiwwr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.hesvh.cn/Article/details/gxqcnxdld.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/ggkqkqtzi.sHtML

[E14] URL 编码与 Base64
来源：http://blog.fehbvm.com/Article/details/gvchnwyum.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fehbvm.com/Article/details/gamsndepm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gahyssexm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.zdbjq.cn/Article/details/gmwlekmjf.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.zdbjq.cn/Article/details/guzranhlj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fehbvm.com/Article/details/gkxzdtldc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.hesvh.cn/Article/details/gcccytpvz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.hesvh.cn/Article/details/gkejxjfuh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gyfeqgrxn.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.hesvh.cn/Article/details/gfvqqepms.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.zdbjq.cn/Article/details/gpadttzzo.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.zdbjq.cn/Article/details/geifbvbbc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.zdbjq.cn/Article/details/gkaildhgf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.hesvh.cn/Article/details/gwdggfgwo.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.hesvh.cn/Article/details/gbdqtgvip.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fehbvm.com/Article/details/gauqxximb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fehbvm.com/Article/details/gypuayfkp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fehbvm.com/Article/details/gbehlqbjr.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/gmekzyjkn.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fehbvm.com/Article/details/goexjmcup.sHtML

PHP:  number_format(1234567);
来源：http://wap.fehbvm.com/Article/details/gvkzwbrcb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gowdfblka.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gkzrtklho.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gnncdlzfr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.zdbjq.cn/Article/details/grykahrpd.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.hesvh.cn/Article/details/gkxfsxwqi.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fehbvm.com/Article/details/gxisujhmh.sHtML

[E17] 首字母大写
来源：http://m.share.fehbvm.com/Article/details/gnhxdpahj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.hesvh.cn/Article/details/gxutvycah.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fehbvm.com/Article/details/geaseovzv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gjxltsjkb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gxyuvnsqs.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fehbvm.com/Article/details/gfaiirexi.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.hesvh.cn/Article/details/gwxwhyawn.sHtML

Ruby: s.capitalize
来源：http://blog.fehbvm.com/Article/details/gfqmrvevs.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.zdbjq.cn/Article/details/gkgsyyere.sHtML

[E18] 模板占位符替换
来源：http://m.share.fehbvm.com/Article/details/gkqmsbwid.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/ggfwntcwp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.zdbjq.cn/Article/details/gsdmjfxrv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gmojoeuln.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gqjagmpkm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.hesvh.cn/Article/details/giovabrmt.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gssryqrhb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fehbvm.com/Article/details/ggcgodzvh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.zdbjq.cn/Article/details/goowuqijo.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.zdbjq.cn/Article/details/galorbdqr.sHtML

Py:   s.splitlines()
来源：http://www.share.zdbjq.cn/Article/details/gdxqkanfc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gocfaiysb.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/grtymngun.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gqdsgeulx.sHtML

Java: s.lines().toList()
来源：http://blog.zdbjq.cn/Article/details/gcraxzidm.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.zdbjq.cn/Article/details/gddgvoryk.sHtML

Ruby: s.lines
来源：http://3g.zdbjq.cn/Article/details/gyrxmkfac.sHtML

C#:   s.Split('\n')
来源：http://read.share.fehbvm.com/Article/details/gkpowetku.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/gtrbqmeei.sHtML

Py:   if not s:
来源：http://3g.fehbvm.com/Article/details/gcbvwfupr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.hesvh.cn/Article/details/gkfnffehe.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.zdbjq.cn/Article/details/gcqarokcd.sHtML

TS:   if (s === "") {}
来源：http://wap.zdbjq.cn/Article/details/gdabygdva.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkaserrdk.sHtML

Go:   if s == "" {}
来源：http://www.share.zdbjq.cn/Article/details/gcgdixpmq.sHtML

Ruby: if s.empty?
来源：http://blog.fehbvm.com/Article/details/gvumccspo.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.hesvh.cn/Article/details/gcfinjoij.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fehbvm.com/Article/details/ggpzyswxo.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fehbvm.com/Article/details/gloknicyn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gfohqxhqy.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gexxjrnsy.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gzzjlcbzd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gaepaimgv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.zdbjq.cn/Article/details/gsywyzjui.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gjhmjsmns.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gyktgnuer.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.zdbjq.cn/Article/details/gkbbvokmg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.hesvh.cn/Article/details/gthoojhcv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gixbljree.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gztxknfzk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/glrdunnxx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.zdbjq.cn/Article/details/giqtdgqmb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.hesvh.cn/Article/details/gvtcefcfj.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gepiorgvx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.hesvh.cn/Article/details/gsyfnudln.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbdfwkdqr.sHtML

F. 文件与目录
来源：http://www.m.share.hesvh.cn/Article/details/gnqnjzczj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gahftdypn.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fehbvm.com/Article/details/gtdahxyrb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.hesvh.cn/Article/details/gwicofuam.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.hesvh.cn/Article/details/grypvkidx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.zdbjq.cn/Article/details/gtwrjatss.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gslrwmopo.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gvpybzzie.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fehbvm.com/Article/details/gfgemlmxv.sHtML

Ruby: File.read("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gkcbqelle.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.hesvh.cn/Article/details/gelaormvr.sHtML

[F02] 逐行读取文件
来源：http://www.blog.hesvh.cn/Article/details/gnjkqmojz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.zdbjq.cn/Article/details/gaeqcrmgu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fehbvm.com/Article/details/gsstmnezd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gpajvlqmc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gmfjzvwuu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gsovdbfeo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.zdbjq.cn/Article/details/gllepyzib.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.hesvh.cn/Article/details/guwhlermo.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.hesvh.cn/Article/details/gitgajikd.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.zdbjq.cn/Article/details/gwpmyleqt.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.hesvh.cn/Article/details/gdbmtyviu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gkbqvhhpb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/ghyxxckgk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gpbczqgwm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.zdbjq.cn/Article/details/geltownjj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fehbvm.com/Article/details/gafolmodl.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.hesvh.cn/Article/details/gilvqkshj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gfwdosecf.sHtML

[F04] 追加写入文件
来源：http://read.share.hesvh.cn/Article/details/grdpawvvo.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.hesvh.cn/Article/details/gaofmmdec.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.hesvh.cn/Article/details/gdmlnwfkg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gyveydysy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gdqebrabw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.zdbjq.cn/Article/details/gfnuuvwte.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gksqbjhwq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.zdbjq.cn/Article/details/gyxcwwarx.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.zdbjq.cn/Article/details/gcrijaobf.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.zdbjq.cn/Article/details/gdzkivckp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fehbvm.com/Article/details/gixspujbx.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gdjbtdexc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/guhxxnfjt.sHtML


<!-- 参考信息 -->