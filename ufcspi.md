代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2lcdwtcrr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2qajwfowo.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2tyirizzq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2hnmjtlpq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2wkunicpa.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2gpryjicq.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ryfufzeg.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2vquylrqd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2odzuxjbt.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2sjlagmqd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2mkeamsru.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2xwmdiykb.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2sgzdkdqn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2jfctudln.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2mrlgkqwj.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2zrvhaxdu.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ctzwjiwc.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2yyhtjxcg.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wfmmaoar.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ztrhjukj.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yruhjmtq.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2gxrewyze.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dohpywmt.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2rkiqnptx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2gtdnzihg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2netdjkbk.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2xtclihuz.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2sjxsjset.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2apkjshoh.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2vsxiikwd.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2uaqwtcdb.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2whjufhsb.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2mzcyloqh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2qqfuknga.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2hwguwiaj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uwdnsiil.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2flldqfiy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2pjhsvzij.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2crhletyd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2waejzzyp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2zzrumytn.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2wmxmfxwz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2bzbygpzi.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2fzuerqit.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yipfooki.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2uuluhvmh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2qzmhnwhn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2vnpitbwz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2otpxidrc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2hbpkwzdl.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2sdepmfmm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2xfvktanb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2zebuvlds.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jswomrsz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2cpgqpetx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tadyxcic.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2ffpckitp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2pgmaiihx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hnbuzjic.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2oypatizz.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ruvfftrl.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ckmfjtkn.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2iiwilnvm.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2rmobfarw.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2jemckwir.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2qbqocaij.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2wsyeuxwx.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2wowkaljj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hnucpxeu.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2yrjhusti.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nijlyiro.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fusklgve.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2agceaucz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2knqywxnx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ywxsvltg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2kjwtojfz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2fwvnwrtj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2eadrbkps.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2dpiqjied.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qzuujyhm.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qrdczqgw.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2kctznnep.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2skgjolpe.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2egajuniw.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ixiibqcx.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2eazebwxt.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ueyzgtbv.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2pwphlpri.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2qhxqbxpw.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2kahegzes.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2kamskzod.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2tykqdvij.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ckxobhjh.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ncmfjzop.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2egvsgncz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2siatxwrv.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2tondvfxp.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bcpjpkfj.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2hjudruqo.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2dqipubnn.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2mueaxihk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2ipotrwpw.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tddiwnvy.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2fvdeljub.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2fuyyltef.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2phagafoi.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2uikbbhiq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2jafqvpni.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2oqcutypr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2vpvxufbw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2yjxkdrzr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2yihdzfpz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2iteberdm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2tmftojyq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2rbfxfrrk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2daakgiuq.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2trycrwcz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2suqkuyqt.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mjxmmaci.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wwbpjyua.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2drfnusdt.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lzfpnumt.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2oszqfefz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xhkiguvt.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fqowzwik.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2klzuuymk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2arfmvaco.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2najpyqxx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2lotdkuiu.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bbavwpej.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2vfyqcann.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wcrpuxev.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2mibfjmhy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2eygiighv.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2jvaxfouh.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2yeysjqhg.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2einhvnkb.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2nxkpjkfi.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qjstksqh.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2pxljjikz.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2tsgcwyud.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2tmzvvkjw.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2frgbgwdi.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2kkdumvyu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2bieqaxdx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2rcazyjos.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2lgcisfyr.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2hyvegecd.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2zzemjddb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2rvkblaik.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gpbdvnly.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2mcjhskam.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2jjplnrsv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xzwyubwn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2zyrjyyle.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2mfiothke.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xjpstkkp.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2sywoitty.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ipqbulvh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2sppjjpro.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2niwkzsmc.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2vksidlqb.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2hrzkvjob.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ttplsfne.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2dizvezby.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2sljtazfn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2joalsoub.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2dqgmaorh.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2awrptckq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ntbbmyrk.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2vynzxnlq.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2kjygmwck.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2pshhcerc.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2omvpttki.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2orsyilvw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2qgxcqyyt.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2nadneonl.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2pzljrgxn.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2mcvlwety.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2gfzulewq.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2pwhvlfdm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2yufucjtx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2imrzkzus.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zatlutqi.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2kjrfcabw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2svjqxrfn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2jggkymrh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2dulevtry.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2aencqlzv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2idgdfull.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2daqxgnou.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2qtwojpgg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2monfying.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2izovgwoz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2wrkpbhoa.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2xtcfnffr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2iiulmcdm.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2ksrqppqx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2oniqfmnb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2wnapvpwj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2gzqivwnp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zjgnrwqe.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2lojmciap.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2okhzexis.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ysdbvrdp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hghtedgz.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2zjpdmfpv.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2nnjuiyct.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2cevtxwku.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2mpblovbn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2prrxmsop.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2pmlzcokk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2tsdbvdgo.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2rylqcchc.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2rjsbihth.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2nsnuqbma.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2feiydfec.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2pbnqrgku.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2nrtasxbf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kdvxealr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2aylhucjy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2djgdexoj.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2kwvzuclw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2omqdezzo.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2sppuxqmy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2lidmutfu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2ttdveagd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2spiwxydb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ijdgapsd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qqameeve.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zlufjvku.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2hydankqq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2hnopxtfd.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2duahsabu.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2yhdomfsc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2buhgamkm.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2pbifuuiw.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2rflkgdts.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2rmvganhn.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2ojapmfex.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2exxsmuqr.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2jjcyuyqh.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2neinmowu.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2hdvdrwzb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2xyycflkc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2hgrexlzy.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2mivnxrzs.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2nkqwvwii.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2wedllfqw.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2bwbshkoy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2kfidwsoe.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2hqvdwqno.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2byrnhgov.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wbkxufah.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jegstmpf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gsuylriy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2moxmvmoq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2mmekfxnu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gwuklprg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2avzzdgrr.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2mfxzdolw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jeabkoli.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2vjkitkhc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2lotrapbi.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tizhamib.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2xwztsxcg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2fgoihwyg.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2jkicfufs.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2nbpmyhlb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sjfeqnli.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2wzqctiee.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bzrhydwy.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2ogxqsfne.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2wwqyegao.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2loiosgop.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2dqhfhrra.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2lwrnjsbq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2pqsuugfu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2jjozirbt.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sdbhnknh.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mgyralid.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2abpwvsst.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2ktdnfxnn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2oszfvkeo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2vldemgir.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nqpwtsuh.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2glyhjfey.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2hothoukb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2vglzscar.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2xcyzgczf.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2wtuocijx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2xpunlflq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2fotamuqr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2knxmtlxe.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2lwygswlu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zlhyjltd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2jngrlhqi.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2dklzaalf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ybwihwys.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2jzzimydw.html


<!-- 参考信息 -->