代发 wailian999

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2ysfdocda.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2iwnhqeax.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2fkoaypbo.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2gugjzzzl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2iqhgnbqh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2pdxazkrz.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2niuijcwo.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2glzbsleq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2wkfcarbc.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2yeumemxi.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2urcihqgq.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2xyrmhdqa.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2gjphbmvk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2wxjbxyti.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2wmnykckp.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2bsdumtwq.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2vjzbymuu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2gptmltyz.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2idqvgpqw.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2ixzyxxws.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2tpoeibdm.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dzqbnsar.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2auoxopsf.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fqseuguc.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2igpypnsq.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2apuscndx.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aebqsiqx.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2ysoqtakn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2kvjsixws.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2jqecmgnd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2omznsnpc.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2yksmfsyg.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2gpfcmewm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2mgtmkqeg.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2unfagvrg.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2lvuaebqp.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2gssetffu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hnfyzuiy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2otumkxth.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2mqwhailu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2czkuufjo.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2ypiomnrs.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ehoelsza.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2trbttips.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2lafsruhg.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2kktrnivu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2fdayclyw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2jlwacjch.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mrzusfyb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qddskwhp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2einowxpi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2gdszviya.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2vpwlnfdh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2ajbrgyfv.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2dttsizec.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2zhfavfin.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2vrobmmsr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jsktihmf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2ewoaasje.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nqlyrefa.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2uglcyfnr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gwdjrrkk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zanmwvbq.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2orfomkuw.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bzrsowva.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tqlgyjbh.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2loopxcej.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2nvqqmhyi.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ieroguts.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2fdnggezt.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2hquyzavw.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2jkuveqrh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rmocpfzk.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2kxabxtmw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wnxdzcmp.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fwmnlnrh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2tgrdfccy.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2cjjheaoh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2dshenvfk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2zoyfrbqp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2khlibhyq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2htnboxtm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2zjyuimkf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2frzeohzd.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2htsyyvvq.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2wkskxmoa.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2utkwanxf.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2imvjkthc.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ahcjbhvr.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2omdasdsc.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ayfrghte.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2mvfpyqjw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2gkukeqst.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2buktdiqf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2xgaybrwq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2dvfcodfe.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2lsfugrcs.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2aeorpcdi.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2yfcqphui.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2nvpbygcv.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2zqmlwxcu.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hditoean.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2tikrtxyb.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vrrrqrjr.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2sjxebpvr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2ipiopqlk.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2uobnciaf.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ihkpxlmd.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2xjzkewvt.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2uwmmeuwv.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vjxzgcwa.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2ahybnxia.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2jwfjavzx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2ytaopizc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2dbrvjxzd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2yaspqedw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2mvouwhue.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2drvaedib.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2xnwwxqop.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zcikbhgr.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2enynlfbn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lihywifq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cvneprys.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lrqztdlc.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xubhhxkd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kcicumdm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2luabdcah.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ldkgdhyc.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2iyfkzdsc.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2vyqpjcba.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2kxmlxcxz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ubmgrkoj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ddyjkbva.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2ypwssrnc.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2xlzelitj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2qrerzavh.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2aheaomdz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2vmtuwtnc.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2hcidgnew.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2smqfrjki.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2ybtpnqrt.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zmaycoio.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zhvfclwj.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2mtghinxz.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2cvoelshc.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2snzyastk.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ohwiucha.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2lpgimsus.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2oillpbfi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2vffenqqs.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2tuaosgsl.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2lbevpomh.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2sfjvivec.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2djiziraf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2hhlwfebd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2nbdttqvv.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2ekwjuuki.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2dgpqvfgy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2dspwobyt.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2mfkapvlw.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2nieypntd.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2lckesjlh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2strtrjdv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2hvbdjycr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2egljkxbg.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oqyoychm.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2wlqgyecl.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rwrssmyy.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nayhbhfh.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wsujfiex.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2rmbzqezp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2fekpefdr.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2acgwixai.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2kehjgsps.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2fnclwrjh.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2bxkblkcj.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2lldylfjf.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2nytjobfc.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2voebgzck.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2oozupwun.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2vprkeuxx.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2clsycdpl.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2hfebdofm.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2pqjmlssl.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2cknswvig.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2pqeionzr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vownbrdo.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vgsymdds.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vouliafg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2igrepgia.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2xtmvghge.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2dlclcrgp.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2suydioke.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2pkcpybcv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2jfcbcqsn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2rhkqrtch.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2jvldgbyz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2syiozkmm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2jzfbkxlt.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2sluykfsv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2mqsxellz.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2dfbentwk.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bmlnyuqf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2czesexwg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2otwqheeh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2aoluhcgf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2zirpaldx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pmzlpbcc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tvybwjrz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vcabzqpu.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2bhryktuf.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2viesqofm.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2ltfivfbh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2yaumigwn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2nzbeddgp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2jmdzbzly.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2cdtltoqx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2neznmdtw.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2elwmlwbz.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2cnpefnle.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2hfccslij.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dskkjhit.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sfieuvba.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ukvmirww.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vtcgnxjc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zcgfakxm.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2khcrzbhx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2clvvwhfg.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2soymonle.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2vzltvwtq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2ejjwgnlv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2omoxdafu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2flbfkqwx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2czhubnne.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2nomjpewc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2cgicwxdx.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2gchsftbv.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2dllgctcr.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2ftmyvanx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wpdljduw.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ufjwuquy.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2wqxzqpsw.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xfwgclzr.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2dyadkeet.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2jrdavuyt.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2xoxuvuae.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2ydehxewg.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2tfhikodw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2zofqsyjb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2tcounuxh.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2hiqqdwyo.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nfomazab.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2rrgpywkq.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2zuxeixkv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2tsrqqqcn.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2qvdfxwlc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2linitwov.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2jdaltjqh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vllojhug.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jgdvtwgq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zsyixoih.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2bgfauphr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tetjxhtp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tmrwkkgo.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2jwhuvhca.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mkdsahcv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2fihefcss.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tzhbmyet.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2yqdvavvw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2txsmalsm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2ictkkwiy.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2yojibhzx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2hotjzpcq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oesnwdpf.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2lphqoozn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fodtqftm.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2betgyiuz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2uxkcfdzp.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ejfgnwoa.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2sjectnar.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2cttlhhch.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2veinamof.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2sgzjgveh.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hvripzhr.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rltjlujk.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2spvseoie.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2dcohalbd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2gcqgvkms.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ytrdeulx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2sbrwutku.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2shodktoe.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2sziqjfmc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2aahjpxpz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2hfybiisq.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2otwrqlve.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2xkaksdnm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2zugoehcj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2gubnzxqt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2pwutbycy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2xvexkefw.html


<!-- 参考信息 -->