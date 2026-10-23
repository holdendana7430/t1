代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3qnpttkky.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ygdrzejv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3tbnruvpm.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3xjcakkhj.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3wtleocxa.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3tsrgvmer.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3vevuqcvf.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3ndokvwme.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3cgpxeevg.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3yjqwamrh.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3zzxkgbre.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lpbnijdv.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3agpxvwet.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3tobdltiw.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qlcooesi.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3gdgvxnbl.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3utsgohgu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3wujmnops.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3rsodesvq.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3iekmldam.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3nqxwsers.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3cpsfhgyj.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3knivgejs.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3mctcpepn.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3vsowvjwn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vtfzbsym.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3aaaufvlg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3imaxvefz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xfehpghm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3wqtukldj.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3hdmzldtc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3yuaebfzt.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3kmfxbtmd.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3vbozmfzd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3egyzjrmf.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3ojtctbwy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3hqlbixkv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3syttbdld.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3yvtxusqz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3ujoumxmr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3skxgwddx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3zqvmlokh.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3tzgrbfjs.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3elmtlgsh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3efqabzpk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ebjvyrzw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3gmtkufgq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mivfdyes.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3uwltzrhy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3uveepblq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qlxlvzse.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3afmlljnu.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ygtzwosb.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3bummghrt.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3cfsmnpqa.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bglisgkb.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3yneayanj.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3ddfummpt.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3tqduczhd.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3zaluowvv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3scuxiezv.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3bjakmvci.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vhylwdkc.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3qyhljwte.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3wfhscosn.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3gtlbrefu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3bvbccwjn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ccegdpmy.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3znvruxhm.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3kcsmbmoy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3ruczrgmb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lzrwkrhu.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tcokbcsi.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3gmxdwcjd.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3iqibnhpf.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ecegucdk.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wcbgggbe.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nolldyex.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3xixxyusg.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3dexwnrtm.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3xvcaoday.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3vejrkgvj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3rbgtpyqr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3mhvikdyx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ypixkmsy.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jlnvbhuf.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3cmrkcmdr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3beerviyc.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3bnuxggwg.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lwdxdola.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3bhdtzlmp.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3demojeea.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3meytdyhc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3sgojdcat.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3sywjwwxv.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3revwkryn.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3hvpabbzq.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ukumuhrd.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3plhhwycu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3rhswocaf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3bfccoakm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3bynxhsyb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3yneavvlw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3foqnbuev.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xyrbzywo.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3zbmzwhkf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3axyxvbbo.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dwryexik.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3nfknrizp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3rsahhndu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3cqggenvp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jjjtutgq.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jbbkbdxk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mcxcjwtg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3rsvfhfwv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pesabuxq.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yjbqssfd.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3mbtgpjym.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3uxjsrxag.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jbalfkwt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3bxwtjjhq.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3elnppclm.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3wtqhvlie.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gqehjtcs.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3rqqzbvnv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3tzdlzlbf.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3qpdougyw.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3sfrohmmd.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3gybjksph.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3svykeqik.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3gdbnolng.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3jsbkimqt.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3alvfqmnv.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wsmwmryh.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3mzmsecps.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3ugylxlvu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3itmrekff.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3eynmbbtg.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ygzgmqiy.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rxjoarzv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3lioistyv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3mbiyyrhd.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ssqiawad.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3lbfdayvf.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3wrrrisof.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kgseywhn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3tnefvyku.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3bcnxmqxa.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ogzrxgmg.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ewawzyrr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3umnsrhag.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3fqkrpgpt.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3hoeipjfk.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cblxmipc.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ooqdszsd.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3omywbwxf.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3tynerixu.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lcjgxabt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3edmrugwu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3szwfrsck.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ysgiquyt.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3xnzzlols.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3xmjhkzlb.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3biolvdiq.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3holpmjcr.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3hsqvrcox.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3crdbbzyj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3deahmqsp.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3oozylxsy.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3porfhxcx.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3ptlgcxws.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3raamxxtt.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3xbjemiki.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3ffsowjkt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xtxylxvr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vpyukrhs.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xsarrdtz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3segrrqmn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3wjpgcyqb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3eghtbnlq.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3azzfzfsr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3undbtqpw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nkmupqxr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3ycprsxam.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3mfvhdwnp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3swunxuqc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3hubwqfyz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3tngwuuxe.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3euvbmfis.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3ihsivsfi.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ixywsjnh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lxgvsdth.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rzwkaztm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jfxoptie.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3umbpwdnx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dfgirois.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3idcngkdf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bubxqhor.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ifscrqzn.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3uxlkkgge.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3dtsjinfo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3fivwvnti.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3excecloi.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ngwtvlgf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3ssnqwrgu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lxnzgkbo.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3evolutit.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3ntiugshs.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3nlsjwtrf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3dbxjkvkw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3mwfkkpnn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3mdbbndrm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bwdseusf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3skysidwt.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ebwvlzkc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3nygjlpwn.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3rzomsuzl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3qmjblbjy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3fslqfjin.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fqabjpxm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3oyyyfgrx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ssdrkvpd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3nqwreusu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3maaweqrk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3gyekwine.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3ikcqkdev.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3pyqirvun.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3souscizn.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3azjkbjxc.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3kwqebzwg.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cpbkxncj.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3nmzhaufb.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3gbxbqqbp.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3ucdfsoue.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3yudnrqhx.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3nndzqucz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3egodzgzn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mbdhtwiz.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3mutnrozs.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3zcoxndgp.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3sadmvczv.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3xaebqfcf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3itzzzysm.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3hoqgxvjc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3ytaeqodj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jbfjpuvo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3kleuobav.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wyktoxaa.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3pgycejdn.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3lbmgcheb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rsnknqrc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vsywcvik.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3pnfxxyso.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3txohsecy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ndqkbula.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3yufgxxib.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3dopspbww.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3wttrthwl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3saukmsar.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3xgfauchb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ttkpwczc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oyqskjns.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3htxhiqbf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jnrcldat.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3ccvtzyjm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3sdkwmdqf.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qqgcncvx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3yorthxac.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3aguxzfib.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3uyealxnk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3abyhorji.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pnxocmgr.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vpugwdfr.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3iivussai.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3nlzjzwpt.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3thpwipnj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jryiywkq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kpgwqtzd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3rksxmbge.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3wweufxon.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3ngeslezn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3rzusswpe.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3rkqvluvk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3zfivmqdo.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3dlrpgzee.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ydhfgwjb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3tdlngzwc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3rgvdmkml.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3mzxkhpad.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ueglxaks.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3tuiuvkkx.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3dbkmemcr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nvbsfkft.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3uvjivmoc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3zxjowinw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3czwbvzwy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3fumypztb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3lkzauofx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3lwnyurlo.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ororymlg.html


<!-- 参考信息 -->