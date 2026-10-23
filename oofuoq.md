代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zueiseap.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3tupzmmda.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3uxaxpnav.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3yfmrfzpw.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3wquapgwu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hmfufuqa.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3otsaivia.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3uinxwpuz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3spnlnauq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3ijrgsrou.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3uvvexuqa.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3futfkoqc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3eafafxep.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ffisirzu.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ypgjafdy.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3swnjpgli.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3guphbgxk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3xdxprkop.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3zaxkmtob.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3czxqiwmx.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3anbhafhj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3alkyfcjq.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3vbfjosib.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3qrqhixpo.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3sjoluexk.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zeimteaq.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3bwbrzxtb.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3bnchroti.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rkxqpcny.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3zsiouwgx.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dhwjvcrm.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3mwsfbdlt.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3rnkshvla.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3yjzuvtgs.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3laewbcfs.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3nxezyirh.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3gnnhqtoq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3jomyojkv.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3ayjtjywc.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jpvsrevf.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3frglvszy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3virgotfp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gznmeigr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qjzaondh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3thaugfoy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3sxankslg.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3xduzejab.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3zxvkfgst.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3cmekxrga.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3wtuagcxa.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3znostwil.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zwlsjqsv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pkfpkfqp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3eiygomiq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3munsmchp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3vfwvishe.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3vezgqpkc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3sytgfipc.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3vbrsidpq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3vtidotla.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3xtqxqplo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zyrbwkwh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3onfutruu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uwbfnfmm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3jlbdpray.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kkebkwqp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3yrxbgyue.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fmpqcsmn.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3rdnsfxec.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vqseiztq.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ikjhqxbp.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3hunlgyne.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3catxsqkw.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3ushodwab.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ycgxnijs.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3epmzbwjv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vfzyhytn.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3pqiiuasn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fzahjgjt.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yhdctedg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3ugtmykrp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3alpdydww.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3wrxomksi.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jlqeapxa.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3khawsofe.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vynvlkve.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3tfihvidu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3othwcwnd.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3tougqhzy.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3rwrqkteh.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3gghsnrxe.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hglzufhc.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3fcxlmwjb.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jcuxmejo.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3hpfvbtgg.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3dhegsbsc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3sfxuliec.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3exnezzfw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3omcntmcd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3uvygofvw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3plhaiqqr.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3gtrqwtys.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ntncmgav.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3lhsmlgqo.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3ppxbniuh.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3fnzocait.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3lmplrxif.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wfmlglux.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3giwgfnzp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3xtkjsvgr.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wvhdehsk.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3zjgbajcr.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3xervqiao.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3yzctuqgm.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3repdaxmz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3skcqkife.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3fuuulwfs.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3aeycyxhm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3irixunpr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3rwnneksh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3apanflkq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3fnwvsack.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3rqcmcsus.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jjfzjkgu.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3rswsfudu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ohiaoyrv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3psvahduv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ydqpzzvl.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hitahvrk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dtyvgiuy.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fvnvpflx.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fyfgqtxn.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nluquoxb.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3lxecbyoh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3dhlmlepq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3zornhemu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3qamzklar.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vccretnn.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3sfobicyp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fkvsnfwc.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3zjqixnbp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3xaodefzc.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3ttcidzoe.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3qtlspytq.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3dziflbsb.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3yzjhgsfn.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3imgtftgz.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3cuizuftr.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3eufqgnnq.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wbxehakr.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3folzfmhl.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3lodwtvnk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3caadcnxp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3xmykisgd.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3vdzbordd.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3nlgdmmit.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3mwqaizlt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3xemxaift.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3cimqohxf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3phthhlxh.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3gtxmiacr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3paabnftk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3pirhbrje.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mwzvkuhu.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3mjgyffoo.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3dtxpegyg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3dupqyzxv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3sgyhpuqn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3nubbgyho.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vegngmjn.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3pghiqofx.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3hahnosca.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3kwpzfjwr.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3kuxjbqfi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zlrwnihg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3wgnhsurl.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ogabjlpt.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3wtswyvjq.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3hhdymqxi.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3schqlhup.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3jwuvfsis.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3gwdmdvoa.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3kybghari.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3qhlrnman.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3labiecaj.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3zkzjxlfs.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3famfravi.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ydfyrgnt.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3gsmboiyf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3sghrikcq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hdmgbbxa.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3wlnlvsuu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3tsaguiks.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kjskvxdg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3hlmzmjsp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3uytjaymv.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3bfnnnpzx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3edivcfrh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3vwodteov.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3swgvhjah.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gmyrekzh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3njufpnil.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3wzgxovxb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3uopdktxu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3mgvxoqbs.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3lurowhon.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3ugwfopcg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3egrutiyc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3mhxhycuc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3xtbjesmg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3tkldzduf.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aaleaamg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3zooqxwjo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jpmfgqjt.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3xwnokfkh.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3igdlayrp.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3bionwrmo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3caqrheda.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3phmfxosg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3furumqgi.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3vrgqeabe.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3uuvuprtp.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3wahrkbgb.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3zgkytaem.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3rpixwhly.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3xilyrekv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3eiejwlnv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3snvsiobg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3gszxrkve.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3eagxkzhm.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3sbtmmmri.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3dnonmyfr.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3vbudfbdj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3knzomoio.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3lniqdydl.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ffhfeypp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rhmtspie.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3llbtxeyb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3hytczmsp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ybnycywu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3bvudnadd.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3wiqrlyyx.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3ziahyutd.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3lwfvfrlf.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3xgzendlv.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3dzrawsgk.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3kzppmxny.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mtqzjamt.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3pstbmgtr.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3kmybjtag.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3qolafdle.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3lbuhubjz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3fjngbcuq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mnneojhz.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3tuadqnmy.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3gfuguftm.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3zistxqbh.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3rrjbhjkg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jjwsszug.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3earitelz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3urnwyahn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3nwiuyqir.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3osouagei.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mfohkfpi.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3igkxaysu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3mvzzoqoo.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3orwgdivi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3izndtsnp.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3apjixnuu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bearkonq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3maligtkq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3cuhxowyt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3udhqgobs.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3pcqjjntf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3jeujujha.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3adqkyttt.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3wxnyjodi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fxgzovbc.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3scdgxbci.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3suszeapa.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3nzcyauwo.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3rmpfrswe.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3szwrturo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3phtxksme.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3savrjjwd.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3thelijzh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3snwrjgmw.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uegwenah.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3slangwgu.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3vdolaiwl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3jlslmqvl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ntfqbcdw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yoaiafoa.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zyhtdkyq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3myknmhrd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3dqhmshhq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3llnekudo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3dpweymfj.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3eoaligkd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3xcxkcitr.html


<!-- 参考信息 -->