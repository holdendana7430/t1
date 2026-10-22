代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2zvfqcjxx.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2azxciubd.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2guspzoeo.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lghzahfa.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2nbyhzyir.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2aswvbygw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2qsopixbo.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2xujajgkf.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2qmodklko.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2obzvukkh.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2cbjehiof.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2eepewhkp.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2gwszaqwd.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uzrzoybc.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bagrraog.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wospojot.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jzxdxhor.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vlooyfrl.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rvyndsex.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2xcdlzzjc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lnymzzhx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2njoupkmo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2ocnpymja.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2uhjhvyqm.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2ytkohzdx.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2slajwgwp.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2vcdouulp.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2giyptfzi.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2rurvvkue.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2yfudlkka.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2fapzzhcp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hatrubou.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2yofnjaju.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2hyhnsvgf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2vimrgkef.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2edqpncqg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2umvgionv.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2dfawdrer.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2alevxlzn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2qlvzvqye.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2odzmngec.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2giihdzkn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2sipquhgy.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2hzeebwbx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2tjckchgf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2vvvbqzho.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2pofhyisr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2lgkaunex.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2mxwqhaib.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bpmjopwt.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2drjyncug.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2veakfaas.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2curupfjd.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qnpjdcvt.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gfosabwg.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2auupxlls.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2uwjrosdy.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2raeobgdf.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2uwcmpgsv.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2pxxzmbpj.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2gehozxgd.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ibaainlo.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2eapstown.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ggqelpcv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ghiafuob.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2fthvjpts.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ezdxkpwy.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ibaynpwj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2zyciybzy.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ckdefoqv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kfpisijp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2kqliacjn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2ckmbcpie.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2skmjpfqw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2celjwuwx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qwyirmmx.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2aumueuxz.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ojpwhczr.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2akbpmbhq.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2cywascvr.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kqnhlejo.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2sdflkhwf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ptfmtotd.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2xwfknoqz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2lpomvylm.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2otolwkkf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2tadoebrg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2uzmgfmnr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2cvhqcrgb.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2jhecduke.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2faqbutzd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2qdgvcsxw.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2bprktaea.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2vmamephn.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2eoyiemyy.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2cmefxstq.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2dxvinoms.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2ijnmhtfv.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hhsxdpwx.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vtpvsroe.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2ltlfhycv.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2tfdsvfrn.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2myymhklg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2qkbivpqd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2eulqtwvr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2vmizvqlt.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2sqatvtwe.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mqltkohi.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2cdqrbxru.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2hnjgslsb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ylvwaqou.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2cudgagug.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2ycihrwjy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2griljqvw.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2sexdfnoi.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yberavim.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yadywoib.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fmymuhwk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vmihdsxt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fxcrbjau.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mmwstqfm.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2cgvuwvpv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2tskimcva.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ekwjlqij.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2pfbggfic.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ybkyaokr.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2ustvxiwa.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zzrwlfzg.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2gvxtrati.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2jfmdnwup.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2rxshphsg.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2wohzgfjk.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2ssnrmqdt.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2mkvgcnhq.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2xphpngqq.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2gsfzulnw.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2sdpfkqtn.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2dsvevsis.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2vdtaacfe.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2xcdkonii.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2oblssvjy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2cmztoffy.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2mgsabcdm.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2yjbfsapp.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2lystcxqk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2feiucjfb.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2tzvudrtp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2reozndrj.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2ogdmramu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2aadbixmd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2ponvasyu.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2szgjgrvd.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ksgkojfz.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2dejxgpuq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2qrqxcgqe.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2uhqmnywk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2gphikayz.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bpmkktur.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2mygebxfz.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2mmjximqv.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mvtiuayn.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ulgrxkgs.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2nctprlnu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2dfajaszr.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2dmcyhgug.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2reihkrra.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2dvgxtdku.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2feyrigus.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2zubtmnxu.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2yjuxxnax.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2lmuettvq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2cxvgvqxy.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2rcfplpqj.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2isgdqesp.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2pkomrsog.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2iqzocuhi.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2fzyfuweq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2uvdixtuq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2hkgzvhay.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2elacgvsy.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xxydsfaj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jeptdmlx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2lkzfdaws.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2lmwsrxbx.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2vaudelwx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2xnzejxaj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2dwcpnyrm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2xufrynuq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2wmfdohqp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2gbmtowzj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2aorwqubn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2hfemhokk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2nfmxrdjz.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2dposnlwf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kkaknaeo.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2fkcycjbg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2ocanifew.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2bpgeitzt.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2upwjoznb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iuqkofhn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2cqrwtknc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mvnrmkic.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2rbmxnelh.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2uagvhtbk.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2avzxvmlr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ifhlaswm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2jwxkrstg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2htbcqore.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2jnrevwek.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2zfknqesl.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2xlqludew.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2cepyrqtl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2gkzmaiga.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vetqocva.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2acrgnycb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2okddxjcc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kevzxhpa.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2xictdvkj.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2cljkypdq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2ktpwjkmi.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2eqliaztn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2xafyfrzn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2byqiiysx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2adlepgtr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jrlrmhuv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hihpszkg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2rvzdiuph.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2injocioi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2yhdbisqa.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2keotkpnv.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2qnstytqo.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2iaymwmpt.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2rwnozuqw.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2yckevwvb.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2temefzqa.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2jsbvcjdz.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2rmnxaijh.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2hmfmckza.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2wzywufzk.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2yidmwnco.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2ewmnebul.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qrtmxxki.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2rrvfshhl.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ikcyrfas.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2buwlakmf.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2wohbmwkd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ilhzyyky.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2boygkyyt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2nghotgfx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2yuveiqgk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kaddibod.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2sljwzzpd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rimlsvss.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2tihhzkvi.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ibyuwtza.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2llthtrmf.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2vzeguxls.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2nscfsytd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2vntivdeb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2cawlvpbw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2nffdljbo.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2jvrqaenp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2pagjldgd.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2isupyejn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2zihkuppp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gqzvddwv.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2relemumi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bbrhawwd.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2diudcjtq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2txrinkke.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bmxcvook.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2otmkztog.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2veioyyqz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2bzrfdmfw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2jbmqnjcx.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ghshuzba.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ccgmkvyw.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2zpeycjga.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2akzjnozw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2xgvugsbp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2evovibao.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2kaqxpgzl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2nqzzmrsq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2gpgfirft.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2oxzthkla.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2hizkmfzl.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2xgpdipcd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2aaqmpjnf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2gakcecjg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ytoezewy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2byngxion.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2peuvukth.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2rnbgoqzf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2neejzurg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2yixyarly.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2blruheha.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2evpilhsa.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2mlynpjei.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2eymjfugi.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2udplaxmv.html


<!-- 参考信息 -->