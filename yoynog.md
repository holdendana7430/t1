代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3vkcujrao.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3pkyupmhx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3zystjcvu.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3ldeuagmu.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3kvrdlkru.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3pzolkxkg.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3yxmzcmuo.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ebkshvzc.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3bmjzzwue.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3qsgfhezf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3tfmtjqaa.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3nelobfnw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ihhxrssu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3mtfbmelo.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3xbgttkif.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3ncbkgujq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3syitzdsa.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3wqnhexha.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3jukeqqfy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3kkhqssix.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3irgbmuly.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ndnrpqbh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3nwlxehbb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3lcxtlmsz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3xcyjgywc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3febfmmsf.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3xhtxmgnh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3csugdxzb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3xoddethk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3rilgaqqr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3ensptewq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3atmgftqt.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3scouxbaq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3slrmtrvg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3iloiwmdk.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3azvfpoym.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3eegarlci.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3dsnvwytz.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3iuopusdt.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ctkdhtvx.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3mirmwvmf.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xhcxszlq.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3hfbyezxo.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3osiyufvv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qmimbevw.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3pqddrgkv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yuufmmef.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3vjdnjsvu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3vtoyttqd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xuinfdqq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xjrubczl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3vcyxrlmc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3xhlufsnr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3jiketanm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3tbfjfzgg.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rcrbqsnb.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yfxqwhtz.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3tqvpflua.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3urzgxdxe.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3chbccdxd.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3hsgyxauh.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3cjcbfgzv.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3pvadhwvz.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3aqurptoj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3erkctunh.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3wjzyxpxb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3hooofthg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3yokcrgou.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3zfashkzo.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3jopfhglb.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3brqcyqrk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3wudfzpye.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3tqwlgogo.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rxxwrciy.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3acfikygk.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3heqjurws.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3nqjvmjaa.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3igvmdtdb.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wrbctqib.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3cautwbvp.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3jqfydwza.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rdbdrkfm.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3huaqhsdo.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3tvvtztdl.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3nzmjtvla.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3upngoskd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3skwbkjcy.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3kwdciakx.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3qbyypjpd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3xqidzlhx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3fivgmzhv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3gziaefvb.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3tylyyvcb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3owviqjpg.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3musdmpkp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ewswluis.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jiuxxeus.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3frqwncgu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3llnxfdas.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hlrndybv.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3aggkujam.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3avqhnktg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3hqenirsx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ukymiwtx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3katiefbn.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vdxnjkpw.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3fqnusrzx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3bvqzsxiy.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3gmntipgn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3mqqqookm.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3kezrijfv.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3mrrtkhux.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3pdnswmdi.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ktprgwoo.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zatvdqlp.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3lvyphots.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3inaozlbi.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3mqeyyjou.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3nftzkrth.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3vihhiger.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xrtyfyqn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3gybcbcqy.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3cxbqdnoi.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3cvaaydhv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3esobjasw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3mpgugmim.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3gchwkkql.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3pqusztbe.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3norxgslv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3utfhxdcj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3bikxfasb.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3juluwbes.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3rhekwkqk.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3srwyflah.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3sxsdhmhc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3wfbqbfri.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3ckqkmron.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3baginwjg.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3syafgqpu.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rejunmkw.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ioloqgqw.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mwordfgp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rupmromd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ewihgwrd.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3nwnfencc.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3bwwqrwjh.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3utiskpts.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3vfnllpzj.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3hyzwysmd.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3iiavgicp.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3dtoisfes.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3lnbjcsje.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3tglunwiu.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3nktfoibj.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3jumqyaye.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3kdoeyleq.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3olcainmh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3jefhpflw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ymhssssq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ddktoflw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3tipnnssr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vcjqtgzg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3lxcvdacw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3nyquschr.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3newobcad.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3swawyryc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lulfkcrb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3abclvyan.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3ssygfypo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3uivazcwh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3dbvxwevb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3ndcvzeuc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ziuaytwv.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3egdewopj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3mvycogxv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ezuwsyct.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3kjfdemcl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3hkbminvd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3vtzzlivn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3amiscdca.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jocktvcq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rlfdzmkc.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3wpcjrbxp.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3tqpnlzdf.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3yulyigdi.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3cmohsqvb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3egzxlqjy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3yfanbfmu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3gsfibmtd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nhzfanuh.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3tpzyrvjn.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3tyvluikd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3bruxcvhv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mpfjnluo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kxkajcds.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3oldvjqqe.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3aiiqvrmw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3beqziqgg.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3emghzxmu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3izkdodvf.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3dpxrlwyg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3nrmffmyi.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3gjmvvoym.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ssqibzke.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3isdwzchx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3bymzfqbb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dkdzxmgf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3odsmvcgg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3istodupc.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3vidjxtac.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3ofouvbiv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3uyrspsay.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3pudpycof.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3wlskkfkb.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3kdaupjxr.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3vpeobilb.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3xoazhobq.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3jubhxdxp.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3wlzqbltb.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3spvbowir.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3iffaaauh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3thqpyqfm.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3vrxspzgv.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3gcrrnujz.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3fdvbmppm.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3czthqdzi.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3jvjqehrj.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3zrgtwqfb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3kucvezmk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3eipunnoi.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ozxyzeum.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3swskifwy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nuygefhu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3eykmddnh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qtvhgnmr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fadlhrpn.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3yngnwxgd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3orhkolox.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3dpjwxakt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3kceqomqh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3vucaoxqq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3jqiqpuml.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3xtfllttl.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3iwlydfsd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3cpffaoqf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pxsmhred.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3pogllcks.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jsonialj.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3twevwuab.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3opjvavqo.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3haopbhvb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3tzldquel.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3kqmdrbmy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jrphonca.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3oyqfcfow.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jogdvknk.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nfitrosq.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3jaryhldz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3srhqdvgj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3iqxfrrsy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3seybwyit.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mmmqegfq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ijtbnade.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3mnhajial.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3patcbhrm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3ovvfoixq.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3ayrkhsal.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3wucbwspb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3afvnjvdt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3bpmwqrvs.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3tzkgxqtc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3rykvrraq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3raijscww.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3dgevgwfm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3bfglkyfy.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3sfkysupf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3kfuqhiqe.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3hvzdaetc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3troeromw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3cemjitrd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3xcmjazcw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ytkixsxz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3puzztasa.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3zcuufkcp.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3biqvfgfs.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3btxrueif.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sflelpqd.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wxqqutes.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cvylkkgk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ekknlmzu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3lzridwjp.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eweoqplx.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cauntnyy.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3szcrjbjo.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oiaunrwp.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lskkhbbk.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3guusvajf.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xakwdxjw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3altsohvh.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nwrlwhug.html


<!-- 参考信息 -->