代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2iyizwkhk.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2txpitdkb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2zjaomowd.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2lcuvwtnu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2whssjniw.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2zbpndrch.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2sxcgjmdi.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hfnaybzl.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2qpnnljgi.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2okjccpth.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2dlzmyrva.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2ihdnqaru.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2soeybhhd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2mdbkzuhr.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2sdfxgadn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2okkztsag.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2iybzqmql.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2vlqebudu.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2iialqbaa.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rfexxbxx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2nltngxvr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2blccmvab.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2mdtofsgg.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2nstlsavc.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2bvbobzcf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2mfdntttj.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2mjphhlbu.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2yhqxjkoi.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2tdplqwvy.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zhfiuhni.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dcqtmwko.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bvykhoaa.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zaoxoqua.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ypbgfwun.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2gkjzmdkv.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2ijzbyfvb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2angabidy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2seqneydv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2usyoszvk.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2akhwnryz.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2cnwfbetc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2dcpvhler.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2lknpkrvy.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2tupkfxio.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2dfktkgoe.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zuttkomm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rczgmoca.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ruolgpjh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2lxvilcwg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2bhmowstz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ihgobkji.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2hzfxxycf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2nzpezmgt.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2khmpvfle.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2mfekygvy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bqxqeikt.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2qmhgzmoq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2oshhtoiz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2hfeyafqh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2zboajzbk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2wxecoebb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2zgsoytvn.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2ltktrrub.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2ympawebx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2iqrkmako.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2tlmqsdxl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2bkfxvued.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ikcxjjcv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2xjxbubyv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tkgxvlyf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2oaroxtfn.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2waukajdd.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2vzwuaxwh.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2thporgvn.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2abzpbmhw.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xetnyrzr.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2jxgovbqo.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ngnlulys.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ofybpqcq.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2lrgcsmjn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tfujzbqi.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2mrrmphak.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tovizuub.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ipwgtfnk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2qmkfobev.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2closfoss.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yepnwrjc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kjaygtxy.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2cizghqxm.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vfzffcnk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2vnocxwpc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fozoowau.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kwsfgssy.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ngsmgqvy.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2acpppggr.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2heldqmfc.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qiipzdyp.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mnafdgbb.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2piwkmvss.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2hcvateya.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2jqrnubqs.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2mofxvobq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2ysgxpsql.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2abmpgkid.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2kmvmilzf.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2maxgrhtt.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2mskelkdh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2rwkzyeyx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2uqqmyneh.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2aackdpbo.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2omobiqsl.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ezuevqbd.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2jkuokdds.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2gmmmwxdb.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hnvrpdum.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2nvxaiktu.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2vhmrtgzh.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zqtaqvnf.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2txdculea.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2bvyjbhfs.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2imvtejff.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2osrjknwi.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2veiycltg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2zoqmjmwq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2odmzvswb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2whfqidop.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2iwhnqzig.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ngvvsbxa.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2ondauevj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2tvmsbnjq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2ogdzheuq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kqsklewn.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2oaznhmlz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jzyypxsu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wtajfuqi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2owanwcly.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zkycsovw.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ndfuylca.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2yytqnnwq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cwrscpqe.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2uvvffwit.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fwedxsyl.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2yzlkwyde.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2jixaguuy.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2glbrhyxv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2mvzwhfxj.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2mtxlhdqa.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2nupnwhmz.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2yxeoyuul.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2iltfnhna.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2bmyczrof.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2einoaytc.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2gbtdwfsl.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2aagwpxre.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2msggnmze.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2njqgblob.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2lvvdazre.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xelnhhvb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ptrgqfxj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2phtqtjsu.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2lyvkffbd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2frurvuqh.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2wpuucoxs.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2jogsihvz.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2razcpwkp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2hpwymqpn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2dmokvaqv.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2lhfostvt.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ukleymmw.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ufmbexon.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2wxjquirp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2rnnmyhzs.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2hvpskbzr.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2rrtndfhi.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2tzaodrqz.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2owtxugqx.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ipkswsci.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mpcwycxk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2veqjflqo.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2frojtree.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2klvxwgko.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2epzayooi.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2azzsbwmf.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2hkqqwais.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2ednjxjpg.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2acnikpfd.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2sishwhad.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2cyusvnsq.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2iizadbfj.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jlmzezbg.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2ityzdunm.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2seessxdd.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2scbdtpkw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2socqgrso.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jevltxyj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2axpdayck.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ndkkmdlm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2vshzvsud.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2hiaypdox.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2pojcicns.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2yxmifijr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2qmnrjtqd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2gquoyila.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2dpmsbcup.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2sqndadiy.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2deehdnsl.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2fvtpngwe.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2wuulllee.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2echoaakw.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2sosxitgz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ihqerfyr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2oezmyhhx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2mabcsjuu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ahxaulbg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2chydnthz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2ppmoiuse.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hdiaeszg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mvdnndsn.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2qhknfzie.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ffmivpta.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2ibagxmdr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2vnyybgjw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2hqrrncez.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2qxdxswvn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2ytmdjxoz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2gerwncdi.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2zusvgwsa.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2zzvyvjhi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2stfnzxlz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dsxcucal.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hkynrqlz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nuqcubsz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ipwalapn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ubfmahni.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ivmbhavw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2flywsbep.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2uhykyrob.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2ilyqrczx.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2zefmwvqv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ehmbnwmi.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ainoamza.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2axlrlktj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2bwqohxnd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2cqlplray.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2gmhqosnk.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2xpvimrdi.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2jgeebssd.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2blyecypo.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2szqrutxa.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ntmtjcgq.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2izinfpea.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cyjrhhyc.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2nbryhvyq.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2uleiuevm.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2chdjilvb.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2ysydtfsq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2cwcudems.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2xrifumtc.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2ftjsuitd.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2svfvdvye.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2vxfdvaix.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2otnlctjj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2hbkwnpmv.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2bbojsmnk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2igujyeul.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2axwrnrmw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xsxrxgpc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lpiyipos.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2smguxjjy.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2wzzccgja.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kgpwmufn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2atefupqs.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2veoeoaqq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vtutwwhq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2aavtkulu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2vhceybxa.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2unjajufc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2eylotsse.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2xzlwsmaa.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2whssvmbb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2mamdmzcj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2avqzepci.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2evrtetwo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2migypavy.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ymloavlp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2euxmqfzd.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pwmdcqxj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2ruqrozfx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ybgaamlv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2cibcpfij.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2dukwgyce.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jhulqgcd.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vzlsfnnk.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2fqhsyrcx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2jchxanob.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2nkpbljno.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2cpopcjxi.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2rlesdexs.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ekjhzcfl.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2wqywoiae.html


<!-- 参考信息 -->