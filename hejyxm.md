代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2lreqgtfi.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2pvqulvlr.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2qgnsuluw.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2ydvvrvtg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2qsdadosq.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2wfpfoiuk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2cgxxxiyh.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2zjooeazf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vanmrtxo.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2zjsfnkde.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2ovjdtkhd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ukpghjhr.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2druocgsn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2flzmvytd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2uphyowae.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2icjbnalh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2pmskuqzz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2ryvriwak.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2ylnqoebm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2tdwxtjmu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2zazcvvod.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2weqxvpyp.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tsntdlzb.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2kemsesaw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2nklzgriz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2unmapitw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2xatccdow.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2iaefvsoa.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2digtunjs.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2gjkaczhc.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2lmsjlrhs.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2hcqxizcy.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2cgblmmin.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2bfktrtbb.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2joisvzzf.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2lpbkujon.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2oazppvel.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yicsuhet.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ovzlpkei.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2afgnfaxc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xqovgjgd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2gmrzrqti.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2jcdrlkbz.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2mfyraqok.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2whmvrrcy.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2yfhzgemi.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2bwrzwbhs.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2uakkxbez.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2tznmogco.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hcunqrzb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2nrwplety.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ftemjtmy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2iqwxjkwu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2qrcecafs.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2brlvitlu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2aavawcrf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2bqvrxaqo.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2pkjhvgce.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2lwrubcrk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2ddzbsfzj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cymbjqxf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ngcqypma.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2nsdykoca.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2tfmabimu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2qjsuygkz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2lovtlamu.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2ldlmasfm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2smmfjqor.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2wtjcvvdg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2evclqqgh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2mdmifrpg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hbxytoly.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2xxkebopo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2sqxrajpy.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2sugyzgoa.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2kvlzohif.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2yuygssqf.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2udbgjugg.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2yvgyszbe.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2winpfgio.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2oqvierew.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2gyzlejph.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wsahhzbl.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2fohtdnzr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rqlhwcda.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2nixiqidt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vqxbwxib.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2jwssshsj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2zwopuhvr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2roihjkeb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xqmjxlds.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2mflycugn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2wfnokpjk.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2cxxdfosc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2lliehcww.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gyxuwxmf.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2fqachavk.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2mqeekbbi.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nksxkxvq.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rpsugvrf.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bgbfjcak.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2nvoisofu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cqvjdryu.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2zetwdqal.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2jmbzilev.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2usbrwfas.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2sdqnuzkb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ggvgxhtx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2zdozebte.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2fnteotsn.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2quppiwul.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2taimymok.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2tcvbyner.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2xugrdohq.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2wobcvfzi.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zbsfcemw.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2xhfuorhr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2dfisentb.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ogulqfpy.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ovcldmts.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2wwqnzytj.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2efqsywhf.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lulborhd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2qplcwubb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2osauswpq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2mfwavapo.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2qpcorthl.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2knppzrox.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2xghwjkfa.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2choerbjy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2puaoazop.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dzhglrtm.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2ukeztilw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2onmdvyxv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gcsnioln.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2trsabopb.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rfzyrvok.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hcyxwxcy.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2jxodxbfl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qffintwf.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2abvgbvjl.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2orgnmaku.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2ekduofjs.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mulpgosj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2olpciyuq.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2rylhmfos.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2kiqpjtlm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2pbpytlgw.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2fgawvdqe.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2dywayyej.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2vscpqmxf.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2tvaocprn.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2bhxtnywg.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2lmckqayy.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2filrlwlp.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2knjmtlox.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2cfhmrkog.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2dorxgcot.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2hqyledoh.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2hzxtbpdz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2cjihmmet.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2ddwsbigz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2uueyylhi.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2fmmrehoq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2vuqlmrol.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2sfugvqvx.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2csxtvpvu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ioduayww.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2kxjgufyt.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2nlvpeaio.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2pxfqweve.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wvgpunqa.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ydfihtty.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2gluyewou.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2taubcuur.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2bybmsreg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2qviadczt.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cjuqlnrs.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2yejyesfp.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2akprisje.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2prpxucyu.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2mkvwsmvx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2nyhlbrio.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2apaqvcbh.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2onduuevt.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2zelaarrd.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2fnnsnoou.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2otswcdmz.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2eyeubzvs.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2yfpsrnnq.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2iksukiin.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2gsusynro.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2gucqomci.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2jtfnrboi.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2lucoryor.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2srgucfhj.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2eddxtwnl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2jdzwqgho.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2tcodefmz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ugwvccsy.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2khzysosy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kiaaglgf.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2hwwgxsnq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rqlerbfo.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2ucuwhsbj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2uvgcefoy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2nqzdvvdz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2rsuiejuj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2tuucatjw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2omgzsjzd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2ejnguump.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2cvpyhvzn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2mcfiqxdt.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2olcrwkcb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2imrfvbdq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2mrckcjpx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2jalkrumj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2lpdpzoor.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2pftjpcnn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2eamsczqs.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2watpepns.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2pafdznmu.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2auonhkts.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2aszyobti.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2ytyqqguz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ibfvecql.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2zffpwoco.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2lzkomacb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2lczanjmp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2kqevgbjt.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2kuvidjfj.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2gdsiqjgj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2cthmrfkd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2auezuhjl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2elmatnky.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2gwpymzhy.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2jiuguyze.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2lhjrxohb.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2nymjzaxo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2iwuodwrs.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2azbrjnzq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2rnumsbdy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2fpevxkfd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bjfcyesv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hmqljanv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2uardsmsz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zktgnltn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2zfscplev.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2sxdrauct.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2plwjqklb.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2dfhhzsfq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2oewlplfw.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2nzhfjpcp.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2segoplpq.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2ddatgtjy.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2lcarixmy.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2mmwkpqzb.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2wkgbleyv.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2xfpyipox.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2fbxvwurd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2kekxneuz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2peadsbie.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2amwqtzzu.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wzzfrboh.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2iifrvwee.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2oqbsrmby.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uhvhtlnl.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2kqxhfbvk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2rcgwtsgo.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2tegaxwnu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nouenzrp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tvcfevnj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jvucxffv.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2rtzdanxb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zhvazjgl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2giwdlpjd.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2noplpvwu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2fsetpogd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2vnmsvndf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fivvdiaf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2oaewpylj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2uujkkvgi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2hhwdutzs.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ttnsiaao.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2rrrjgzyf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rqzfprsd.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2aqpuopnh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yoduhhhv.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2ngzldtgh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2gvygnxfq.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lwllwhix.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2nadjxnwl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2jbzkswxo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gmbxgirc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2oopyvyzb.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2imhsoskl.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rvivesdo.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2lovzlgwi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2yfenvjat.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ubrqbmfg.html


<!-- 参考信息 -->