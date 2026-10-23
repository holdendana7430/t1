代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3lwxghppo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3cqrkbumf.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3hvooovut.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3goibocnz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3jlacpaxp.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3fnyqivpp.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vdcsoidm.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mecfrxci.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3hojygrda.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3rgddwnie.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3jrejtibz.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3euoqhysy.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3ekcrfiru.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3wasndkns.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3upfcwgsu.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3xdtdizxf.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ijhtzphl.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3raphqepk.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3igdgtutv.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vgerzmbp.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3iqcymxlz.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3eidwlqfl.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3iohegqht.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3krqtxgvz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3ghkqntov.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3cqbbpgmu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3lddebxnr.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3fxalwzyj.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xvfncssm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3qkvilyma.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3lmdgmtuj.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3ybbouany.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3gbohgpfj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3taglzsas.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gcdtcqkb.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3yjacdfur.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3bkxswfdt.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3gnmkdscz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3exnkdebs.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3pjmomjry.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3czfrlqyz.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3wmhwhwxt.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3bddvapln.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rkqaskli.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3qukxrtho.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rfbbqfna.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3urtaquvy.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3bmjycqtx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3tcpyvanq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3uyrqpgik.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3fzxfwaew.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3xebastnu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3fbetnbuo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sesqwzlp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3rnyxjleq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nqjckhpl.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3ultsiyrv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3yztwgcbn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iqretqxv.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3urskxwre.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3mnvchcfv.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3einlkdvv.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3igtyizuu.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ajpyditz.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3knyhqgby.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3drvsjatx.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3hemxmepa.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3yvtgfmpp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lnhmsxgh.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3apunqkxx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3twlbzsyw.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3gyzmciob.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3ksuvispe.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3yvjqtbpg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tskexise.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ieufqypr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3nnvrnuur.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3aedfxspv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3upuvlyor.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cxfljicr.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vwkcpkpr.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3cjcsqtdq.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3njyuqcvu.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hdpdmgrw.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3jfdezsom.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ckhpflmu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3yervjvae.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3uxoiexja.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3lmgklbia.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3hcdohrlk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3kwzqdats.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qdddgbjg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dtlkkunf.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3kwbfpylg.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3vrqieabu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3oicvbtvr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3cwoqyobm.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wonxsehw.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3nzzbkezx.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3daksdydb.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3abdofyld.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3guctlrgx.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jextlgbv.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3tkvexaob.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3iijscdjl.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jmboxzxj.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3iqiibyeq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3fubcotdy.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ffpivkbw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3aaygmewi.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3mjzfqttv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3lnewnjwz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3nkzckhsf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3ytsbfxba.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3erulvbex.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ifoheduu.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3qraobwmr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3gacjruyf.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3svpfgoft.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3iiehoqyr.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zwkigxmi.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nfrkfxup.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bzjopdpa.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ahrukmxq.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qomsnrkg.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3kqzlwlej.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3jkqjncbb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zyjimbrb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3uthllsci.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3fyngnjlj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3hjuljtlv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lfgjylvt.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3ktalnokf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3dvqnrkob.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3tisewrqy.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3izmgleln.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3sbbwslgr.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ituskcso.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3rudgnnka.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3vjzgknjr.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3ojebkgzs.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3iskqafbr.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3knympmei.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3mecpxwin.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ktdliexq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3kbdjpwjh.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3sesuyfyn.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3bakphhmh.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3nhyhdfkl.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3qjnnxoxb.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3bkyycrqv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3vltrocpu.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3blreoieq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3xtslcfer.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3gabiabxu.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3yjyimghk.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3gcypyquw.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3nmgqgety.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xjcwfprw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3zvpvxlcv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3wrcczrjg.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bpvjdlnm.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3dmddwgem.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3eujujmob.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kbxvnbtk.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3nlfxzpeq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3kscvlqgb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3asmjbqwd.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3campexzh.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ihmpajwz.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3fmphvxqw.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3syxvqokm.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3jbwocjxn.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3atiyamcv.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3iomzxkba.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3bpumraor.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3znnfvfcb.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3lecjvepc.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3pirshnwa.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ounrypxb.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3qvnraxcf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3nggyiiwt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3sjbtvxcd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3gcefrvry.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3iebnmgys.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3yofjacho.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3jrveblxn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xabbhocn.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3ejnvqsfh.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3pxidaohr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3etdzssqw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3hcrkwchd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yegkftng.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3jnyymggy.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3wtlwuhah.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3bndnmetl.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lzwxbusx.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3qlamlupp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3hupxrpwc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ofmqrske.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xyblxvtl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3zorbylen.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3hycdrpml.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3tvrzahmp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3sloemkgp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3vxmvjndv.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3mbzkzdyx.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3eyhtkqwr.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3yahdmpzg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3xemjcsom.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3gkipptae.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3haqrimtx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3lxrhtklh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3rxltglqp.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3zjwbrwqz.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3srlitmcy.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3sxjsbvmc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nzvmijem.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3uoebooyl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dltorzug.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3vvepvxet.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3yjikepba.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3viyxdkcf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3twlyfwfz.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3ogjjyupe.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3kxcsputv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3ihjkyrez.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3tvqgffuc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3yoddxdwi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3cwdmyaou.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3znvaaeua.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3jrfluuax.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3sndrkpsp.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3imfomqob.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3srxaiehh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3grrghfxw.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ulcwicqf.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ugcugvaz.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3crtooaci.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3uorccmyy.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3pfoqedju.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3xvtrtfcd.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3ygfscmig.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3zbwsqdib.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3tlabhqeb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pgdymehe.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3hvdaodze.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3duguvuxg.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3wzduenyu.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3qencvqdb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3umesjqfk.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3spysjbto.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3hqhkeamp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3znqbewfs.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ivyclczy.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jfgwyxxf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3bvegelhb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3wnmgmpao.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qrceevqv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fewcpmuz.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3ulqhtedo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3odbcgeek.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3cstvdizm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pvpixzbh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3kjhzitfr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3wkxakwyb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3gwsoydcf.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3xucwhwaz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3yekyeepc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zgwdkqpq.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3medewwiq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zbioqtze.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3caxpcwpd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3kaeyfyil.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ttruwvcq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3ptrcymkt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3crxvgrgc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3fmxzrswz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3qopjgisz.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jtgipbvd.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jxhjcvni.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3ungopwda.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3dpmjnkcv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3cykylbgy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vdvcjthb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3dvvttvje.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3rihtjmqv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3syivxins.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3kokdrfpi.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3sitddosl.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3xuonqgqa.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3douhrqmc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3xhyrmlfv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3vytyaofb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3wlggfada.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3jgvwzbjb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3qiqxibku.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3frdttkay.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3nwtvfqhb.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3ziarrpwd.html


<!-- 参考信息 -->