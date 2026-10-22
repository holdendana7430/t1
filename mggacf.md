代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jnaulmbt.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2fznwjffe.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ucfstfqm.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2zgzqnvgf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2lzuulgtd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2cecwvhut.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mhwcznpp.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2bjfhthoz.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qzssbnrm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2fnqsjvxw.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2jalbewfi.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2zgjzgqme.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2cxswbnkr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nhycqatd.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2lrjlqgwp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xzrmuihl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2wfhazsgm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2outqnzth.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2swptwodl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2zcidrcbt.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2tgtirlrp.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2xzooxymb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2wuonilbs.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jlcwyrov.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2swvqildb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rejgucgl.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2cprpqnev.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2wpadbbbt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2rjkcqnnj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2vntwlzpu.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2bidmhvqi.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2xqubxqfm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2hhhetlei.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2byoojqck.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2ajdlkwpx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2gqmdltqh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2zcwtkmml.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2uzmuootd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2kpvipwqu.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jcjejqva.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2ssbcivwi.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oekzveeu.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2zqfjojko.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xkdtqbtp.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2vxzcbwpa.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2tasztkaw.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ihqzanek.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2krvxeqpm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zgwbusne.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2xqzerzod.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2brwrfrwu.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2mmidlrib.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2goozljiv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2dnoscsft.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2cynrcrkg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ouqjkbdk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2nkfgecah.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2vydaxvkr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2nmkhnlgi.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vufhgbnl.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2fshfwnje.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2dcsgisob.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2fmczpttd.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2asebwiar.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zzjihltd.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dgbkamsr.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2htjunehl.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2vzbnhvqv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2kcrabonb.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2tmetpdyz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2iqqriaxp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2lcwcqdmr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2wwlvjsat.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2cflbamte.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2yxadmwmm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ursxdtfy.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2bznhxikv.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ddvmggor.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2uqrhhmwi.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rgewltdy.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2iidzetwj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2osptigyp.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ffaykjer.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2vloiclkb.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2cgfytwxb.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2cbuzjmta.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mgtrvmgp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2bnvkyvnc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2bgdoipxk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2wcsjxvuh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ohucnosp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2oikkzioy.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2foyrxssx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2smvmqvne.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2prbfmwuo.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ywmswprp.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2ycrwmmbz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kyjeyjlh.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2vrdtjoef.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nzolzdli.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zdqudoav.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2asfepwan.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2spixjchl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2icwrpiqj.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ddyyhrfj.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2ttjbekia.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2grulkhiq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wckofozc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2jwmkuscv.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2ruuxeqwe.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2nemsxdzp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2vefghshm.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2tturantq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2ydhckakm.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2pjledzos.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2stgwzoer.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2jdrlytbr.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fnjmrdap.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2rhysawnk.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2rzknbtoz.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2xwbjwcrn.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2xhisysqm.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2zskklhig.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2myiatexa.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ajifmkhr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2qagqxvpc.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2blxsmloj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2bnpmanop.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2vjmdcenl.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2ywslxuzs.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2iijsgghn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2afwbqrbh.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2gpzofhgq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ovlzwdqw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2nbqhkpzt.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xnwojhpw.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2zaauzyhx.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ccllfzbh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jlislffx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2bgkywjin.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2pwfhioxb.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2wrwwurgd.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2cjktbxwm.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ixjviapw.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ycesixzg.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tuhllzuf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2obgbawzl.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2bdprmect.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2texahuow.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2anzaxjhl.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2uvleqbet.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rofgfebf.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2yzzjqlbt.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2skopylal.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2imemoaje.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2bqusohdz.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2knaijpbe.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2crjtivro.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2xiwflglr.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2unumbuqc.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2zkfnxipd.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2asbcrlem.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2wjyqmbib.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vfifpqvr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2psjllglp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hdfjmavj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2ihqivjok.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2tzahhvbo.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2mrikpmsg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2tnoobkur.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2aphyiygk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2quwypxnk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qzffbtrf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2gvnyrcet.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2nhpiiyej.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2snrveahi.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2whmshrld.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2ozrvdrpd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kuonwnzm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qvmnlbup.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cjchwcmn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2pphcnfmg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2wwopsnsp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bwdqswuh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fqlykowt.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2mdgiaajb.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ldxtmwsq.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2cpnldonq.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2dsbrhtml.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2zmealhhg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2wqdqtlwh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2gwhtyifw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2pnyusxmk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2vawfqqwy.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2iymmaobw.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2ylmxrtzr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2qzrynkgu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2qjzuquyu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ytyapcca.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ibthnxlj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nbtbursx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2njrznoqb.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2zvhebgny.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2agwikyal.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2mzyowvyt.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2wohmouot.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2xikzseny.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2cfbdpsyt.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2kestzcab.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2uevwiswq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jddncbxm.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2ljcuuznf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2brqnhsru.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2hgrtquza.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2ztgviuzz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2cumbqoxq.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ttyzrujo.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2gdtottlo.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ynskbvxn.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2oqibplsu.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2kjlicnne.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2obajmexk.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2sojpslqq.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2wahiblfm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2ywfovqah.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2bnyftfbp.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2qnsdtnhf.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jzgtjohp.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2wvpdgaaw.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2znludlff.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bnrilkhh.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2ygdhhbnp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2muvwdufu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ghshvcmk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xoqnoscn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ibivpzqw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ihzdtxtp.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2qbsbxefm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2otrpbfwz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2aruixads.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2ffraqdbu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uswmacez.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2nufptqoq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2jftbjzhc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tthhypoi.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2rwdxqoxs.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2cwoapbhn.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ikwtjoti.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2rsdsgeao.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hovyztok.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2dahlrqxe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jbxwcdzt.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2wjgiekch.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2bqlwegac.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rvmxajel.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2aarntwta.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ymskoevw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zrjjcodb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2ysgpdehw.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2toxygfit.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2znchygov.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2hzkvblca.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2ouipseyv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2qbjxoybd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2cpnosmya.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uzdnfedd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2mwravubq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2xhmxtkic.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2dfkzwqdx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2rosjlmnr.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2bylocszw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2vvcisfhv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ccwnzzgs.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2drqykazw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2vvuvghjy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2chnrhfig.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2poxnuedd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2msivfacb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2vlnzgyfw.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2lhhmafka.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2wmrukgqt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2fajibhwj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2okhsxswm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jifbbdem.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2dvfzijsr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ghjinxkl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2zlpzcbpl.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2ieaxktdn.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2lhrizxce.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2yuryvpar.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nioxvcxn.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ihtimnlm.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cdbtipws.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qojtzlob.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2wbuuqqcy.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gbpcjcib.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cgjkhuvm.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2mracvqyk.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qvjawfxy.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xjwzmzub.html


<!-- 参考信息 -->