代发 wailian999

Ruby: arr.tally
来源：http://read.share.zdbjq.cn/Article/details/glsixrhsq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.hesvh.cn/Article/details/gxfhnovni.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fehbvm.com/Article/details/gfonlekdo.sHtML

Py:   x in arr
来源：http://blog.zdbjq.cn/Article/details/gfuptsqsm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fehbvm.com/Article/details/gnkeghwvn.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gqzliuirc.sHtML

TS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gxkzuraox.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/gbgevxthl.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.zdbjq.cn/Article/details/girvjujnt.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gpwwqjldv.sHtML

C#:   list.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/gvheqyxok.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fehbvm.com/Article/details/gzcockeba.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.hesvh.cn/Article/details/gbctehtgs.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.zdbjq.cn/Article/details/gadinmxrv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fehbvm.com/Article/details/gqjdmrogv.sHtML

TS:   [...arr];
来源：http://wap.hesvh.cn/Article/details/gwwglqcbx.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fehbvm.com/Article/details/gjdpcwlhs.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.hesvh.cn/Article/details/gemjjqpau.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fehbvm.com/Article/details/gipvbsxuq.sHtML

C#:   new List<int>(list);
来源：http://read.share.fehbvm.com/Article/details/gzzwsbwen.sHtML

[D23] reduce 累积计算
来源：http://mobile.hesvh.cn/Article/details/glxcuynsn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.hesvh.cn/Article/details/guaymxofm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.zdbjq.cn/Article/details/gqkdcuozw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/glfzmdzfj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/goryadjpj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.zdbjq.cn/Article/details/gszstzzii.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/ghwneudci.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.hesvh.cn/Article/details/gmyywvhug.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.hesvh.cn/Article/details/ghsmgsavn.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.zdbjq.cn/Article/details/gpvrzotoh.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fehbvm.com/Article/details/gsbmctzqk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.hesvh.cn/Article/details/gfksuswhe.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.hesvh.cn/Article/details/gomhjnqgr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gereyvcid.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.zdbjq.cn/Article/details/guhkkcbgf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fehbvm.com/Article/details/gfdhseuhr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fehbvm.com/Article/details/gzyyipahd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/gakebdubr.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.hesvh.cn/Article/details/gqfjhdyam.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fehbvm.com/Article/details/gjvqfdijn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.hesvh.cn/Article/details/gsnszbatb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.zdbjq.cn/Article/details/gayhyxilc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.hesvh.cn/Article/details/gadqongir.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.fehbvm.com/Article/details/gltuwqgsg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.zdbjq.cn/Article/details/gtgsgkwqp.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.hesvh.cn/Article/details/gxzmquujx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.hesvh.cn/Article/details/gonysvwsf.sHtML

[D26] 数组转字符串
来源：http://mobile.hesvh.cn/Article/details/gmoivoyma.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.fehbvm.com/Article/details/gtogynboy.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.hesvh.cn/Article/details/gpbogyuyl.sHtML

JS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/grpvrejoi.sHtML

TS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gsmvkzmmp.sHtML

Java: String.join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gkjxvbuhc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.zdbjq.cn/Article/details/gicptixcr.sHtML

Ruby: arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gpvzdclft.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gtdakcyhd.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfojxqntn.sHtML

E. 字符串处理
来源：http://3g.hesvh.cn/Article/details/gkwesizhd.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjprvcfai.sHtML

[E01] 拼接字符串
来源：http://3g.hesvh.cn/Article/details/gmcpwhnpn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.zdbjq.cn/Article/details/gfeqcbbax.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/gotjiojux.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/ghnkavgjr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/ghfvqhcsv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.hesvh.cn/Article/details/gpipvppou.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.zdbjq.cn/Article/details/goteufbpc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.hesvh.cn/Article/details/gheelqtfr.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gitajzerh.sHtML

[E02] 重复字符串
来源：http://3g.hesvh.cn/Article/details/gfvywaezt.sHtML

Py:   "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gbzakhzlt.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.zdbjq.cn/Article/details/gglnedrxd.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gqdssgbhz.sHtML

TS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gtalatkgc.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gfsdqhbhh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fehbvm.com/Article/details/gdpeovxxm.sHtML

Ruby: "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gwonvbmtp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.zdbjq.cn/Article/details/gbiksjerr.sHtML

[E03] 截取子串
来源：http://wap.fehbvm.com/Article/details/gjuyljzfy.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.zdbjq.cn/Article/details/gltbtzumq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gqynrciwt.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/gjneuvciw.sHtML

TS:   s.slice(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gemrgtfvn.sHtML

Java: s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gvovqnibs.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/gmrpgbhsh.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.hesvh.cn/Article/details/gcvsmlvya.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.hesvh.cn/Article/details/gvoslvnpc.sHtML

[E04] 查找子串位置
来源：http://www.share.hesvh.cn/Article/details/geahiqyqt.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gshopgebu.sHtML

PHP:  strpos($s, "x");
来源：http://3g.fehbvm.com/Article/details/geivxagpt.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.hesvh.cn/Article/details/gkasjoxsx.sHtML

TS:   s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gsrxllxgk.sHtML

Java: s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gvhjmidjc.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.zdbjq.cn/Article/details/gkujbmnfp.sHtML

Ruby: s.index("x")
来源：http://wap.fehbvm.com/Article/details/gmilfuryv.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gstffrkrl.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.hesvh.cn/Article/details/gwgqvfzok.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.hesvh.cn/Article/details/gkhodnifv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.fehbvm.com/Article/details/ghhxyssxc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gfzrqpigj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.zdbjq.cn/Article/details/gzytbgwvh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gofpdvfiz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fehbvm.com/Article/details/gcmybnjrh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fehbvm.com/Article/details/geyhvzfro.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gmafvhyer.sHtML

[E06] 替换子串
来源：http://www.blog.hesvh.cn/Article/details/gasvoslea.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gtsvorvnk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.fehbvm.com/Article/details/guxifdipq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/geqfbxnqy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/golhyvmys.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/glcgovrnx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/grahcwitv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gowcxkusk.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.hesvh.cn/Article/details/grxaholic.sHtML

[E07] 按分隔符拆分
来源：http://www.share.zdbjq.cn/Article/details/gpvjarzyw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.hesvh.cn/Article/details/gdleotrvj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.fehbvm.com/Article/details/gvzvdongd.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fehbvm.com/Article/details/gxjorkjnt.sHtML

TS:   s.split(",")
来源：http://read.share.fehbvm.com/Article/details/gjttccdho.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.hesvh.cn/Article/details/gvldvmttt.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.hesvh.cn/Article/details/gkdgbgnfe.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.hesvh.cn/Article/details/glhwwuppt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.hesvh.cn/Article/details/gzvifycgw.sHtML

[E08] 数组按分隔符合并
来源：http://3g.hesvh.cn/Article/details/gjnwdezxs.sHtML

Py:   ",".join(items)
来源：http://m.share.hesvh.cn/Article/details/gdmlhsdvh.sHtML

PHP:  implode(",", $items);
来源：http://baike.zdbjq.cn/Article/details/gqczgsdjw.sHtML

JS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gmmlishyb.sHtML

TS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gxhktvgjx.sHtML

Java: String.join(",", items)
来源：http://baike.hesvh.cn/Article/details/gdxhqfwuz.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.hesvh.cn/Article/details/gfkuferwm.sHtML

Ruby: items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/ghmkgnlrr.sHtML

C#:   string.Join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gvvozfyry.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.zdbjq.cn/Article/details/grioriehl.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fehbvm.com/Article/details/geoeavbdp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.hesvh.cn/Article/details/grklltdna.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gkkeftblk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gspesmkyu.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.hesvh.cn/Article/details/gqhedljyu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.hesvh.cn/Article/details/gymxqylsq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.hesvh.cn/Article/details/gfrlyxqcg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gdwhzcqly.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.hesvh.cn/Article/details/giwtnvdgj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.zdbjq.cn/Article/details/glejdjpjz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.zdbjq.cn/Article/details/gwohtzkmo.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gntirfnhp.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gfxklkcwq.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/guptntanl.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/grsyjlcio.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gntjgkzeq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/ghvedoxhh.sHtML

[E11] 反转字符串
来源：http://blog.hesvh.cn/Article/details/grjhpgmex.sHtML

Py:   s[::-1]
来源：http://baike.fehbvm.com/Article/details/gzmdmhkiz.sHtML

PHP:  strrev($s);
来源：http://wap.hesvh.cn/Article/details/gyrotscqr.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gzmrsikhr.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gkjfuyzhd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.hesvh.cn/Article/details/gemrdonfi.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.hesvh.cn/Article/details/gzuqtrixm.sHtML

Ruby: s.reverse
来源：http://baike.zdbjq.cn/Article/details/gqcbnbqzk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gzmotaxct.sHtML

[E12] 统计某字符出现次数
来源：http://3g.hesvh.cn/Article/details/gzkqvwzna.sHtML

Py:   s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gvbvpkajp.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.zdbjq.cn/Article/details/gisqpbuok.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gcidxddfq.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gokiffend.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.hesvh.cn/Article/details/gsfgfhmxc.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fehbvm.com/Article/details/gsztoqtod.sHtML

Ruby: s.count("a")
来源：http://3g.hesvh.cn/Article/details/gfmbylhey.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fehbvm.com/Article/details/gvlplonjt.sHtML

[E13] 逐字符遍历
来源：http://blog.zdbjq.cn/Article/details/guzaikgds.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.hesvh.cn/Article/details/gxpypbzkr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fehbvm.com/Article/details/gergputtp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gyhtrwdqm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gwchmtmjv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gmuaixbca.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.zdbjq.cn/Article/details/gidqmfmcz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.hesvh.cn/Article/details/gheltiooh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gqjnerqda.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.fehbvm.com/Article/details/gcslznthe.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.hesvh.cn/Article/details/gceywrita.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.zdbjq.cn/Article/details/gdjptwuqc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fehbvm.com/Article/details/gwufdlfvb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.zdbjq.cn/Article/details/gnhndjtby.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.zdbjq.cn/Article/details/gksaadoff.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.fehbvm.com/Article/details/gcywsjyrf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.hesvh.cn/Article/details/gkiloxyxz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.zdbjq.cn/Article/details/ggyjggqzm.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.hesvh.cn/Article/details/gcckxigun.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.hesvh.cn/Article/details/gxuamrdju.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fehbvm.com/Article/details/gjswequdv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fehbvm.com/Article/details/gxnsxmjpg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.hesvh.cn/Article/details/gwhnoffzm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.zdbjq.cn/Article/details/gxuoeoyda.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gpbljkbeq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.hesvh.cn/Article/details/giakfampw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.zdbjq.cn/Article/details/gdsexyfzc.sHtML

[E16] 数字千分位
来源：http://blog.hesvh.cn/Article/details/gbrorizyf.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.hesvh.cn/Article/details/gubeyxgtd.sHtML

PHP:  number_format(1234567);
来源：http://baike.fehbvm.com/Article/details/gsihhrnbu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gebhzmvgl.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gxofnvryj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.zdbjq.cn/Article/details/gggjuxxuh.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.zdbjq.cn/Article/details/glelnzrde.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.zdbjq.cn/Article/details/gxwiylahf.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.hesvh.cn/Article/details/gtufqzglp.sHtML

[E17] 首字母大写
来源：http://m.share.zdbjq.cn/Article/details/gjwbszqur.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fehbvm.com/Article/details/gkamyslbq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.hesvh.cn/Article/details/gklaweoqn.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gbvnftpiv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gicedgfuw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fehbvm.com/Article/details/gkikwqros.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.hesvh.cn/Article/details/grwaxjvkm.sHtML

Ruby: s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/gqhuuupdt.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.zdbjq.cn/Article/details/gyhskmcdy.sHtML

[E18] 模板占位符替换
来源：http://www.share.zdbjq.cn/Article/details/gvjtxkbsj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.zdbjq.cn/Article/details/gzewssrzp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.hesvh.cn/Article/details/gabmlbphj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/grfqinchc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gqkuwqjac.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gqnupfzvf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.fehbvm.com/Article/details/gkywlmsmn.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.hesvh.cn/Article/details/gqlgvuzqh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.zdbjq.cn/Article/details/gjazdxgzt.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.hesvh.cn/Article/details/grzjvktyu.sHtML

Py:   s.splitlines()
来源：http://baike.fehbvm.com/Article/details/gjyxrndgf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fehbvm.com/Article/details/gaczdfgwo.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gqjovnoeu.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gepejliod.sHtML

Java: s.lines().toList()
来源：http://3g.zdbjq.cn/Article/details/gtcnvrrhc.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.zdbjq.cn/Article/details/gpxwavkdp.sHtML

Ruby: s.lines
来源：http://3g.hesvh.cn/Article/details/gvbebgeuy.sHtML

C#:   s.Split('\n')
来源：http://3g.zdbjq.cn/Article/details/ghxphiiwn.sHtML

[E20] 判断字符串是否为空
来源：http://baike.zdbjq.cn/Article/details/gfcheppvi.sHtML

Py:   if not s:
来源：http://read.share.hesvh.cn/Article/details/giuysdgak.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.hesvh.cn/Article/details/gvyxfmlgp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.hesvh.cn/Article/details/gforuzbjz.sHtML

TS:   if (s === "") {}
来源：http://m.share.zdbjq.cn/Article/details/gastyprtn.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gyabapkzb.sHtML

Go:   if s == "" {}
来源：http://m.share.zdbjq.cn/Article/details/gxyrscedu.sHtML

Ruby: if s.empty?
来源：http://baike.fehbvm.com/Article/details/gphwybctw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fehbvm.com/Article/details/gktcebmfq.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fehbvm.com/Article/details/ghixqwqvb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/gyzfcqtcn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gfqixwfdh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/ghehszayn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gvolmybph.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gbqxovwhd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.hesvh.cn/Article/details/gyomzdwcl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gnttwtird.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gxemvjqru.sHtML

[E22] 字节长度与字符长度
来源：http://baike.zdbjq.cn/Article/details/gqobdjevx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.hesvh.cn/Article/details/ggqrvlxrb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/ghssspnnl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gbgmagzcu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gfqsofrwz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gwzgcxmmh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.hesvh.cn/Article/details/gsjdmzlfd.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fehbvm.com/Article/details/ghpbzautv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.zdbjq.cn/Article/details/ghbytrhxx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gurrsxked.sHtML

F. 文件与目录
来源：http://wap.hesvh.cn/Article/details/gojnsxgie.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gebhilizs.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/gvtsnflli.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fehbvm.com/Article/details/gxehzumfn.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gesncxojj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fehbvm.com/Article/details/gmdlztlmb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/goigkzhol.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gvudfqdvd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.zdbjq.cn/Article/details/gvinwpjko.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fehbvm.com/Article/details/gnfyjrmcm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/grkabiwkv.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.zdbjq.cn/Article/details/gvonhjpys.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.zdbjq.cn/Article/details/gfnhxgytg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.zdbjq.cn/Article/details/gnotmltwh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/ggvmmufup.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gedqfxivi.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gyghmshku.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.hesvh.cn/Article/details/gdklywavj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/gzyzdnyfo.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.hesvh.cn/Article/details/gdruvzkvw.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.hesvh.cn/Article/details/ghbtaosta.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fehbvm.com/Article/details/gptqiivya.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gyylyvjmz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/golzezgte.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gpcsrezdb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.hesvh.cn/Article/details/gomavinwg.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fehbvm.com/Article/details/gpozhqooi.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fehbvm.com/Article/details/gecfnietb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gfvfabzlf.sHtML

[F04] 追加写入文件
来源：http://m.share.fehbvm.com/Article/details/gpwzfccew.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gbsipqprg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.hesvh.cn/Article/details/glmaoeqha.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/guppulfys.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/glokhxxgf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fehbvm.com/Article/details/gtudveykg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gaimvmugw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fehbvm.com/Article/details/gsedteuvx.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fehbvm.com/Article/details/gsxmjxskq.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.zdbjq.cn/Article/details/gzojgqzzi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fehbvm.com/Article/details/gbwlxasou.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gkpehobry.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gnsqffmhj.sHtML


<!-- 参考信息 -->