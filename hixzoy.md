代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mjcslkxj.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hmnenkrk.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pfcnjmdq.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3mbzsyvnr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rvcpidve.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3uivsqzrz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3klxctuzp.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3rruankni.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3zwzjltpf.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3fiuiavsq.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3trcrsxcx.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3llrykktw.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3gaopbrmo.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pimlsivv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ljwtkgyi.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3zcbmwwvc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3qlqxegtm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3muiyjqdo.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3mvergtnp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3qtjysuyk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3geedyzvz.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3cptumdhg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3dbjxklzc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3uyspbloe.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3fypjnptw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3wndhehgo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3dwrgdyit.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3qadcudsg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3zgnhactd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3vlqtijux.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3eqthwqcb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3swchsuhw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3xvuoeqvo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3zebltrhl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3nkbdmlmq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3oeeohyil.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3vvombwdu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3lswnqsbx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3wyrctraz.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vgmmkmbt.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mfpvcrrh.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3twcpezox.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3nhovbyle.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3swczevdj.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3kivhbdok.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3pqmagcku.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3fcqbbkbw.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3qspxtzat.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lntwrwlj.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3ubmwovmf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kwpfyloo.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3obgeayqu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3ygtpvcgv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3odwwjouu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3vbnsmeda.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3aiukzpvn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3hwjzdxhl.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3sjxzblam.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3uhegmffz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hobggsal.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3grxayqli.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3xbwqusgi.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3etoswppi.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3wvpeyftj.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zynojyqj.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vopxhgiq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3imcbbppk.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ifjxfelv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3difxvqon.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3xmdyrdnx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3gbylgzsn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3gkbmbkzn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3tpnvqjnb.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ghookpzp.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ydqfnpuo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ygqdbrog.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3nbpyyxik.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3etdymjvz.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3vuvextfj.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jsjonzue.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3rxsaweic.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3kehvzvsg.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3fsafwrmg.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3eqrstgjx.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3ekzhwdjo.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3zhfizyxb.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3plsadyvq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3fkicvvlo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3qzytltob.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3lqruzehf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3mwhssgmz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3jgsfvxts.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3aunaajub.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3ltqpaqyo.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3raeirvcc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3vzksyoks.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3vmpjshbs.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3luvqsegq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3pcwbxjko.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gvgvcigb.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lqbuhcof.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qieqaxzi.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3sggyrgjt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3voxysdgw.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nyxnblch.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3wunydaga.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3bgqbaucg.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zsmewels.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3hrotkzsj.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3fkqyrzbe.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3vdlbxyie.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zxtreyni.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3wkgnmqim.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3esvxnunl.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3ybrlldva.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3petpkyfp.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3bmkwsayu.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tgdjadgt.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3mllkmnch.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3knbostxu.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3ucfixspa.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3elheyrgl.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3weguvgeu.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3pqzbjwlo.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xdmayfyn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3qjezinwr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3swkfvdso.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3bljiyjyd.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ssinafxi.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3zczfudnk.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3qwbdrxve.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3nbcmfyon.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3sgmtlrzz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3clnuabtb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3hrdflagi.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3efuulmff.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3fhwkhynd.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3zqzuyhhc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3natufawb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3puymtfxc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3mpfftzyf.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3xgwxkjbm.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ewnzjptb.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3vfhkcfnj.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gpnlwagh.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3pgdgijjh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3zhejebqx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ekhnamqm.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3vsdtstdz.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3peqqfyzt.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3jsusejnr.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3fwvrqekx.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3gqwqerwi.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3bfwphrsz.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3qgotzjtz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3xzsldyro.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3uxtlxcet.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3jcexnbdt.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3uhaxqlkp.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nsmovrjd.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3wnjjpspo.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3cgtnxuyt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3psxvlqte.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ssshwpev.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3eoasahyo.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nrslvqgk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3nrcrechr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xmqpnfqq.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3loemnorq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3dwvldjqv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dwvfergs.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3idcwjppa.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3toitasok.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lhnpywfv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3fqpeajoe.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3onlfnggn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3agvdbewi.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3forsplan.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vbcwbqgr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3wbbwkjgo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3wayzllag.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ntmbdaho.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3jkgjnwbn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zfrhemec.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3dftabqmp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yndovkbc.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3hyyfhrwm.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3dluwholv.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3raazkluy.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3efysiksa.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ashavbrc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3jnfqlymj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3wxvrumdn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dzrjmbtd.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3fqckteih.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3qoivluhv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3rdfdyftp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3rrpruyyt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3nbxoufbc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3nxrsikba.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ktotsjnn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3qwhphvzu.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3qgjzozrf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3sdoogikt.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3jadpykdd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3hrbxphxr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3duqbnmue.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3orfmvwgy.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3xxwtsnak.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3hcnblbhu.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ryiexllf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3aibgchhy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3meyebomd.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3luhzdbjx.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3gddkjhtz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pkketwks.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3hkdyumtc.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3syyyxvlu.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3eccwqrlp.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3naetskkb.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3mzgzrpfz.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3xhyewtzb.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3notyceyt.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3msmohjpd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3ytqjdfmu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jfijqwyz.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3vkzajqgd.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ycchciwl.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3qwiakhbz.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3tlnscefm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3ejagswwb.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3cyqnnlpz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3ldbxfhtz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3zucxotkm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3chdrkwwn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lzjffpjw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xqbfetkl.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3yfqgelho.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3syxzmliz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ggpmjwwg.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3bhbljqcw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3evfmzwcp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3kaskpkei.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3nkmmadmf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3kvaitquy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3pehcwipw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3pgepahsr.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jfkfegwg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ryhujtip.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sifqvwpm.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3bnlwthlc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zlywyyzo.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3lqbnjodf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3aqfdvbgd.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mhvknjla.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3uyvjhtbh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ithpnsje.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3cofjlblw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3dntwmbcq.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xjiftsbl.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3geyjnloy.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3zoqcfybs.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3vbawjjrz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3dmqlbrck.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3evjwmllu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3joufawfd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3dzunpwiv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3taevnqvh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3gccsmlvu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3jiwkiwrb.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3tslnffuo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3wvnfxwsd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3whejdbbd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3szifzmqs.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3velcitld.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3oozlftsc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3sjdaangj.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3lmqswcto.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3jrnldpai.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3xlhttzem.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3duiyswya.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3usbuvpqy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3srqonlef.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kudgyyvf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3xsnfbsft.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3okoqslld.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3prruuoxs.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3gfauyuge.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3fjhstvzh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3ekjvlcka.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3amaofvsc.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3huqzmait.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qljqtlus.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vkhgjrqh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3cneexkhd.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nakefvnv.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3erkcpwuu.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3xepepdrw.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qrkyeibc.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3twixxshs.html


<!-- 参考信息 -->