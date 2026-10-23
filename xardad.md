代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3gxdzeirk.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3riuqnpls.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3uuvzldmj.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pzzbcejf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3kbtfyqzl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3gisjoeak.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3nscviyrb.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3tmorkdiu.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3xyhqancv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3oyeigzfi.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3kbmkcznz.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3buqkyary.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ddelqrsm.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3vfkrcazn.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kcooecge.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xoztrgbf.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vhegfpox.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3pwzglgca.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mbinhbfp.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3efwfnfyf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cbvpteru.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3dvqnygfm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3alxrgbra.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3hphxrowz.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3ewdmfrhl.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3jawihjwp.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3aaxpnbjv.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3ezxdjkui.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3tzkcdmqb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qsrlbcpk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3zpjdwvtm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3kttsenuh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bdaqthua.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3xejzrixd.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3heogbsxb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3utdbjwbh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3nqvhroew.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3tzpwgzmk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3uoyzsjyg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3pbfxhrvz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mydllbyk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ppazxnwy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3uojxmbrd.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3fnylgvxl.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3dfudhzsl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3lgknrtoo.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3pabnjufg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3miadrjnu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3zapioqea.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3loevdbvg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3yudwdecj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uzqqjnuk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3evnzvmyp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3gnizpxwd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3evlgjfab.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3psnlbkrx.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3gsvzfdbs.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hflfhydh.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3nutbotky.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zmlrsnii.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3pnmkuche.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3urzvydzm.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3nhqnsrek.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3uyboqiix.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tafsofje.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3lxowmzuz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yiztakur.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tfmlxcox.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3kadwpqbw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3efoqbdtq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kjfrvqhs.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3tfeqpvcz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3slonlyhi.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3anhsofvh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3bnutfyhh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3eixgncqc.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3jqwugvid.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ciwlhije.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3vnzlrnrm.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zyigylps.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3wvxpvszw.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3gmeiycef.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kuetsysk.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3gxhloxfa.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ywbdaqew.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3bhxtlcwq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3yoxkplmh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3gbewjxzu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3jboyffbu.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ajuhhojq.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3mzesdrhd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3hqolrnzw.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3qqodnaxu.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qnyomtur.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3vygwbxbe.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3qbvpcecz.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3vcljbvae.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3hsuzdrnm.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3fqvicytm.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3djfvsquv.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3hlhhsnga.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3vmnpifho.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3lrbczkgh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3kvzjeejv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3mvlhfrpt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3hjrfpysc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gkjkewdm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3hciilqfl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3natdqpqu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3oiesphyp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qtopixhe.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3unyctndt.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3ddhjpqnm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xujdlpop.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3fsqoufxn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jjoztbwg.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ewejazhu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nearxiyv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3euqnigmj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3oxegkkty.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wcgknhaz.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3wseccpxe.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3bjymxjcw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mumydufj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3xupsyqxl.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3ywstucrh.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3xtsqitbv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3cxpkhkta.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3nakrohgf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3sgalimeu.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3ksrvmccp.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3zzjyhaqf.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3lyhriolv.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ufoucqxa.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3cfsnzsiz.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3edhyzksu.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3kdpnkmbn.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3sfbftgcu.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3kwkaflmy.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3blivydbw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3hnagajkn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3bhwwcsjh.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wdxabkls.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3efdcbkpl.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3fqrdsanf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3ulqbyhrx.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3llzgebcx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3yibbjnox.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3wqquzxnp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3qyxociop.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3ktfefkdn.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3gsismaqw.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3qcpgelfg.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3rfovwrrn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3eozqgriy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3mqqrrlri.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3mkgmkvmf.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dtrpayml.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3easlipot.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3hchxconp.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3lgdqbbfu.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3satqqkvm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vhkyifco.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3olwjxvcv.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3cqzjxjaw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3jlmtdoju.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3tnvbavfy.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3bwutbgpl.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3fzhsuxqv.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3emdeesvt.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3tusxxgib.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3tncuokjp.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3ytwplfkb.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3twmkrylm.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3wovaktvt.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wytldjea.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3pnpagxqb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3hxiqolxg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ujkjmflj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3fatxzucs.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3yvevsmxt.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3moemralp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3ngoquizd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ettjvnqx.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3gdiqhlxe.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3lutcaubr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3dchikegd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3jaxtszpe.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3hvthtxhf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3qlphaitt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3ygbcmamk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3grelizwr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3jdcxbzvr.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3dylfbifm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3etlklame.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fepmeefz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ajachfpf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3gmyyhxph.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3huwrjteo.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3cobkfwtz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3immtecrr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3axrlnjzj.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3yriqeixf.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3tzutvnsp.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3uzgpvplo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3cywxqgug.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3dypiibne.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3gxsjzwzs.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3rxzyykhh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ednowtyt.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3horrlwms.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3rfutbwna.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3kdpvpojx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3elimyptz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nztinhev.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3phwraexv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3lrmcarbq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3giwkokah.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3dxszwwfr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3rgagoriu.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3gvfkfqgy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3shijjdww.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3iltegxpc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wxxympow.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xfwtdwgi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ioauijyf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3oeafnhgf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3djkmcucu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3nombwjej.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3jcpwkfxv.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3zxuacwen.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3yntoeuiz.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3epgccmcz.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3axotwaje.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qynilyza.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3ceozhlnv.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3gjkwgrkc.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3uyncjmsk.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3taaawgta.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3etncjmfn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3wnlazfdf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sbsxyvnx.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3ldkgwwtf.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3zuohxgkt.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3mmskgaar.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3jyfbhhyo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3qvwowlpf.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3xbziwfbd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3kgkzplkx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zqsilniq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3sneurjok.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3kwnmtfyx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3shxhydvl.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3etaqrmbs.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ljgvsjif.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3pvzyifst.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3dpnrqbup.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3bflsyhvc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3brwadlkc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3opvyiztn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ronixobc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3lcwyalnv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3dvzggvjy.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3dkwngtun.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3jgqetlhl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kfpjppqc.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3fquasrzr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lmkijsdj.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3eicwkgnn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3pqvknpwt.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3idtszhen.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3yxwmeitk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3imvtdptj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3hvfcnwcs.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3cjpyiqel.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3avktfave.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3njulkyja.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3cmldbcyg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3mqszxatw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3dsbhoqse.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mtibduxd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3qeghzowy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3vvkcylmp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3mmvoqzfv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3dljsgovs.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3vqpsvqyl.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3zhsbvxfl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3srfspmxp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3zzcxyarj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3rpigabqm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3vxabbcmm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3diypkjda.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3awsnqixf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vkruqzsk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3pvyjbiln.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3coutnfju.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wfjononv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3eamslwuf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3tkwaqdws.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3kdqpjfuv.html


<!-- 参考信息 -->