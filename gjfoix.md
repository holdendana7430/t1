代发 wailian999

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2tjtxhkyb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2mdyvcgcs.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2vgebcgsx.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2hrwycmbk.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2apbtaymv.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2prxmecyt.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zpmoojeb.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ozemsuxy.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xxovajry.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mzdzdrqi.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ysavjyit.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2awbmtexe.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nqigqbja.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2briynevd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2lnzteviz.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2lkbpfadv.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wqznxiim.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2pxzpkjrm.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2obnhqgub.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2gafrgicz.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2cdnyqugy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2ygfmqppn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wrcspzft.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2njbmrphj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2atphgchs.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2ngqouomn.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2auwnuoic.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2xtdujyze.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2nvmwjudq.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2zeqcwsbg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2ghymvgfa.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zuczbozp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2ienmkjql.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lomvhzco.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2fyhdyabr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2ixscniaf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2eusykpkd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2awfqgzfo.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2dgnptexz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2lolvpstb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2hpolllro.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ekhdddhm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2yrpqeegd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2yapfrznw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2dgyesxze.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2ttmdfrki.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2egwgtzht.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xfeshsog.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qdargrpu.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2aiawczie.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ilyfskjm.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2waxcqyxf.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2joooqiuu.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ehrhwcpf.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ximzbwwo.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2gswpxrfq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pledrnsv.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2zfkfukug.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rtsfsmll.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2zhslfzgo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2luvogfgu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2ygtixphg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2qhtwhoda.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lqklwupr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2neoezbpb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ptcqrwqe.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2vtppcrfa.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yhzhbpxk.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2jthsfqrm.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2smqggzkm.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2ctnlsioi.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2cjtejbjk.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gztydgtk.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fehlfnvm.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2jplvodfi.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2cspwqxdb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2rtfmvxil.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2iwllrnnp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2lcrkkgnt.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2isnauuxy.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2lrqdhrlt.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2zchblvak.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xgyrnyig.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2onxzxeiy.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2ikscnkqs.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xllgtvsm.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2odkupawu.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2zcifeyst.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2lfhfqbwa.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2iwyaogqo.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2csoblrwg.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rwcyljtr.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2htzgvvfe.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ghmqcxde.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lgapaybw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2lyurlhbe.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2wgegkelt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2gcvuzgjp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2pgkeojhf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2oompekay.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hzofpejz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2dullcabf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ufqnlmbm.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2emakhnfj.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2jhjvjpyh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2aqwcqjns.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nwvysvjl.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vcyicvxz.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nwbswhcp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lvnnukry.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2becvlmix.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2omvufzdr.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vykvrnog.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2ktzplmcf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2vupcbbhd.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2gsjexiui.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2bnbcjobo.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2hjiyfzod.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2rrwyhsnb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jppptcyw.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2awdhuooh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2rvjoazhm.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2rvxwssry.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2fthtoryc.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2wpkrrzpu.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2yxxvtufo.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2irsrezqx.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2qccxxqro.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2lcmzfyyn.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2nfxobpjp.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2uarnrogw.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2gnjvjige.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2iestirtc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bgnefbnm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gfsiwozm.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2mhcrwsib.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2kcuqobid.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2ksyhbwky.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2puiwqiwr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2jilgilgt.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2hznfbjzr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2yjfqpteq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2keqtfwpv.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2goiwrdnv.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2gypmldhj.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2cxihhrrj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2cgkhyynr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2bziisydm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2eyjbcxxi.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2vtexpbna.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2kyrbfktq.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2jyexjhnu.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xclxbwyj.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2hzozmsbk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2zgfynlxc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2jdkhvilz.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qoxxkfnk.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2oumiakna.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2zcaonbwq.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2iuqtiopo.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2dzimhqth.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2agdmboii.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2lxsnayjn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2qbwhxwji.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2tbtdauyx.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hozhtmlh.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2nwajhdth.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2dcmiwznk.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2pikqcxfx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2xsujfxri.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ugknvtas.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2bqxjzxko.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vtfwwwvd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2idexmjfd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2zxjmzcsf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2soeujgct.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2uhcmklmj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2wduvqrym.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2qclxztdy.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2ggcawsll.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lhqtrxhv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2bstakbqt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2pnnsalyz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2wxpwrrtz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2cofunhhc.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2xjrfdqmr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jgitljit.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2lshwvnio.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2kxatcmbl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kghdmnzo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2hhgujnzx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2pyxoqgeb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2ppoigibf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2ykwkoyud.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ruiailir.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2kxugarhi.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2rtpwzlfn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2dduaixvo.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2clblsjnl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2izdigthw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2bxzqnqku.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2hwcypnzd.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2afduwfop.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2isrnqexl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2chkotcwp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2xejxwwlk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2taftxvpa.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sbwgvoqm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uzijimzv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2susmihwj.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2xglmutbn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2ztuqdvth.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2invucghv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2tdguqalw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2dmikojtm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ufcgopdf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2prhccucs.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ojsbrubv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rqalijba.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2uoaaitnl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2qkakhvgx.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2kyuogvqo.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2knltgtov.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ruszqela.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2yghcstnq.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2jhzcbvca.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rjnbonki.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cvctwvbn.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2dmxseady.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2slrkcqrv.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2sflnyvcr.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2qneufdjc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2uygrimbu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2efsmmmjc.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2vmxswrew.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yihhpyea.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2fousajkw.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2zqvmsavj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ritjghjl.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2meijznlm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2jgdwfjtk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2mocyyadj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zataeexm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2yvedonkq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jwlzgpeh.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2karxdmgt.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xunavazm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vcrojmty.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2sqmyadaz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vjikamrt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2sptqaueq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2iufmdalm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2hyssztgr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2bdappavq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2gdgdxxkw.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2iokxyxye.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2rtgekjip.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2niwhtxtt.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2vilqnhdi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ejaxpcvi.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2gyulopvu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2pssddcgm.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yuysacjy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2frbxrkxz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2cgjzdahc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xuupkhkw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2rnljinqk.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ofzhfhwy.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2udhedjnr.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2qassqvwz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2uqmsgnsr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2ookzqxjw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ueudgrot.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jcsvjvbx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2skksaono.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2cyvksjvj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2yeodqdze.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2vwpikrbf.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2otflomog.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2zvkbvrag.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ttcblnbb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2llxenyfo.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2hmfoakdd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2twdrlggh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2mdlbzdqm.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2yqwcdrvk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2tmuvagzk.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2oogbnigr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2rlichhhz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2rhfoblsh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2iybfezec.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xkrgqxgd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2xucrueej.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2shgkmuua.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2llcrejma.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2oshbqrvt.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2vxocajwa.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2fkwagfpf.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ojniisvj.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tlaskkkv.html


<!-- 参考信息 -->