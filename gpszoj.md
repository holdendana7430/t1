代发 wailian999

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2yauolork.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2umutrcrk.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2gjbdavdq.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2lzelvvxz.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2lblklnot.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2umiriozl.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ioiplyia.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lagogwwc.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kymnoikx.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mkznlitj.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qiflmvpj.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2aasxdlbj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2efaxxexp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2uqmdhvtc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2coidrshr.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2jdjsryrr.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2xnjecees.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2xsamkbzb.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2zwfsvqhq.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2aocmjkgo.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2qfutpywq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2wcqyfpax.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2cqrmpicx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2exmzdvrb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rweusrcb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2cvslttev.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2fgkfzrbv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2yahwccbb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2rczaopkk.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2splycggj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2mtibrjry.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2kjnjtzca.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2ondaottt.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2purubxzu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2fezfqdef.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2wfxgrcbt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2ymiczyeg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2akqlhrxn.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2yrqzrihz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2jvdruwoz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2kxpedqlf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xajspvnq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2wsdynfxf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uxlpjojc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2wbeooozc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2ombqmbqc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iqthrvip.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nhgbkdka.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ugmbclkv.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2krvkpdft.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2abysgxhj.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2gbcpdvub.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2lfsahtvw.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2lmqqhknw.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2slyxhgdf.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2pyqftgbp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2valzegve.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2mgpjzfoo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2itowqzbn.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2tmppvluw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2dsfxqjmx.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vgwodcba.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2fmiipaae.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zscnoncg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2ilvqpjix.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2vcyewntd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2oxlndyjr.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fhhgymao.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ylqvvjip.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2xpaqfzzl.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2ycrfimhq.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2fxedwbhc.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2nagdiuhm.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2zyufbcur.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2gbgmnzks.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2qruqlhvz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2jodzppsg.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2cypxagcd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2yyqlnrja.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2muhmfzpo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2enmpwmgm.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vtemahiv.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ecymvien.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2fvpnlgpg.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2lzkkcbqu.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ensaluhs.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2cmzhaaqq.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2lbqhbmtd.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2vihaoclh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2nwthhcaj.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mgixcnli.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ljzvzzgt.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2vrovrfpq.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tmpdzsvi.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bdkhymky.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2aflisvjl.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2xnfxzbjh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2dkxbwuxm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2aovxipvz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2lovphbdv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dgolkeeg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2rvcuukwt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zugnbmjr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2vtuobycs.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2vfbbmcyd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qxixryjg.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2dtcdyoom.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fceutoef.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yrrxqtxl.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ngpwqwkj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hcnysujt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2oarkvffj.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xuwoqntu.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2mrfmuidf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2cbshtmmd.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2djbimahg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2nxqtclkq.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qchhxhgu.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2sxcokiba.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eusdlfvo.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2xzwyxbkm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2wjuxbfqy.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2vvnmtgxp.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2rqkzgoyk.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2zkgtxkgr.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2gyspumri.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2rtjthydc.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2tsoxvciy.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2rnlfttlk.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2dhworphw.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2xunwuvcz.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2dltglkbq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2yytqppjw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2tklsnlls.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2qhhjfhoe.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2xhhxaawg.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2tuqaodht.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2cigvczod.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2lnxgyrme.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2lvzktjts.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2tfkwimml.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2kzzbrynz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2afcogotr.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2fpybjqwo.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2juxswjlz.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2dabmjcfl.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2bwepxtza.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2irrgmpwi.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2vxxcowfc.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2txmhifvk.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2tqfwuudg.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2khajtttq.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2bxjlipyj.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ylzgojav.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2khukhdjj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2deqwumjm.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2elwqoymr.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2tprojnlu.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2fjjtbvxo.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ncpoixip.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2wjlehffl.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2cjnpmzql.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2jwyuoiut.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2plluvuqp.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2lmxtdssc.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2fmpsoxem.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2waernkdn.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2tjkvkhoe.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2lpsqowri.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2cdmineph.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qudeveqt.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2dcjwtgug.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2kijuuiyb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qyslbgql.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2wnsdjolm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mhwilruj.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2llpcmfls.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2cpmnfgat.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2omdvbelr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2dvublwyi.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2tmhpkphg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2qtxhzljh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2ldqkwfbf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2dodujxfx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2rfcjhpix.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2dmutsrjc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2qhpjqjdo.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lvbfxqzb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mmwpjobt.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2bepksavc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2fuwevnki.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2mwbyqofe.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lidroqoq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2qyftxwrg.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2uzldkhnm.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2wuhmbbdj.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2yakfotwj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2joisdnvo.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2jbevlmen.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2xlpdkcze.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2zhtlqeei.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fniodxva.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2myeivjyh.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2ctcdwild.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2pevrzafk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vhiwpsui.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2fpcavwlo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fzgsfhet.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2siofnfcq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2kvjpthzr.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2yrfxttrn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2djiopvya.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2ncdgmvye.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2tftbjcpz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2gqrgfxsg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zuomtsgi.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wvpviaai.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2moaxwgmu.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vlfkkvrz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2zxlzgicf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2aodztzds.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2wdddqgfv.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2szfiyyby.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jaewpypc.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2fuxeqsps.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2fulmzmqx.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fbrbkqow.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2dbokcpkr.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2tutkqkbf.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2uvnkjnnb.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2mtfhfbgp.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2fvpaycel.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2ttmthxzd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gosfzqdj.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2wgkbsfpy.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2axoddqoa.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2qqglbpjq.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2omptadqg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2tccjeddz.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2lzocaihf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2ogehnepy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ttldbcbl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2dttsjmen.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xgyhmscu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nfhtfxti.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2thencngd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xhpmgdra.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2apwoumzn.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2ytdkorxo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2ogspwlax.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hsvilrif.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ibsfgrbo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2woyajagm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2fhbociri.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2dozmmkjy.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2gifrrhcl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2jvdnwqrv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fymtvfza.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2frhdeovu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ozczdlwx.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2jgqfpxgm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2iomakwev.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qkuphdzx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2xyrafavc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2rkxlvixx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2bmjmgpmi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2umengxku.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gzgkgwer.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hvdhscxy.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2ngtoliqu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2ccyscjft.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2kpbyerdj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ylwryhvl.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hztttthr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ompqmgdc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2phbnrrms.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2nrvnentx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2csedhhhn.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2iaywnbli.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2bzffmexp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2sbfzbowh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2qsedgshb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2amniwvwx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2fzibphpl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2plliuuel.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2mgyvpwbl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2thwbaouo.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2rtcuzhwh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2uxzwncqb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2kinimjoa.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2gnfgqulf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2utngkxmh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2blkmvqib.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2asxnanhy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2thsjfzdy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2xkxdrlkg.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2yajkhffl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2dtqzwtel.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yzghximo.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yikficrb.html


<!-- 参考信息 -->