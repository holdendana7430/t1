代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3fdfeaflb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3azhenijj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3ekderctx.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3aqweklno.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3jhgusntb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3kkqqhbaw.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3rhjmgqzp.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3zbmfoywa.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3ejtgzhco.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3oagqkqdf.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3prbqznas.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qrfcdjwg.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3yiwgoszr.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3namlikpu.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xrshnyln.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3oxpxsldh.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nsfjqqav.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3yvlpnmau.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iognxxrr.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3qfzrfxvj.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3ddnhuxsg.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3xlsgrkfs.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3leojwbdc.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qgcxbynx.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3ofdwpgww.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3namkvree.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mxcsvyxs.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vtftgivk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3uncgckoc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3wlofksgm.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3wjuheitq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3rjmldkom.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3obicdrzu.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3oejnxnzg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3iaghmmbq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3tjukczyh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vvhzkcky.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hnelydyq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3obcgwawj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3vhtutmwa.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3phhinrkf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3ogdtchme.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3lqhkzglz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3ukefcwup.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3oahqgekv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jfmfpfxr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3ghgvqlvq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3hyqofkvk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3ecwzlagx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3riwesozp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3sexnqpmy.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jnyxowvm.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3sfxlipeh.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3nieimpfx.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3pshreckn.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3chkepxkm.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3tnpozwtw.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3ymuprela.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bignlkvb.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3kuxovwey.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cfwqapyk.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3akvczmhy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rzmvqsfh.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3enlngixe.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3xbzxmseg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3nlqllzrm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qkcreegn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3duagxlsx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3sugaycxo.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3iffmhcin.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3nhnzrdfc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lnspffeh.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vhgjbfci.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3dfbqmrpv.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3ccxuhkkn.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3fsidtqyj.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3cxybckju.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ypjdkmjg.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vsdzyyow.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3lmssufuq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ubmbwnnc.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ivydsvbo.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3jpttewls.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qjddqipy.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3onndpwvq.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3encretnt.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3rhwilxdd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3lartcdbj.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3chdbfkwi.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ruccylgr.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3lngyuduv.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3onmdoltq.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3ddoaysgw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3tguvqgua.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xbckccum.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ncyhkbyf.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3qxvoskfr.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3wgxfjndh.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3lipaajfe.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3znhtrfri.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3jfmrfqax.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3aufwtkoe.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3frqktuyf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vsqnjtlu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3hrdiclmz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3gjoguskq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3jhwlcxvm.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3kvptwxtz.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3utlrfhcw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3oofqzfdk.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vmtwelyk.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vihhppdq.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3atrmynhj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3srisplqm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3lhtdafsw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dowghmiz.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bxgfgusg.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3sidynsvg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3wiyrmlqs.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3uxqeabqq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3emeupirg.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3gjksuaui.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3bseiinyn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sxxkzyvs.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3gsjqvybz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3llybbsok.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3vuxkltxc.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3jftcljsp.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3dulhyvud.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3tqeenegn.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3aiiebhms.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3xftcbwbh.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3gclyxcyo.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3pmwppvhl.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3kpcehemu.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3olxfduvl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3zcikysda.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3sauzecha.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3rffqwckj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3puypimph.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3hfscrzxm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3fulmkxjt.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3crumpzrw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ifsdpptu.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3berbpwvf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ywyeenof.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3gkwtcais.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3iyszcawl.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3lickekaa.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3fxrsttwr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3nmictjhk.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3aucgudax.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3xmsukqfb.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3fkciwuos.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3dgbrzhxt.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ixbnhxok.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zukrxbkx.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ygvglwlz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3ftinvylj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ltnlcwsy.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3vewetkja.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3kunqhphg.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ghlfdawj.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ppmimlui.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3gipccuon.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ldighijd.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3bzzmalam.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3bssqzvqe.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3gyhywnus.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3nnpezqyc.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3ivbsxkah.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3gfgjvyhc.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3fxanxaxe.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3czcuqpwp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nncjwwss.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3uzqwdtaj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xocxsowk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jpbckaos.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3kynlioau.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3kqtbjfat.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3rmasecfg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3deanredc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3vafpxyrk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3fsoarzbb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tvzqojjq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ceyycktn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3falvlkic.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3ihqpvmtc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3gkgqyjtf.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3bcgowcxv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ohspgjer.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3assiidlw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3pbqmoeba.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3msjejqmi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3tahonham.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3alynqfoj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3lhsgazwp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wmblajmy.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3nnrtjsxb.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3hzxetvib.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3nljqsvqu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3xcwpmafx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ecedjpmh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3dsnvlzbf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3vzkwdkac.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3dfzcocvl.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3mzntccib.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3qolfaypv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3touaykxt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3qjxfslxw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3bepmsofk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nifesvpg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3adlvewim.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3tblglqbb.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3xypwivey.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3pexduoju.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3bjymsikp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3xzilgyis.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3yfhsssyj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vyqgidaa.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3igylyxpz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dmmxgrrx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wxqrzwyp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3bygnxezk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3xvqjkbwu.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3utkefhzu.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3sscfuzqb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3gikgiwsp.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3dqtmqzpk.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3oclefdut.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yysrprem.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3fceeuyjn.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3wdhzevzb.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3tmjlefou.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3jiybndrn.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3gvufbyjg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3owtyzdof.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ocbskfbj.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3tyyyjpsx.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3tktmaqcx.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3cnylinmo.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3iggfyhlo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tpwpxbsb.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3lyxopoqc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3kbddzmjz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qxtsjrct.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hrwsnjfk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fsduinec.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zrslyyeu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3ejuaocsd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3awsumpdd.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mixapcps.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3nvvdilkw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3whwrlwfs.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3zrsezvbt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3rpkoxqhg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3dawvfzjm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ubtipzvp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3cjthjkoi.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3dabgfxth.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3wrllxglr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3knrboing.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3pnznfiqq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bqgjazdn.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3iewzprwo.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3hlzvwlgf.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vblgonzn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3vlafdvho.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ltwozdcq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3qjfredag.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3bchpjjww.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sppymtds.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bcgezcpb.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3aslfkprm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3wotwilub.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3urvqihln.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3zmapajjo.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cscvbcqb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3umdseanb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3rsgiwjcm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3vcisyadz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3qnfitljm.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3jlthiugb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3udynnqzn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3mtwxmcog.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3rzhzzcdm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3fafwkoib.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3zfbnydsg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3bmvcvoak.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3fugbosqr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3pkkxspck.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3mhhvvfli.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3wjunylvr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3ritlsrej.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jnbflley.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3eddjdwck.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3ysqhdidj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ofzoxiho.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3uwcgmrfk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3iodhzmmv.html


<!-- 参考信息 -->