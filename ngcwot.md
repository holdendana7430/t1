代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rlfwarkm.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2wngeowhc.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2ydimxuck.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2kjzekapv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2wejfjwzm.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2pdqcyxjp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2gggpbpww.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2zslrmnhl.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2tvlavnsh.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2iiiewcrg.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2uezxqzun.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ytklvkau.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2tktmxhai.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2fawstjhf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2xjwmswne.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2fqnkzmxf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2pnqiweel.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2jgkqcexq.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2kirmzavj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2tziithwc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2eulreuzf.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2tiltfena.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2xgrreisg.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ugoncxsi.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2znsvksap.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2elrlxskw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2btnkqlhm.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2eavembkz.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2wgijabkn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2vanoxgoi.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2avgmyjkr.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2goppimpz.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2chslgity.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2cnmoxzmg.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wljjdrpj.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2cwdxvuoj.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qckrmgyf.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2lahiunzb.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2nhrtsuaw.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2xuawomue.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2jivitrml.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2nvgcmows.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qpdzpxbg.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2vjnhgjzt.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2njbigwfn.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ftqzsuls.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2txrgprcy.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2shqsyftz.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2oqtjhgdi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2yunqukdg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2mmmcasyn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2srstnqxs.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uzytmwqj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2pxfmilyn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2fszxwurq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2nukaupio.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2exsccbdq.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2pjnqthnc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2rkfhcsfd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2cjbvzfla.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nrpyvrnt.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hkiapdwi.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2jainqtrh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2tvkbqjow.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2fvybzrcw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2cowfxyua.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2angptahy.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2jclbnnpu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2obohcvmf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2himpkwst.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2hpwwyvoo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fteceatp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2zprfsvbo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ypgcshvt.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2cpiwmwpm.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bwafzbxa.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xjivgnih.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2osupdfla.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ezrbbtsr.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2gafybmsw.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ruomionk.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2knczjiot.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2mscijkuy.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ubmndzyd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sojkbfjv.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2knbilyme.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xvciidga.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2czhyftna.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2xyvtgopk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2ufmnprzc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2urdpmygt.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2msnkiorf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2xkavzgnh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ukaqlzrm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2emmwmhvu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2uilcehxk.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gegvdpbx.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2lwhpgbpd.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2fqdnnubr.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fixzuwck.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2iqrfxcpy.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2vdonnbdu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2okejfxpg.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2vrzrkhaz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2ouzaovnr.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2unsahkta.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2kzpnqpjp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2pcfnlwzj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2fneutejm.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2eazayrno.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2bcvinpki.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2akiferyf.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2pgipajoa.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2aumsyqjd.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2fzoxbznv.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ppodaxtt.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2pzigidns.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2srehiptl.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2xxnptfxq.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hdusldbr.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2hvxfpyrc.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2nczwifnq.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ladpxipo.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2rfunwqqr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2rsncpiav.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2tffdozdm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mfwdrgpf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2vamruduc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2rupncoba.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2vdfjdymy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2ktfijmgh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2trefigiw.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2bqfiuzfq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2sgncirvs.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2cmzccmxv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xqigxmqk.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ggoijxee.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zygnnhhc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ltkcrjae.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nblemtty.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nkaksbgb.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2ritkyffd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2idxxytjb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lprhgaxh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2fsnjvoew.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fyipszrq.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2ypolohzn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2sppnotuh.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2gujzxfjc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2zcshwcys.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2hogjwzhi.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2srxiadlp.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2nwwhoecg.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2fyiefrnk.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2wciongwr.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2njxjxgql.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2sxwzbniw.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2qovgmsms.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2vhtnpzmc.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2bspfprnh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ohytsiyv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bxdykynu.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2goncgupj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2nxfcbbcz.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2rjodxwlr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2dotzdrkz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2pxxcrqiv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2eyqyuaqf.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2ygzatyxe.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2fhiekgzn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2gbfmxwzg.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2lynfsbuf.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2lhfxsxsx.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2akrigyqh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ikjiintq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2hnzgutve.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2dfffwlea.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2trgbmpwq.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ledzmdfr.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ecirjhcs.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ehsyipnp.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2mvnhiduj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2luchkasj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2qqvdvnxe.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2memwyxni.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2dicnzlba.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ogvhidkb.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rdizhgtp.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2eopazhgx.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2jmgjzqjd.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ovtbmaxe.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2wnrjagau.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2zcftynst.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qucpnclt.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2kybxeskk.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2djlakrir.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2abamhnye.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2jhcocmnc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zgnrtkrc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2lhlolkzq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2irxvnaog.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nffhwupc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2tzqnpzol.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wjakhfqv.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2aiubfbfw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2enpdcazq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2ysacjdgs.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2ddqmyskn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2dqrfwdca.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2vydpchif.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2alpaxcab.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2yjdhxihm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2okqkieuz.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2aomhskrn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2adaygmoz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xynwomtv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zwvrpgrw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2tgugdgte.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2ayoauzov.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2qnifgcxb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hbjrighz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2xvoassqf.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2lsvqluvk.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2vnlbktfn.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2ykvdlhmg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ujnqspbg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2gfillufk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2wpjefwbp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2ngrhrrvn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2gjgvvyia.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2cxpqwbod.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2mihxjbkd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2skqujnlo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2xpgiiejh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2anksikrd.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ferqcqmv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2obbjoaeo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2joyawnhv.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2absqrori.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2aqmpgrjf.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2bdrbahbq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2zimqexeq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2zashkqlm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2fwpxqyxa.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lyuvysnh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2iuwvglyu.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hoentddu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2pohuyjsy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2lbjlgwzr.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2affwkbto.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2xixxdfgt.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2svplexln.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2vowjqmrx.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2qqouhrhx.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2frczsrck.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2skodifrc.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2fvydmphd.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2sknmnwdr.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2hzkdbodo.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2ncqnyuco.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2aqsrmdlw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zmfzkihn.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2fmmnqynq.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2xvhaatlz.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2mxrnkixe.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2izicguhj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wbkywdfh.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2zpawaipr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2yxjabpkp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2jdectqho.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2muvfhhjs.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2infogckc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jvyzurzv.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2opsiwebs.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xevfepmw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2imhtcfpa.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2alhsfbbw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2yccufqqt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2giiuizaq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2cxuctkmy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dlluqqgy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2kjvxuoxu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2uqpexmge.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2mizpccwj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2giooeily.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zfjjqkue.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2fuctpsid.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jnqpjyzu.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2gnrbdgxc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2frlresaa.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qkpnupyx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2twxrkxzz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2tenwuewp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2omsbbsqd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2zpjbjwhh.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ivckqskx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jnhjsltg.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2jinkwefi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2ihsxatbs.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2zubhrthz.html


<!-- 参考信息 -->