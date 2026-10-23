代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3fchfvzem.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3njvjnzne.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3gsfpynoo.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cbvznbng.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3acmoidmf.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3qwbwxjyl.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vzpnqwrr.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3zbqcqcmy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3ldphnwvc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3massycsq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wdwcgdqd.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3mfxmegxw.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3djxeopqe.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3pgaoykyg.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3nthopoob.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3moswykdd.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3cqhmxttj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3izlgnjbv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3omxwfvhu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3xtaqjpas.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3bifqxocc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3ruxjjzcn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ajgetymj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3uunbsukn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3tmjugsra.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3ixybdbsu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3kvsqsckd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rsqbkbnv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3eaiphocm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3slscvwel.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3wyvwywyw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3toxvgadw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3fzhdifao.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3qcglzzqz.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3vgsbiwld.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3zsyexpbe.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ugjzbkik.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3eaabwgwq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3fammbvct.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3amdovjeo.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3avczfrll.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dfigfxeq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ipkrxice.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3ecdaormp.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3xemadwvd.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3livujycv.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3slodigtw.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ngzgoauj.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3augmwzme.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3hdxiupuh.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3njvjqeht.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3vsbuxqlo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bheizfde.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3wqfhkwsp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mmgxklqy.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qivohjyt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3zhfxwmrd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gledesso.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dcmxduny.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3akxvnsfk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3fiiftjma.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3dziilbhd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3kxyubdin.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3aqevjzdg.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jgompwje.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3tlagqopm.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3qxieangy.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3qarwecfo.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tbwgrzlh.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3txcqstyt.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hacahlgx.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3azbkrbkj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3emrlrqwz.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3osffgrsc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3ivwikkgv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3slnjwjio.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3fwpsfzyc.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3lsajdbva.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3lxtfzptz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3uhjzbzon.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3knyqiqyw.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3inviopxn.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3gnwgglkx.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3jhduzpkt.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3jvdznjha.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3jvqbftih.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dkkricxb.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rgoycbbw.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3dqkzuhmb.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3dydtqplq.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3jwvbezto.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3tokubmas.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qmuytayh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3bsqcprdt.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3fnkklygn.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3arqhywjf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3zjvrxhpm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3zyftiokn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3yivsxseh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3xongdsjj.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3qsppuqyf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nemlxavc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3vjiyqnkn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bkvljdvq.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qaqtnirf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3djvldhbf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ghhepcjo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3trjosebe.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wodlhpxd.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3zxbetwhf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3duzshvrk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vhpmtjax.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3fjstucgo.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ufavpcud.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3ltnycpxk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bmtogsbo.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3yyjgvnek.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3jdcwefyu.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3gpoiloup.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3kyvykltr.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3nsmwqrqa.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3pphaxshd.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xxpelsep.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ppfpmqdp.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3dxhucwib.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3gmokqqww.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ppynzyri.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3ttcdebeh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3cjhovjkh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3htpksslx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xenwxbyl.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3kpphmiyu.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3zqigxspm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3vqsbskby.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3ufpdynxe.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3fwwxvzaq.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3xsbjqjih.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3pkauuhci.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3rcyhqsqy.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3znullqzn.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3hpgmgkgk.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3gaydgcih.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3cfcpmyaz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3jpqykhmf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3otqvfrnd.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lkcjnloe.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3trgxkbqm.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gwwfmech.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fwprmyko.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wytycioz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3wkgkfepm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3fkuefvlj.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3lvawrlcy.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3vgkjrpts.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3fktwsmrd.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3psyxwuvx.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3lzapjnjm.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3zrupwpou.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3fjuvccci.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3ezsbbnkd.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3vqxhhyzi.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3cyppnkbq.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3uhlhmvsp.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3ufhkwpxg.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3uchtmnsx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3jxyzutea.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zbejawel.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3lieslini.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mwnstnus.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3jwbshflk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3zbbdvgbf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3pkamuhqi.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3pekqhosu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3fqegltje.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bhklrwse.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3xqicjiii.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3mpzrgpdi.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3mubnpuia.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3lklkijio.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3tzxbxuqt.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3fptfuzmw.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3cqckocjc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3iztdzlmc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3smnwofbi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3xyekysbc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3svmndviw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3nasvuxxg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pfdttenc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wcptngbc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3awriradv.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3tdehqmxu.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3cwzaqnea.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3nxqtmsku.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3vpcjxaie.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3pmyxaamk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3nvcqkfae.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3jvjyvcdl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3geupvvho.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3vyaekmio.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3hhcefkam.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3efsmmjdq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3gprljjlm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3nqhnhypb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mcmwabhu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3rnuozrli.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3grhyqnen.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ttiyuxgr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3dsicykjw.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3dxdycomi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3xdwhianr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3wggnavep.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qqewgmje.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ttwdpfkk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3robiuotl.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ooycnvyl.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3pbkzshic.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3vxbmynjn.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3fkmkjfjf.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3prwmezxi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3dvtxtyqq.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3tzefmwcm.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3pycwemzc.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3tvamgfia.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3kwkrnaby.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3ofsnoxsc.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3yohflfub.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3kzlcizmz.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3cpnoxmmc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3cgfbspre.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xypznglp.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3gyyskyrq.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jfgmapjt.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3iljjrxbn.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3tzlgfuae.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sxazidxk.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3ugvtoiro.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3fxkqbwlt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3mypuqctv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3pmrgsjyz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3csokgixq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ckfmvent.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3fdjujrsy.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yclzzgpl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3yfcvfpnu.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3nwspbskv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3pilntubs.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3emdfefbt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ozjuzimb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jkkvtxdk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3vzpfabet.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3seukhfye.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3tnuclmnh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3qhyxkjrg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wttxudsq.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3baknngdc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3senivfbx.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3hboyrmzn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3myqcwysl.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tpmglzga.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3njmzhglt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3blqiwnax.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3gvtdshwi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3imgngeea.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mopdvhgo.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tcnnmdtn.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3rmfnokne.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3hogdoblp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3vfpqvpcz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3lydjaxbm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wqtoomua.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3smimughm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3adqmhjit.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3jpozkqpg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3wvorcfru.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3kuwdfqbk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3iretiyte.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3qwkctlfx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3xwnadply.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3dddmfpqy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3yuwgvjji.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3qichbwkn.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3waysqdvb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3olloneon.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3obdmebnk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dwmkdiaw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3mpbipuak.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gcvzhrjg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3kbwecxwt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3kdbkqaqr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3joordncw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3nthrypkh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3bzvwtouo.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3zdnscgjr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3qivmlolb.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sxnakztv.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ntifehzx.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qdrkrznv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3nxqoekop.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3rskqljtb.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vbuyvqxj.html


<!-- 参考信息 -->