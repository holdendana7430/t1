代发 wailian999

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3ywewenav.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3tecmepcy.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3voheyjzt.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3bfhazgti.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3sphlkqng.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3iwacncyh.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3joiigpjo.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gelyzffp.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3elegmxyq.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3wqmwdrqp.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kttmzgip.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3kpmkseyd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rqxxilcc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3cvpefcuk.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3aglqrmwg.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3pugrhbkx.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3tmpmlztv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3nooerida.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3siqenixo.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3qxvkaeci.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3gjgciriy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cnpzlvto.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3dcjifwzo.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3dmmivpmf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3vryprdro.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3ujkytalg.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3zicawckj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3wwpgqlfp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3kxopjgpr.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3yuinlcuu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3pzjnwmoi.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3adddczmf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nffaayzc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zwjrwppx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3vskozyry.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3nfyqyuqo.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3kxqpnoog.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3ovyqakki.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3diqxclgd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3qgvuyisd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3yawhlcla.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3ihvpjiuq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3pcivvhjy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3sgunjihb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3fywvnodb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3arzagisj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3okopmdrv.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vvqeejcu.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hbvpolfe.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3xsjcmwuy.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3thowvmgr.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3inbeesmo.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3acuesums.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3cpkxouow.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3absymywk.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ycwizewy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qklptnmm.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3qzznbtan.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3brzcjpch.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3birlcyvh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3izhyvujr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3eufgyzfo.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3excajqkm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3vbecqtde.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3uudadsxm.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ccfaitxg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3jgjqquhz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pfbbnhyd.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3vpaokrsz.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3fgtjlidi.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3pxuwasjk.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3iipkttmq.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3asbrcuoj.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3fopmazzn.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3eqsqrrma.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3takgrtlj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3zvuuytnc.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ayhrncbr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3bcpzvepp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3orfijcgf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ofgntpbm.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3pyhhjgwe.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3hqvrqioj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3riwgxvet.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3ntcxfvqi.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3zpfvacat.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3wzuubgpq.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3tnrifzex.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3vzjdkapu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3rcrpvawa.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3sambbrar.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3mezuljis.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3oqghvqlw.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3viozsgsr.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mmsjdisu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3zmktriol.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3cqtfsuod.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3ltyotqzf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3xbqtmcvw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3eablzzpr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3udveuvlb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3xcbwxeyy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ipiddhov.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3njrcijig.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3lvkusbkp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3zsppuihi.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3yrqvarqv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3udvoabfz.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3etbepmao.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xrgikvci.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3szrqpxyy.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3poarmdqf.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ysiqrtmv.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3inmhywzz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3ggjjlptt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ntxztkuk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3zuylloov.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3phssezoj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3sohrqyxk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3nugkhnsj.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3xkmhcsgh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3yysvmzxs.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3lnpinhdb.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3iewcdoks.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3bjcbmuix.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vvzjmckv.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3wpqdafwg.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3gktckstr.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3ngdrplfs.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3nrafkxwc.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3xilgcaed.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3kkgrjtem.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3pyyexsia.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3geavmjbz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3sviclkjp.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3uydzeoqh.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3qnuvbksb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3cnopfxsj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3mvoyyffj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3tixfosju.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3vtkwbntz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3naxmlqmi.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3hesgtbxm.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3msepiprj.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3vlqnmzvk.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3yuatgrdm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3stzozwne.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3iavxxmmr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3fynwxnah.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3erdfzotr.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3tubxgjup.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3imtsdhpt.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3bzkcgbkc.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yvmtnkpr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3rnfeoqyj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3xtoadber.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3mcuvyito.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3pnoeqxzt.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3lvkaywzf.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ztqyztmo.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3kbxgbdai.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3fdvqfcop.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3pssyxkch.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3vaxpwhuy.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3wwftskqq.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3uaiiltci.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3gzqbiwxv.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3nupttcel.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3wiwmmnbi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3lreawfrr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zxebxflg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3sjezkgen.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3nudfturw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3sgxiynal.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3svxydegk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3znhbidth.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3cfaseztk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3jfnbadez.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qtgyxxqa.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3pdcfrkop.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mhlbrdsv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3zefyvrls.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3mbsmwguw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3fdqtrebv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3mxduopiy.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3cwcmvvhg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3nvamyixm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3kfhyivqw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3gougrvrr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3eacsweia.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3nfcbxmca.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3horihpzn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wustsmyt.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3kyioqdxh.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3twgynsps.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3jqvvzcvv.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3ihmjbban.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3yctmqtrt.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3itjtoinl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3nzebihoy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3tvhczvna.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3poihbazv.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3jlsnkpsw.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3jmwcgjhp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3uvpmewko.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3slqwmbkz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qofpxrtv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3srorardq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ebdtofqk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3efkbcbxy.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3jvxdhqrr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3bxyjalzg.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3vpvjrdai.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3odarrfkv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3xpwpunsu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3pxfsnfpc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zkegpovo.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ajtqqivh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3bemuxcva.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3houaggtk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3qlsrkbid.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3ukexwgxd.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3lnrdiqfi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3sgftkunk.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3aaougmvl.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3avaduhff.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3fzmvdnbu.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3flzjhdib.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3anzcnwwi.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3fhpdrjyl.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3njnihobt.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3dprplpjy.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3cbufsshd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3emgjvbfv.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3zkfolqzd.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3qvyklnsx.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3unxcerut.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3kligmvuh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3rchvsevx.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3yhwuhmfc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3upjoxypv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xxxpgubn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3igexmbpk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3olfdyayo.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jkwuudtn.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3lcwefgpe.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qpukvubb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3unfvmkbs.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3bxbuhxln.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qlckrngy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3zuawesto.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3osruoxal.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3tadyuqby.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3enzkhqsi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3okgesevd.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3earxpupg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3zserhxiq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tiqpwgen.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3ywcoanzu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3esifegwm.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3tbsdqpwe.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3cfgvamrz.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lhikjwnu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3acsdkrsz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ybvzhsvq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wetrcfna.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3chtkucny.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ldchypto.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3igdnkbng.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3bochtzex.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3jdgjzqiy.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3skozaqim.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3wfaspdgy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ibxiibhh.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3vbcnzbhy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3dwodohur.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3wpieotpa.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3rpdikawm.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3idkywmzr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3wcihectb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3qcvgayeg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3nftifpmb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3fkzndboq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3xapdzgix.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3acgbxzfk.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ijgvbofa.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3itzaeskt.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3lszacplq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3btcumhuc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3lbdtpwxx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3fkypplfu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3sqxbxoty.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3hklhgnvz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3bncftzcp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3dryklxer.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3obrajcun.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3ozjilsyh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3gjqrttsx.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nxefxcyq.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uctitpxp.html


<!-- 参考信息 -->