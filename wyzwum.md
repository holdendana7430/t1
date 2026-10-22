代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2dtnsicwy.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zrdnouxb.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wdstbrkl.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2afzvaqko.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2keyjwbra.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yjatyupi.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jtlgsnti.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2mjdajymt.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2yxsriofj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2hquyzeno.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vxfodcvj.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2yvwvpnyt.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2bwkyvfcz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2svgvioca.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2jhcbcyqp.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2uorfhbfk.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2huilzspe.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ogioycqe.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2mkovtlzb.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2atxzbirf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mzxamrgn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2fxfyxwrp.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2kmgloipp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2swldkvzf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2etjryemr.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2xetdpemr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2nopmceyb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2utxygdcn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gcdktkux.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2evrmuwbt.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2zaqbfabz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2pvcujfwy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2mtrgasna.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2cgypzqjw.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2pjuxbqlp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2qurwooui.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2crgvouue.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qhneszrw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2vrchtxuv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2qlplxjpr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2sthkydaj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ggbsxjcf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2isovopsf.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lizfdawq.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2fghlilnr.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2zdomcneu.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2koitwbjc.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2wyroxgzu.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2peviromj.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2qkolozte.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xxrjgsfz.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ecjnrdqj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2neqphffb.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2nqvlfgso.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wtqtqziv.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2cuvvtivz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2yuolzywf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2trygyxux.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2pozrlkqq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2uabjbgkt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2fwlvwjnf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ewpkfenp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2wekxecdy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2sfybqmcj.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tdjobnxh.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2awesokau.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2phbhljbz.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2dapsnsct.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jqvdfgnd.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2uscbqkvm.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2acisemnp.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2oebfpouy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2defhjqyb.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2lqmbtuom.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2uqjuzkmm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2dgjncejt.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2jzrybduu.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2bgmwkqvs.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ucwhddns.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2zkfuttqq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2tnwclzkx.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tynhesdz.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2mdosrrqn.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2hnelbkes.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2ampimlpc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2fydnxdqj.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tcwdjwbx.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2vilotjes.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2ownpilfx.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2sdakwcai.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ujmhjxkv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2uugftuxr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bsjznene.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2watwxgbd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ajicybwr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2nvocazpg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nsjoqahw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2oawolben.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2jnpldktr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ygsnxoqc.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2becygskc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2xqdmbuwz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2ruosskmj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jxjjzidq.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yocscnck.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hoaahzqq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2peajotbe.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xgflyyxq.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mwwzpvzc.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2yigrruqm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2cuxqakau.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2lhuawdkr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2aipbxwty.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2diguatpm.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2vqdumbtg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jopttbdc.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2rfdfpjcv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2utqcchxy.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2mmgaetga.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2gkoprcah.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2fdfozyqy.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2crlypcao.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2lanjdmlw.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ewlwzfbg.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2tpvbqdpf.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ruihxesu.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2zbythlnf.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2lhwcvjob.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2bfjbzgup.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2kdjfugvs.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ulnramdv.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ohrxdvhu.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2vqzmngaw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2bkbplbuq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2xnmtqisg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2svvrbfvg.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2gmcebggx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zgbkxgpw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2tavdotvl.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2fezikpob.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2dzjhfkjm.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2hybszphn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2rbldpqsu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2oucelkpw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2ywtbpnds.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bjrcdhio.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ozlrzfbg.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pbeajnix.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lbvqhduz.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nkqyiffg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2kmdlksex.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2yqoeuttp.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2zjrjqhag.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2hnjsuqqe.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2rixdnvao.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2evxqvzak.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2kutgzdte.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2xsllqurr.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2rkgqwptb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2hcxirvhs.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2xtfllugr.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2eaqpcejj.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2nikjntqx.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2jfpgxqla.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2slylbisi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2jzvevmuv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2nfuitvpz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2oewklrsq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rfopivdn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dnvyvpum.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2uxxcofhp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vxclghht.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2dnsjnhor.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2vbumsbhc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2qxvsmrjz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2klczniqo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2dkbfnoyp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2posljzoe.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2rlpkeazi.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2hslvcowx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2gptazmvh.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2rtqxvwbl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ekmdsihs.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qsxnisbf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2susvaxtw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qvncubys.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2fdhppgfs.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bcxpqzps.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pceladfx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2hfpqoifc.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2nywzqels.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2udstqiud.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2hjcxzjqo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2klajnsyx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2mjonopiq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2qikixzmo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2guyyrwdo.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2aveivagi.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2uztzcjgs.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2ivezhtjq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2rhafwyzc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qbmzhgmu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2uyzjejvp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2edxojdhi.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2qxwixsxo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2bdcpurls.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2zbwwwvfg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2yvwqtrgl.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2tgcnqymu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2teobbonc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2peukkftp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gmomciot.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mhtzsrno.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2esdrqdaq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2sgjxllgx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2atddyuta.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2kwhssnge.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2pxrgvsrf.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2qutlohlp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2geojdhne.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2cnyjmgfl.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2curwykcn.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2rmowhlje.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vnafebzp.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2qqlsxawy.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2yfzsyayc.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2tdcjmdsh.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2wwopavog.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2jyypdprs.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lninawvn.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2gbkhnezk.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bitdsnvo.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2kaxlcsoz.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2gxpaaqix.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2hryqrbpk.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2kgvmswga.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2ofnhhysg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2sppseubq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jefaxegl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2idbufwol.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mnwsicdc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2rqofqhho.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2fzekihpo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2psuizudp.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2ocbsbhzq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2swdztdbi.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2owjftshi.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lxbttzhc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2agqxbqjp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2rajiremd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2phzmczlk.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2anatvjrq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2aimzbmno.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2umylggqa.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2uitoqsqo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lsffambc.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2htlbrrmh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2xawizbhn.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hthyllwc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2zifkacdk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2npyonjfa.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2nhjexnrr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2ketbqmyd.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vbmacnoo.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ywmzucrd.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2escjcjqk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2cthrjfng.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2kwkstpca.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2djoqzgyj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2hvdpesxk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ffvbpkpj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2jqxcljjb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2daafevwn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2fijvpsuj.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2swqcuhlu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2yrbejnqg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xoaurmvt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2acnghiew.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2xnmenlxb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2kfbkoqaw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2wztcphgj.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2rndiesfb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2vvajrqwz.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2cosbynjr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vbthkmtx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2xjheospe.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cttavcuc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wtdqfgng.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2bogrshwf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2fcmjyxsr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2bfkzzmip.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2asoiupmh.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2uqflazvr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2dhuingvp.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mmnntvho.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tlgmitoh.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oisdnyav.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2nttsmlkh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2tjdjzdoj.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vnilfxho.html


<!-- 参考信息 -->