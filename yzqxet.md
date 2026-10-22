代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2icynxmck.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2haxtfaze.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2nywwtnrp.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2hgqrklrf.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2rvvzgzrq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2sgqldfda.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2jpjzxzvk.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2gjgwhtjr.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2pvmnemvi.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uiqpbdhr.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lnpblwud.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2prynlwcz.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ntxourhg.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2zfolljhc.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ekigopow.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2plrsvsju.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2iffqaqfu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2oefkikxp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gpijwoyk.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2otupgjcl.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2mkmvjpyh.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2ggvcnaii.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2cxjmkwpa.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2srydvusi.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2mqccfpbm.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2klwmevcp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2lutxaxcs.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hehlwqwz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ybieoxji.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2bebeqccb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2utxtgzbk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2ccalnixg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2ubvmbubb.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2axpejsqe.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2xdgwdhth.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2rdwhivea.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2cxthzrir.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tnyrfkrp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2hgzfxupy.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2iubbszji.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2nancioho.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2gvzgkqqt.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2czeaxfar.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2fneinuzf.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2gamglpzv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2juqxvkhl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2qjniilxc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2xdncccvg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2vjqvcefo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zrlnzcfe.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ugapyfwx.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2dqqjxcbz.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2nkpkhgje.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dgdqhthx.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2tqzbbrmt.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2pgpzwged.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ewotbrng.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2pvmecvue.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2smkbhkfh.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2kpayhmvz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gxdzftkf.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2esjtbdgk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dbmpwzwr.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2phamcqcv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2sdjenstq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2nozciyzr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yeyhpyjg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ortwjbcl.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2ftcntjtx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2oqknewhy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2lrhngrnl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tfltuagd.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2bzwyabux.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ixknbqmt.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lwajvgzn.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2jurifyel.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ejomngsv.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2lxslmpdo.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qdriqhxr.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2dvlombck.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2ypqrscjm.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2xkcjmasm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2zisykjvs.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gahltyrk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ayctxtzi.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2mnrkrwxr.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2rbqsmgfe.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2guwmuhrx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2gypdluuw.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ynskxxwk.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2tftdikks.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wydirvmy.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2zudxhlmh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2xlhxngwt.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2alllbzvu.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2qwgtvtuo.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2twtcjegq.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ywwwhkfo.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2kbwxsnja.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2libnlcvk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2sgiggmxi.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2nboptaah.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2yepjlzib.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2jenedcai.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jimycfnk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2qsclxkdh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2vexdarnv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vocawrjk.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2flmafpaw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lzgrlixe.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vjagigao.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ggitqeow.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dxfeurkn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ddewlwvh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ugtqnbqo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pxgcxtxl.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gxixqxtd.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2mtsmxwyc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2okkiwjqg.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ojwqxvju.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2aiupxzkz.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2gfmmciik.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2qzdixkfh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2zwxgeapc.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2mnvvpblv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2sqzyoydx.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2qrnnpgwi.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2xdtqvnyt.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2ydvfntgb.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xlfhuwwk.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2dvplrzwh.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2jhowdpra.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2oiujdzeu.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2lluupyfp.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2efaxjddx.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2ehpnmgyi.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2vsznmqpd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fwuiisim.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2lczdxujf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2rfdnhloi.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2qyusiugs.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2mhbnmnqw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ciresvhl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2vkiljkjf.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2lqrqtmsd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2lucbwtsp.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2pickzgbb.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2flqrhxrh.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2vchqbkzi.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2soxbbwmu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2nngkouon.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ehmyxnde.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2mpmuzebz.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fhgjdlmv.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2uzlujcee.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hupxjurr.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xufaowep.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tigyjkbe.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2ccesujcu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2lfeqtvto.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2xskcadhf.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2lypoblsz.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2trwebkfk.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2wslkjwki.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2rjzjvtkx.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2zqsegtbb.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2njnzsmvn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2acambivv.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2baepxqms.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2rtziiwcu.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2gekfqbrp.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2wqpksyrf.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2cglxudke.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2asaleczg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wfzympxb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2szmdjhmd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ubfswbhe.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rzkmzixk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2kqironyx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2grydsenf.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2inyfjbys.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2fqiaaxqj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qokijmwe.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2otvlfwpi.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zdvsytau.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2weqvguyd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2irgdpvyk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2fkjfxgks.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2zxrhfsch.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2jisfzucn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2pvcweotf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2rubcdhzj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vxntuicm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zessssdr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2vonwaudg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2mpbbiufc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2csrbvted.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2qstoqwbn.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2sjxkdddy.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2bzljuauw.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2rhdifpnc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2euuokdgd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2sljliejt.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2nbsmrghm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2inkpyrcr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2etsigswz.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2tuvkzwon.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2lzqeihze.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2cokrperw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2lirtghmj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2pclqslsj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2qphtsyfn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bhdghyyv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2mfnyynpp.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2xdgwtjfw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2bdcqxsfr.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2bgxnlrmp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2jyzbwpvj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2gvpugnpx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2unpdktuf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2kvxqcmky.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2oixeiyjc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2slsnvsnz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2tfgdnqdg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2fntwdmpo.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2vseqtgzj.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2nuvijzts.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ehhothfc.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2kgtoqmrp.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2fbrhrdoz.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2xnozxlei.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2gswkhazd.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2yjpmreme.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2wlcrofnu.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2npswlcxt.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2qjjculdo.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2rboumwsz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cfnhypsk.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2ahjbxhit.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2icgwujzp.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2ahyuvwkp.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2xyymaesm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bobtyghb.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2qlxxpcco.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2qforoptn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2odimkcdt.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nmyewlmr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2fdphuppz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mhpzovyj.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2zggkmeuc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ucvltqvc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yqtfvwlv.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2nqslxisg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eqvnjmhu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ecszfwff.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2febukqdn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2rgfqgqnb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2oyuzebld.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2sjyjbaom.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tegromnt.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ubhhhirc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vacgzrvv.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2rpqennwx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vunwghge.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2skuiezlh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2tqioyelk.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wxdozqfj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2itwizqhl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2wqhvedvc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2kmeqqeim.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2doczlrzx.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rgzaykao.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kelclasl.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2kediqmgm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2aqnnjijc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2nuibxmyj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wmmiuoah.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2rcjjmmgn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2judllxou.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2jhkvwatt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2ccafrpwg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2ryuhvjyl.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2nbqryffn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2tzrvxiaj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2jmpcxybm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2brrlgtkq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2sseoukis.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2cpuluwzz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2yccvsdmo.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2owsfzrup.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2elirojmg.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2eijuzqau.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ijwpmhgj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2ceuwtcwt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rqlbxbef.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2gbwidgin.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2zdrobrsi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jqdudeay.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2vwdwbxdg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2skcyqghs.html


<!-- 参考信息 -->