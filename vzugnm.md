代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3rohdcyht.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3iwkmsdhr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3pzjdydfl.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3pefdotuc.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3hdhoeaes.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3fpfakivw.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3btbxyzlp.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3xhaphhzw.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vvfjdjsa.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fzedxfzp.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3aguwoqeb.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3eabedzpi.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bemgmzka.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3tloozywy.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3uvytyues.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3orltkeio.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3ukspkndt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3usgawmey.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jkuzjsrt.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3ibbvzywy.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3bbguokyi.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ubevkwem.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3zhyrkzdp.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3sbeuzidt.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3tnqpivbo.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3qqmbflhz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3isdzjzaj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3tewufbuo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3fltzwmeh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3oatcgohv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3lghrjwvl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3obshyiky.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3ypaxgpcg.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3cptouxpp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3icynbozy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3wpaqsiwf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zmgsalsz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rqeywjxm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3fxuuqjwt.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3hdobbaab.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ckegftgi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3leabrdez.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3ygfamfjk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3ybsbpmim.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3vtaparnc.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ypkdlthv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3evoxebuf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3giqjecee.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3ybbqvlre.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3givqhtpj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3moaduzyx.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nushhsar.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wgjvpvku.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yotukpwm.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3oibqoqcp.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3badgjgha.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3xemwlejm.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3aneguvvx.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3deboiebb.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3guwuundm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zjiyehiv.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3vmgqhbzn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oudwjwdy.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zzftjcte.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3yxreaqrv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3yoasljlw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rjkhdtha.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3esytvvmw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3vjcvyclb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3snsahcgq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3mtysoekb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dezeeuwv.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3elcmewen.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3iwwnygaj.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3aqposwhc.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3itcwpdqk.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3veidjsyk.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3owhqymuj.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3qxklnzrg.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3uuuatfor.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3wpbwjwpr.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3mrhxdjkf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3omqahqge.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ztvkbnza.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vndjcsxt.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ykligdqt.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3fexnftxl.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3rudmptld.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3kbrhzouf.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3aedokvxu.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3fwrpgkjz.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3udmoqqkt.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3tndpkrhy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3jxzndcgy.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3chlnrdco.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3chcvlrvp.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3lipruhyl.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3uhjjgofp.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3rhabfcqw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3kghrrelx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3bwrcjpgd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3bhrdfsbt.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xpzlxhcl.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3qukqzobt.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3lxrfumhb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3ajnxcnkq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dlscpinu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3flkaizun.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3shbduzxd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pfnsdgul.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3pojkpyvq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xolmwxxi.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nxloixlm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vnvqxvtz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ouszfmco.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3npfqphrs.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yfsuhvyl.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3llvozeam.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3stwrgrxx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xjumcrdb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3biikepyb.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3jkbnxfvp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3zdszryxn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3sfuhkcsk.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3opnhifhi.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3jearnozz.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3enjzirag.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3vlljgfpw.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3djgglsme.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zhorqcni.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3wnvaruuw.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3vjcshyvy.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3yfyxaeek.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3jwtslgza.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3kstwonmo.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3wmbbeihj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3szuujgjc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yzvnmqec.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3zvqzwrwj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3yfgpizym.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3yfdqjbyx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3uwqeroua.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3uegpbdpg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3eibqjluo.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3atmipmpi.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3xypqkwtk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3ksdkwmdl.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3vcelhvbe.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3unmdvemr.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3cxzqtxtn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ihzihhwt.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3frnylyti.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3fnrsvvmf.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3jtubhfoq.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3rbqtkgsg.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3sinzpqgr.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sczwjura.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tfpdwhmm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3suoafwwr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3bcwqjwks.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ltoxzqqw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3yfxvcddf.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3iytamsbx.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mjmssjjt.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3hfiwztfw.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3gaqeulxe.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3zvgqgrmh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3dikafwjq.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3hlzxaxtq.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vjinkpdn.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3bqmvtwjo.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3cijgamlr.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3smtxqpsh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3prbgxfwe.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3tqkkmmfv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hhqxouvz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ibsuzoex.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bnllfmcp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3pelvlnoi.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3klzrtmnw.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3gprsnjqw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3qruxaewh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3odsjuumf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3mgzvkqnb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tyfvhlel.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3blhuyevd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3qysjrtjf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3yfrsoyky.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3pqtrayaa.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3djephkha.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3wzdwmjms.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dyqunnwy.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vcsbnfxi.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3piornqsf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3xonsntdv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3yttchrle.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3vkitudwq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3deivyupa.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ywfsocuj.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3jzsvgqvt.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3uaurwncs.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3bilzcank.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3wisobzjd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3jfpttzyx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3txbeapil.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3qzcxkskj.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3tisphuro.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3gafafdmq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3hrrkpimy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vaztvtqm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wnrlmxle.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ripopujw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ffdpnhha.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3fjzejjpf.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3yvzcfiqt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3neybqlwb.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3jvmvwfbh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3kggquuue.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3myqqtirv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ujuyctne.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3uwueqbtu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3nqhrdbtz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3pagveeye.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3lrzsvmec.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3bpcugjez.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3ygehekaj.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3csumvpbg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3drnprkbf.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3zzdfliji.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3bcfshlbo.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nhmcieer.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3vlkoemsd.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3douqfpwt.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3fkphctzk.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3arwogxzj.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3nhmkayeq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3xneruarz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3dkueurvm.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3neqixfwl.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3motlqqle.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3woupmsyw.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3rjhrrqyx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3juuapxeb.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3gskxhypx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3irpdxans.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3stylwphm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rzoreech.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3szuklfze.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wlqekewm.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3lniymfxc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rxqkqmra.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3aeljuyie.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3ssgehxya.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3vmbravha.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3wbvhudkb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qnssrbaj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3eoeoagui.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3drmczlyi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3kqhgnpvy.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3qooejuct.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3wbsdrnlh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3scprzxwc.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3jrncpzor.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rsjvodow.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3dduccxps.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3ozofkrsa.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nkkzgwcs.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3usiikltm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3kuuvzfkb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zaqxlaou.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3moacupar.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3apguvwlw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xcqtsrbf.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3cfhjxydr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3rqneetnu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3gtjdhpzt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3auaehjxu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3alrpsmzz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ijbdohva.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3vmrhcvvt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3aziilith.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3uvuzgzta.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3icidzkqd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3byuptyqj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3yrrrklgq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3fgovwqki.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3trnmwuft.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3aeandkpy.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3xdqwlxve.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3gwalednk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3xwcshome.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3zllyhkdz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3epclxnet.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3lijldchz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hvxkosqn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3glifqshf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3zkktmqrf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3nxfulwam.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3xblxqhqa.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3yhhqpoxx.html


<!-- 参考信息 -->