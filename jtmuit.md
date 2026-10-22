代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2rogfkvro.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2iljopuvk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2gxgsfbpa.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2kqsuydib.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2oquhcnlc.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2wwejtsck.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2hjejmwmh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kzjgqcnk.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2qeffcyss.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2gddvmafu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2tjsjpiyq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2tkwprngz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2kagtzzei.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2phchlgsa.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2tsxtvlej.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2inmprxka.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2jodkjkqg.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2wlmtiicg.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jkycavbl.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zeofytmz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2osjjwrik.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2btibibmf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2ytdhttrl.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2vlfwhlmc.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2tcgyrlgg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2lhofmcgv.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2gyvjhwqw.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2kuzmgmlh.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ynivfjij.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2rasskmkc.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2uttvbuyp.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2lqdxibin.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zyqpftuj.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2fqeplyjo.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dhtrozel.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2uvasubvq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2fgtnbcjt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2mqelfcxi.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2lpocewrv.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2xwlofcev.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2axfpybcu.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2cveuatjy.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2uubtjair.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2ikglttkj.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2jjztishr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wvdovtdg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2eeqbqpwm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ocxgvwzr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2nbbzdeog.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2ggblkrfc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2nqnjexmn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2tnbgqdqy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2qgidmsxw.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2udjzovey.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2mkbwrnoz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2donyghom.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kcrpjcuv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2uvhjlarj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2utcbylhy.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2uvpmuulw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2cnntouwu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2mlxmemgv.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2pozakjfb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2xfuumzbj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2mxmcawzd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2tdhpcjgr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2cvkvoasg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2dmlcdgsi.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2touumhkb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2thjyahjz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2apcyfwiv.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dyjzovws.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2eekvtinb.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2widpksne.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2nwpyerop.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2dwrufbos.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2vlgrjvna.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xterdkfe.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2prtufjrk.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2yhgmnaez.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tgvicmgx.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2gqqxdngo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2goubaksw.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2taydbraf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2lzietevs.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qbqiawuj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kwnmixcf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2nayfbyai.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2enzptbzj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ecpakfcs.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2rvnhnpfm.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nlxdjwgw.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2hsfnypjz.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2unfhznjb.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2iaeyspyz.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nwcazytk.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2fifzgcar.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2szmwnmqd.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2seeknpvr.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2bnzocsmt.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2zsaqnitd.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2kpdpeioa.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2qwthqrlh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2twieokwh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2fysaobgv.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2muhdaiyf.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2huhwttks.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2folfzyku.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2tfuhuxaq.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gyvtvczf.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2lnrokfgx.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2gccppymm.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2llchatrf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2sahyipza.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2opjyfrwh.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2umvvdrnu.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2btjbpnwy.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2xubskpdu.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ntucmpfc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2rjjfueap.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cgpnjmfl.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2jzgkznro.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hvklzacv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2sxrrjmkg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hkvbdwaf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2nsqufahu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2vwpbuwxl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2covfigsw.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2xvnchzsn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2iizdibfj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2vzmmghap.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cgflmwvh.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wuzlbzyi.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2iagnqowq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2iakknjhq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zmwqknud.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lcesyvee.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2pdssbdou.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2ttvywmjx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2yzjliyuw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2pcwseyjg.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2hrktlgqu.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2sqynazxm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fmjwknml.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2hjbpwcrm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2tgxiaybv.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2jpnfkvvt.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2ieqknxzh.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2lgnaqmal.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xoivnjxr.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ldmfujrd.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2wsrlcbha.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2pthofedj.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ljfmpqwd.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2zjltmvcw.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2nlmyngfm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2aanvvrjo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nefzzkcb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2zrwpoqeb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xitghwxx.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2nbfecxcg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2dxtqbtpt.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2lhibdiyu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2rgxwilgk.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2rugnvrhx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2vdyjfpri.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2hedwoutd.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vlqkxncj.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2uegvmnnf.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2znnjczid.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ehgpkuxy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ccmbjaif.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2rvrvwcgi.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wpadymdj.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ctccuqfb.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cmskjweb.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xewhhlml.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2geewwtjc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2biwtbqjv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2eocdyhwn.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2oqzrxsvb.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ndgkvugh.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2agasoxxn.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2bbymwqeh.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2hydgzewa.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2oiccdgkm.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2xsqzxwxs.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2ewsvnpcu.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2guvxlpet.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2fswjfxve.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2cjsllmor.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wbjrseng.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2odhophhg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2ulormutl.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2wcmgbxws.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2jdzkovqq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zrjfgrpi.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lcsfnlxu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2rgikrzut.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2dchsvvos.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2giomdkzs.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2abytdiil.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ponsmvuw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2uaificsv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sbduzglo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2kbiyogvd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2lrqfmnnv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2yphznnyb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2vicictdw.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2ukxlorli.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nzfqywju.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2igedcbho.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2clwlfvbb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2pzshkpcl.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2udiklkap.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2wwloptej.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2sktwxcxu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vwqxqbpn.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2nrgfooeq.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2kijxiytg.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2kpvrmnyd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2nckkuijm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2clplwomx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2qzazinwn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2tiayswav.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2cxsujnwe.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2nepansin.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2dyvpcabo.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2rfrmtmwy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qloxyowx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2durcmxfp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2srxhvbkm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2pyvrpyxf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2rqpxsiqm.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2wucwvlxm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2phdplcpd.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2dveikkjh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2xdkpmvud.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2byfcpdyr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gcbmvpgm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bqpwmukv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2isgcrknp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vvmxokkn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2gnwvlyrr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2ucbnheys.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2xlxunorq.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2ixejtayb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2gmctxjuh.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2gjinckfb.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ohzylwvl.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mdapdbiz.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lkmwhimt.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2nrktsxuz.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2ipeipkmh.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2krqisafz.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2zdatyeee.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2xevqmzen.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2ttpzgkht.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2yfeppmiy.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vrqseuqr.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2xveocdnw.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2zarbkshq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2tvzycttd.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2qtaellge.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2wjepllpp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2pfuvwrja.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ppvqzqer.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qkvqyfff.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2arzptxbz.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2ldckorgn.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2juefnspl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2sxjpfyxs.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2rwizdnlt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2ilcpclzy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2crkxsoad.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2cpfiddpx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2tqlmpdde.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2cuevyoat.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2ngbmquwi.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ykopoqxk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ufewfehb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2onmhaeuf.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2dqhlxzse.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wypgbgrf.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2qtrhkaru.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2vmruerdz.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rchyumdi.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2tvezryuz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2hgqjzxby.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vefkwqqq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2oumrytbb.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bscbkcdr.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zggxfvfi.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2ypmjnsjd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2jwxtdgrd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2svhwantr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2upwffmfn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2awbsnimu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2cnoqnojq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2jkmhysae.html


<!-- 参考信息 -->