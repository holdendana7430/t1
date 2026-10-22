代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2tempdvhb.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2vtoegjav.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sptcpjqw.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2ngvwsefl.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2kdkcvwde.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2cjgaixtt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2retwcstk.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2rqkpjyve.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2kdeoqgib.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2tzhcvueh.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2ztgkjvmi.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2qgkcadcv.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2upfcrrqy.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jwrhttim.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2giewkdxl.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bbrmdfho.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2obyuadwp.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uqpjmrmx.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2klzohiit.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2sfsmthkb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2mueytiae.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2ryyickut.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hmsxryzh.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2lhihhxij.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2iuugtlkw.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2bnngqkgy.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2xtktexkx.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jxhmxttn.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2qxviladk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mrjmfrws.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2yejumavg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2nhmlrkjb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2oksbjptx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2fuzcujjt.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2pqkygjvb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2txoxlwim.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2jexlwgwu.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2xjgasvyv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2pajeusvv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2yifcvrfp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2yzjhyveg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2yocoqutz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2giyujgyv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2urceghmx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2ydpbtlbu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2shndjryl.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2skudfiro.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2hiaxhifl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2rqvgdxdb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2uixgvqcq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2yqfwgylz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2txumdwjx.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2fhnuyzjm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2crqqvahu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2llywjjbt.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2jnbkbcsx.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2shdjimzf.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2dqkwyktn.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2odgxleap.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hmyutpal.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2iofesilo.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vhnvwchr.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2mxbyguyj.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2puosdwls.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2egfuhjsh.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2fbrpmuza.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yeareccv.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2fzlqmdhs.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2eokjqnqx.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2yweusord.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2vheoneon.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2dwqgukrk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2hipylofr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2whpwlxff.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2jqaxnsik.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jaqhnxix.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2lqgnsvxe.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2zpmfvyeb.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dpyjycpi.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ehhpiear.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ugybashv.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bjsqiteg.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ktcfjrtm.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2inpiecui.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2kmwwxtcq.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2zlusrbtq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2jlfibzlw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gtbjwgdx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2kihqlmyn.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ojsmdppj.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2hdhlagrm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2frpheecy.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2jxgdxgzw.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2gcpdmawj.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2sxtmedsy.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qcbeodnp.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2exjalnvp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2cpdrztbo.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2yunkqfhl.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2jtmmqrxo.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2gxxuydqy.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2zbtkkcit.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2oixulcwe.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2qkjdjavg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rcoxvcrb.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2mhocyfxx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2hwyuqbsq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rrtrcgym.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ybrepubm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2wndpueer.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2eeaobgqa.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ttckckhc.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2pyuyuwtx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lphyvqyp.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2rmyajllw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vckqcfxq.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2smeamkke.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pffdjenw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ehyznclu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fvzuewcj.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2isojrfsy.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2qjyuhuka.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2uymczwwn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kfgojlic.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2kgnldyac.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2yikzxndv.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2ymqhyhww.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wtigrilh.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2ntgvprkl.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2mlnjzdel.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2cgatbhih.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2yeregoqu.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2zppdtmrd.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2kirdvjct.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zeiulrzw.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2obyzdsvz.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2jlyugkgb.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qxzqhpks.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2lmgpkxel.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2revrnpul.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2hodttzhu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fvvsbvtm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2kgwepoyd.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2nkzyuvcp.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2jnkotmxq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2cwlgbfdx.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2tnzvocdu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2xhifiyce.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2vuddkmxu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wfvybwje.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2bcbbhahe.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2lsbuepmy.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2kiabfsbl.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2uiiwpnlh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2jdnmwljg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2zjwkmyjx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2nqjwujkb.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2vqftnosh.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2braytiel.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wihyisuo.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2uxtkarrj.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2irnznamd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2vndhlayr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2fzxrwnwx.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2qzjqmigm.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2reedkzdn.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2efgxzoxp.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ymoqncvs.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2kiuvtlrb.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ipjfgvbd.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2eugqoznf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2yvlvsnhz.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2pghznehs.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2aywafvxf.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2jbmurluv.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2gxtdqyem.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2xgppctfq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2yntzzrua.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2pmbleqcn.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2apimzlvq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2snvgaxmr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2yifwqqqu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2aghjbhrd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ffdqobqc.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2bwkuipzz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2pgtgbcfc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2bhcwpbkq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2yseaoeqr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zerkjrqz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ksudlvbu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2vvcqmdvb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2uclumucp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2jgnnpoha.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2dehmruto.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2coobzhio.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2dkhncmtp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sibqkjbp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mzdfunth.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2zffnmelv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dimffmpw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yipulvbr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2znsvtdyl.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2xkmmgfoh.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2oabtpvkj.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2kdcfcemy.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2higizhxz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2owgqijpj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2oycvsgvp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2hfrbabix.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2hrzabcih.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2pvinpwkj.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2ynxcknhf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2rjypefkw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qaxgglhu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tvzgusgn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tthplcte.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2ucovrjzv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2ukitkefr.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2tfetvxlu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2msmpbund.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2dhmhhtee.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2ngsofbhl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2kzywrbcy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2pqhuwkpk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2setrpjiq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2yfkecxta.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hlokvjmu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2pycgavhg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2fvjdbagu.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2eopsshqf.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2givrgzra.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2trqkydjo.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2bfaftjdi.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2iiygqsae.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ujipnmyr.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2trwoftzu.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2urzgqxxl.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2uxjzkdjd.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2xdcbenwc.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2lnmqypsa.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2qzlgxzav.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hnagkftd.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2kgxiivim.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2filxyrvu.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2ufymsczy.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2cfokxsyf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2ghzljwvq.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2shbapxmm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2kwhnhiew.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2brpxiqzv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bdcglqsl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ryoptfmz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2juugcuxj.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2dotonhcv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2prhkyqqn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qmvpsxkh.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2qpvoopge.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lwnivzzg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2zzcejtbi.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pmurhwjz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2wuetdxbn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2xaprrdyv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2vpuenjxt.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2vijkerwh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2utydzryu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lypzselw.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2ohehovlv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zcjvhlsn.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2uwqgspng.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2mbtibzkg.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zcujmibk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2bfpozeai.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2aaivykix.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ygdvkhgj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2bvwtohat.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gaiuysim.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yixhskhb.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2ekujbeqc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2pbekbnpa.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2vpldrasm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ocagtyws.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jrnwwlso.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2txkzoyhn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2hidejxlt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2psqnyzxw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2vvslpfyt.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2avpbhpog.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2xcibufhj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2udsbeyal.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2udsncenz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2uwyfidht.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2omfypcmd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2stegwmrd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2bcbvrhyh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2bceolqzs.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2bxsjxctt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2mylnsezo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2wkvzscqj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2erenodac.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ybtkuzau.html


<!-- 参考信息 -->