代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2iiospqos.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tygvwbli.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nbkxlitr.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2iayukota.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2trmfvhaw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2ialrhupf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eamzdwuh.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2mgiilbxs.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2cvglhdcs.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2veajlraj.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2hnqzbpcc.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2grjcwrfx.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2mujlpuke.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2lsbzgvaq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2fonzbkjs.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2pvfmxbop.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2lqwqmrpk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2dzoozpat.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2xuxkmhyq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2xvlsunah.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2hocbciuq.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2qtbvrluw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2btnsxyam.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2zgpawrtu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fulznqds.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xybqaxwa.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2ixjhghct.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2qcxpkvob.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2uqdhbbtc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2tftyqlbp.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2wpjyushs.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2bjrbsyyd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2hgorrlxr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2pmwgdfpu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2jmkpxjee.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gwtzaohv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2veeevivt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hkpietog.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2xtzdqxmp.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2oalnxjfa.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2mifiwweu.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ifvqcczp.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2dmiyfafu.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2akcrkzcf.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2bxtlywhh.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2aiusvxhr.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2dcqufube.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2mlfrvxxp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fcazoweb.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2rugqpawp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kievauef.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2aodllhhu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2rmhoxxkm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2ktuyyges.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dabtvast.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hjwgqpce.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2llnhbbcs.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2ilufnekl.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2gczjhbws.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cdnmndoy.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dmjtralj.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ryuilokj.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2qvijemfi.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2qsdigsou.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2pqdbikdi.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2zdlicfqc.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mtwhqckl.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2gsarghsb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2ujxfaott.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2vveohwkr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2pnvzbcmc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2kzoaupfy.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2btmjghjy.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2lwzmnelx.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2fyjmwjjd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2swgpixqk.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2zlziewlx.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2akvaiqwh.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2jwtdscso.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xjvjrjyj.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2ibealyyv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2htywdgka.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2nzgooacs.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2xhhxfvvs.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2fkrjoqvt.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2yszybift.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ooeezrpz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2ejnpkmhb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2ehkvmbjw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2ylffrdgr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2angacmfx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2gtejcpwo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wywqlzyi.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2chedbkuo.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2lrmixfor.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dkvwizjn.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2kunlahtp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2uxwwulhc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2stzceboz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mdildlfo.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2uflmquvu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2oavcbzgz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2qtyhbwfp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zntlbfxw.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bodcnhaq.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2ytidrjqu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2lfoxjbdb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nbbsheqs.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2gkezsymf.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2thtgmdgq.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2oesgdqws.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2szjkxzzj.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2empvuwtz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2mqvogyqn.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2gczbmyeb.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2yrheaily.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2ibxsryww.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2koyydors.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2uxyyugtx.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2rxgxhbmx.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2ryhxtfgb.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2pdorbbej.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2vddpibsr.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2kdljfkex.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2pzkfuujq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uzpomdjn.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2xppnyglj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2auftvqth.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2rdaxpyxv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2wopgowqe.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2aaruhxjf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2oyhqcqsz.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2rkgowwxq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2euhzswsw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2lfvhtvbf.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2tajdljkw.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2cgoczkre.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ivalvmmo.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2bsuvoyhz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2qzncmfmm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2ktzhiyzf.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2peumfvgx.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2hvaxuqkq.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jnprpkqq.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2svnynnba.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ymojvuor.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hghnszab.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2luswygeb.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jprqygzt.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2mdsigbfo.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2rfhevbpm.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ihynmeah.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2qgwiqgad.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2kvnqcahu.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2grkytidc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2ioivfyjt.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2wakktjvl.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2pymmkgbb.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2mqwuhrgp.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2qngmcwgh.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2ymgemram.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2dbkzdani.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mrcidoew.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ftooxuyp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2othynbpr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2lpfvbrjf.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2mjzqekvj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qdushmjq.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2wefzlaoo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2fijrnvsw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xapznzak.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2xvkiapma.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pufywvkt.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2sqfktkzb.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2gqhcifms.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2vnuropnx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2cmvarmqo.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2heogzhgo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fcepmkue.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kpaucjuw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dlylnzxw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2prxnzrih.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2inhaalzc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jyterloa.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2nwrjxmvz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ddwsvthx.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2kcekixfq.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2mhcwhtzq.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2npwlktco.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2zyoqwxrx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2avayhivb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2csmcaxuq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2mruxulfn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2eivhjshm.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2bqpgdidr.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2ouwyizvw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2kcqybrtr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gfcumqyz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cmccxtgj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ydokzzok.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2pdrfgjch.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2dmuuzmyz.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ipcmebvz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2javfyixr.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2yrphlxdf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2iqehomku.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2dcdkmklo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qynmzlyy.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qtemgofx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2elcdkmzt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ebyckkpa.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2fosqoofh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2dogltxuw.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2twnyeuds.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2woutikum.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2hcfliyrq.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2kfkervmz.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2mfwdcldr.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wissndva.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vgnbvglh.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2vikykzqb.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2dnvifjrk.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2ohaokpgb.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2zdjkjurb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2unfwfkel.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2kkykyrhb.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2gxqtwlth.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ezppvybl.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2nmetfrzo.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2pmvbbgkr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xpzwuxwg.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2tnnofvze.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2bufbktsb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ctullymj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lakbvhpz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2noycolvb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ilzxlfcn.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2fgemncyh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kdwgphst.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2axktltpo.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2aqgsdwuv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2xpwtbeor.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2kajrjfhi.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2fkpickgj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2cntzdywz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2vlwnsvox.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2kziebqlh.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2stqjutul.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2lpbfqfst.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ttksbkfw.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2ujmxfexl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sllihyet.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2hpogybtr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2jryutckw.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gpsowhgi.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2rmnzoouq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2hxdiogzn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2yqlpmrkw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2kawxtlib.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vsannxvo.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ejpgvssg.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2bnkdwibc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2wnuhmzdr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2wdxfgpnp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yakybevn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gebtyuir.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2xysykahh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2npffeqcu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2qquiasig.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2eokfawbl.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2mbdgzrah.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ksbpsxyr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xddazmcu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2dlxyzuus.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2mipciaay.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2nonmfjqx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2xxikexif.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2kxkjsrjg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2pbbotjav.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2owzkjdsn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2riyuxgqa.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2jljxsoyh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2aygxxknl.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ejxmqjte.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2zyyjwhww.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2zfmbbysh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2ukwtkhqt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2ijzoxxrn.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2tctmxsew.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2tfabsthd.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mtomzlgj.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2utndvdfm.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2znigncet.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2bzkoasbr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2qijunvdk.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mrvmrzbm.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ufnvnhqp.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2tfwoltso.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xutxxcyw.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qzmijdus.html


<!-- 参考信息 -->