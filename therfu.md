代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2cnpleiaz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2yvinveib.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2ricuvhzi.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2bmgrgdib.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2lqgmcscb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2ownssknv.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2qftvdcgm.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2bqeiluzd.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2wjwmszxi.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cxgmnxlt.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2uylxhhxg.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2oxxzmywo.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qqxbodwc.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2vohvpfox.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kgmdjrwt.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2xugppmvg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pccglpbd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2cwjbslar.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2upzaobei.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2wswzmcqt.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2wwatcuel.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2jyetpibb.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2vfjrnlmn.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2snjgngqg.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2bzeuglcx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fjimevia.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nnmyoech.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2utysecvi.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2njqhuexw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2kadpjgqq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2obaoklrx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2hfafvfzz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2kxjbpmby.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2wmrkgywl.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2wuswqqil.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2ygeebbvi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2sidnokch.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2slblcgai.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2elopizqh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2jzshkihb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2sbqlndgv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2rzqzbtfr.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2jpjmdhgt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2kxiewasb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2sfcenrmj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2gprrsjli.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2rzdsmrra.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tfleuzpp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2ukzjfdpu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2wuumaxvj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nwffcuus.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2vdwmurkx.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2vcetqhcm.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iqotqgmy.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2fjwodiop.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ldmncxox.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ttznwemf.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hwtyhkar.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2otmgmcay.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ewboaofa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pqtclgts.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2uesjmqiz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wgvlqziy.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uoqfuwqi.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2veiyomga.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2waqlnmrc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zntzbxaa.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ouvsslnh.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2wcaefvcc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2pgzkekgb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2oobflatu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fjpmyxbh.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2epxypbfp.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2rpjgizuq.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gvcfixup.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qvfxptkj.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ufkeuetf.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fvfglist.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2imxroqtz.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2xiphuvno.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2xiiixvfc.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2kuiattfb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2kpwipcaq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2zxirluvk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ezdoqull.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2pbsdfvvi.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2djsxhcog.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2qnsytvxd.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2vhesecov.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2vqhtwfqb.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2mmbngvhl.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2vzswfvwt.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2aaiubmgz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2qsbujfhq.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lfahlvlp.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2meurgjeb.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2hptwpbpm.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2hjqkdpyf.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2awowoejl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2xypjthne.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zhfslexv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2bzqwyunt.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wqvndmde.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2isuhqack.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2lsakxijv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2yhfdrtpy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2drhyegfq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2lnwltgup.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2mqpjtxey.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2stzamgim.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yxghmhrs.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2roponxxw.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2meextmwy.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lnudjudn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wsbllwhw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qaiamyrz.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wjkrqiac.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2ciqtntyg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2yzeczdut.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mwsazmhx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2xtkgphbu.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2emvmkeaa.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2hrwazdft.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qgxaowip.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2osecakox.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2xarmydon.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2daazadev.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2bhfgqrfj.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2vuqdhqip.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2jacugbat.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2riasxkcv.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2siawjkfp.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2zqybxmfg.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2cqtjceym.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2zxubfgcx.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2mzjnuaip.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2dbozzezv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2onkuyodn.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2oghksonl.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qedybwki.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2yjwbyfzq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2jzsixqvf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ulcxvioi.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2jvuvovnq.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2muukiarx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ehkuspyz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2pzkllzwk.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2sqgyvsrx.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2mofoppbl.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ddjrjqlo.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2rirewvca.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2hyvfmxaz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2wmllrcin.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2qaccfryc.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2wjsxnfhy.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2kqykzrxx.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2eyrmszdd.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yemmsbrw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2npxonpon.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2htlheqhu.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2dwedogyn.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2cphezoyv.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2eiwtqiji.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vvwgejvq.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2utazwcaf.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2hfcijfgd.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ykctcwbr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2qutbvcqz.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2gfhazxqk.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ipcpopye.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2joxpjape.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kciivofl.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2cdayzizn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2zjwesfpv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2iyoqudqh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mfotnkcy.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2jgtbyuoo.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2qwmhmvtr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2ecejkwkk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2urxmwpvj.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2kecwhysm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2qgbqbjum.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2vedzmjmy.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2vhdapfvj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2annqbpgb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ehtmlurx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2gjjkmnwh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2ckmjlsbg.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2narzorpw.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2ueddnjaa.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2oeslpoer.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2eabohikk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2kekckfrp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2uptkznzt.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2kfbugnph.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2ywgcvwkj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fspcymzm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2wdhkymru.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2iwxqqsua.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2zbwpkuap.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2rmmtqlvd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2afbseypb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2djlujxky.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2afcgxnjh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2webgttdj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ismqiafn.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2lghfdncg.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2xhwbnqqf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2jjrflmfx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2stjjmipl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vjgizrju.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2acmihcth.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ymckpdrz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2livgfdxt.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2livsfuwf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2jeofgvxm.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2exzectzr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2jvnlcahv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2nexabdek.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2pzdfvucm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2fqwmmzda.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ijizqfhz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2hdklpdkp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2rgliwuzi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2kmiywwwb.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2wtooswqu.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2ytfblmzo.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mzbuswfk.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2pwbqcnva.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2uhnffpki.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cjbvdzmi.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2dsuzshxr.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2kbjubwvb.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2yfrvryko.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2tvlelrmt.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2owkepcuw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2ngmazitw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hittybyb.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2hujjneoa.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tvcihdit.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2yodtpagn.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2nxdfgvlh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gncupafu.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2tjvmndui.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2qkyhgbbz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ztdrxjoe.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pkaoprrz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tsqpdjtc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ikhnuxfs.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2xetysoja.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bfbnunsc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yavyomfx.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2tcqikzso.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jzjuehsq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gluvetwp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fbtnbirm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2qegmghay.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2kddmnugu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2mxpqvjfk.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2gxtklhsn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2hpbaczag.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aqfvbrkq.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2hsdpsxft.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dkhakplt.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2qdoyfxnb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2pacuxxgs.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2npihxsnw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2cxnzmgev.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2xpfwaqdo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2lkykhcyb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2bbbvzuzp.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2owgiante.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bedxibvg.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2wyoxtbvr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2ioevtjei.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2ixrnwhaq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ghfdcqwq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rtquxwmu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2cxhjmvwv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2phdtkhar.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2fmjrljim.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2hzvlxvxn.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2bgnsoaej.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2xtbzqszb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2uhapggmp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2photoqeh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2oqcpqmwg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2eulwlhis.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2djzpccek.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2lxavhuee.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ovbxftoz.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2mmbbyfqx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kcbdnwaf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2xbqthucz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2txvqnyob.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2avtjhtvo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2msmikbje.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2nkbrtgvp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2cfeiriwb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2rwzdrohf.html


<!-- 参考信息 -->