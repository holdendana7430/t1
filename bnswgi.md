代发 wailian999

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2zfbgnzag.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2tuqwtcya.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2pvdpckin.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2yzofearq.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2lgwbkgow.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ssqlkcgt.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2imzcbkzo.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2awhphovw.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bjdjcebt.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2gntygjkx.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2fqznhmhd.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2qexebfqy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2szuaqaaw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2qzgvmtpd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tejosvhx.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2wihytspt.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hfkhkgjn.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2nkjwvuvk.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2zropsnxu.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qvwqhibt.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2gvelmyco.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qlhfqrub.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2bwzksywq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2kiafbrgt.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2kwvkwvme.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2cyysoste.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2mhnaxzdo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2rxjosdcl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2kzcstxse.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2qfithpnz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2hchdcslq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dmehketf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2xkquhmvi.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vwnfyyim.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2fdztbosk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2tfuktecc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2hnrpkpjs.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2wwhpfetu.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2ohrnangc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2ojosbqjt.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2tbrchxxo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2lzebpvgy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2hexfgyvd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2vrxrkgtf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2qcokkzyx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gnygvemh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2gviuwsdc.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qnjzpeai.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2dsrllsat.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dudumenn.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qegkgwrq.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wmbojgzr.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2mbizsjlc.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2wmkibeya.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ybxtgkar.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2gqmcegbn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pibjkyit.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2khophrdu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uxaikqir.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pyafozsn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2zebdhuae.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zvdzujie.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zfygapel.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2bkgelyto.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2qovntmfw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2dkuysvrs.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2oxjgimfe.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cjuwzfix.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dhttobcj.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ngycunzr.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mkkuexwb.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fxdochvl.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zctfxsbo.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2utjegnnm.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2snhmyvuc.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2kccgynev.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2vkevnsgx.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2fxpogkxu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2xwtbrrqi.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2tlvnadgz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2wlydbhao.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2btueygqb.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2mddviakv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2txycublf.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2epqlhghb.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2unjglgzk.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2dqhrphva.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ajzahint.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2itedwtdk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2xxqqblcg.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xtbsssrq.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2udsjpuex.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2zcmdyiwm.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2llcwoklw.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ynwxfxlt.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2jnxywpjt.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2lpvkyfrr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2tqilzzor.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2djqxqrfu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2uoqgtqqf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2pphhnvbx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2tsnwtzcv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2pbwvutrg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2mbmcwpac.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2mdplhzdj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2okjoduct.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lluupzzv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vekknkow.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2herbpinh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ognfpgae.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2iwuppwht.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2boptoaem.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2prqiztjo.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2lsrrsamr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2wtildcsl.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2tebwknxi.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2igkrdlcy.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2mazjztyc.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2jyytgtjf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2qsspllsj.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2wrjymugl.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2mdjpxkqz.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2rxlcughb.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2bywonduu.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2snfcvmms.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2qmbfngfo.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bkvpqszn.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2gdulmknf.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2zitwlhms.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qeblcbsn.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ksejjmoc.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2llnbqxnn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2iehuszqd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gturxzkt.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2hlayrlaw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2kfbtkote.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2jppogrpl.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2bzumihlo.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2mlovjbgd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2tguohfzc.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2oayokxbd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2viuguzew.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2jmhnzgej.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2axpvvzws.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xebzfqvq.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2tastpbcn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2cilxzhoe.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2uukkkwtj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2acujzlmx.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vdsrcmrm.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2jmbanwyu.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2pcnpwlzr.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fjpibsbd.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2shzdkboc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2xjztrrhr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ilvcxyku.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2uialebxc.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2mimqzmku.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2rubnxbeq.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2spfwnida.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2zzvzuzxy.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2lnweptvc.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2hsazdlub.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2czwvksko.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2vmtenftj.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2odaxscan.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2vraogfhz.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2gkarvyes.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2vhbfkuwz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvlpgwig.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ikgmhbyw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2yhnymdvt.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2aybdibko.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2dampmbwu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2bebpcqwf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2gwkmfmxk.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2pxgcoqqa.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2lhorexhn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2vnljdszd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2ztabpgwd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ffvnmqpv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2xeomndov.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2jrkepcyd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2nnkdpagj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2tmeuzpkl.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2reoxlnrd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wfpqvlxb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wdjkhfqd.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2ecuqgiqr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2preppnkv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2bxccttdt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2zxxnoyao.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2aaxvvlxs.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2kmkekyah.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2pzjgxtkz.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2lksngbxj.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2vqjniwwj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2tthijecj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2yxuromel.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2mfbkkjnv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2forawhfm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2qlxsfxzn.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2stbzxbbe.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2gaauvher.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2gxmbojul.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2runxujvs.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2syzuvscf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ozstiquv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2tcmzmzpy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2sgjskdro.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2jallwlya.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2paznqztk.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2hxdhspmt.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2licrksih.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2vkawuudi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2egorqikg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2blkbvsly.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vjgavcyi.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2nzxxiigf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2wrryqjnw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2rkynxmap.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2vecuicsz.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2nuwjwbmz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2phkqnzub.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2wkkjpeim.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2pwyflwto.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2ukdxchkm.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vqhbwloe.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2rtxlrixw.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2kikpqhmk.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2sbxymzfr.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2bfnjpdns.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2evebgdsn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gycyquzm.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2rbneakkr.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2didfqcck.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2bllnycsj.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2wgjachzq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2ijvqdvuu.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2vlnyawyi.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2ugwjzyim.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lfmsorby.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lbmyncsb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pmlneknc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2erugitby.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2fzphbvme.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2phkbhnod.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gyeuhugm.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2wswcmqyj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2dzedpefg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2zaqnnfin.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2weykoaba.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2leqqoilr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ydozebtf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2ekpkfkzt.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2chlvghgh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2lwbvdjzp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2drjnbxmr.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2cpknoehf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bzgndcvq.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2zofrgpic.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2nawifkah.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rtvttovz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2gapzakjs.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2yvsdnzxf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2srxgrffk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2fkbahpnj.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xnvltzqd.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uilxjxqs.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2wrnruoue.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2wkgfuvvs.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ykzyirnl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2thhlkwwi.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2uftmelcv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2slroblbw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2uyiditeu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2jnailoqg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2frkmidgu.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2fbgufkav.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2lzwhswnu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2aiqocqpn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ujtsuucq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2lbmmexvk.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2mxhwcozx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2udkqbexo.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2gfpjffhu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2fpxchnph.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2fepfrdvl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2svwgqucm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2mvmwlfmc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2hthaxxsd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2duokqxkd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2cegddxul.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2qmgzirkt.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2rjipjjhf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2anmwpxlr.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2zhbfuycv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2lfssrnah.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vlnkaayp.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dpbmfuwk.html


<!-- 参考信息 -->