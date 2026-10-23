代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3eorojwea.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3bujlckek.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lugmzpdz.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3xwmtfgfo.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zsihrkhg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3lserntbi.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3ulaznuuu.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3ourxvbxh.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dcxhigwq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3njlfwmll.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3ibsazhow.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3azkajaxe.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3tgudezsx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3aqpfkvoj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ogipsmim.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3txrlsldf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3kxprwhwj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3ntwuopeu.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3abqblogn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3todjsqsl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3hupvvhco.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3cmwslguo.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3npiswpbv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3tfldmjsi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nsftdkqy.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hhzivtht.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3uwtqhfkm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3lpdmyong.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3kmvzomrm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3ewjmbawp.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3njxhhiwe.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3nhjqinvm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3oxvcdbrt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kjvljifo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3nzhjpdkm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3bkkrrfwf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3abvzfhuw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3bidlqaxv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3rasdytpw.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jzisdcwx.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gxnperao.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3eeaphiux.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zkeinpub.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3siohgrpu.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ddpgybfu.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3vicglzxo.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ueodxrdp.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3oulfrdli.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3anwitfqz.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3prtncisq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gashyrbc.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ldrdsjdg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3bkkibpqs.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qeptrdmo.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ozkqrnlm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ppcrnooi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3dlyxgxde.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fcxqkbgv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3kfhbkfqz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rvmshpnb.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3bsjkuvck.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3rkckwesx.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3aprcazgc.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mybuluyw.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ocnmywvf.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3bzeidrxx.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3oldsisaq.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3dkxffovl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3qsgccdji.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3fnotskjg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3ocropdro.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ouanmaoh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3bunedsws.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3itjtuqbt.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3nlurabca.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3skzjbqwe.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3unjbsogq.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ppookckd.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3wytfcvii.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bicjoglv.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3tjchdoie.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3wdcpcicq.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3hnxoybsk.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dtpurxwf.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3ukwiaveu.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3udrxripw.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zcksxxma.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3vpdbhljc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3zbkcxgbe.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3nmkxhzjz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3tqqwpuvl.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kmwevbig.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3upqjpzvn.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3iqnkzbsq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zxnvrghm.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bfyqcjrl.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3mmtldjmk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dshzitji.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3hvzmkssq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3iiazjrgy.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zqkbtmbc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zehoomaa.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3hlzvsxme.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tivegggq.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ssntrxyk.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3ehmeqfmk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3cimxzucw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3glmjouhu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3bomgpupv.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3gaqfatqr.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3jrwlmljp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zfskliih.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3asmejjcc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3qsmjxuoh.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3ltjfzpdf.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3rojsoqlo.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3luvwzida.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3nkgihgyf.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3qwdzdink.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3npveqgej.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3lijoqgnw.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ecqdaqyh.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3cbjyxfat.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3vbkggnhd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3vyanaaxl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jsuqksok.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3xxppfetl.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3prrkiavx.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3umvojvik.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3ugkcbxxq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3pqoowdsf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3azlzwqeq.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3cqkrxhyw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3bzkzmlff.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3rlprjkgy.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dzyjckqz.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ghtzecsd.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3jsvgcaqc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3dhooondg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ibwiymbj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3pqfjjuhl.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fqeurpwh.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3mvjelykp.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3tcuwlrfu.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3eomahzmw.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nigjbcvs.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3hminektv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3giwcmyzx.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3jamvimmr.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3pnofivoi.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3wpxtvhvk.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3fkhkjown.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3akexxazq.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3lzgnduio.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3pkifftle.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3hgudhgmj.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3xeksjjrs.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3wpmwliwe.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3btkizoww.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vjjolzdj.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3hfrzrlvz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3jofhofda.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3hubnqkym.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ajrgezdq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3csuddxhd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ybwmrzlm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3jasvbfdg.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3shqevhat.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3wzoplnra.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3zddojceq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wzrsibtq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3mfelrhtw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3paecucyn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3pgokblgh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3dfmzpvfv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3burbmqod.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3iqqplxjf.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3attcedov.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nfwfoyys.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3hjqmycbm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3scubianf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3kblhmkth.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3jcqcydjz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3yiwpblpq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wolyapgv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dglmbkzk.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ikwwmzww.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3wbplcidb.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3tkttnjwx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3eaqkltlo.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3rgrcadcu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3dhgzqdqr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3gakxtpcs.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3lvnmntlc.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3movilere.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3nxppmhyl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3mkwcxdke.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3fykcvppi.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3rtezzohc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sbljfluf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3odpnajfc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3aiqchwdh.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3oifcrlmb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3ijjrkasi.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3hyduqrcg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3avftbexj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3mgmrscgv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3dsgipsaq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3dkazmsvh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3unghsagw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rilxkqgq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3xdxapqre.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3reuuznhv.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3smxiiulm.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3dlscsvvk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3imgqrtca.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3vfcihbqg.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ylpyiuyp.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zkhpublo.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3dsyolrxd.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3cqkivrwu.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3jiuvckie.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3resrngfm.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3wicyunkn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3ebbjfzqh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3lryykbaw.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3rpoqymcx.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3elcvefga.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3ivihkynn.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3bmouqyib.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3ievmyhmb.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3qziwhcdt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3cbqopxvg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3avwdrlzy.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3synovnxt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zwodbblf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yoyqeyvd.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3bnvvtiex.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jhrzhhel.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3kplqnexe.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3farthawa.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3atfmiiqi.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3eupasxde.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3mxhkjsdo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jwpcxwfo.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3pyptxdhk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3mvkkvgxo.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3azfxxqwl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3etawloxn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yifhufrz.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3ucfjmxhm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kcemkaik.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3ylqntitk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3horcxyem.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bzuzsbnu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3exgvifhe.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3adqauqtq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3izszlekk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3qjzgngpz.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3modhshjt.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yyrrjcwk.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3gmwgpayw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3wveximho.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3oaotmrwv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3okuxgshg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qqfidrze.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3jqdzrdhf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3jyhrnnbs.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3zintioah.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3zzwsnayk.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3bhqdobfi.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hvkiwagu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3yttekcnc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3fbvjwhmn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3gihxuwqz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3dwwrfwka.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3qcrhgauw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3biwmkogs.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3qchmupnm.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3yvfvykvg.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ouommhsi.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3viqshusw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3rgnqabcl.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3eefnseeh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3adyrbqpk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ojrsutaw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3juzaagqx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3wjhwauap.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3ydhwrnul.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3zjulkefr.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3agrzhiug.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ltnvjvvm.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xbwpzexi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jfiqauri.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3vtxyahos.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cwghypwh.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oxqvcjit.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3gwuyvgkp.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rmslajcb.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3clgkunud.html


<!-- 参考信息 -->