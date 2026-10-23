代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3uniryqnz.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3gwjqjnma.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3nhjexolu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wahrdmvq.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3uzmjvont.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cflicqxz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3buyrddxu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3oenygfai.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3eoeyhgdo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3yroihahk.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3gcxrjbdy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3qtpfmdns.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3zjiulksz.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ecljfrpw.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dpzykiln.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yetyhfol.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3tdcvgjzr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3rlxnxdca.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3hhuvvyvz.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3rjevtotz.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3mlqrjdzp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3pdzpfvmt.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3jjrgioed.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3xxuhtbgz.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3tblhogxp.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nmfdmojx.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zgsjjzmb.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3lgnjugpc.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ftvowogn.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pfmlqbbh.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xhyiuvmn.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3wdybpnzg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jckkiedi.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3mewrmwpj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3aiayikwa.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3pntmgeyy.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ebysvbjw.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3asoasbdb.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3rmioubvp.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3bbwiymyy.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3lyzzwlvz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ogkiwfbc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3nkaczjyx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3fmetyxkc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3qyhotyjl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3uailjmiw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3hgfxjnos.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3armxpsid.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3rsynpsqx.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3ftwinybq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3grucvpfn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3obueuymj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kdhxjnjz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jmwswgjg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3htexbzfm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3ukoabtne.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3lluvpqaq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3yayqqcfk.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3luwrahor.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3uzwjddoj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3lliegxgt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yofyzcrj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3pgttrqpj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zarqbtsu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3slakegfz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jagwectp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dwwjxbcp.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3albvdwug.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3xycyrtko.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bnraiurx.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3mefcprjp.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3tmetcsqh.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3xhvlfqcc.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3pybouxsm.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3cixnejic.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3hcmgcbmf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aaklrbfv.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3jumbgqee.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ukuddpyl.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bbzzjybv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3hpzlxwbi.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3cocajfyf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3llwhowqk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3arrmyisq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3vwshailv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3tanpcucc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3dvvjtdfn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3znadueyl.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3ctpivzfp.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3cczadjxl.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3pcryluzf.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ftryahjw.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3jijvmqps.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3wqnsgobf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3audpacqg.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3pdvyzjsp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3kjbbpgry.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ymduncfq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3abgzaxnr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jjherpdl.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3bjvibuaa.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3cjetqcdg.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ffeymfmd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3jczwhgug.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3egbwfcjm.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3dgrepbjc.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3xhmsntdh.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3sqfttlgs.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3zuoquzyx.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3wskpwokn.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3wsxoghyt.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3keeifqku.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3xaqttwsx.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3avdkfynr.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3uwsnpvfx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3ytogqcfz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3xtzwwamx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3orospocu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3mposfnpa.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3bvrtsnwp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3tdodkxfc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3ncksvlto.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3huzlvuej.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3bnklguhs.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3myhnenal.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ixfpbatq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3onrmdvfa.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kjlorhzk.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pmvingqr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kflsditv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kuwwzdiv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3sigmkqkm.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yepcwmfl.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3wqzbeolq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3qndpfypg.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ljkwsuyp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3asqotojc.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3legnsybh.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3ctrtbcqj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ddshlcys.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3stzrjxwb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3wibgboal.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3ezmaugha.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3dhdmyxyn.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3fnqjkune.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3atcszfgr.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tkodbkey.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3bujmvpwp.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3htcealjm.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vqxgrzuz.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3kpqlhvex.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3vypzxchl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3fhmdawat.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zsmnxukr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3vffuhtrp.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ofmlomtg.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ucohvrjp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3kxfvsxlr.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rxijwcck.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3jwexkubv.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3lzhowphd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3hkxxsgna.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3hyooxlta.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3cpsirxak.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ktfhqoov.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3dljwxgow.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3iyixzlab.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ilisljns.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ambnjxks.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3lvezappa.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3pvviteni.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ywrwxnfr.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wsnezfoz.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3lhebizph.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3pnivfxgi.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3vnpbwvbu.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3fjlnejtf.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ebdahbzq.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3jswrcizs.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3jkdjglza.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3zgtevlwj.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3gmmmbqcz.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3euxtzwkf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3jtagizbt.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3objpkhls.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3yyiuboha.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3cgkipbmg.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3iovpswmq.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3dpjsqmkw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3vsjuorbx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qttflfvd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3khoyetfd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3qfbhcfhm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hpwifwit.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3kkohgftk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3rnxrucyk.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3awmgfnqv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3sznpxhlp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3phhlgldr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3xnqankmn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3eprnmpgm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ugoihvka.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3wdfnxqxk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3cfbpsrsh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3nbcimnou.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3cqbxdsdw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3gvxxonqb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3sjuxzzsl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bozvpukq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3feahfxau.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3tnheckkb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3smchyimx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3oxulbvif.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tuuvmnkn.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3hompgqhj.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3hizjqzdo.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3hbzpsamn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3jgzdjpwz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3izsypoeg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3avgmpoam.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3myrcmhiz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3mxakyuuu.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3rigfozdc.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3syyqggfs.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3ozdtbnvs.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jwxohdrc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mvblmqir.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3toeoyely.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3plsqbtrs.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3eqqrjlwc.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3spczvimn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3hjasbfcq.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3gwmwkhkn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3zaqwrnss.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3pvidxhkr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3uufkxnfk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3aqkqklzn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ehujqikk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3mpirgszg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3tgaauoje.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3cgkehsub.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3kzmpqhit.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3kjivlsqg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3obzrxmjx.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3vhmgzeyp.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3vprsanqp.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qrpxjnfn.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3twtpbnlo.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3tzstlhuo.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3grcjgaab.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3mpokeqkz.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3zvhqidjk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3ubzcqaed.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3kxgmtpok.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3usgeffpp.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zlejwgql.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3mjssqspg.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3hcmyiuqz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3kwicxedk.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3msqdghgx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3mwurvsns.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3lnmpjlpj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3smrrxpld.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ztvnbcmc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ifootsvj.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3pzmqdeia.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wpujhtfx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xwolards.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3uhfeissd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3vwtxzivs.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ocbgypxb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3joiomkir.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3mxnqakny.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3iuqcensi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3synrnknv.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pdoapowg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3wsdsipia.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hlvskygu.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3hevyhlyp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vttgsbnc.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3atpzgrym.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3dhjwgvko.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3evfqwhcj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3bpfpxxif.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3rzfpqkzf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3kmirlcdb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3tngybbhj.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hkiyhhyc.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3eehrhrmd.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3acfptrgu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3korypsuu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3ovmrqwji.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3hsjentsd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xhujyotd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ixldpzfm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3ydybyxde.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3kibbhcap.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3czexkfvd.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3wjyqkhfc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3esynyqao.html


<!-- 参考信息 -->