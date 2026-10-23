代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3lpkroruk.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3dqtebhij.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3zvklkaaw.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3pmvscpcs.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cdxreenh.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kcvuvqyc.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3btcjiauq.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3dolupbkj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3xxelpdpi.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3vailoztg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3upvtawef.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3nststthf.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3oiaqicqc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3xwadmlkf.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3fxdxivdj.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3pbxcjkwe.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3iwphjksj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3mcthddos.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zoitvqyc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3qoozocxf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3lzcnfskr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3trwbwfsq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3eqokdvsn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3etbrxzey.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3mbltykwo.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3knmzwuek.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3qaydkdzr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qaujltyb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pikkcxqe.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3lntugbnh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3atximfhr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3eoixncki.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3tlzyhnyy.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3yhvhnyhu.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3mjbbbrnc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3vxifbmic.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3etenzltp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3rdncewtq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3nlauivyp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xyvrotqk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3atancekr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3szeeljfg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fvbycbzf.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ghpylddz.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3vqxuscgn.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hpamrdqi.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3assxcivp.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3bkjadqgp.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3elvkugtd.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3gvjcohsm.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rpymjmyj.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3bckskpji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kjddctfv.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3nvzrtclf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3myzapmmj.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3aqkuskal.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3zdnzqpqp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dwjefqjc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3iusamhjk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3bxytnwhc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3lqckenob.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3mxivjtvm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3iuttbckf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ysnrthcc.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3ydcexyll.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3xyzjiblz.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3zsglecsr.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3xhmvzkid.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3bimshlbj.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wtynsmll.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ycrczkds.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3vymbjouf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3eeupzwou.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3fecioioy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3zafbdnyi.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3dqpiqdbo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ufowghnm.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ncrjjucx.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xbkbrckv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3amccbtof.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3guypyetj.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gaojhqkl.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3bnarmaal.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ukzjcjou.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3jzovqscd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3shjanfbm.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dlhpqrpa.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3axsxnfbc.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3htzxvhea.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3sxbiznqn.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3pilobpzq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3bmtqypul.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qkivkcym.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3fdlfxjgo.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ggluuwls.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3nganzblv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3dtfikpuv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3jckdoimj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3ivhzawzl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ceyhbjsq.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3ewujzyzp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3foxljbfe.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3srinvkie.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3idvnsjgy.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3sdlihcsf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bqjovhed.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3anhqsudm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fyjajwab.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dryekhtu.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3khcuficc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3djixxudo.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3nohvrfkl.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3higmetdz.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3ghoqbvhw.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3srchvtjh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3iefjdnlk.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3hlcwbojo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3zbvnhmma.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3zzzacnut.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3wpllgydg.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3uowtenhb.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3adncxspc.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3swxtyjow.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3tlmavbwj.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3hgwejgvj.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3pjcwarcu.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3yfzssxga.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3biomxzeo.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3jnolhpnr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3euvzwboq.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3glpklkqu.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3jcvpcqbt.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3vfszpczv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3olxzefsj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3gbgclqmh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3cjdjgali.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3odyqoctp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3efhqpins.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3meenrsfy.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3wktwofay.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3hivuxffd.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xcumjqsh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ekdzcemm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3juvfbkzy.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3gtkgivgh.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cvplzdac.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3dpxcfwzc.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bkdvxpvc.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ownanjsr.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uibejhpf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jonevwtt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3eqihzikv.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qxbusyju.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ijabvcua.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3rjjqfqah.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3nasftqvp.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3elmsjiun.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3noqbdmre.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3turepnmb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3dteuxmfn.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3vujuxsmu.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3guhxdqgu.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3lnddytmj.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gpmoheja.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3gvtzxhsi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3buuduusi.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3uzndnthw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zqplagpc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3tfeuqdri.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lvvogloy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3tdlkehff.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3kgvobysz.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3hohqsksc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3fsmkpuej.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3lailxcnq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3eerxbwuh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rpsxijlc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3solfaeyx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3adyayqex.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3ydelwbrx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3dlkyxufu.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3udfmkugd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rbbwedls.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3yynnelot.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sbwbuyec.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3zumemema.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3zhvvsueb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nrvgywxn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3fjdzzvio.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ilrsigex.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3oohjryxl.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3cfntxesf.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3kkfobttx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3wpfrwcab.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3cvfjvrhg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ptftgwtm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3cfafdnrg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3zixqjibf.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3qrghnxya.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3jztwfzge.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3anaafjea.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3itbxfbma.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3phipxeka.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qbadsviy.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iqqijqob.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3rwjemago.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3krbfauyj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3qbpvuhzk.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3kusqnukj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3sfknbghp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3iunkistd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3kdrqtbnj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xipanrvp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3pzrfctuo.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3dbvddcfj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3sqmnffmw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3kerblpya.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3glqgqqvf.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3isktdezx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3eivhonan.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3qfscjmas.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3paxmxguu.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3tramadil.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gsilsgby.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3fnbyezpz.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3pfictubx.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3dkafxzxf.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3cnzllrev.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3bsoxjbzd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3bnjddtlz.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3plmnitdf.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3elsdiizs.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3uicgjvum.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3jfsouaab.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3tsfmnzpi.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3gtmtrlyu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3ehuedzty.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3gdroyvbs.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xgcwzsdq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dtnjxcvb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ahqrwnic.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3fnzmggde.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nslogvte.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3lupeysxc.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3jehiwxgr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3quyxreei.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3afkvbcjr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3busyufrx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3wxgpbwje.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3pclfiyxj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3aubjpviw.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3lronmsaj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ujgtaako.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mbwpaqhw.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3vlherxdh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3judqnkub.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3dujiuovt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3feqdahty.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cmswktpl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3jeudiyyc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3xkpgknkz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xaehcafe.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3cgtyjpqv.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qdmabxuf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gijdlktc.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3ibyukvsn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3cxikkhqi.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3lsypoajl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ggjamwku.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3rdpoyawc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3jeaouxon.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3orzamrgr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3rzcbluwq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3xlcwbhbq.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3bpqfbnfw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3mzfebmtx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3kesixkqt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3nmqkazvt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3pecjmldg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3ttjscpou.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3pmtxtdaf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ipzhyhiu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3lejwhwlo.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3xqvcvmks.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3gdkmljrr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3yztlobfs.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3dsgzoiep.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qcuanymn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3rhxbpbdy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3rrkdpkia.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3pgfefahj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3qixgxozc.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3rquiggwl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3txnzdtnr.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jthvlkof.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xcolpetj.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3udhkxmdw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3chhpazvf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3gotpkdxf.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aevrkzyr.html


<!-- 参考信息 -->