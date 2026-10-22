代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2aggqadln.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2bpyoguqy.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zftrhqod.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uyldghvu.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zvzriqcy.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qxkonftg.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2igepapsa.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2sxshvgyb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bsmwdcpi.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2oottzsdf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tazwzwlz.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2plolqonw.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ktyhgavj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2dzummcxm.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2mpzgktbs.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2iuibkujs.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2wduxcawa.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2cnvqimio.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2exqjijub.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2biomcnmm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2xbpzyqdn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2dojdrsvp.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2vqhsgztn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2oorxptuh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2hrqfcjqi.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2zrvibqac.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2aokoalvp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rzwhxmoq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2egskflgd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2jfxirjpq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2itqjyqqe.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2aajqqkhm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2wgqvxdhc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2yhcudksi.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2kqpifwgx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2hztidcne.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2uybzkbsf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2vwhildkl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2akjtluxh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2xfusruqd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2zvejmmnz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zbtnjvaf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2hgopwsha.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gjjkivnc.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2krcbubhp.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xsutpgpo.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wyrbhpmo.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2xwassxfk.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2wqlcwvco.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2myakftpj.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2biavklzw.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2rvwsbcrg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yxxbirsd.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2bkejkqfn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vanguipd.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2idxrjckc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2irfvnrib.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hmarryji.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mhlbbosp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rbomicnu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2jezrsarf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2rjflcxbn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2snntggls.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2odcpdxrr.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cbvwzmkc.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2dcxiyvwh.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cqgxohhm.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2oupzywbt.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2dldtvxub.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ivfyogqe.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2mmxgpduh.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2faqvospd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2acovsgld.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2smemtjoh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2vqmbfipt.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2dvxxlgcv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2gxlupbky.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2wmdmfldo.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2oullppxo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2wrodqdnj.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2chcrxvkg.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2sbwuruws.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2abolixlr.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2yvqnnktg.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2gdtaozxf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2lpwmlicf.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bnkludqa.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2oajhlwto.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2egcpqolc.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2xpzbtubb.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2cxfzjycg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2hbxwbrkf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fsuevgil.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2ltxvllaw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2orlgtsmv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2fvuwfrfz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2surfpvwg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2wysqejim.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dvmlsgrg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2niydtrdn.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2inbnhzwf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zuvhkytk.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2buobiljc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mausmbci.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xlkudvwl.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bfszxfeu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2mbmmuacr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zchtwoyf.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nqiyugzf.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2cnbckbwm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2jjsyduyv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2skuqebks.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2tdmgaevi.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2yjkkisix.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2mbawswpf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rbotxtxc.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2qdenxaxr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2reomsgbn.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2brxtijwh.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2vcmjzfwt.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2okoinodf.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2dawaztxe.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2bvvjeyqe.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2tnayljty.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2sfnugebs.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2uppazaei.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2mcdbstap.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2fnjdsuxu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2qganlsga.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jnqvnadb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2dqshxcec.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2tavpbxma.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2traipyay.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2gnanruxr.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2frdppeue.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2lltkxupk.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2spavzsgn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2tmlzolkr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2ppvgvgxg.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2uqcpwrol.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2icnikosy.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2lhmhoqup.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2qpbuhpky.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2kejapxev.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2xiimwdlc.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nagrjyql.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2rxvekdnq.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nompdzwx.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2rgljugwk.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ydhzzrom.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2pccqbbjk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2btvaykga.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fnpskams.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2aujtwkxo.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2reimwfip.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2sfhvulnl.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2tltatynb.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2xhgwvpvf.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2chxnzqrj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2ytpvxexb.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2gxrvvkiw.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2epatvofr.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2bpgmkorr.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2dyxbuwiu.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2kagastxo.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2gnxpzauc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rgfcpusr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2arvxvlyw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2edlflcor.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ejujfmhy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2wpcwxqsn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2gllwxlsr.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2xkyessbg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2qjervxsu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rvaltpuq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2slbvactn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wmagxsru.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2szwrryvh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2ywewzidm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2fzgsvcal.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2uwywjcah.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2cemffdjp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kcffjfic.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2xqgdzoyz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xicqgxrz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2iuzabsci.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2brfklzaj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2glvhlcvo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2dtzjekbv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bnmjerqs.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2onhfbzhs.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2nwyafisr.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2ygussbzq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2fzmhjqho.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2mbovnzhb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ljgctrip.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2irrztmbu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2srvlhuhr.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2cramgjmm.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2ohyfjydx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2gbztazus.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wexxxzff.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mumgiepw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2lgvagsmc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2czjwmkwc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2lcsalgzq.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2zdaxhjwe.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2fzgngfmq.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2tipujnpk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2rmnyoerh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2zvgslzka.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2bdgmcmqu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ldqarrwv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2xwhifiws.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ctrvzaql.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2lpdlagwm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2kwzhzyqq.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2sydmwvnh.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2eyzncgsl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2hdwosawe.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2wbldiysm.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2uwvkbpde.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mbhdztob.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xnyznswf.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2ygaivbjy.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2ouzivzcn.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2wixhhbbh.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2atzvjlsu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2degxusyg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bdseyjmp.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2nwprhxuw.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2zwkhxwcx.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2bhpfiuus.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2wojklrbu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2edhxkuhw.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2oipntjbg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2zegvoisq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2esyttvis.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ksmoagjm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gummacmq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ruefsmdd.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2zefmjytw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2omcmlymj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2fvlawwwr.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2ejuqsdfy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2gixesoxm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rgfuytza.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2gpglwkdb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2mphozuxl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2jvypzybq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2rorlsbiq.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2uaexrmiv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2oyuinnxi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fejddhxi.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2hnkvksxm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lwvvdsra.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2mztonmhq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2qojdiddd.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pdrwvpwp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2bvdiplnl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2vkbpudvf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2uahnvzxw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2ajlxrzwf.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fhvloqqi.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2aumvdbck.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2gkijlvus.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2wptmuuye.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2prxxyvgj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2zsjklfed.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dwpgjavj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2blwgzxul.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2uyhnqjqe.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2fofgemxe.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2yfuhwiau.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2dnwxyoya.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2ifpjwxrt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2brdunfev.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2rtvitrdz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2zpivhofe.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2iaontkuz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2wgkuetwn.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2qqsgglrz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2gehuzlpu.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2svawubgf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rlycwpqd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2xsoahjrz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ziybwenv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nyodvfei.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2gpazshqx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fwwhykip.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2fbaczjcv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2swiijius.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2tndlityz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2zfpmrbav.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2sdhesvxq.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ifkotqel.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iahtefdc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qgbkmhra.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2zvnzovnc.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jlvegbvc.html


<!-- 参考信息 -->