代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2uchxssga.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2tekoocmz.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2jzrarfox.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2rcnkpgrr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2rhmlodoq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2wofnetkj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2rryhxtko.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2dfiadsxk.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2tsrmxipr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2hatevvig.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2zpmgecfp.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2gggxfajn.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2qvbanbsp.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2mfffbegh.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qnwzqsks.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2irvdttvr.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2friaiavv.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2eklhjkej.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ivrzkaat.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2gqapnvuj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gueqvklk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2pbjfhivb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2ekjaulfd.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2fucbsijp.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ctzqvkvl.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2agcgykup.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2vxfdlbpy.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2reniznsc.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2kuqdfyia.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2otgcxkhx.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2apfyeicx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2cbkzbgrx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2psqlboip.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2wqckxjen.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ztvsmdsv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2qbfqjbru.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2fcyrjwva.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2xubatsxw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2wweppnds.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2hhaeobkz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gtuffbyt.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cmwwxexf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2lfusscww.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2cbttegfk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2gzibnzpw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2awwmqapt.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2hlbqnyrb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2kzlcmgxx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2bfemieyd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2todbnscn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2fabptnhx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ywibsorv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2polaeibq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2jvfaienl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wchgqron.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2uifuilzk.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hptmnxyn.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lsdrgbql.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2wxomovic.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2kmucnwqd.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2srawcadq.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2dkczmnjd.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2lwbuomwh.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ohvivhru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2clqqotzq.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2uoschrhu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2okkqycuw.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ztfgkscg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2ufrgecdb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vvutpeal.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2dpyavney.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2icxnswzx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2aemnqscr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2pbogmbjr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2scrqwgjn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2oqhiimae.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2ytlwnrjh.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2utqnddcb.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xtrvtqvf.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2duzzbzme.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bfsruuzk.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ujogxggu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2xqqveexq.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ffzdfbpd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2aqvqdfbs.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2qlnfcwgr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2khtuxsqc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2bctzhnmp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2dsdhxduj.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2mxibrhkt.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ziupmmsj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2osncqdhh.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2jgrhmlsw.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2fmtucrix.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2bmznqqvh.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2noqflzga.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2jakfwyfl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2synmvdyp.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2uxtdifqh.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2kxhqtxzo.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2hnvxhvyw.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ilifhloq.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ouatmxmx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2yqplodgk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tqjusaey.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2zjbksuyu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2lbqjaswt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2nhmayyiu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2prgnwoem.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2pvsjnzfs.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ajeqvnwf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2lbyhavlx.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2ocryqihr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2kkwqmoqp.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kgtaxycv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kyookjht.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gkmeqnud.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ofyryzfq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2spsgygpm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cpevjxmz.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vxklxxkw.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2pavkejno.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2qijqsylm.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2rleceocy.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2rebaymdo.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2sphpycyv.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2rgjrysjd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tjnnzabm.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2ujhrxlkr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2wplthtee.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2hmtjbbxa.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2ljgbioje.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2eabyavuo.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2nuwhfcxa.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2gujilzca.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2tyblprbp.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2hvhhpglb.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2qhkwzbyn.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2jxvyczdq.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2kupjwpph.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2rfxldudm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2uarihpyo.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vjdlstjd.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2vjozmxfl.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2cpulldzw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2zwqwxgre.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2kehmzdse.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2lgjrzlwf.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2pulailsk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2znsokjtk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2fidsbdtm.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2snnvkfwj.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2lcplqylt.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2syzagkaj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2zhhcpwjz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2dfdimuht.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2ezkjrxxg.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2jwwiyeit.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2fczknvor.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gttgazkf.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2azmlqvbz.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lnrkptrc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ehvelurr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2htsxgtne.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2izvftaff.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2vudcajff.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2gvfvvnyh.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2lgirproa.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2yckyokpx.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2mkzqmjzk.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2fvatmmvd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2nrrplnyi.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2avazrlcr.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2xuovfuis.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2aazqdbkv.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2kfsswfyq.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2moacsjob.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2bghytdgh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2bxhawyye.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vxamepmg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2lihzbphr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ceqogcmz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2dhfvhtte.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2aehdizkb.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2hpvkqyao.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2rbudvbox.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ezqmwrkw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2qehidxxf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2xtkuxdgi.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2vbgatfgc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2tvzkuail.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2arwgqbha.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2uhzjhglz.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2xiwourvs.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2deyjgbkp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xhltpnpc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2ukjgrrpf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2twkkyder.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2snaaniie.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tiarebbe.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fvomzxdb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rtmsyjgy.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2rlexaofd.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2hfeubbxc.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2bxppzgpn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2pxpenumy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2oidsnzdz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2slyjnuab.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2wyqdkzgl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ohkwwiga.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2fslqlmfp.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2aoxecqar.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2evbgdafn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ygzlfwug.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2pujndpdk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2scnexikg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fdtgyrtu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2baxyfzve.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ulhsrxxf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2xjzzdnqv.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2zsyhcbzh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2mlumyyif.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2lrtxwlef.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2yndkkasq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gdfokpzb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2acumescj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2nsvxetkh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2vstsloqh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2dxhreleg.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2xbrtbwtf.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2udvdoffn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2hnlfgmgw.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2wijqbfvh.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2xamtcyst.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bwgywhim.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fjgsovmm.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2mnkrsncd.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2ewofwzfw.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2nofonolu.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2mzknxdlf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2lqfetyum.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2txuhzhuh.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2mchqtgni.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fbcgevhe.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2xqkbwzfu.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2qypbauom.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cnzkhida.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2lwwgvdcx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2qztggdgs.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2mkmbzhvk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2amvmmltr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2claozqkg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ycvxndzr.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2pdtyuttd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zqktdisz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ajwjagna.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2gkfgqadq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ieyvhnfl.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lzuqrjlj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2lssopiru.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2aheukfwy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2kiouvvzo.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2gbltddpn.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2shtnudeo.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2koiighva.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hwfjyfnj.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2gfdirxsj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bakspzda.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2baicvyns.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2wxwhbudz.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2sgenvtyh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2oxalncvb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2hmqcdlbu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vkfftsdm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2owtozbly.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dyzwkpyf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lwvznmpo.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2anstusbn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2hpmoatdi.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2gwjttiyi.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rurjdyip.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ywkvqcvi.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2wzblxpfx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2bogkizai.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2oogjocav.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2yslvgwpj.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2jritvcoj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2cnkeuiea.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2jwvaldse.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2webjgmjj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2fgwvjxbk.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2fobzzeym.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2wbyldayk.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2jgnpkjdj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2rqvmbpbq.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2ozaololm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2utbdqkup.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2otfqohji.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xzlnmehk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2nqficjho.html


<!-- 参考信息 -->