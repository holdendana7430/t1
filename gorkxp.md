代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ygkswxms.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2smmrtanh.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mldfuaoj.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kfnbhizi.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2azbeuibc.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2vjhustmd.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sdykgnjz.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2rcdepuap.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2ubaznkmn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2piqaacyn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2jmhjehfr.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2uslcivkm.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qmfidubr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2pnqjxyyl.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2efqvhepk.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2abkdcvds.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2pmidimxl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jdhkctle.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wgydydcs.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zidjjzpz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tybbhjaa.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2tnxzdyrz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2mnrouicn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2eignhfrl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2cbynizok.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2bqiertdj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ceahtbkr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2vpjbkeas.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2enjlvxft.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wrwjbdao.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2oruczdtr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2eqjeetqr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2aespqhbx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2fjqnxuzv.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2nnrcfroc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2ookypyyn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2hxsmcpsv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rhkegiir.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2jrtmeljx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dkcvezdp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2quvdsbfm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2hkaewqli.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nlsgpcga.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2utgoffry.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xwdsmmra.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rttttuoq.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xrkofaxh.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2uptocqyo.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2mdhdhoxs.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2tjiazmsg.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2fjrasepr.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ezwspxwd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rnxostbj.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2lgftxnnu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uwtvnwoa.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mzetuzzl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2bsnckvoc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hwhrhvxh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ehudijfs.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2thyotjvh.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2chcattnp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2vgzzgfaj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2pyysntix.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dqzfvmlz.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2izgpjhht.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2dhiyvbba.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2trcogjkl.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2uqpzvvcy.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2enzzatau.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zhtbjkrd.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2ikisitce.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2cazwbxjz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2phrgfngg.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2qieucvqr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2jcrspuep.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2orltbvlo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ppftvwli.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2liwfvhcw.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2yosykebi.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ocaczsgy.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2vhpzaxnr.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2kqcytuun.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2sdetcyvk.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2zadwvieo.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2uoefyegs.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2kbpbktqu.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2mksbslbk.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wsjfllyc.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2qroeaizg.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ttjizqzj.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2byoatqiv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2kxilwwmz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dgxqrwlc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2fyhvazbm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ikajwero.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2svmxxmpo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hwslxfta.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2drmjetgq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zmlnxgjs.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2cuijsunv.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2eqxqeayi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xftcaoii.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2lybrtdut.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zhnqrosh.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pqmdodra.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ewccmfpd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2brcrxnhu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dpetjxti.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bxcoqwex.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2yxmcvdhf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2teylszks.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2pbdpnmeo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2kjemwpbh.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2cwnavrym.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2yzerbbvr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2vdnqbqpb.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2ulpufgsm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2gejdxzoj.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2glrcgfqh.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2ewbefypp.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2vgssprdo.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2kvqsmjls.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2truldgay.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2sbhdizgr.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2bgontxir.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2aptgvcgh.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ltnmkflc.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2amyfcmth.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2yjxyeveh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jdsbkzin.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2pmvahrks.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2kifrpgfa.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2mlaohpip.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2rbicluxe.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2okqvttwq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2dpuvldjf.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2yhdfwdli.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2mzlqahco.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2cclxclqd.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2omcyrwfg.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2rupsdhwg.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2svtgbetv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2qreftqoh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2aefgvzso.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2pwrqyoks.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2cwccmigg.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2azikblny.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2bvohelvl.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2kmfoydew.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wmttrzwv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2zcqwomzo.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2bjzjygtd.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jwkqjlvv.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2wnbqatlb.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2nvmuogcq.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ecvnkglv.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2ssojdbms.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2jhotphye.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2pphsvhag.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2mlwalaez.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2flubnhfp.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2nrstfzmm.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2zdjpymek.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2iaimrjvh.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2nimdakro.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2oooqpkfk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zkechppg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2crnhcxps.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2dndhgflm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2wgdhkulg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2ziamkeij.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jvareius.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2kfxrfcsz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2ytvjmkns.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2prbzyhke.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2bjqohckx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pyjlrtpo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2nkcqrbgk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2ikaqnbxu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2kkqiqosp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2sdbkvgek.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2avlhhmhh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2dtszohrz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ruoyymqi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2gggczvsr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2pfvqclca.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2hsdrqmar.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2bvdhfyid.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2llgfffff.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2itfpufgj.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2iigybjcs.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2uzishssf.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2grmgzidg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2mofedkzc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2wrpbpvzt.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2eeeacnrr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2lbocdeyk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2qvvrvxax.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2gixsadmr.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2hknbcqst.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2gvhqtqnz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gvpbmljt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kgoasimh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2bspzewnr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2eegggrmb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2hprexjva.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2gkfzbyxn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2yxjrwhpp.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2mzvnlcdk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2bvarlmhx.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2fgxnunas.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2sxxahwsi.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qhmoekrz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qjxocvhv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ddhbwubl.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2qwazirfg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2rztlabsd.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2nyccmttg.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2gvtujcip.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kobisvsi.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ugwdmyhg.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2xnwppwxo.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mgxiyzyl.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jgimaxxp.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2kwvzpqlj.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2xiyesgfu.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2zmcemcyo.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2xpfpafir.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2vdpttifa.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sczbednt.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2pzwtrrwd.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2jkispcqw.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2jcpclmsf.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2cwhnyikq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zgetuuvf.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2evfkdyyc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2fujiokbj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2sitgljty.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xwelcgxf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2yhignntl.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nflcuiwi.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2veqxrrkz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gerznfcb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ycxylhjo.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2soiwkyso.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jlqlefeo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ghrnxfed.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2kpidcprc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2iqtnotlt.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2foaueast.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2lluxwryh.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2smmbikjj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2arswsapx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jkvtzrbs.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2aglmlirs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ykrkjnzo.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2kzlmhlsb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2xfwmdruj.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zcxezqqf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2vvhehmbt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2hrckiqkm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2gikoertt.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2ytryrsay.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ihqwuzou.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2aszmquhp.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2jbaoewls.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2oelolciw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2urpfgqtz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2kgulrjgw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jtghzlfu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2qofcwkqw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2fjykcjni.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2kplifixo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2paeipwik.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2jmommhwc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2kmwxqlim.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2opgzwwpd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2jlemktkt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2deqkeghe.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2gfqrdfsl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2awlkthwx.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2viwupyrn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2mhhqfjyh.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2xsvquefn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2avsmnkjn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2easycfft.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ipznsgtk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2epiheeyt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2dksahqtp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2clvknsqt.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2nmmqoxrt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2owbhxslx.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2cdsvpoug.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2zpadgmsv.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tayyeewg.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vgzfnpaf.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zzjsektw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vckljydt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2nweovqyl.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jnzyybxl.html


<!-- 参考信息 -->