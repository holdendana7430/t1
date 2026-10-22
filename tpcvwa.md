代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2siqoljhz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2bkjlpnwc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2qbeideml.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2oieqkztc.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2bvymavda.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2mvihuwlb.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2utkdorvi.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2ehxgutfi.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2afjjyjes.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2moiieuda.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qrqjntbb.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lthdizii.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2aixjlavt.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2cniaamyb.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2npmippzh.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2qtcwyaab.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2nskqfqbd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2qrbmlwrd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lcwtgmho.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2krubodsj.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ydfeljat.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2zkhxvxmd.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2ypeufphh.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xvgitjcn.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2cqdkdfuw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gmxozxwb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ruqwivkt.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ulnqoxhs.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cjjubojt.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2qyqlggcs.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2wmcvfuls.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2hnijhjge.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2ylzebktv.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2eilfrulc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2aebtdinr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2effhslhr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2clxmwptw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qhrxrouv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2abgywanu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2mremidcy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2kicfmloe.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2incmlxda.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2qdynzend.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2urwipvox.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2nrybheil.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2neewbfph.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2kmcwpjbs.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ahhhrxay.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2jtcuvdze.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2bmikdkua.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zgqdqkau.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2iqdvczyw.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2afuimlnf.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ghevpjpo.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2kcnqoyez.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2fljsvktg.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2nfbfrzbc.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2izvdymqy.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2inunlzvo.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2wwwadstk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kidbtiru.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2ozilgeff.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ztdvjque.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2xyxoqsfn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2hbffjfdj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2vvbxsjsw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uuntefzo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ilpzalma.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2xbpfnfgt.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2akkngjjp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2lxkmrmer.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fjaobufk.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2elpeaoeg.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ctlzqpho.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2zfobcmtd.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2prtxmias.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2gvbdibdz.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ebfvxbfk.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2vbkyvmxo.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ekcwaefq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2bmlwictg.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ylxfuhqa.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2mnthnehh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ozlgsdjv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2xtfvgfvg.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bfvlfapb.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2cvcldyqi.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2imlmaqaz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2lahoqvuv.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2bqfoyubd.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2bvwgfkqp.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2xybufbym.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2yyuopllp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2fdialsyf.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2myeeixjk.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2aaebbsuj.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2emszjhqk.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ttbvbszx.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2sefzwfmp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2bqitpvgz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2mmdjeeqo.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2ugspwefj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nbobfykd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2ikameolt.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xxlwewzd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2oohdserk.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2yjxhpgkh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2lidjargv.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2hliordtk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2hiiqxrdy.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2oczfjzfy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2irhfqtmb.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mxsrusvl.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2veebhoku.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2zryfhtez.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nsuatcid.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rfrvmtqi.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2rkmyirip.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2yflgmdvz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2twdybyqi.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2nmhmkuba.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2pzxuilgs.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2wqjonqda.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2czphwkao.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2ksiohncp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2lbyuxibr.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2pyyuerdv.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2lgqccznr.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2xnlkslyu.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2asqeaxuv.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2hnfuatcz.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2eetetbql.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2bxeynpcc.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bqwimicn.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2dvfxcevb.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2trzqhrsv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2osvdcbzc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2owprsxvv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2igenhfpt.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2zehdvbba.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2pssuojrk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2aweuzdxi.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2zvcankny.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ghawwtfu.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2mmcqlveh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2salfqscl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2bycwzsre.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2byzyjboh.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2irceowir.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2yfanvtds.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2tsqsrmlm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2jrtdtbcz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2tjdpmxcb.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2izscuyor.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ewvihfrm.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2yrulwxsy.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2joljbumd.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2whwsohng.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2tkztmupq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2vlbxfsox.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ruufwtvu.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2sbrhvifl.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2ypcfmkug.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hshesxmz.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2vlkzvrfo.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2nniplrgq.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ovbytcid.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2ibfbeosz.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2btwztdqx.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2wqquhbmc.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2ircvjlxg.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2seglyrdt.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2ltjrtwej.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2omzzqxwr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2okboybpd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2itttnedj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2llqywjye.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bxamfmgb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2ebzhwfgt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vxvunwuf.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2eroabmwo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2njljcgws.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2xjkwhdkt.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2qlrxulhy.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2zjexnekg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2srcvwhqc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2cmgxvjwd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2vxecpnbj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2tjndygze.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2tpglbrsv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2ppujwknv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qhfbshdc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2smjsjgvd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2lxewqqyv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2ctmuqiwi.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2tenomlzv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pxyvfsvc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2ovavejwl.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ucgxvzbt.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2xrzbaaba.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2bkusarkr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2erorulsb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2talysjdb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ekfihqcw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2fpmmhkgs.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2rudgxpau.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2ltoirysc.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2pctnroby.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2eldtropr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2nodpuotn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wyyqsnhu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2engbaapg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2gpjkeboi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2eahbvjjj.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2fwpoumek.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2qbskmaiq.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2lsjslmcb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2nyoofgxr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2hfqvmtpg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mbuukkjv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2rphbghej.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2asxubpdp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jjuqazhw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2uyfsgoea.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2mpftkmav.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2irzppmhk.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2ruhyckes.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2iceeounf.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2dsuoaagd.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2xdxnjgwz.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2txdhlusk.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tetqwtok.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2hejqxtri.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2jwfelztz.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2lulorham.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2ahdrdckg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2llloeavw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2zsvssyzy.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2jlmztqym.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gmpfnvfn.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2sowtambb.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2hwxtrwsl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2oilhrqeb.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2gzspqzoa.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2amwxfbtf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2zgzktwmf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2iaqdwpoz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wbzohxfe.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ccyxsnzh.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2qkmbmasl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ijiqaoyw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2byvhngvm.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2qcqudlza.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gmiuzsjx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2dsqeutre.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pspwyafr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2lndtuutv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2oybaxcxa.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2prhzbuhy.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2rjhukatd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2pqxvbvav.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sjodtqoq.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2epbryoud.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rfzbzpon.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2fifmmsfa.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2yxomslqs.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lfhnizbk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2lhukhgmp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2zrsujzvu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2nzdscbzo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2cvcvjqhy.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2evtcndyw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qfkowsrj.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2zwkhblev.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2acywrkrb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2uhbjekvw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xqmnigbx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2pmtyehbs.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2wlchcfup.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2fcoagxmr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2dyiubfiq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2aehknfeb.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2yojpbafy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2kkwqdeny.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2caqvuuoj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2gffkgivz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2kmavbuvq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2ilabmqfv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2hwqadqnr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2gabjkuuk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2upjauiaz.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2glezvqag.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ddwgejca.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2zqqibieq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lnfcpusd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ysxxuhtc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2bnegmtfg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2qgmujegl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2wfbnrtto.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2dvotzllh.html


<!-- 参考信息 -->