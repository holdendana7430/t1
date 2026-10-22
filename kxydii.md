代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ohefrgox.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2fzwnwavk.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ejkptrcy.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2imjenxay.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2njqkljuw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2rheflkpg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tcizixxq.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2awleeftx.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2urspclxl.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2blodbouy.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2mvegishy.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2bgdquxxm.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2cofcdwfi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dskkwtyh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hycirrgx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xyfyxuoc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2jtzpwgdu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2tuyabwdo.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2uqkzsnay.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2mtcodrse.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2yutzrrxu.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2hxqdxvea.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2pkdnivsp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pgewathi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2pddttejs.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nzsymokz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2yjmwvqnx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2gasohuya.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2firzrhvf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2eyvgeynv.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2ixybzlxd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2kzctyecl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2arrokemx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2vgjwzssl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2vyggnnam.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zmqccdqi.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2gfdaugje.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2didfuaeu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xmespmee.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2phlxhdmf.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2zmqvqsne.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xpnqxdjv.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2iuhehkyl.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2eugafypv.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2cuypwrch.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2nvktihyv.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2fnlsntpk.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2mrvhgsom.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fydlcomn.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2ehxrdsez.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hvazvdkw.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2xdxibtdl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2aafbxfdn.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2zefekyaj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2kqngzfof.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qsujygdp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2nfrfibwb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2ihfepxit.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2huwfoiee.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2oofrfggh.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ociyptbb.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ddyubexr.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2lywboluv.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2jzushify.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2bnrjchtj.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2aupdoyyr.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2lvdhvznz.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2iijmeghg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2bxafmpfr.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2kdmdonnc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2bipklicv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2neesyfxq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2scdapsyu.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2jmdtswfq.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2mavvpjho.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2gcawilzh.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2csrsiogd.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zwgztqrn.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2iupehdpu.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2arhhuyje.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2jnwopdzt.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2tyfmhwbw.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zolpcovg.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lkagtxxz.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2gjuqwnjv.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2crrkwnwq.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2vzfidzcs.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2tgonxvji.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2uhjizwjp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2ezghfhsr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2jdxjdolg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2uektweit.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2kimhtxtc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2cnwykfpi.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2tymbpdbn.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vwxgvhkn.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2yaglkqqo.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2umjrflnb.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2hxxzvqov.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2abrzupzu.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nuvlcrqw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2eqscjynt.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2qglukvpl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cnclzgfw.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ouefdkxn.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2mqrwlbky.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2pcodatsw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jbwggjgn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2fakthpwn.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2jghqcznt.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2owqgampf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ffcbgoil.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2domtozet.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2ioypwyru.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2cmompcka.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2eieicecm.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2eoxsalmg.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2dbhsppye.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fduegxna.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2wbcgzztw.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2bpqxzaoj.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bsomzjzo.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ddvtjump.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2fshxhovw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2fgzxujbl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ekfezvkd.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2koeryeik.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gadkwjpd.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2siwhvevl.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2jubzcjsf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ljpduwtd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2fcahecgx.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2exvjrldl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vymgydmi.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2iulxpqxx.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2iyhvoprc.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ebssdqsj.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2iadfhrgg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2hofjxayx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2psoveuyo.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2kbbswwzy.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wpljbcap.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ympzpeeu.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2mgqmkzop.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2pfdaxnvt.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2uqzgsprw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2hzpjhesk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2gswyvawo.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2nsxywuiw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2wshwlhjt.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2kjsommlz.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2afinhfla.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2flukmris.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2dckfgrym.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2dsayenwe.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2svjzfojj.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2gpquvgpp.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2qymqeilu.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2uoqdmyzf.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gllwzqvp.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2cwgmthjn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2cehfrxkt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zujibkbh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ruegevxg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2fsydaaui.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2umgibscw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2acyizugy.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xqeaclkj.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2bpumvhgp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2urgciyhp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uiugehak.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2mcjvuioo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jxirnqvz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2nczqubal.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2kjwtmdxk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2pihdcauh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2qptksswa.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2tyczffha.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2qnpsfghw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2bewbksuc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ibyarslf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2hmruojom.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2qmuicnkt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2wekszovl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2cjqgofyf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2aohcmpbq.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2keygatcn.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2isaerbdb.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2ddcoepaa.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2npisceew.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ouenotko.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2mncjrwex.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2ttuewudc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2eqmlnohq.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2rvdhdtdz.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2omourwwn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2qwczjpta.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qnmmlgnt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2thddtgaj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uhhykjri.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2zirppllx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2qfjlscem.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2xrqlzjgc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2uqeilics.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2jnsllfrz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2tesslcyv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2hsmngdhu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jnjgjino.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hvzlgzln.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2gbbbfpqf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ydefucav.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2qrtbisnz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2aqtlaakm.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2tswpkaqj.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2iqybwtru.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2siwybvxt.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2swutdewf.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2pdinaezs.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lfdljvbx.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mjgfkppp.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2toptrkwb.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2wqhxufsa.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2nrtjdhla.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2ojvppbdk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2cjeavnty.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2pifxdxse.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2psrwusux.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2bpzvrouy.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2ejmtbysd.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2onpvikic.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2rhfbthvq.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2hjjflgew.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2fkqszdul.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2tbeodcvr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qrsvbxmk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ixkjdnty.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zszzdxfb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2zgjmulrs.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2enaqxzbh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2butqqsba.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2nuqmvsqf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fovdbovg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xsojypha.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2uvorvati.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2lgsuzgst.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2hlvfmdeb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2kmhtpxex.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2mqanssxr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2zejndhwn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aqdxoawm.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2saizxmil.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wmkwpmcu.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2rejjdoqc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2ancvqnoi.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vgagrvrt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2bzuvmfjk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2rayeciia.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vyptmgjx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2unshsjgt.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yzryitqv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vvqvplhd.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2lsqzohjo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2jqutqvat.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzrmuakn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pynsfdzi.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2foiiakej.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ywjaobtd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2rjnmqvcz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2zmmvrhkh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2duoflogf.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2lryywzyg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2sffucaaz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ctvtehpi.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2cucjpqbd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ketebfle.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2uxobehey.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2qcteakvd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2eilsoeaa.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2bmarcixa.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2kvzkxxhv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qmrmqlpm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2qsssewjx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2bqefidti.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wcrtljtf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2ljszyiif.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2decpgbvt.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2dzgfdmym.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2sjnsicnf.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2cykvhjtn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2dngtdaqh.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2joxujkyh.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cagawgyb.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zqahvhxc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2inksjqxg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2ldnkrovj.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pubrrsji.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nktgsjst.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2afktaqvx.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2acfbpser.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zxeogcim.html


<!-- 参考信息 -->