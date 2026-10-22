代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2bhsblgkd.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2rxmegyja.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2uuvkyoyz.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2uxyppvic.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qsrisdtn.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2umymcvhu.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2uzdzmoxg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dzuaiskm.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2xqncyyif.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2eghakkla.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2xsbyldhb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2xhqzbsyd.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2fuweclqo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2rdihrvtb.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2uvxriyhj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2hzywvrre.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2oqkropnk.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2rlrikzfj.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2amnecctl.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ljtdprgb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2sfteospm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ndxzsvvf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2eycwrjhn.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2lgeiynhv.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2mxuuevzx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2nsksvujg.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2nareizyh.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2kzjvfpws.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2giqqtdgw.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zcvjrfoz.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2exyzszog.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2iakzkktf.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nshwmmrd.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2xecvjtea.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rrqjdiln.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2auxoxxpi.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2sfsuyyyx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2pbnwjmsc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oyuoifxt.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2oigsriua.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2itonqnwx.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2wezqchnh.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2ucdkzsqs.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vdinlydj.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2yawiukup.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2luiizawe.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2jllctegg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yzhncnnu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2apryqslx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2ayfzhaop.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2wxpvtkgf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2fzozjuxi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2kymtocpw.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2mxjbvozd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2vdpgklml.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zeezywfc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jijsoojp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2itmfixnk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ryuaxzcc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2vmmhoazn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2zvhgorin.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2vskwfjsa.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2gfbzjvfm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2zmdmfznh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2frvhtdmi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2jezmdaji.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2ymzultht.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hvxpwaua.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2dumxixge.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2swoimibw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2njqyaxty.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hwdfhamt.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2xqqhwfpi.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2nchnqxcu.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2iyqjowqq.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2mduvejuz.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ucatlgrz.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2itmhdlbu.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2sxsppiog.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2reyxyjso.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tzzfjiih.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2urxnjqyt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2upgbtazb.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xjexggxo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2ljoauvpp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2rjzuegzl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2awmbjbrp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lidzgxgj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2usezagkl.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2etwlicwc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2velqwcsw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kkwhtwis.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2andsbhao.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2kjpcnvpq.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2saotsizf.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2rqgifvkq.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2qxxfslam.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2zxtptzzo.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2ehptwdan.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2skhualxa.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2nkjnotvc.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2hlttcwig.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2fhyaxhhg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2thhogdcv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2riffbpml.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2dxqywuhi.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ryjejlda.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ikzwbyto.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2bucjwtht.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cukdvvky.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2rfwyrvnt.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ysnttmbb.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2wddkbtop.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2bmxgtvgs.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2jasidqjv.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2cjxsgiua.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2ctqiaeqi.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lbllgiby.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2cvkefsqr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2frlqpogm.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2bymkredk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2lvifcinp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bdfomhkn.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2jxdoldsk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2iyksicrz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2pgmazoqh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2hsqoyzqy.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jehbdhxr.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2jzeongqm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ueuuygdd.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2ojahrzrj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lrjeujgw.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2trlhwaew.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2plmuxjeu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pwjqxneh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2todnzaas.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jxligawa.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2mqrfcfmo.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2xjnhfbks.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ykifkjjs.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2ozagcvqe.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ewfjfjoy.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2infhhwgi.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qbipgbjz.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2mpbtassk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2xtewolea.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2uyoijccx.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2wfjhwytr.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2rwjrpddd.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2wxqifgbv.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2gqyhycon.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2gfqutzmr.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2saqdjpos.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2imdvslxn.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2nfqgfswi.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2xgnruabu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2ddsrmbfh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fgtbygtz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xuetgmjk.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2lrhywbct.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2boirtqss.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2ckczzyca.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2slsngwyh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2sxhuypss.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2yssfvngx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2jarflktd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2ypkaynyv.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2cbdvacob.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2iiamuxcf.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2xvaxixws.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2dwemceev.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2uapgbqqk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2ragfgrdh.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2csplbqag.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2sfnioors.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2cbejcfiw.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xzgsrola.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2nyidqsms.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2iypvjrnt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2hdvbmyzy.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2eukmneao.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2pvxmpouj.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2kbklfpnz.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2biciuocy.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2nsfhvryz.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2tudphxqn.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2rysoevrq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2usdbltjd.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2martsxxa.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2efdusgvk.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2pbrhwqta.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2cloviqpn.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2pljteoog.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2xpvsmcsf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mfsezint.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2skpauoiq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2scscbzcy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2zfonnjwg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2bawjtwyn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qcrtitll.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2sefdreln.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2ezuugjli.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ycxduumf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2aozuljky.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2checcmow.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2lqbdtmae.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2suwwaqns.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2xvfwbudg.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2kaiqqghj.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2afkgvfnk.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zvamljwq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2xbtwugth.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wvcdbask.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vokgnblo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2hgzsgyfg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2ovieyhme.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2spzhauvo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2azvwkwfd.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2zilweqvw.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2qvpxgups.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2lnbtqynz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2khmmdxnz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2srthgfty.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2arezasjs.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2gafwuccb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2qhexiddn.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2titvitfu.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2sohoyhct.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2jtgxhtpb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2aseemhsu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jrhhrhqx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zqevdjmb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2hsrfepeo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2jlcennjq.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2vdodunba.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2emyzfpvv.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2rquqwsja.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2zlcdjmda.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2lpxxpdtr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2nofbytfs.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2davxfezj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2krjgmxyb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mfomyvjd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2cgszoqco.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2oirsajug.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2lkxrhovs.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2yifffdlf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hryanowo.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2fxitvdgi.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2vmgokgof.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2uovfnluj.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hgziattm.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2ucbxmqux.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2ontvlnpw.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2klyfpnsb.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2uslhsvga.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2aehplrbm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ojrepadf.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2xtxdfbet.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2rauhqdlx.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2akzzwfiw.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2bhvqbnjk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2cccenhob.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2qmycwevx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2zggkoxbu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ljvsgnek.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ihotkkgy.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pplfjdaz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yqzekomq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2vubhqrzt.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2elrkxxyp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2adjdlogj.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2uxzkvppz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zpukzrwa.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lzcsfrci.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2sxqtejsl.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lfjsxxqa.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2hqrdqcmz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2tgomplqc.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2iishpasv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2aiccfovz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lbnrsujv.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2vapooyxi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pkasjirh.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2bgdifyin.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2ywrqorpc.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jgfkvnku.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2uvejhnzb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ozcdfrfs.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2htvexkvy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2rbbqjews.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qpbkmkxk.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hjovcszm.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2mamsjreh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2bfzzobbt.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2nnyayiby.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iyfpkqpy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gvvaqkyd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2yxufluah.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2sdhyphos.html


<!-- 参考信息 -->