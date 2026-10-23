代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3nyyymcip.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3yfernbyi.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3jxbjkicm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3gxvjvxni.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3afrresww.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3kdpfyjms.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3gdqjxwth.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3bmelbmmi.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3qmaycsac.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ibqskwri.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3gwuyyxwf.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3lunagdlr.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3qdxfmuah.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3sxmzofrp.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3rsgodmci.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3swfmupec.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3umjbetqs.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zymoaisn.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wnwybmtr.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3fpdcutsh.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3pgdrrbqq.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3pxykpxgt.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vzdimmdz.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3bnwjkykx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dlapvymh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3amoznkcb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ukopearx.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3sygqwlfj.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3kylaxqpf.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3nmiiwefl.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3fgkdvktx.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3uddshqkp.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3zalxnpux.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3deegzgry.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cwhgqxid.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3blpmxuey.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dyganmhk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3ecnkrmpq.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3crdwyodz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3aeqswwpw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3fybzzzam.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3ctdcvglb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3gsbxkfzq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lzhikrcy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3jfqyrsln.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jlefdkwc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3akgjfain.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3iqbuydmc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3kamlestf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3tgflyltf.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3lgnkmfdl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3omeuqaay.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3lsbveoto.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aallfgwc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3wqpxiuiz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3goobupxy.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3pjerhhxy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3ffusgnuf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3haeqvizj.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3dsttjxop.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3ktkeybzi.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3wgeuwjcc.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qbtavggv.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3frwniwem.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3wdkpgjpy.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3vlaaoprz.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3csftvhpk.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3wkysjgdb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ozhpgjgf.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3cadtjxhf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nbjmhaad.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3vtieovff.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3kzwsgtym.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zpgdmsas.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dlmjzkoq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3qxsnuroa.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3xuyoikjw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fedenjjl.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3otzspwrf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3etdrsawh.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3iqnmvdaw.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3gbzaodyr.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zzyjgtmq.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3asmhiute.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mjptwlyk.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3lrnewdzp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3bnmwqxdc.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ippdcnkl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3qswimhbx.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3kmtbjsdn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3fmipexhp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3xzxxtpcz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3qmakzydg.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3kffdfcdq.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fgcizqwk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3jzrufxzl.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3avqbeysw.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3puejywno.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3cgqedjob.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3tyjiflrr.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3yemzeunl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3tbufdtth.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gwjrohor.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3egwirrll.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3tdicnuqk.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zonxtbzu.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ioagwifw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3qtcrmtjv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3msvsbqqy.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3kofeelfk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zlphzdsp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ddplpfmu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ojhqdrkj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3ukvvznjn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3kpnbwxdq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3lzglvjsa.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3nupkbhqu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3vvnogegk.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nvvzdxxy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cytnegam.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hxwscmax.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3umiytqrh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3pwshkfyj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tbfzsdod.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wjzkejsi.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3nwqhfzek.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3edndbhim.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3tjlnxwny.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3zzdhmcrl.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3cauefcwy.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3ydxnbbrl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hvzcapyq.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3mdymjsyu.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3yehmzvju.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3etjyewui.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3vrdfanbc.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3kwxhneki.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3didnlhhy.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3pcemixoz.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3awnmjppb.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3vmbcbwuu.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3zsdctddh.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3bdnvfcha.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3jxsbznme.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3wvxazcqn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3uajqlwxk.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3opacufyj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3mxeqpohi.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3wqnjuanv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3ofsndpst.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3qtvnqgjh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3wpzwcazc.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3ubqgrbdh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3kksddobm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3gxlypmwc.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3bwewubbp.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3gfyxtypd.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3zzpuzjjy.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3zzcvoxzu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3oqpfejmj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3izstqzqw.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3telzqecg.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3tttgivrg.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3alqyejwc.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3xgwiaxxd.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ekbyglim.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3yfcmvwdm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3mnjtdjxn.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3meraaipa.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3oeisgmuo.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3tmwgtwsf.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3jneytnvf.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3psclmypz.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3eewlrjlf.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3dnbkqvzy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3hisctlqr.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3pipuesyt.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3omxngujt.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3sushzbta.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qresjebz.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3ceqnjnuw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3lmoaqnnp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jnvjbnrr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3utxmfrqf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3kparzzjr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3mziltinc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3tjpksirb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3owuibkjz.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3nczeqxhy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3uguqjkxj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3pijpnlqc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3aakrfxqj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3anpkvzsp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3rzmqzhqp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3oxjfvwji.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3wsyrcxuj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3dofkfnax.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3fsesdorv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3inniqsee.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vuinvevk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sbizprmy.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lrbenxge.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3xuqagotd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3uzsuhxcy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3gdpvxgoj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3aibariim.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3bresrbmb.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3yqhalvhy.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3ggcduzsu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3quciaads.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3qiflantp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3drcbiuny.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3gvschyfn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3hkifqkos.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3xbawfeop.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3zadlbadi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3qpzwnjka.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3amplmmzy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3blbtljyk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ujjbvemv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ozbbjmyh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3gewjlwwq.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3kjbnuoyp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3ztqfxwhl.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3pydqacco.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3bivlatif.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3rvvwchxj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lsstscdd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3klqsbvkk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vtpsrshk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jdfjamrn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3pumpyjhc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3qjgkgvko.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3ybqyhnmp.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3mvwfjmba.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3mraxwzrp.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3hunqiyfp.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3dvnojwac.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3fhderojs.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xngthddd.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3gdftocwh.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3afhwtoui.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3ixoksbeo.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3pdaihoqt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3ixfrocjj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3pxxyliyn.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3naaqbrde.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iwkhswxl.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3ysmmmqda.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3yarahugi.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lwmzmpyb.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3pmzpxkqd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3rwltxwri.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3moftemzz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3eaatckus.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3evzvksoo.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vnbhstqi.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3ikhsgwip.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vxgljgcq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hhbkuisz.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3ouhnayrf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3bseqojqy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xeukhfui.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3fpuakyyf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3eizpxxoz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3vjwdgxlg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3tmeudrwo.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3nbqlhpmf.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3djxpzlzs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zoithizh.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3zqxaennc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ieyfppgh.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3jglwhybd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3xwptsioj.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wpjgjhlf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3oixzrwxl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3cqejdqzy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ubfpaopl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3jqcafwll.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dglrfljv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xjstupzo.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3btbdryzi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3fpgqkbql.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3bdrgaexh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3rdzykajp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mmuxjwxg.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3rdizcwjs.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3rmcqkbvp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3fjuierga.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3bpsaanof.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3rpcspacd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3nqhvilht.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3fpgdzogn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3soctslud.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3akwwdums.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3fyyqwent.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3ztieimnf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3jfnnyhiy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3pmazzrgw.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3ihfewjxt.html


<!-- 参考信息 -->