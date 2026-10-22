代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2jbqpcktz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2iidfivxb.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2snvbctsv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2zahsueca.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2fhxehwkx.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2greeqyvz.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2vtnemmby.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2odgktrsk.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2crppjxvi.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2pqnbusgf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2pllygoze.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2xysbosda.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2egzejsdg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2cnndaknz.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2ywuogatm.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2gpgqevez.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2tdikyztm.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2irdzzznf.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2cequtnou.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mdqroxux.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kbwfpshs.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2huzjpjti.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hweshjic.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2cibxbhux.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jhuteqjr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2ppeibegj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2yprsutql.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2kglasjzl.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2pvupleun.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ruutgexr.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2mstvurwh.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2yscydwuo.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2xfzraajh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2xugaftyy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qasokluz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2aljttpsf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2vchilyxh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2vqhhssmy.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2sskznzil.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2ewkvqvlk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2uqniyfym.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2gsosnlsf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2qdpwshss.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jmjltmsg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ipnegkzg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mamrlice.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2rrcojqfm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2wspvrkkn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2xmjbhbji.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2aqhhwdci.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2xdpovtmx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2kqxxklyx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2ewnwssbs.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2pqklrgoj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2ihlbulwu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nqjxixza.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2sfowoowz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2xvpzjpwy.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ouuzxodg.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jsdnbkib.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2eswmjhsl.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ontfopwx.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2smidajxa.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2mzigsokj.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2rboprxma.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2kgfvwneb.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2pynfezup.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2akhydwpt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2injlozfw.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2aljvamxn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2upvjvalx.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2omnwfqim.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2hlwekjat.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2qjeuwgiv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2iauqoboz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ckpinoou.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2zhrmgqqe.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2tfkakmfi.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2bcgyufjl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2raflyvzu.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fusvfaxr.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2hbswqrhj.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2oudnceos.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gomchgmr.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2iknlgcwb.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2fctdpyup.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2yxwkzqiw.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2tjlhjlfz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2lqzyrruq.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2cptsnaot.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2rffhmzuz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2krurudym.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2fzhjmfcg.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vrxyuerg.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2rvdcvved.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2jmwtslcs.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2mfghouhi.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2lkrovynw.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2agmuuwwj.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ohjyosml.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2xngksoex.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2uytxychl.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2sgthhvoo.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2cfxocknd.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2zcrluedu.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2jpfdcgoh.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2htvtmyhc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2vtbpidad.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2xniinseb.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2yfupyysd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vmxdixzy.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2iawbiggo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2hislqlzf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2bvvpaygo.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2asiafrsb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2aemuxbim.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2misbjmxb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2txiljutv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zazfzwdm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2stiihckw.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2miumopky.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2aupmvidt.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qedqhfzu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jsztxtnx.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2sejppmyu.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2drkxeozj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2hzuyjwdp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2uiqixdgu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2fpsvmshg.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2dymoqnix.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2laearkmz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2jdaurzdy.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2vbtevguy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2zvwnuwbc.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2kyzjickx.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2oubnczry.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2veghdbcg.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2efbsusun.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2hwtowrik.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2jtvzmcmi.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2wcvzmyxh.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2lizqrofi.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2anexizlq.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2yxfthass.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2nsyzrlga.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2lfskddxd.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2zswcfmbn.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2rjaqymtd.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2qlxbxvli.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2rjhzloum.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2jcjcskbk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2tmmncnpk.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2otrripvk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zfksvknd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2tdtglzdc.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xcosnhvo.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qxyjsbnn.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ybaedjii.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2khifptxf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2zyctpabv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2mqpkzjfr.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2zyqqpfgi.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2zoukxfor.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2eajajowp.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2izebmpwx.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fyyefvjt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2kxaxlpah.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2kojvfuxc.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ovdprucb.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2acjrymmk.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2dkbcvdrj.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2mxmlrisc.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2zbxmriee.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2cevfnwid.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2quvfmbgo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2uayfivia.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2jjefcvig.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2gvmetalz.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2daezmbpn.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2oxylvmee.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2klaxcjpk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2zaqhkeum.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2covrudcq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2kwljoajb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rcnkxjaz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2sffcxwhf.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2bbnnyvjb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ojuwvlmo.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2sqdevkdo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2haguhsvc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2kdskkjdd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2mvzkfqjf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wcnqqome.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2wlkbvajc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2jzvqtauq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2khpoqunq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2skqzoyvr.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2nryzqqpr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2gjudwpdx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2cobzdpzp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2tubdinon.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2znoccpdz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2nrohhpsk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ajnphmji.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2puwytbaz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2kgugzxdj.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2cbzitxmj.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2fgtaqcbn.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2hnatyhvb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ktijzxrf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2kbfajjww.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2izkkemef.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2zdbfclvm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2qwmptznr.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2azovlrbp.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2ydijvfub.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2gotixrpt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hhggfcgy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2vmlnuoop.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2toudrito.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ojtddjdw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2jdevbiog.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2dqyourgp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2epnmjfjl.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2ddxvuhdp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2tmrdzxfp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2aplhilek.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2miiffpzu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2fedeqysl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2sawjjcnd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2udaoglpo.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2esmhcjeo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2trktuboy.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2qlhtkucp.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2nsvnscas.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2inhkshot.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2mshxlcmi.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2fhkavown.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2oqymwftn.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2yvqoyryf.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2whvgbcib.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2dkgvhreu.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2vwawxjjm.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2gtbcxxar.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2tskgoszn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2ledyiwbn.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2chxagybx.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yjagoral.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2rlnkqyyj.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2bcosuuaw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2dqzjrysc.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2ggvlgddh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2lxdysgxr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rmicfpno.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2epapmorw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qbddlkcy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hnlopsdo.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2vesgivxf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mgncsdjt.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2udoliswi.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2lksknnzm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2aztrgwnp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ctfvvcju.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2hbhopwnh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2knnzrwex.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2bpqmbikl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2hzymkyxv.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2teylctaz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2gnrhblis.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ekoxeyon.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2abxuoxko.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uifupqws.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2cdngzfsv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2pytbvofx.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qdacjsse.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2ajnsiucn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2zgzhiihs.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2oegmahyi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2basbkxgg.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gjrhprtj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2anhtmptt.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2olumeyrv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2mieevemp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2lmdcqsoh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2vjqodtes.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2vopxgsdx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2gqwebeuu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2xhvkbceu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2aykpyexe.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2izrvduaw.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2bbvfnlvi.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2dyfmdxuu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2gqblzoln.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2utyrpyaj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2hsznpesu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2ezrexbkn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2aluyxkgs.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ojwnjazp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ofsvusba.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2xisunopy.html


<!-- 参考信息 -->