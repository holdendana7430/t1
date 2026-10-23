代发 wailian999

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3oclyyhcu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3bdflhiqs.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3ddgcpvav.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ienyyrmr.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3ynqecgql.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3zkqvgpre.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yjnduzpq.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kadgyzjb.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3veysqbcy.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gzyxfvem.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iszrctil.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3ddabjtto.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wwbfovvi.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3lxrmzhws.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3dkqhtwrz.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3uwowszzq.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wdwcyybp.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ogcahfxc.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3jopwtvrv.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3kggokbij.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3bkyvgbog.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3aqtodfij.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3gepojgqm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3xpjomdvy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fnbreoxw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3zyueeclt.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3mabibmnv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3ezhgpmoh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3irudrkjs.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3ihervroa.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3vgvawxlg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3mytmrbjl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3qnjnynzw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3jarziztv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3xejqafjp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3gtfudjip.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3tvlxerws.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3izhpqxpm.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3rtwqjnxr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3rvheynfh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3egwbwivl.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jkfgpyyc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3mplrrgan.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3shxjafrf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3sytxyszb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3oazxuxet.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3irqfegru.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3itokljve.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lnxgrtih.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3rpwlxzjf.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3rewvkdsx.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ycfzvqco.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3lkfdufqj.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3lvjdoljh.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rtfvbxdd.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3balowxhi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yzgxbgvb.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3zycvhyqz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ztcrraqb.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3settssvu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3akvesshf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lijwpzfc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pwtxvvzx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3fibxvebh.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3vxqfuprv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3oaiqelag.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3ampsujsi.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yaqclyvb.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3pscebdhx.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3dnegaarx.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3uvxiaxtb.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qrbljdux.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tfbzcjvb.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gyxtqoof.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3peaighzp.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3obmbnxae.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3lhvezuse.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3jasuxfbd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3fjftfizs.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3dvmvfdae.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ldythpfy.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3godvsgzl.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3wrmxwvkd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3qkdfiujy.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3xztdlopq.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3nmsreczy.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3oiiurjho.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3pfxetoac.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3plxsfbte.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3woxqlvch.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ynkqhybq.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dzvordgp.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3odvjfpqp.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dgttrzlj.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3nfrfbjmn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3hjvxaxhm.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3zatmzjit.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3lpsmwvpb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3tiqbqlhg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3oiuzavas.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3aorznnjz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3pwodjvil.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3euekhgoh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3bdkcybve.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3gbbwbnui.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uydbuvfl.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3orpcdjth.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zghoiztn.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gstdpisn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3uuzpchyx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3jgvfyldi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zaxudwlp.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tprgbpqy.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3hojfwhog.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3lowceqjx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3bnlfqfgt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3rrzxoiux.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ztdegfax.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3sitdpogx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3ljojywxs.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3brrvjhbg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3uslrbjyb.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3xzlfhorp.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3tqdvpizl.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3ndhnhnvo.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vcmuzhla.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3hjkjymex.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3rhcteqir.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3eipxdzbu.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vgzqafls.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ctvrdxko.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3zasyipse.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3jnttbcvr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lyyyfoix.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xdcifbib.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3hfdmjvhc.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3erzxaquo.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3zuwefemq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ibinrahm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3zmaetjmy.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3hscsnias.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3gvgzskqk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3fvbmngdm.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kogzkljo.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ekbitumz.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3owhavokb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3nswshqex.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3cpbidxms.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3bnfufzxv.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3jitkgazc.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3iimvpulc.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3affrcjmg.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ovnyvixc.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ceiitypk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wuapuufi.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3sbkencyg.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3zliobvkk.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3engcmhsc.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3jjzijxnd.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3nillckxo.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3gguqsvuh.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3glmrfgqu.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3grswdfhk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3sckezxmz.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3nwlwhghg.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3lmllpaho.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3pivbwvpf.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3izgnpnil.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3exzkiqgo.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3ryamqwkr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3chdefjgo.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3emrjgije.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3sseotaif.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3syarzxcu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3huvmsgvt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xyuuspds.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3jyfvavpa.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3bxwpuxty.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3syllljvu.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3qvhhhhjk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3jqhevnti.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3oyvdjxrw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3piwyxawv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3xbwhoyrp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3uihyupun.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3xnuxupnj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oagihozr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tblxdrpo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zobiiapp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wmagnujv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3nmjinkog.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pieprynj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3altfmnzq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3odlgojth.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3fmoqyesl.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3bduuuspk.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3vnwvgvwk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3rpmljpht.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3hjbtilsr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3athhsfzg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3nppjjfzk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3psutqbnx.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3onkelkmt.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3tikubead.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3wijmrtnr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3chxijduy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3wpduwlsn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3bsicnnxj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3rxzdahnk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3tsmyfoks.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3znebhztj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3upsmhyiu.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3nbrlxaje.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3parfxwmm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3pbaemjjq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fdbywnjq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vkjtqcdn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3yoxjbalo.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3nknbdush.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3fgemdaau.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3hrldejpb.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3kovhwxii.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3zipwwmgw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3vyxcsarh.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3mfmpxqej.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3qzbvdyvb.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3iwcqztgo.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3ylmcqdhb.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3vthccfak.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3ezrniroo.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3ybcvjbez.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3auxxmygc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3oqqcdxms.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3bmmriyuh.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3oscohcmz.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bverodmq.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3abgfymqw.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3zilffupf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3borxjsiu.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3sbdjzczs.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3ikamxorq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3eiuqfvgf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wljnligm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mhaqzwxe.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cyqhsqia.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3yqsmmvle.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hicukuib.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mlmuhdzt.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3tzachdqx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3esvoefwj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3fecozetg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3haeyrite.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3hwtvvnzk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3qhnamfxx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3diullrsw.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3oiyktfyz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3jnomiwzi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iejynfdb.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3vzwriecu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qfxzeywr.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3tauvdbea.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3wagcvjor.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3toiqcuga.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3qyasmktl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3dqntucwa.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3mmnqfsgn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3kkqscoxp.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ezwtfyge.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3akbhxddj.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3kujldirf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3eansbklg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3xmcixlea.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lzbxipgv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cysalsvf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3hszluwlo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3zmqhymmc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3zeutxryd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3pqohmyxv.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3xahbtslv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3khcctlte.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3urmgsndq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3enjwltkr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3jdmqftfy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3axnhyvdr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3sjmtruga.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3cvyhqktj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3tozscqko.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3xorgqfer.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3sppaysqw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3irmjorem.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3oavscaex.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ixpogcir.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3lacneuav.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3bglhqdqe.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3oanbowor.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3uxtexshp.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3lsvojpbf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3sfxatjpx.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3eobdimzz.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sgcsetyg.html


<!-- 参考信息 -->