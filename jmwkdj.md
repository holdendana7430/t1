代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3asbasjfy.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3qimtovfl.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3mfbzzljw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mathrqsu.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3xhkbkiwl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3mabujxrj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3amsiwwij.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3lhpdopow.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3yhgsxjzl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3loxiyndh.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3fzhboqft.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3raphdvgp.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3eajdsbld.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3blkbddhv.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3cawmhtmy.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3xenlqovw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3pfbhlpei.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3cntpervz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3deduiqja.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3ynzimnjl.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3sxrknmfq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3motlwgmi.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3eeqhbpit.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ivfdryak.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3thdvmdzz.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3kwxqphlw.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3wtahplqc.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zmvdtxzs.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xfpubxsf.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3zmqthdoc.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jhspppju.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3rojerqdn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3xwryhkyv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3wxwaukio.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cfqzrcal.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3apptzgjk.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3gxhwbeau.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3txfjwedt.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3adkgpdho.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3eoxegycy.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3wfxpiatt.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3yqgmibwg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3waliprpd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kqcwggrx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3qnxjybyz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3cowenroq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3vwixiafc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3rfkycfwx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3txnvhurf.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3jpredyfp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3hvdlttdg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3dphxqfeg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uyxhcdrh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3uxrhlfwk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3eeslajef.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3cwbzypye.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3qmslkfii.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3mtpwvczz.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3qzutztmi.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3jidvbvxn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3mdvedhpf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vqibsjvc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3kvdggywq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3krupconl.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3uquzinbj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3xqqjinkj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3siitqhlq.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3qtckwmwp.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3hqjedlfc.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3casijpph.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3uizbhioc.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xqkcweej.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3jzirnupy.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3udgguxru.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3jcocjsss.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3zlxjawew.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rivicjcw.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3uzcueayq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nviuguoo.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pjioetdk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3cuyhvxql.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fwypktdd.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sdehinuj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3zwpigwxb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3hyngbaox.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3yrbpcseq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3gsxtdyza.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wmygusqb.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3lyoxlmkn.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3dxnzbzxe.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3udcdjnpm.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3xfssztzf.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3sfrlabjp.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vsslqaxd.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mheqebgi.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3atnhgowx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3zdcrfuuj.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ibjuqwil.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3katwmuus.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3womwznbj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3xoyraxyn.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vjxusfzb.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3wnwgbeny.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3tswugrrp.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3awcqczpd.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3dnfybfrh.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3hjupycon.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3elanfkvt.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3sbjnbsqg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3szfsukcn.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ygvalnit.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3buchjkyb.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3msnbaetg.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3blbsbpqn.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zwcyadkb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3ljmiwghp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3luiekeln.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3ejaacskj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3pexrgmjm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3qezcwhze.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3jxsuosvy.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3pjwtoqbs.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3osuyslmd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tmmzcoll.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3wwwlnrin.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3hnwglikh.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3weesnmyx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gmlarpsf.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3johdffpz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3iterinkv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3veykupus.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qdbmypgw.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mxanghbd.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3ngdvkbxr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3spxbdhci.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mzngfucd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3zsehedaw.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ivsiltvx.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3bgivhfli.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ylejuufp.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3gtldvdxt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3pfpssctb.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3rdqblbxw.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3vxjytotn.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3pjlhfdpq.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3dlmjgmvy.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ifjqbohh.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ahxaukxo.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3frocarxm.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3gabrevmg.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3gwxrmrim.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3ocsjhmin.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3dozfowxl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3tkycrzpp.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3zocohzmh.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3rmmtzxvm.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ddlzqqgc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3dzjoqclm.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3kbxywexh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3vnxbrvib.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3axtqbpen.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3juvfjeht.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3plmrdjfn.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3lxlexker.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3csbcpvbh.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3dkeuymml.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3bzijpdwo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qdddgqrd.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3nmnxcqts.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3muwrzfsd.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3aylndtwy.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3vzkivgkv.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zpnomxnk.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3owxtjems.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3bkymkffi.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3nkqwzgjj.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ejfpxtxo.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3kyonscje.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3ijgsjhqe.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ndxfnpet.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3yihoiaea.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3bsnnrxhw.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ixsxlkmj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3wpueuvxj.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3trpuafjy.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3uhsgpfpg.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3uaanbcvg.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bejtywhm.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3lzdpwlod.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3vaqltdak.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3tebqmamx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3cdnvupui.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ahulzgap.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3njbspihh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3tgnjxpsd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mvrilhbs.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3jvrycgpq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3ldfitlrv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3rwcndxzv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3ogxdjpwy.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3ybuypioh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3qzqnqhsn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3vyfxopna.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3arsdrzxb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3twewkkwl.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3vmxauqeu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3inpgdukm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bjcjrabt.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3pjxbojwk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3ovjuswxi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3ivnpytng.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cnkdcozg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sfivmfkz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3aeosugiz.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3nbnwxytk.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3icflvbup.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3yoawpvlg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3rcypcyhx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3einchsye.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3dkmentlk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3jiytrxyv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3zsadhpdy.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3kvgbnyus.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3dqfgggsp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3lhamrwuy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ugbpmchh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3zomcztwm.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pawiguvn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3zlwroreh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3wuqjlhqn.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3pjdlsjgg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3nxgeqpdt.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3ssipgilq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3jtltyier.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3hesxhnbb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3llrzqavd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3gkjwixve.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3sygulhez.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3erthboho.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3fpymphoc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3teogkywl.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3tvkudixe.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3xgidcmwp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3mnzlrdkr.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3bppfesuw.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3tvzqufyp.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3dcowuvgu.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3calholec.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3pyjdwtdy.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3dhxccsiu.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3mzxmtqqg.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3hlgtvbva.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3qendhmvt.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3svawwqqq.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3kjsxwdqv.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3uqiwcapv.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3fynqbvkf.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3sckugzzj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3hpagjjyn.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3nufnntza.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3arwlairr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3pqgadgzs.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3upvremym.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3iuxlbuzg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3oxasukze.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3ibwvciqe.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3spnfpxyg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xnfjwpkq.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3bdopgolg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3toyloxaq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ocvcdrbs.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3rxdclwxv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3wznrwusn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3crnvfccw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3yvaxepzg.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mgxjcwrk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ikrrmtiv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3osozsbvz.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3vwtizlew.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ikhnvffc.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3zdjyfkit.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3suqdgess.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3eqfuwawv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3wmopyqzt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3gvlrpuid.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ilbixstk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3sxjudorr.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3origwotb.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3onpmfttu.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3brghrfui.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3pnmxvtpq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3bwxmvdsw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hdhaiawb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ahkloupa.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3etcfkxal.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3byrafujz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3bvnbjdva.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3dylqozqw.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3jxshtmti.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3wodylcda.html


<!-- 参考信息 -->