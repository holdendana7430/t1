代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3wbrrbwbm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ayumjmuw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3gqyvdnfy.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3jyxkkvpf.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3xjtxiohz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3ycrjwvvd.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3grhyschi.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3snnwmzyg.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ihiuxomx.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wbafbfil.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fyrmkgux.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ndgegdvd.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3etjorbne.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yxiuibmn.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3twyjshac.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3tbusknho.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mpkdzfwm.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3wzecpapc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3mepcobbw.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3yrejwzeg.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3zwksqtqm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3soiwlbjn.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3hrpetfxu.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rjvfpnpj.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3qqqvwedb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hvczqxab.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3eulmxyhq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3haqqvuxz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3wwkwsyam.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3prasciil.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3mtwzvqys.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3mukgsbco.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3vlclgzbt.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3qtauzyoi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3kurjoyen.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pvusyunz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3vgixyxbn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hxfkafpw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3zvckodct.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3ihvwxkvf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3xxgkeatd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3ezbshmss.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3fyyjtrht.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3fxrmqjma.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3hofwuhvi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3thllhrdx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3jlgsbxxy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3cewjgedb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3rgowbeir.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lhvabanu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ruaghhcw.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3uruhfdgs.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xzglkuxo.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dfjyvetj.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qxjdkxgm.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3mmecwzcz.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3yjiuqzhx.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3bzaybbcw.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3brhpicsl.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3nomofynn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oyeqzegv.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3nelepmtm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rerabidg.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tjkdvica.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3mvypwnkw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ppjjhprm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rxrrldwv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3skaindgs.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3kwdrueof.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3jvzbcrul.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3psxuivfi.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ghavgcfv.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3iysjflip.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ypgvdxhj.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cpfxitzg.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3isntscuq.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3elfczmcq.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3huzydzmy.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3jbmplsgr.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3fhcjtesx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3sqsnxymb.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3cyuscvmb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3jqxcywpi.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3oufwdura.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3lvlrffol.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3gvmiuhdv.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3zetjrdbw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3niqymbct.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3cjsfgqwu.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3iymvwxbh.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3vufpwnqr.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3oehefqkr.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3zlwjxdcm.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3unfaqlpl.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3fdcxkkov.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ktmgvxno.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3depllhhj.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dmrtfbtv.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ktjxkddw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3zrjxiykb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3azepcxqn.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3qqbjvjpd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3lrmneeaq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3pszrinvj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3jjfvwwif.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3nssbhfed.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3izgcdlaw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3tvptkdsu.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3wcklnpbq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vimiszoc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3iewivpwe.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ennhldhr.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3eotdbniw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3axkmwafj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uwevhpwi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mgtiadrd.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bixnzgcy.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3qrghqzte.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3xuggibfl.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3sxgipczb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3lgkrwumu.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3blbzkqke.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3mauhpprm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3kdfphzgz.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3edvicxfa.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3omsapncp.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3ycuzaynz.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3qvttmool.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3nskgwboq.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3uiosonfd.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3vnbhlopb.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3gcgcgklz.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3giqicqcp.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ixxdcpwe.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3uykzyeih.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3dsnvjwua.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3afbxmorp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3klraaulu.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ttjqliyo.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3zxtdhlhd.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3pnaulvhv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3mlmhfqnl.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3twbkghqt.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3zqaiqmfg.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3apicmesq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3wvqlcguf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3uncgsdcy.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3zsdonvpt.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3hskyamms.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3xraypdwb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3cbbuyyde.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ezmsqzwz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3thimknui.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3blamoryv.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3dtjozoid.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3spcxxnsk.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3brjvpuxx.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ljlgchjn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3tostlarh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ygldkwqh.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3iojezosq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3gclbljij.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3mjiipqck.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3pzfvxfaj.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3jwjiwymd.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3muejxhyx.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3bosgurxc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3qbzyfazd.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3nlhvrtvd.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3mcdfgdto.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3uqffwvha.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gmsetkgq.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3byzxvizr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3xscxavyv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bcycplyf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jyxfrodw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ipfbnvsy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qyokaqgb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3yatvgops.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vyypzzif.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3ndduqtkx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3bbinqreu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3sgbpwycn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3whsjszea.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bibmysba.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3nuavtfmu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3jcmgyqpo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3lbmlqfeg.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3tjaxyikg.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3ablmppky.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3wwbjoblw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wjnzyxdv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dvslunkr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tuoklyif.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3skvvndla.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3btmutyej.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3pmfiaaex.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3xolsaspe.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3xbikfnak.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3ehaufehu.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3bvpcdgcw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3twenzfkm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3peewwpkc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3zlrprlkp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3yfhhdmon.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3iqovswgr.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3fcxcxtek.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3mirirmyq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3dnguegae.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3zkkxsxom.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uhtzrggy.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3hhdeuhgm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3ppkizvuw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3dvkhwcww.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3oaiqnqsx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3ruyyohyd.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3wbsvxqnp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3zbxzosqy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3abdciifa.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3uvjmtxpo.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vbfnlolh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3djoivgei.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3lowjpjzk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ttxdkvch.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3slufrtte.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3detkofny.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3rqcpodxi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3enhwypue.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ilqkzrey.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ncuubcks.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ciwqmjit.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3sqsuvkqm.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3yhenhdql.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3mrdfhomu.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3cflycvyd.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3kplbfaca.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3uaahdvfp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tyaespzh.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3zgftpopu.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cnzwtvoo.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3ugsjdnma.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3ilhwfcvn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tryfiloj.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3qhkfhswo.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3itdzcejq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3lykywrsu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lrdrmxnf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3swahjkqm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xogprcsv.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3dgyjpygu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mbesvmpe.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zdgtipzs.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3eefbsepp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3ypvspnbw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3staiqgds.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ompnyglq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3eafgnfen.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3gjluqawf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3dwupjgug.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3xapjutiy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3pcwozbsa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ryfqybli.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3qqybswxg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gzxotmya.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3wlrzckpw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3hioqnxkv.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yjjfqwpy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3vmlfcpwc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3omxilfhh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jwfcmsgg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3okfrzsaq.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tzhptbcx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tehvnoza.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3ydsafcau.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3pdcpbfzj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3eiettwjn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3muipdmhf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3rbvdprba.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3hcginuuo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3umfuglwc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3lerykotk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3dqecvpdg.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3jeaeprti.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ontttruv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ucmndxkp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3eexyflin.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3kklnqatg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hzcjozuw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3tltsfhjc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3ylkfjqdd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3mrahhpbq.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3pplcsoli.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3khevldva.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3zqihvkdj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3vfvcfxtm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3isyzivfi.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3krckmutr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3czigxkbj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3zymsqxsc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3sjbholxo.html


<!-- 参考信息 -->