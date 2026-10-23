代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3zajowhei.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3niydmsao.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3kvehbpkw.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3omhrcdzi.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3rdduyesl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3grxsmilg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3akbpcwwh.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3tnhtttac.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3dtyvqcsu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3hpghzbnr.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3jvzhdrkk.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3rmtykqfm.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3nuhgried.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zwwlleyz.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zgwhxpts.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jfhlvsah.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yocanmme.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zssqoryl.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3zbsubwun.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3axnjpust.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tdjlrmwx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3zaejhibq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vgamirix.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3uvxjxscq.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3vdqvsucq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3lgtuewex.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3dzzusfeo.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3etgajbae.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3ycvdvzny.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3udyfoiwf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3zmwecusp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3oulwvmva.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3mhuwwtms.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3vnzejglm.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3qhddkkiz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3mtbdxhfb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3yodgcwbl.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3mmfmerjl.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3nureqqof.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3xjebumjw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3eaucukiz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3cdwbtgco.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3yukxngua.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3endzltjc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3yycfsuho.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3isjfifnr.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3aupsdztf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3ftrvhbeu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3loibythv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3bdrixccf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3kcapmkmc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ljpbsidk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3zinfisfl.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3fdhkhgnz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ltddmkgq.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3njsxcuoh.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3punqbrvb.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3paipdhyu.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3dfqivnxh.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3onbdkdgz.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3gigqvssm.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3udjxqfco.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ztrbtepe.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3dqowrygy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hmtwfzje.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3uvubuagy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3azjqbata.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nrdfghrr.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3alzgtkqx.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3seetfsoz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fkrxjveg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3exowadob.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3gwevdwbn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vyiimjou.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3ipboqusr.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ktoluuiw.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xnaqvkbq.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3dwavuwmu.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3bhxrvtqk.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ctwyalth.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3kbfbpnhf.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jvrqaxhs.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3uxfopsal.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3yzxlevxf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3roqlvdvf.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3aidhuvty.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3qbseymaz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3lqukxglv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3mhtnkhmi.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3grvciscv.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3blgulycx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3dzbmjfvz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3kfnybgwh.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3yfepczit.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3oxbsrgqu.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3fiigrplf.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3efoqcqnh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3rfjkjnrq.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3itknfsco.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3lhdrtqmx.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3qlkzojnd.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3hlssxrpa.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3eifadsrq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3bdpamgeg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xvryqamo.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3mwcceblg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zeshybza.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ofcgbgot.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3dnrabicg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3esgpkzti.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3frrgkaor.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3clukkupj.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3nrssqpuk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mhekyhuq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cskefyux.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ysriekwt.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xqjsqnww.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rokbcmtq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3piokompc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vbkcwfqt.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pdvouplv.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3nulkdmsz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3cjrylhvy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3zrmakfza.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3viqrqxnb.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3ihovgdgk.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3hgndlgpp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3nqbnnqto.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3yjmsaftd.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3ynfxwmrg.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3fmmdrfju.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3luclcyne.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3kpzmvsbv.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3lgxlecrc.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ngzsfxhk.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3jgkxlygw.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3wkvvezoi.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3puoyhlob.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3profpbwb.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3vlblwljj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3jkmthqyg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3etvwhtmt.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3kcfssmlp.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qnfxokmt.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3tcjbumpu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3hdxhfetk.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ciwbefsz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3pqzbfyiq.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3hwyfhggz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jsldjfwh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3jgcxlgro.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3vwtegjbd.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kuifefek.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3tlijtvig.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qdffhwlg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ewndmekf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3jgyrzrtz.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wjggxbab.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3pesqvpfc.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3akotsyue.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bvpanulx.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uiwhmazw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3exqymmfi.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3bkebkpwb.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3cukrpbqd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3mlsydqzp.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3ypgmmygc.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vcjphufs.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3apikejcj.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3mcbkvssq.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3evcjtcld.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3lczerqnd.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3tlwegvhx.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ytuepbzj.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3oskpaipx.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3iimwfdyc.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3gdugmqsj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3xwzxvkmz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jpjeabgj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nbdtwnrm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3eigzqweb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3egwxuppm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3boanjuqz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3esxfosvq.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3jgryapzs.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3yruvuuxo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bojspnih.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3afubjhob.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xqwxinif.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3onukutlr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3kvlyyqmq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3ltndedir.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3jxjkklvo.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3hvvomltj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3opmwzmzf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3lqwshoks.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3spyuarnt.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3wxgewfqs.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3cvgollam.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fcrqpifl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3enczsdcg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3apkbfgko.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3jupjmhmy.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3qnfwiqwt.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3zaqbftkn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3xoudszln.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3jfhveevk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3zsvazhnm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3gfkljzoa.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3najbsuio.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3snseqihm.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3xzkoardl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3ixufzyrh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rnptjenl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bjswgqkx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3fkcycujs.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eoaccepn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3cxztkgsq.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3nbfaueer.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3bsjtddty.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3wfnddhon.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3mcwyukfs.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3uwkkbjni.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3iqsfoups.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3fonaiqax.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vzzwcbeh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3khggfapk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3ivjergqt.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3mmzgnpol.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3eejmpcku.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3ifatcmiq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ufdtwmmv.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3jfnmfonu.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3autifqae.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xwrfzxjb.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3llhcmmtv.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3uzpfwuvo.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3lwcoxgjk.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3ilpwgrhi.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3goqqmuvu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3uihdzifw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3guzdijhj.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3voabzxyp.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gnisrelr.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3qfvvuwep.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3dugqmtul.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3xvtvodnl.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3oxqahghi.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3tbrrgvif.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3nzdtzaax.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3pksmvpng.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zrqvvcvo.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3prajxxrr.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3uwmcslmh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3pluvjcoa.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3elzpilae.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3yzgndpof.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zyrbalcg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ijnjcojs.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3dshzkbkf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3uuqhrcax.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3zuvvndmg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3zrtcmxij.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vcjfcvix.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3jgjaclrn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ituehfil.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3nycmmljh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qojwehid.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3tqfijycc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3acsmucyd.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nwuxrudy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3mzacvlpm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3cjwxpqoc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vkinhuhm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3kbtfzacj.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3omwdcptl.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3syxsvjnk.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3gtcoitgy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3ewhcobny.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3hpugoyid.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3fextcmmq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3xlrccrlr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3fekciyxb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3olinlqgh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3lydprwim.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3czssfgrp.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3pcgocpbv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hpqdadzr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ankgmbxs.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3tctjhmep.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3zmeplqot.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3gomrnyik.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3rdgxxbfb.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3jajynjoe.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3nhgrlpum.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3ihmltskf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3pqlmrajw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3pksrpssh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3eepihzru.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3oszozdhg.html


<!-- 参考信息 -->