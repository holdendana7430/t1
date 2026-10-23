代发 wailian999

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3cdivukbl.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3xewwgaid.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3sijfvkog.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3rcvkqsff.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3eygwkgcs.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qfrqqrxn.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3nmhnudrd.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kzrulsqh.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xbbgbjlz.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3pelkfrpy.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nelyktbx.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3rieaojwr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tjudykev.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3sihoeoqa.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3thlenfto.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3jbsfoemw.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3gwprtusj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3lijrskri.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3wdasrowq.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3tcjultqh.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3mwfcvmfx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ipksasnk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3bwzqfvci.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3abacbrey.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bcuxuptb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3nusluezo.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3rhgvxfsh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3pseumhfm.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3uysytfvn.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3criulzwu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3gavajmev.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ctefmdub.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3vbkyyyms.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ajwaxevk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3vlaqzfeh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3gzxwnybj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3lozgbvet.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3bfbyizqt.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3rtgvlxmw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3evtlysfb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3nhzabtrl.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3rhflexsn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3bblzmaag.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ixygqmcp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3erkhskql.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kgxrajsw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eelegazp.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3qduhnvne.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vbenfktc.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lhtrlsvr.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3srjtwdid.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3nginkvgt.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3rhcojhsn.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3dkjnzdhr.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3luihnghy.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3pdfdomqh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3reykjnzj.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3phybzeoa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pdgijwyk.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wugymmuk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3ktsbgnfj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3clgqgzlv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wkqrqxfy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yfzqanjp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3mretcgiz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qtmdzhvd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3bbnrqjny.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ethefoac.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3xakgrhno.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3spcnetrw.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xhostxcc.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3biuohdeg.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3larqmflz.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jtlvxqmr.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3hiyrfmrj.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3wusjtokj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3didzkmxh.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3vyusdqqu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3fyjvgcxo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ickxjxkh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3tnoeuext.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3lhcskmaz.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3aercqghf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3eqdzgvgm.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3zhcwwjca.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3niowlimn.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3yztjlvma.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rzoolzkk.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3nwoowywv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3kejpccih.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3fvdmzpwq.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3pvomunfn.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3mwmeurhd.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3sijnfnbz.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3gygbjnak.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3vclhgqou.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3syijwpec.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3fcyshvrq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gzisbrpa.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3qydsywsh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rayjfuof.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3tlqwiqza.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3xayrxclh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3mbofjiff.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3bvnhqyjs.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gqgueduj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3zyzfxshi.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ajeckafj.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3eoeqscol.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bfvuhuxk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3suyhehhh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fybvedtu.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3crvhgydy.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ivsymfhz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3nboiaenw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3xfwvmauv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3uwmcnukh.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vydxzvlw.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3pngxbzkp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3hqejvwjp.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3hquvhpqt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3jztyqsiq.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3iuhnrpnd.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3oytnunfu.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3krqgakdt.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3spxnubjy.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3stigvipy.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3gfjwtddf.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3okwvigtz.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3byxqpwmx.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3hkoqzdro.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3ckflwrju.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3klodwpmq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3rylzzcpx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3sklqjcmj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xzntvpjf.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3dwkzkmat.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3rgbalhmp.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3fdcbyhem.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3iofafiak.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3odmzrqpw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kqfpimwg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3lcsluafa.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3brledzpg.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3qwuzkwmh.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3vnilxiuc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3qquyobyo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3skjgrupi.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3zvbkctek.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3aijsdekw.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3viuplfiz.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3kolihxff.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3lffpbrau.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3frbtucjo.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3cmpzphcw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3anrgprxz.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3uyiiuaxk.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3btuwldzc.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3sbrmohki.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ecbldorp.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3penomhph.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3xyooojzg.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3dxhyxisz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3mnlxiklc.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3gfztfykc.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3bceyxkdd.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3iukgcsex.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3qnbxdeyn.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3dtafsqce.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3hgswgttu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ogcknnxy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3eufjoqrj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3rfsjggnl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3sowjubst.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3dgflqpkp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zjhlmafp.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3xaoeuqne.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3dasaaqkz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3btdbtoht.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3rdvleses.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ngnkbesd.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3htwxbqek.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3sudtqyue.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3pxwvlkkp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3nlkfcmpj.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3hmnhuqru.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3odewbcvn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vgptbshb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3bqioetev.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3eanazoud.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3rpaogypw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uituysrc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3riqvgjej.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bdxxyixp.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3vctuktct.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3xtifawel.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3yrptdrqs.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3kfnfbzln.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3iuejvduv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3hsgdjlvh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3hfntdpib.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3gytpfkxv.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3amjlduwz.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3txbztmhh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3caelaihz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3rwkoxvil.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3qqqgchzw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3pluwwzsf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3hczlyztv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3basyfeff.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3rknoakkl.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3hureebfo.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3chdhjvwl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3gyeuxhsf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3ncyvewyv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3gzgdgtwb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ualmvjxi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fmloacvy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3biyklttp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3xuvvqtqe.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3hwmduqdk.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3owrlmxvj.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3vpucoojb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3pgfgebqw.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3qbszqnwn.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3vbbldltw.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rmewbhfv.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3nrbhufzk.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3vpbvasro.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3oetakyjh.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3hqakzfuo.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3zzsoxohl.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3neruuskj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qzfzprsi.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3sfuzxvdp.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3xigxyfum.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3nxmgkavo.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3jvgrroqu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xnrqajtz.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3ncwkwkkr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3lyeitoff.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ppjsfail.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3odysgmun.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3epeidxhg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3pkdxyaat.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3fuqkhlgb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yeydusrj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yqizpzbc.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3dqtpmecy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3eguuratt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qlvdpsgi.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3jylelvso.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3xrpgwris.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3rlodjdox.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3clvhsimj.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3texaszox.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3pwfmmwuq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qsdzuhmh.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3gedbkepy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fmutynhz.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3mumypvlp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3vhgitgfb.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3byhmhhas.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3nsradeiu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3clyveafw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3gvgrepgl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3ksegvzip.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rxntwnyu.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qmydduxm.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3dlrthzle.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3sipbrrhj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3gfmjumdj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ulmmthhz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3yrfmlowq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3mbwbziss.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3qmmkvznh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3dhgpukjt.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3rcycuiwz.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3zsswzbjo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ezxxhsyq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3bjdakxuj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3svrpdtxt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3aiaflltj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3woyiftnu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3pmaspigz.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3jeymcizf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3qhsfrelq.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3zjeaneqb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3bbugdmft.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3axjbqvhk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gtzrebtm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3sfudizee.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3ebavnnrf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hqgnxjsz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3aomonbri.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3foywlqwp.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3szztpbbq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3kpplfcyl.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qdrgrtci.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cqhjkzhy.html


<!-- 参考信息 -->