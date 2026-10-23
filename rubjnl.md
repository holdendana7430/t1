代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3jrkkkljk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3macrndpc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3vlbowrax.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3qvdkgksq.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3sgticcrh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3dhndotgm.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3hrpnbqpg.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3qtmlkerh.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3fggztlec.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oyjdpqfi.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xcwqgcgn.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zndytent.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wevmxsre.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gpbkdqvh.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ursxocnq.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3icobajgk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3pfitdbca.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3axxjygbn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uenrplwc.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3oxvtagfx.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3byaurzwf.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3iguhwdtm.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3ljtseykn.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3mjjtdbow.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3yczvttwc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3dpdbugji.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vcruieje.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3azhtalcn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3drleojhe.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3nppxnauu.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3nuompfce.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3ujkfgurm.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3pluxgfxp.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3zgilpagq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3qdbazsku.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3oklzfuyz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jzkszvrj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xqywqjjy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3zqoioldg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3cnuzwwou.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3iyifyppf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3zvbraxte.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3xehwinoo.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3lnuogygt.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3hpujcczg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3tejiueff.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3heascirg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3atghmndq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3gbfqxjjp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3utfingtc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3whhcaomc.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3doahpqzd.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zqxtbpda.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3rynlgtqm.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3amzxpthh.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xzakuszn.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3xxqlyagx.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3gplndqgm.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ujisfzgd.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3npofzpjm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xlfpofao.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3cxbivajr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wrnybwsl.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xzmicmqw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3lbhaohlv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3vweaunkm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3atdgbmmd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3isbkozpn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3wwsflfvs.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3nucwtuan.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3nmedskfz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xwmmssqy.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3bitbxbuo.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3tdnrktqr.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3awdgiaci.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3zhlstmgs.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3azdtyuwk.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3oieqqydn.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3xbwjccqk.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3tbojlgvw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3zdctiyob.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3qsuqojmj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3jznmnmva.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3dxbsuxza.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3inpsqmiv.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vtqlpojg.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3hsumffit.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3tkfzdddz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3pbnsvdoi.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3iepyfywv.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3gmtdxyzw.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bpeiuuua.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3aakvdpir.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3lczwwhas.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3fxuintvc.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ccxbdoch.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3xmsbecrg.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3nnsivqep.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3gmlodtdd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3qweezwat.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3fkbmmkyi.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3wmekxyzt.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3yfdfeoqp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3txxtckbi.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3netffxsk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3tqtoxvlj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3scdycyda.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3saohxblf.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3wdqrooyj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3bphxfmqn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3pupqeoco.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jwxeucsc.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wqyvzsxh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tgbjpbyt.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tpvquwnr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pmjiziph.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3iicalbvb.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3uxzngxfy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3mkwnlogv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rmnqbhbm.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3dndytexw.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tvcdlucd.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3tvbuyhwc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3neefyeer.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3yuoqdqpr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3hlzzugdb.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3xsjzykih.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3sikaqlkm.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3hccbzqia.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ibmfirqh.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3yzeuwqat.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3plvfiuut.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3bvctosii.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3nitzwxht.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3kcfvddyc.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3zvoxczco.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3nqynmpkw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3rwzonxsw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3nwbgzyph.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3bsdsreay.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3nupheenj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3ogdurbau.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3qawoohik.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3nlzmbjuu.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3ebozcfse.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3nsestrti.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3ysclsdbl.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3wzochysw.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dswdsgxa.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3fzspllie.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xyqfhcvt.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3fahkqxfc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3wtqyqorm.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3qabnjegl.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3xsornkfv.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3jhtyehsc.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3xolyvbqg.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rmwortif.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3gcbumazk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ieydergs.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3xlutbniy.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3iqusoxfi.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3uiilfiiu.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3rnjrwzvu.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3swbxytph.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3rykbjhqc.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3snkvatvj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3demwxreh.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3adnujexp.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3gkyuiriu.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3nnoxuola.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gievakhf.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3zcezpako.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3upvbmxtx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3irizazbq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fdpwublt.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3kilfnlyt.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3lfdbckrj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3okqszzxw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3yzyxwmrb.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3kapjibqg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3vqdfzshe.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3vroxyuyx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3wjhurgde.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3msrvddug.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3rkreugbe.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3bczljmkh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3wufrnvoe.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3vypavgrt.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3jfqdsjoo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3vkjwmzyl.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3giiocrwa.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3xtspgmob.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3werjzvwj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3uzhhayfi.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3wnnaexwq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3zsnuxpwa.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3enfdyezt.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3wwivnchl.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3hyaeffdt.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3bqcyejbt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3uooblbfc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3rymmrwiu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3zxgyljui.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3gdurgjjv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3bqnldnpd.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3surizdgr.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3dlifqjxz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3najehfns.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3lmknggcz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3epqoozbz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ifmcuagi.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3litvcpbl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3tmzhjsyz.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3pcavhuzb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3mfiopuau.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3auqhwijd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3zyoiwhwh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3ypktxuyx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qlqamqgi.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3blcvhbxb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3pvfspaca.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3yuwzfyhw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3mnlbazqt.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3qgwlflwz.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ashthxlc.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3upjcqtmy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3splanchj.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3bnozjkxv.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ttxngeew.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dyebowcv.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3tdccqaiq.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3mcqrfnbs.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3vcyfulrj.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3nsiiveal.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3gjowxcwv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3uydxzdcx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3aoibmecp.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3mgerwdqz.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3washagps.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3zoxyoiia.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3cpojqgpe.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qiveugun.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3zigcgors.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3brrzvmhv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3pnbayuoy.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wqgxddgu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3stybwnxi.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3djyfbfft.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3jctnjexw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3heesxcuv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jvqufttl.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3wkzfsrmn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pcffvvms.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wqxyuzdo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pyqrclsy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3hxlvhptp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3kekvxvul.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3bvyswqzj.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3nhyldvmm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3opsnykzm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3geizndjw.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3lgrnjopb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fiqqgekh.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3zhjechkj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3abpwpevw.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bnfizjqw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3qdncxgpw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ksazdtah.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3oulidccz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3nycwemke.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3intazepx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3plsuqqql.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3ysnjxddg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3xopyozpc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3jfevfdsu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3matnocpu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3bexyatxn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3qsejsbro.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3ouxtnfeu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3qawtuqqo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3dywulihf.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3ewtlvkyc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3lvvivsmb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3nmqalgut.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3mbkypsnm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3aexnechd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3wucgwuxe.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3docuozkm.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3qwhqivlx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ypxecayo.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3dwtwwtyo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3limxactv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3uktqcwmy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ytaeufsd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3zvyfrgef.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3aanuaevl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3exhwglgm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3rhswvobj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3kjxlfwgz.html


<!-- 参考信息 -->