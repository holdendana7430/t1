代发 wailian999

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3rjoanxgr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3lnmfutef.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3vxjzytjn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3dnvhfizy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3iynzcfia.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3ddpftrhq.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3imzbqjtj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3kqzogabg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3tznzzqhr.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3lzsjfuja.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pqwpbsfd.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3ckqzwjxj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3uakipjid.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3rfkweedt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3uetvzgzd.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3gidjriap.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3xcbijebo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3mjdkzoyf.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3dwswfcxy.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3piincvxq.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3cuawedef.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3odfrqugd.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3tndeyzdh.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vsshkggk.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3erdcxjqz.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3cwxzzace.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qcxnvrat.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3okvngpxz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vzetseyq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3kwmnhrgt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mrlmyxql.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3gyfircxb.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qngqwlra.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3gdxegymi.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3emoqzmkv.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3yuwymuro.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3dnjgqxog.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xbszjfch.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3mvgxcgdr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3birikfsa.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fvxemwzv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3krdlcltl.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3wqitxzgx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3tzwjgglb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3jhslfmgi.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3yhfjadjd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3kjasupck.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3bmdjnhwt.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3rmrmipfu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rnxfivah.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3qhlzlgna.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3upxhyzcb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3vlfdezfy.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3zaznrqdd.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3bvpzaslz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3iqjjvafa.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3uhetbxhh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3zmvjkhxb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3xmqnejyt.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ljunzplw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3dotzsiyt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3znlivxny.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uxntorwm.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jzgjrgmd.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3gjimknja.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ianpmwfx.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3wopcdvpp.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zseirxwz.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3gxzhiumv.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3gehqbunn.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rcxoazec.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3megkccqh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ojivtozx.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3ozadekrf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jkgycido.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3bhdgnakz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3tduuskwb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bjxsceyl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3azakqxzv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ewjeigtf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3vkudbzlt.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ckckvixm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3myzazimw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uiizhkyb.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3eswcgyvd.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3deyzggjx.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3pzypsvsh.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3lzozfhkh.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3oaopocjy.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qydmrqvc.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3kavbscmk.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ksmfvipa.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3mulqyiqz.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3wtqrjluy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3tradcpdk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3umeqsrow.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ukfntwpf.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3memymjyh.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3rccxltwr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3lftnsgcr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3qcbhkica.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lngfppau.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3ntycarii.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ijnvqvoh.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3fcyoqzhx.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3ioyhxlzs.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mfgdnskv.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3iecsjuua.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3jkuxxfyv.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ohbrlzhv.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3oawbzqbw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3exxtivon.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3sdwtdrih.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3imayqswt.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3khzmmmxt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rgplfokq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3taagfjgz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3vmvjbgtl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xlzjcwtb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3scsgqknk.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3zufqcgcj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yjcutgfs.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rokxdyts.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jkzmdoyt.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3otifdzup.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ztdzxrax.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3uzxxxobq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lwigqrtq.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gaxxxbui.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3sgywfhms.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3zghandjf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3egpctfdo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3axwbexyo.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3kwwnsfrd.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3mcqishst.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3awhylgui.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3hpimjrvr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3jsebhmlr.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3cizuqaim.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3lseyssjw.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3jkiswnyk.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3hwtkbfbv.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kfwgysaa.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3zishepko.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3lylmtweg.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tehmjkhh.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3cqodruhy.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3dwhqneyg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3onslptyn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hwhdyltd.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3gescufcv.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xpohfdrn.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3nihflspo.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3fajbguxd.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3uctyeehr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3zkdohqha.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3jdhxgblg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3qbxkmcax.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3dfagbazw.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3mnowpqjk.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ilzkuzsa.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3lzllwsar.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qmpgkggy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xqixjjpy.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3srchfdkn.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3rihrenpb.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3pzimaxyk.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pkskdjrw.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mpcdvera.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vbsrfywx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3fylgvtfj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3vuntwqhc.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nlhewjwq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3pnwdutjr.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3iwkgoalg.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3vxzrrgja.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3xsmqmbit.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3rgjnfyzf.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3nyqzqzus.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3rntdhrzw.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3mtdvdnmh.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kforaveb.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3ldvthzgs.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3cnsmpmmo.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3eyclsguu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3ptjmwwxv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3szxiqsyu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hxwwojjz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vvelpsxp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3ibuitwgg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3zuphflyv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3pndyhjrt.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3lsrvzkzm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3tqwksmou.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xlgpzmyp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3nysvrkdq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3gonscooc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3rnmwrxky.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3sxcwoxgq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3vgedvamk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3guoaoesr.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3dwzgwnmd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3bapegyeq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xtslyjyw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3stwwrwug.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3zxxciwvu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3rpovxovi.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3axddtkpg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3ngrkfcau.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3kwpreysi.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3tiwqpdgz.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3yafcwwgv.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3wruvgfpg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3rgsqepvx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3asekwiod.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3vhgcyoik.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3erbbcoyk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3pmxpkzuv.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3tmmvloww.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3oelfqxyf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3psngstfa.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qpfwzgth.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bklngtsd.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wwrnxfus.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3icmzkbwv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3zalhohva.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3drhajnvq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3kduxtohm.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3hqqfcogv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3yiptixun.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3tlvannug.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kymiqilh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lhjrxncv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3cojmiyxi.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ugiekzbu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3tuolfbub.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3oxzbqszg.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3vveqseaj.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3cipfawcl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3xvhsunxs.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ollsbwyn.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3srjpgpdy.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3wxsgrzra.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3wwidrnfm.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3aoiajfww.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3qkqayscu.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3ifuntgyw.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3rleasuwo.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3guqlddyb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cfdzgjkw.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3awehvynn.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3jmnnykln.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3djhckghz.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3tumhcknm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3josovqul.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3tjbcyyit.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3kvmtcucl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3tcjhiahd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wzuuyhav.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cvcqexsm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nlkqiccm.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3rwyxomvz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vplsxqns.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ffxwcgrq.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3koaepdgi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nbbicxcp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hylxkmfj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ffwxzsyc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3jeeverfh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3csdediqi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3krmxkybo.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ihwvhgfa.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3mlzcxbyi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wjcrxuxc.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3cqamyvzf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fvqdussd.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3smqivguw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3dosaziyp.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wednemqe.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3kbifpanv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ouwxxuzn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3asnqoiyl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3kfaytnyp.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yyybbuzc.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ntigjwqx.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3ycecjudw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3ndulwuru.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3vgxskrqp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3mzefqfxr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3blgsptdp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3dqabqwxb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3kjxsqxbd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3gbfibnpa.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3rwicgfsg.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3uuqajxkr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3xwribglw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3zemtsnmm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3farjfkuu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3dgwtqeuv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3uxcemmlh.html


<!-- 参考信息 -->