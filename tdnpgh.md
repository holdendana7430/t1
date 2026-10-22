代发 wailian999

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2csodbvls.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2rglxqqhg.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2ggnomblx.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2gktvzrvq.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2pwshtnuv.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ncohcjvx.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gxnjcvhp.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jrrbjlgq.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2glsivtkz.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2prgnmxvu.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vipbwqze.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2tiljiaof.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kmkphqfj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2alryykvq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ddllubst.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2jqqovfwe.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2pczfwkyu.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2htfwdore.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2jgkctzxb.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2ogzqlfvn.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2viwddgqc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2zivuqrua.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bazzyocj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2hkdvceop.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2texfsuwy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2omhitcti.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2cdbdlars.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2fbiinoso.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2gmhhuzpi.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2bwnvdemj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2albmhryf.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2aeuypfpw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2olzcxrcq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ebpkbrzg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2ztjplmxr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2nzorbpki.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2udlpsgqh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2kruztfxh.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2lfellyhu.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2udpxxxln.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2lbxztuyb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rwtgztkd.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2uztbdcro.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2dlifzuhi.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2buvtuqxo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2vonvdwju.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dbdpzlcb.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jhqnvbdj.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qyzqzlad.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2xosxyljo.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2mxkqmbym.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ibxsihys.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2uyltltus.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2ebzfksjx.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2avcfncvp.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2bezjgehw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uagabchc.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2kdiuksta.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qcmejctz.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vybzhyjt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2vppliefi.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ludejcci.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vphrehqb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2orggymut.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2vlpyswfj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2cuxgddfc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2kyqnezwu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nifhadkn.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2bgjfmtfl.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2pzgqqixo.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rszkwlue.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fsbicqjc.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qjhlvmvf.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hlbstwmh.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2qeblgpwe.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2mxyowoit.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2vllvjfuk.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2cdcazrtx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2immvuxce.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2viqsiqcy.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2uzsgzroo.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2kjtmvlgd.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2fwfnbuvv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2nhdltyyg.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2xnjhnacz.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2rtpmoyjz.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2srqlyrbw.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2gzszdfqg.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2mckptylh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2wieiyjip.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2kiykohhq.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mnolsbse.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2ndapcnze.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2fanzphiz.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2euijvivl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2uelqgfzb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vbwzziji.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2ypzpzzaq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2dymwjwga.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2ysdqyckt.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2vckonpfb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2kwlgyzlm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rslgsrjc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2glgxgemv.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2ezkbumip.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ummtwcmx.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gjmpvhbh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cvihyizx.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dotkovxy.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dnhhnedj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ggpoewmh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qzosojyo.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rmywhjlz.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2fyndwpqo.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2xlpebavj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2upqpjhgc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2fogqrehf.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2ijnojxzt.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2syxibexp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2whenczuw.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2dbagmmjy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2ubaqoyaa.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2rdhssphs.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2wdcwqadi.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2cleuqadh.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2sqdrflyc.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2vmkzjjrk.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2gcjiuifk.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2hfzreykc.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fwrqbbqv.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2tqnoetjq.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2hbrekfvl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2vlhnzslh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2gnbnkekw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ahaqhpue.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ozlhrkhk.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2xpsapqeu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2jpzqcgnx.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2ymfeourg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2htadexmq.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2ipsbogoe.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ogyhjreg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2gbpibtoi.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ugswlitm.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2mbfxiuhu.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ukvorkyv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2gjxdkxqo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2liqqrrzq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2nmexalpg.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2egoexleh.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2mayboxaa.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ernzfwcu.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2brotgqyc.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ypawswvp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2txelklnw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2dwpgknqg.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2xlskbslv.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2rtwkgxrq.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2gwmzskyo.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2yabvncjq.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2lndgcojq.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2jbrcaewv.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2vcxwlsxy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2qpeiztvd.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2rnylcido.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2qkuzpuci.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2gnxvgnqi.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rdvjptzu.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2zykmmmeb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2eppppffr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2bqidoovb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2biyuiifr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2jhzqzcnn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zbkzvrzs.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2swficanb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2bdmibmfd.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2ejzkeupq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2nnprkopc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tvkttwpn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2ukuckarb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2fuledevx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2djwvghfz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2wqmgoeby.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2bcatdcpe.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2zjqeypih.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2rpytnpvk.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2htoantbl.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2dwhkkamz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2oeefcolg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2egknhbam.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2dxfvvteu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2aopzgcep.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fndfbcyq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2alowstcy.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2suenofop.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2ngerpima.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2rtrczhee.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2qnudyaxi.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2eusbmzsk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2dirljwdm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2apauwqca.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2kqsyponj.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2yecdemlp.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2rmztdyxc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2sfvzksfl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yqcsibrc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ojlevpjq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zwdjnnng.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2inmnejtt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ntseggby.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2tomhgyeb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2etyxxnql.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2owaccsoe.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2dxxiktnx.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2lfrummql.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ejpwteju.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2llzcqxfm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ovaisdnf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wpzdnjdc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2vevpgvjb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2oymziwwx.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2btubrsse.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2mgmwndvr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2liaihexe.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2npxxaxlh.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2rwxxwgdh.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tnxkswfv.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2bbqovlxy.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2qyntxike.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2gkkahhph.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2pbreyeaj.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2xjxrskpf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2vlsfrupk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mhcamvoy.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2fdbztzll.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2wbcjbrhw.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2mxjidyrv.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2gtjninod.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2kpdpzaxx.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2bgeesxca.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2aeqwpetn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2dzqxunfl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2unxykfvv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2temxkbkz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gnnjshez.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2xjxrurvj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qfgdrwra.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2getawwiy.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2uyazzkoz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2akwkdhoe.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2aidyakfr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2mptwaeoo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2gpxrtmqx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2zmuocdaa.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2mlcrplle.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2muqczjaj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2rrutrnmt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2egrtzbdh.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2naabfcvy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zyltaffy.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2zcujfasx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2xzbxdbnp.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jerzceaf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2pikevmwk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2fjmeqoba.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ovgjwdsw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2iwudukqm.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zlsdmtht.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uzkiaweo.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2uuhqsjcs.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2outmryku.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvpzqoys.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bfnlodxa.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2kopzkscp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ewfqhwbr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2uhdtwfwd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2qfgpwywx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2hlsrjxkm.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2irajybye.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2xeiwrwtb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2cinbigma.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2zvufwgor.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2vqhqsanl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2olebrfsw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2kgptwpra.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2fwoblvtp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ypyywslk.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2cpgylalr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2vubyzviu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2zlaqupnk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ubwtktuq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2riigjmrp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2hkvircyd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zyfobtjy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2soprfqec.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2pvigpudk.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2schgwsxa.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2jzjlyfqj.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tnxwwsyi.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2trpvhjps.html


<!-- 参考信息 -->