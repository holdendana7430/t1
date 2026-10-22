代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rbyankef.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2xjaxetmi.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2ifvyrmrz.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2xjitpcay.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2qgtntpwc.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2dngmiazr.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2zeyouoen.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2vjxgswwy.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2zaustwzp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zlacoxtt.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2gmfbkgvv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2fmsjcjik.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fkzmlvbs.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2xgksisuk.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2hrjvbzjw.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2qqwhwark.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2gptbvacm.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2gxfkqsrf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2tbxcpsvu.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2riqeaxgj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dcsgpbty.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2wrteuxbj.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2vrlyfqlk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kohwnuki.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2hwbkwaxb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2wyujhner.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2guycxpby.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2davaxdqn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2lxkscjyr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2mhfcxtyf.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2upynkzfj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2myplpfcn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2qjohyeai.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2sgfegtqf.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mnobomub.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2vfdydvgm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2iknlayhs.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2jtdnogfn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2qrboodrm.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2zsglujoh.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2ciivnumf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2cxfaazbh.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2jlblwhxn.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2kumkdvfx.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2agfgmfrg.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mvhsqazv.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2etbafiwg.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dlesysun.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2joterpic.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fhdauvup.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aocspqfj.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2afaxvkfx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2sphmsoxw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2hmkikyey.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aojqzrdr.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2vlpodeza.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2jwmpsfaw.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2arxmrdzs.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2kqwraape.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2vqhaunqo.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2tpappott.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ljknucjw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2iuawbork.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2yhxwjszh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pdnaftqb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2bcwhfmzm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2jftnsczi.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2becobjgx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2tnethnzj.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2wwhhkmao.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2tozdtruv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bbxelkhg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2aqmtgilf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lvrbpfxk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2scfcmmyz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2avjsngxr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2ffwjykym.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2rryanjvr.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2rsubwxqk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2pokketoz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2jhljuwum.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zlgttufg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2xxevefgf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2gktsiqmu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2gbjoycmb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2hhjezhdg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ateymvix.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2vxihczfa.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2tcvmkbgi.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2gugeiaef.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ronbhirq.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2eabfbrdx.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2wkxkczmq.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2fypimhul.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2fjbmfcro.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2iikdmxex.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2utnalfeq.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2yaqzamgu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ikdiqkpw.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2nyxdfboz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2ozakezxz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2niicumvq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zvjixwnp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qxpzohih.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2oexjysir.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2vcyeyecp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2toymghtm.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2sdfjlpah.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kpegnuyy.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2bjrodqlx.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2craksirk.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2lzidaang.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2pnyaotsx.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pnofewrw.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dztbhpyw.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2njdbwtme.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2wuhxjzls.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ubhhxtit.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2qkqrmykc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ozefdxag.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2zsngrzwv.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2teabdtbk.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ovxxgxdm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2dcgcbydn.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2pccxoedh.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2liyjhabv.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2qyqlyrvw.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2oecwpblp.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2qczmygkf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2sumlpgiv.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2iqdglnmo.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2bhktbyfg.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2lbnmbpss.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2fpnxtufm.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2duwffups.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2uqjpwohy.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2tmwaeajx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2qpgmtqab.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2rccggtga.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2xmpzxxff.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2fgftjpdw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2nvylzmez.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2hagudsos.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2pdbvgzqe.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2wuhwohrv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rzyxwfrg.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2wyjjhaic.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ffuehenc.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jeyqgget.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gcnkqsqe.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2xjqaldqi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vnffbind.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fdssvdxk.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2xvcirddc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2ksoyctai.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cvehqhqh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2wvaqumrd.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2yvipiedu.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2zxesqmpz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uxdjpalv.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2gzayupet.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2ifenqoff.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2joyzxiai.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2hdkwpyyb.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2wlhstfnn.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2awxptsxw.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2mplcaegp.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2hareqsfh.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2ggbsabyf.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2uvnedqjt.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ktjjxwdl.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2mbdpxiei.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2azhbovtu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2fzwdlrrw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2mkodijec.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2lhhxuiks.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2uvyiecvj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2rqwlspec.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2ajdnkaof.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2djoywcju.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2soelbmtb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2sfwbckmh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2qfsxxhre.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2rkztmmfc.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ojhvycjb.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2anofscpn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xriyeqpm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2zdntbhhh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2rnvwtuqq.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2lmimbzsr.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2seutzrnz.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tqqfhbcn.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2pkudaosh.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ytqslgni.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2vtyktxmz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2kpffqygs.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2oacxplwx.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2azmqrmuj.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2iutsrxkf.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2crppllxi.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2gzlwzjod.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2qccqwcgt.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2woxhlmyu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2dmwftjmu.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2ppxiulxu.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qokksigo.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2ckjoriku.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mouexvnd.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2tbeujjvx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2cqvhfgjm.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ekexdzrx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2lzhxfwov.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mzuhppnr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2axuzjlmy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2nhavbgza.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2innhmqcs.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2qwmrxmro.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2eztuwnee.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cmsxqonj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2sapmopbj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2vpxaoent.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ndivnash.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2nwtgmyaz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2ytoowpkx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2hbccmgae.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2hgcurudk.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2vhcnnrxx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vsziezri.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2uxejbftv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gojsiolw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2tqmynzbg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kmsyrjeg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2vnetamub.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vjkuxixf.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2fystujde.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2vozwarpg.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2ekxiyrbs.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2pblrhara.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ncwfkbkw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2gsvmzibx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2tvpijqyh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2bxzlobwy.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2pkoyurwf.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2vjirnbxr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2nlfehpmz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dofxhjzh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2zyntwdsu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2irkuwgjq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ksjrqooq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2nkpyxzqa.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2piecohql.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2ymrmxpus.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2feakymnb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2vzahexjl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2tvycfolo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2kzrywvov.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2dqogbxrj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2deesxxgg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2gxungyzr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ciezozzx.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2qtcdbpkq.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2stdsgsqg.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2zcicoqnj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2xodiiwxa.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2wmqfvubp.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2vnfauugy.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2vazrnzwh.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2evvnnamb.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2kjmqpdhl.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2ldqtdjpd.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2hatqpazx.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2zijmbxjv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2tajzctmq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2idsmpsld.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2rltdaqox.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2zqzzdepv.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2crwsscup.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2lwrjfmlo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zncxgmao.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2lsehlyez.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2tuwgmuov.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2fuhkqsyj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jeuotoem.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2soywrfoy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2heusdcga.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2gcgammof.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2dujqyanm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2sorzaven.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2sjsdiemr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2xbyhyngt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2pghkhlew.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2gvlnzvni.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2eumwnlgx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2wyhrwyfb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2kqookpbw.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ppinlppu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2jcozjeqt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qntgoirj.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2ympaujtk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rlwntbpe.html


<!-- 参考信息 -->