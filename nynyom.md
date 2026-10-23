代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3blnmhaak.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3bnysfunb.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3vozdwzsb.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cnmwquyk.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3askqsygp.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3eiciyiiz.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vgachlqt.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3oufpcyjd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yricqhal.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3vlcselmo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3urfgwkxr.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3fuvfshtw.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ognckevy.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3feqffxum.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3wclzeduu.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3ardnypxb.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3clbilrca.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3javfjhff.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3bdfibvxo.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3uizrxrab.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hvmcjcqk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3vqhhgote.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ilywibcv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3dwvckwod.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3ykwhcyos.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3cvsobeow.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3jclryfru.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3sagewjpu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3npfdzbip.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ertqbayw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3mxuxdxur.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3jtdbqrde.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3mtujynex.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3fjxrdrxn.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3tompbked.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3zgikqpgy.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ipmslccv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jfqfcofz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3xwlcbvqo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bxnbasgx.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3kjnrvrwz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3syirqdib.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sfcsynqv.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nzyzwroe.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3tnmvjvbc.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ulrwcdob.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bmcrjbye.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3tlbufjpr.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3nchsfxmb.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3jvgbzqzx.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3uvjrzijh.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ezvjkvys.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hdymjaek.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3zcfuudjh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wncbhslb.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uapyyztc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3iecaxgnt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3tvigdhau.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3slsjqoxp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vtkvhxlb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3pumxwuwx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3yolqdpmi.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3hozqwykr.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3taxitlvt.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dpmzbguw.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3awpuhxnj.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3osptszwa.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3xbqeaogj.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3hllpyyyk.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3thrkrtqa.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3eqncjjnj.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3rhbpswpe.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3lubuhple.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3uyftcfzj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3tdayldke.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xvggitfg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xrvbsblg.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3govigigz.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3nhkajlfc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3wqmfglal.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3qjzomyjj.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3hgsgkdrx.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3krrdkqsz.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3eqcslwtk.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3cghflzqg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3ardpwqqe.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3vfjrqrfy.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zbabrkhb.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3cztbskzi.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3cpdadamp.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3owmobtqv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3fukgmxry.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3frdcmgmw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3ndpqgqbl.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3efjbpuhi.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3esrqhmra.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3bornenuj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3rdyspyuh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3dxlzshtj.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3khvssmkd.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3mzxarwfp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zuysjyyv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3madscyae.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cgoccqmb.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kyqkzynf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mtnijwya.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xqxkwlba.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3sknsxrsd.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3damsuvzr.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3elyciddp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3llfcvmih.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3lnbucmxn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3iaprtekq.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3eclsrfdd.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3zueqtozd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ovjubysm.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3phqrykrm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3whqhwgyh.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3tpboekxi.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3eekxnbru.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3jwfrvhtp.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ldbtjfko.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qkphmcqm.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3voxlmnpo.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3nsqyttjs.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3vdohwrlq.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3mbdsmhmo.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3ciiwvjmj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3eoruxjqq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xjahwcrf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ghvfihuv.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3mjzkrekv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3xjwxvlmz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3yrxadtwr.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ufaffhqf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3bqqlugqg.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3twtkxwoq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3wxbfumqy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3cpzjodmx.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3wbldsnel.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3pbgfsnqa.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3nkyooonc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3tzfuwsvd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3xsmtwfhd.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ydritaqh.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3omnhutpw.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3sihvrqyf.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ihdoxnjo.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qcssmdhm.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3rgziljyl.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3dggveexs.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ptdgnsiq.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3pymhegxb.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3xgzjpnzw.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3kiayybpq.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3etrlgemp.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3eoeninre.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3wvpwyekh.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3bvieiryn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3ywpiuzqc.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3jsgiyiek.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3zsnjohiy.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3mbtbqeug.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3heivhcxw.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3awppntvm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3nnebpzgt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3mwqfgkys.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3nppvfblp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3cbqpflip.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3xnppfhju.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3pxmyxyub.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nkyadgep.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3cdxmpbem.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3nmxqbdql.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wuytbbmm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3jhqibnqe.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3tljgwhgo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lltposhp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3ogbgjwrl.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3cijbaiyq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3embyqwqa.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3ycomplyj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3zchuwhku.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3rkzdtjky.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lzrnhbur.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3yrvbdmcu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3pvsaxlcc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3zaqgqxwt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3ffvfihtc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3pkasdtjp.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3sdcwrmfl.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3bphjjryv.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3prnwhezl.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3inpbamfm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3uputelme.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3anpyakqy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3sppptakd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ctaattbb.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3dijbviys.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3btjypxle.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3uatizjlf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3epkgntuv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zfnsxrll.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lanhlfrr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3rnupciyv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3vyrzdqpp.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3cqsdxqzf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3xzruvndr.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3ojbozasy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3csvgouge.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3mdrbxidk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3diuhcnss.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jusjtokh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3mwdbnnmv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hikqirmf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3tcltyhjz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3wcshjtwr.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3tzenyrmx.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3dsniwzxl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ycswuiqf.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3shbigaqd.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3alcndhoo.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3byfpzerc.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3fsijtwfs.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3vyudezcu.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3jekfwbhq.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3ulvmwmtg.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3gqgxtvro.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3uamezgen.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3dbsxvmxz.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3slkwlunx.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3cykiuxyt.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3wutzsuhb.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3bkuhvcez.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3unqzgbtg.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3viomrxrf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3gavyutvi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3urhvpsmz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ncpgifmd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3awbirpmq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ihslbpkx.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3ilfnzbue.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vsmigsig.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dpopvnnq.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3eoupmljz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3danfdiut.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3nfbxztfp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3rbsnlgro.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3desgfimx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3tfzgxcav.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3suoapfkc.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3zogpaazj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3mbmocpqx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gwawmgjr.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3euobpctk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kypdhyxh.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ldinfetc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3umzisutl.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ouqpnvcs.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3cyjscufo.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3hgyfvpag.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xvozeomj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3uqvtqens.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vqenpcoa.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rykgggkd.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3lfhrmvna.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3jpivxxno.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3iauodmvs.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xixjsqxh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gicvobqp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3lmqfiyfx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3uyanvzlu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3ghbcbbpg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3nkojjmrc.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3rqxumgcl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3wrjqququ.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3qryvtewh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3uhhqsuhj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3guqfxbdx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3amyalazq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3uugupims.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vexgmyyn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3fjhhxhtj.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3jqwetwzn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3eysxipdk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3ghbymxop.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3tugaeipb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3eoululrz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3amvadrtz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3lkyaiggz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3qjhmacwr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3rqenxphl.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3mohpinkg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3aaoflbyg.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fxnkkupc.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3olalucbr.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3glfwpatt.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3sgustnlw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3ricoexze.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wzinfnjc.html


<!-- 参考信息 -->