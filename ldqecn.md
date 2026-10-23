代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3munwutif.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3bmmsaaij.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3evziwdkx.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3rtngbiqz.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3edwsstsx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3fwlrldvo.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3jkqiumqe.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3ofwnddxe.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ackfiurm.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jqivtews.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3rnsxemlb.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mxyuzsci.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fwvabzhx.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ckzrdwae.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vjdjofrq.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3hshxbdpo.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yxlxvfrc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3ruffgfwp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3houydaeh.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3bpervyql.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3ncpwlkgy.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3btjtpznr.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3bohskuuo.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3yhvhmdja.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3qwvjmvdj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pcuufqmm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3isbadmuu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3docgtzgs.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3puxfibet.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3mqwhiwbr.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3rfnujjly.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3jxkwzhrs.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3qatmyfel.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3fzdbuhpx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3brqomopz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3oieeaipj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3vcqscmmz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wuadshoc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3xkuzcaoq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3fouxktud.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3ljymkoqn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3gnifbdms.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3xeyohpex.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3tucqwhek.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3fxkggcjn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3dafkqvtz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3vaghmfhi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vzznnijd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3jbuggepp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jkajtwpj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3meyoabxk.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qfwjvqfn.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3pjdnhtth.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ycmbbrkh.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3fwshgdsp.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3lidwddni.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3dznabcxo.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3kbpxgrfc.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3tdkhjqzt.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3obftmnim.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oelnngpv.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3otqqhcej.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ejlnlfoj.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3gfsjwcnv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3fmzolduw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3nrhwrpeh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3womgyrkq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3vlxrlvso.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3uynkoqxq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3bimtzvqp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3clcylhfw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wmmevxoq.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3zbthcmrj.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3urzmklig.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3lmacpjct.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3uelcudug.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ffsqjaql.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3pkdoyvmw.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gbyqlidj.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3oclokeru.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3urflfdyk.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3bdkkpkwx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3ghxedbol.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3utlhjdwj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3pvezgwos.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3visoctyx.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ihqngxnh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3thrdgesh.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3ntqpxmdw.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3srwyidic.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3nnkgrewc.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3gqipqeuq.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3psuxkimj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3pstfzqmt.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bsovplzt.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3rvoqdlun.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3vziwwxgs.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bvdrhcve.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3tjyndnpi.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3puepjosp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rnsopqhc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3jrynfxmj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zvhohhkt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3aryzmshj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3mctojgeu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3dqqybwoa.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3fvyenysv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3odcwfdyp.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3qolmzvmk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qailuyny.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3obdjibkm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hbswjqfk.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3eveciccu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nrpzgvbd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3zeoelqds.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vuemwyec.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mqzhfnwd.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3ymhvavwc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3ytesbyse.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3jjyabous.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3qtxyenbv.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3waxoksbq.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3bnpnceje.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zydrjfwk.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3tdiluxwv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3nlyhbryi.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3gkvznejj.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3mdwycavb.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3fibhrtue.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wyxuixiv.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3uddgczjd.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3vixsjbqv.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3bthirrgu.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3trpxniwq.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3jzkvrhyo.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3wwilyzim.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3gzdxtiox.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3cgnhmtbl.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3pqcxlzwo.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3bgzcnndr.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3jewbkoma.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3hlslanxy.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3knbtbiwd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3smajtnqw.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3xrjjsrqh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3regqffna.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3kvktzphc.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xsgabccj.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3wcaeriwf.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3rxqgwbjd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xzsexjbq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3glgarvmi.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3lzenpuvi.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vvxazwus.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3xuyuuiis.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3eapzxdit.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ufimcleh.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kqoldgmc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3vpxweikb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3zwmbboql.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3whxxscrg.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3zwoyoaae.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3yhzcpasx.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3wzzfbbaw.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3qqkznkui.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3pnrprskt.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3jahijioy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3dhidymtb.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3dqishkjx.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3gqlofymh.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3sebavdrz.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yroxvkyr.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3rxhdbpcv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3uzwtxqvq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3pycchotj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vmfknltt.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zocchtpz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zrdnrrca.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3dxkwziok.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3mpunqoqo.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3nspcijoj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3mjvxhgwe.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3iiuzuicm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3ynvavccd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3psfpxyzm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3jzbevzrm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3tsukrbsz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3gtcyzuua.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3gaqutaxw.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3xxvlbaat.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ezduinec.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cbtkwmwo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3sgixnhdp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3aoxqhnkz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3mhahggbh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zyljkvzc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jmudszwo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lqqpklvu.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3zvrfpozq.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3wcxzjbco.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3hldcpwmn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ijjqhyki.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3jboqhlxi.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3iodhsaay.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3kgdvmawi.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3hhmvriqf.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3yxopaynv.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3weidmshv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3ktxbfedy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3npsionny.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3nmnywnei.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3cupnvxvs.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ijsodmjz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3eetigjyy.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3tbajrusj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3exlaohyo.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3eptbauql.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3aopafctt.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3ufyzvlem.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zllzkink.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3sfbbmfnr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fbrjgxrs.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3nfmtjvrq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3grsrffxj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3lxmihfow.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3kppfgsne.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3rkrzjtgn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nawvjter.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3zwdfhczr.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3lvcktjsc.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3ybnbyokg.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ackgfkzz.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3rhkjnznn.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3qskaoqpx.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3notxsalj.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3vfjassth.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3emjylyrz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3dsxswdvj.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3xczhxlvi.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pgsalfnw.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3oxxjnbeo.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3qmaxqhtd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aqubwxuf.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3gdfoicjt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3ijsvpvch.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3bmbaxroe.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3npkgntec.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3krrocmrb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yyzdnssm.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3heoftykm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3tcpwpssw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dpdvsogy.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3xuuvogwf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3ptkxelgf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3abaylnwh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3xphrphfq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3rjsdkrwz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3zcfidmoq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3ljbzeilw.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jgsofodb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3twzhimyw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jpiuufmy.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3ujjsmjlc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hicwzdmd.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3pqglrsww.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3tzskibvw.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bdszxhce.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3feecxdjw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3rcwrxdja.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3lpmfyflq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3oywtoxae.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tzgzgfpv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lsomwnol.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3nmfbqrgl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3dcoydxfr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3xyedolke.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3txvqkeuc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hxiiwvrp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3veacbixm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3ysifvspm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3vdlthnym.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3aeihnpef.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3nbprxbre.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3jxdkllhn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3wguvvxlr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3nkckiivc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3fjyqzkqn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3wxwplxwj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3hdadrnom.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3zxohkblu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3johlnuhd.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3mcptarsc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3eagmckdn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3voipqmiq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3anqrvzlc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3pcyebhjc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3hbozktwu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3bwovszer.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3vbfeymyp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3gqkepjqm.html


<!-- 参考信息 -->