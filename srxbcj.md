代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3dvodogoj.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3vvncusxr.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ebpsypsr.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ggpnqcyn.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zsimvjvy.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3spgfeisr.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3melalsti.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3pfpynomk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3wtoeaegs.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3fkxifbtm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jckbnock.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3ybubvnxm.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3waethsyl.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3szztvkos.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3qcfbgsnp.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xvicxlfa.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3jflctrqe.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3ixwacihp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3iykdxqvg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3sbstlgfh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3dogkrwen.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3mhbgtqct.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ysuhazwq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3jkjdnqok.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3migffdhc.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3iobsxbmt.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3bazdrhpn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3dlrwyzhl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3xswzhfba.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bjvcognp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3dkzhtqjh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3mfomteuz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3tndcemim.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3utnzcapi.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3rxjtaldy.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3vcbqnodz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3dpmymzxg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3hlsmregs.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3xvirnonz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3cgirdhaj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3hjtxwmnb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3sdmvvxay.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zzqgyjoh.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3kmofjlxr.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ecigxmnl.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3cfburfcu.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3vwuxvwlw.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3unoxmjrx.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3gdnmxvmo.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zegamhso.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3cqvoctav.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3mdebdbyj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3svkqncyb.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3ogtakmev.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cxicsvxr.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3usergnpc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3aqygoonj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3rwpawres.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3rvneilub.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3vahqvuya.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3nikhlcav.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3jcjyoyej.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3aghotzun.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gziqdrmk.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3ocovedcr.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3jodzqwge.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rnjdwrqz.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pxhjauki.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xzlmzgmg.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3vwzxswbo.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hbswtijh.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3jfbroesu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3qoeauiqw.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3avxxgaxg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3qnwlccqg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3mupqzfxp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3vpwfvajl.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ecrsgicx.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3tcffklsr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3xopmiyge.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3rutxgkzr.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3mwqmvfaf.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3yhepqgwq.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3fdpngtgy.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3peieegsu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3iycpivkz.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3nbgsmqew.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3orkqjwub.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3snlwudsv.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3isiiksnn.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3uwkdqyrb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3jyxlzcms.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3dmxuonkm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3thfkyryy.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jdvidyki.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3tpysxyzy.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3yfqxsvqz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3lozwfcbn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3udcaqtrw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3cgvicqwu.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3brxwauvb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3xhbarkic.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vskolpfb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vltuomok.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gvnzidwd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jguttwus.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mdtbiimu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tfnaxdex.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3btggdylu.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3aqppfgpx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3qrylslkd.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gqpfgksx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3smgcvqqj.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zimdmnjg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3luipwzbp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3jjdpnude.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3ufiwpwrq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3bkmyctch.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3aumdgqjo.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3omwckvsw.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3ntxmvkxt.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kcwmampx.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3oqvkbarm.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3eadtltql.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3fjaymnvd.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3nbetdnzu.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3hllamcst.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3zwxowntq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3syqezzjl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3udqwxziv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ykxuobgj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3lxzraxzo.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3vrekexgm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3gzxwbnyw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3odehmikf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3uydkpazj.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3usrdbmuw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3gsssebcz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3jbbeqsrr.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3qdfptabv.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3yavcpuzj.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3aaeiemvc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3xifxvgkp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3sonfimgt.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3qglqijen.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zfxrqufx.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3bsugecyx.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3hdvfeivz.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3emxuxnmu.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3axskbhki.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3yaivhxwy.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3nweqbbvj.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3hvabvlff.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3vqinyitm.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3vzrxpvbk.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3axjjqryt.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3izyganfi.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3drqdvwpt.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3xatdpxtx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3akjgwfca.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3chlbjqph.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3odjpkbah.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3uaspgmny.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3dupjxong.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3opwhuzfd.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3ywtfbcrr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xqtfruyp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3uipcnnia.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3kxamolzs.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ykgdhosj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3rwhuvkjt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3kspvisgo.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3jgonaubg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3viorfjpw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3wccfutaw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3tvmruqtd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jlrrtqzg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3fexsymqj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3tevvsxax.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3zhpiutjp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3kizsveod.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3xmkyotal.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3qiirccjs.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3guwlfrrv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3zxikohxy.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3soypveki.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3obeywefw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iisqdspm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3zuwlitut.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tjxldmrn.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3zedmrmbe.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3vpybyxfo.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3qxxxzaau.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ohsfqldr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3xsqgrkxo.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3uwhreqha.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3hacspmtc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3zorlbqas.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3nvtbgfpg.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3clkoehwy.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3hmclbruw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ydhemnow.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3legdtkdm.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nylsxrmx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vahvbauf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3ipldawhd.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3tdxqitfn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3xkmcrqkq.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3ewozvelv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3vdoznppz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3yljdyvnw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3prxobecg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3wnixnslg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ghzxalfq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3bnmnthrn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3mrjzeovk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3dutijnny.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3edcdnurf.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3mojsdspr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fdunqaaj.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3dnaagvfb.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3yzufldbv.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3updprzgs.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3virvncew.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3iwtvwjww.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3qxjdftdw.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3xatuzrrs.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3bepssxhh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3abgvycbo.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3xjtloaug.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3lpmmzxgj.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3bscrpyfu.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3ztcrzihu.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3fzgsvbei.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3jeqyykxj.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3laedizdz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3rbtvuqgx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3nxpnmciz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wghrvmsp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rxewazls.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nlxrwxce.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3wlsgxewu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3cgylaiol.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3icqwcuet.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3fyfgfeto.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vfheqpxh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hctmkguq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3elgywium.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3hquhrdup.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3qrfmyiji.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3vtuzkidy.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jdenuqpu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3cohntvtd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uvqmjqeq.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3pyimpayh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uuqsoygh.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3jnpjqkmp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3uydifnah.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mgbqmkum.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3qxtlfeez.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3axrbblcw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3sjsforfl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3qjfkpoxw.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vahswflg.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fbhokxmo.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3umnoccge.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3eerriwje.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3ancmkejp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yqrlppkv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3nmbmjwsp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3djuxmept.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3xsytqtcp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3vdlfcblw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3kotgjagw.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3unhiyvet.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3iuphuyqo.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3tiwtewhx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3baqpofth.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3obcawipj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3fabcckmv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3jaxqhwyd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hnlyykaa.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3hooktqtu.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3gjglbpzu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3lkahcgbd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3wfyiiamo.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jqifjvwg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3iycvoaeu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3dvumbzuk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ycrkgozf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3vbixtooj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3fhuqgode.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3mvbvyjyu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3vvibzwqy.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rsftijhm.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3doudvszp.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yjghcoyu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zkisbuag.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3clnivluh.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3khtcealc.html


<!-- 参考信息 -->