代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3eosbjquo.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3onayupwe.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ivopfvie.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3puuskpha.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3gmquavuf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ldgvitzx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3cdmqpfna.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3lpshvzjn.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3okkmzvqf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3dhoaecei.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3xljknoef.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3wgevowzq.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3tophygtm.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zongvaxj.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3wgnikjse.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3yfbacmuk.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3flemimbn.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pcpmwqyy.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kycjnbhz.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3aitvhbmf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vjkjxgjf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3ssngjgdq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lcnfhktg.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3wnjpwugm.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3fjvdvsbm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3khrxuamt.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3uzwmdbkn.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3tbduklss.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3asxfhrot.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3gajgdrej.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pkyggveh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3drqiqlgz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ugbyakji.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3avzppnyt.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3iznlgdnh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3uyqxwpxn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3whirzzgj.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3jyowfuyi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3stozxedd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jsgwzbrl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3usuhgaue.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3aesojeyj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3mejenhyk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3hxhafrao.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3eydwghnd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3kmnmaruo.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3anfszehe.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3rxaqrzze.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3yfpsxaxu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sxwmooqy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3nczfyiai.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ajvtkepw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3rihlafsn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3wmfjvumv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mqiulmgk.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wxeqokpr.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3tgdyofxg.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3avzjmmzv.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3iqwtaceo.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3oxnjfsjz.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3thunufeg.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3jwbzyheb.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xpzztvtb.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3wavvbsri.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vzntjfab.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3pgddposf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ovgbgggm.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3widfohep.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3kacrzwxk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dzxlhhke.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ocqxehhq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3oazxswxb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3hmefovtm.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3crafcsjg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3wtvfgnut.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ddvhytux.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3jmmiwutg.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3nhaomtjm.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3iyiahckv.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3wlvupyoe.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rywbwrtz.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3mcdhobbj.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3roswibpo.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3oyphdriv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3bkxwvfhf.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3bmupygci.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3ajtadrir.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3eqtjbsld.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3pkftdacf.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jlowrcat.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3jiwzipxo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3oblebcya.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3qllswmsu.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3rtkmlcwj.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3pbxsjlyc.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dcvhzpyr.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3xqvbidjh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3bswkuupc.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3kcxxokie.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vmoouvoq.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3bwsmujhi.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jnavhbkd.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zcrhsmtg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3xidsbefc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gqwtnzqg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3yzkmapza.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wzzhehsm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3clwhzutg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ggtxfchj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3fqhsvrvw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3haoczghe.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3rttuvdbm.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3imtmezjt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zbwphuzk.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cxvmskxc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mqkfubvn.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3villqvvm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vpqoysfq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3oyhmwdru.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ukrdmyoe.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tmqskygs.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3hweszcqb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3mlphhapp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cheblerx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3qltjrwcu.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3ccgnhams.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3ygdzrmtb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3fsngvmhs.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3bmbzfmcf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3oscocrgi.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3xqmzbpih.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3dokozrzw.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3cannkhpy.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3kcwsimyo.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3qiifrsav.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3mvzmjbpg.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3biqnywdv.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3fqllffjt.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3zfclfuyu.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3xcxzzxgk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3nmvdgukd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xtpvrypp.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3dovchdzy.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3uwkabuqj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3kigzacwy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3cgabdtlr.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3jpxnicrj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3zxyliulo.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3ilrlffvs.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kfsltdkw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3nrsemlrc.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3rxfjwlhw.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3hueekplk.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3axprsdas.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3iahllgpd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3aoazpcrp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3dydnjota.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3yigpbhxc.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3iylxrwtx.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3sebedcca.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ejexfdko.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3sxqivduq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3yekczfft.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3vycxmzyl.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3cfixdamy.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3urmajzwd.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3uwretppd.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3qqfatkul.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3fkiutgkh.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3kwovtaks.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3rkdaawsf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3cwmsilwf.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3uptmsulb.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3byyvntur.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3bhnvazms.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3siidmjfp.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3rjapxgyg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3nttgwyuf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3azojzgxv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mucormns.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zgsyeiuh.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3afdukjrz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3vpkqgnao.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zlnjxmdz.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3qjrhlrxr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3htmwgiwp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3utalyeso.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3gpekzmzh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hkwnkocq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ivxqsxpt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3eweecmtj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3mpvcytzd.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3qyqdqjzf.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3lrcryhrp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gsmctbsm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vjxjqqgm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3mjscjdsi.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wywqtrka.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3hoknsvfv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3gkvnqsyx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wvunowxs.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3joijlgxb.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3cgvzjnlc.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3mnpykknn.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3ijmyhqyz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3vngxanth.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3xknmepyz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ybxlrjwt.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3pndtzyzq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3sggpiony.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3vffaanqg.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3mnbtmsrm.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3tapekaje.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vvxqvlve.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qpglafxw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mttgbkvh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3wpueyirc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3jgrwnaos.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3xaxvbwkm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3iickmbmd.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3pgszyavo.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3mxcbswwu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3nrlbkrur.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3kyeazcaz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3bmrmgjcz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3kwrnippw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hbrjybaa.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ihwuwrja.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3nqqnwfgo.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3wnrgmafx.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3qllsaxwb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3qxquvkmm.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3gzmwyjkk.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ssxfaxeb.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3tucqqcsc.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3oqrrggxw.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3myjtpzqh.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3obrwgtzs.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3atazcsli.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3hyipwiua.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3fvbwnztd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cxbwgrba.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3drguhkbx.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3asyenzsu.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3nofysfat.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3yongfaxm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3mzafxhsz.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3oxcxeniy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3qucoabae.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jbnqhanb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vievynru.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3atdpkhbz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nearpnfw.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3bcrnmtaf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gmvrbxui.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3uzmjuufl.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3lspbfqpv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yqfewfmf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ioiarwmq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3kmjokfpl.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3iobdjvkb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3uixwrbru.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3xpvtcrhu.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3zbvsjdng.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3mbjqvmwx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iaxvqtvv.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3orniwnzw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3esztaytg.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3mjsnqdgr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3tqueuuhd.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kfhfyajx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3bycknfbb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3gwsgjtci.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3qtilvgwb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3ibsmazku.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mlmrvnfw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lzczrkqb.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3dozlovri.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3nyuqmljq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3creggdkw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3gvmlpfbs.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eslgqqiy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ozdpekpj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3wbrobuzk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3hmlyyiya.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3ukzguonh.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3cyjbeiyx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3gbrelnkd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3swycnudo.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3vsnvcpfe.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ipazmrmp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3eslkiftc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3qebyzgcx.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3xvocswoj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3bwwvgctg.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3tbwfnymx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hyluqcce.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3kxszylpz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xmubreoh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3uvbusttz.html


<!-- 参考信息 -->