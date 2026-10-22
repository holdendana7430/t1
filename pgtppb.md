代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2bnzucofa.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2tlgvsltq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2ykgaqacr.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2nreailyg.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2eoinpcua.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2beeboirk.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2aptmliyv.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2fndigdrh.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2bamhgohe.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wtzhbxcc.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sesbbbas.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ksssrimj.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ksiprerm.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nfolxysb.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hokvgxvd.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2fwkfapeb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2mbunghvr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2ketrgatn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wbujmzfe.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2hxixrsvh.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2gooxsvmz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2sbdmzxbn.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2uwysxqdi.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2okbueoop.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2hxrzxezj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2oriuqkzx.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2oijnspxe.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zzhevplb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2yygwarqg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2hvykqptt.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2csemkzmw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2pbbjhcjg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2wptecuwk.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2ibncrqjg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2uxmzfnsx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2wppthbja.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2qzhgzmcs.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2itxipewf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2mhccmbtk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2szmqknhb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ueyqfkml.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2orxkxetr.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2cngpkemw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2wyusjhuc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2fqsluysx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zymamifr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2cookxezu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2wlgenmub.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2mfhtogrf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2pjomkzmo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2hcchogim.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ljlvcezv.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2esalqgvb.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jqpfjhyp.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2xuefkfzn.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2lanueqvm.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2lzcdcifh.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2mybfidbt.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xlgrxmzz.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2zkzaxrcd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2omnxkfpr.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2tllnfcdd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wbqjhenv.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2xbsrugbc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2savmygzo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2jamcruyd.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2lnqcleah.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ulvedvxn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2abovxejr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2kklltkep.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2cxvxzluw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ovwaonol.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2xlucwohw.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2wemzfsit.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2hwkgjlxi.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2fpjletow.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2budukpkv.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ezeswkah.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2uutbnjmh.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2vbvedugz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2ojsiupro.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2akbqicuc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2thwqgane.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2gmlhbtvm.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ftmsupre.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2cpvtvpnb.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2itddloim.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ihtxtqsp.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2qcybwzmp.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2omltrjcm.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2yjfabrdc.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2spugyybx.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2egrloeib.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2cuvxsiup.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2aibjifpt.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xzcrbuxk.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2rmbcahxx.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2lkdhpxzb.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2sczljypp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2nbpnkcji.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2acqkstqn.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2zlgqvjfe.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ohtwlkgk.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2fyauemtk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2cxuofrhf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2zmfmlzcy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wblrhtih.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cuyiiazz.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2ydzjmbuq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cdrxdppi.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2sfxrzflv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jnmfmuxn.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2houwhykz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2acmvbpfc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zbsihola.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2uzctlvaw.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mtaywimk.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2ewhhgdsw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2drpxlcuc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2tketvdaj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2knxznxem.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2icwvbdwt.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2aogqfyhp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xuognnjd.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2zecmntrf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2hhkzrvzb.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2dtnnsjqu.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2svtppkew.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2bgvygkhe.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2cflrhxkn.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2hvdzlzpd.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2nzrpngwy.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2bqcmsucf.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2nckuphwy.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2xkwcfhvi.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2duzcqayn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2emgdoyrg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2wjtaukow.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2bxsszvpk.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qizegvnr.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2kyrmjbcg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2zhqglrzz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2soqlyrpm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2xwzdrkdo.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2pxubxgqw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2bvytbttd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2rdjpmeig.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2keehadxd.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vgbxytej.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2lyptuqvr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2gsrqmzqu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2weyiwnrl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2kloaffpl.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2ixqumrnj.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ubszwwrh.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2oaophgrz.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rlcioggi.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wnnsuolk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2gclllmnn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2zyctiyrc.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2jhbuwwnl.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2pmmdjswm.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ylunhwgj.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2hjschhem.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2wpxosjfi.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2supanrqw.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2vcwvtxpr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2nfzgemgw.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2bpdbxeoy.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2hhiukuec.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2rwctbhmq.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zfstuytk.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2kpmmmgdp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2zhjiufnl.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2oppmccjq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ysnzwblg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2odnhprmr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2negstlyu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2yqeszpcs.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mdlcuhdc.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2xzottzag.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2nawcycgd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2ppmrfkuj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2nmkputge.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2esjmtiyz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2lrybqleq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2gyqqnjzi.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2jphehevt.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ewbrlpqe.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2kbnjyvxj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iqmigimi.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vvmbqewh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yqudbsmu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2goedniae.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2liynaxwv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2doxenmbh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2iqmaejpo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dccexyoe.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2fjbubjie.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2xifavfge.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2ofutkabj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2jmvkekwe.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ocghhvrq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2eleezykm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2qxdjxawc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2wcwrhbia.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2pjsromzc.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2etogkttc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2rpwxwndw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rfkaklyb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2soinuuko.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2dctwyhha.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2mssgdxdz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2irvtctsy.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ialwlkqe.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2wgjgicci.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2iryyfrjv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2aydnkcpo.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2plkkcitf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2cyywfmjw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qbisjkgy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ldkhliru.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2orqlxook.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2yufwmqmv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2dmonptac.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2vyalfdih.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2vtxttazr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fyxtsafk.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ntqursnj.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2adtyhjjw.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2twnxwjcr.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2rmarvfol.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2evdmuuec.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2fkuznhis.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2jrtllfkn.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2dclgrczz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2bdnbqcno.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yorcwwbd.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2ggblbfux.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ulbvpejx.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2innujarb.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2dumcuxtx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sesexeaq.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2hiivanlq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2pytjaanb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2vqizmgod.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ducjyhsa.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2uhejqkdj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lhdvldxm.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2ktvuvzjm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2msyannte.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2drnpbpyx.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2ssshqyhl.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2klcqijvp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wajrkikq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dlzgwgjh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2fdmlmjaf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2rxqjuujr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2kcyptubd.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2enbkeomq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2oyjmgckz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xppxrmuv.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2ocsvvzug.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bwuwxgru.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2gvxoalag.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2yhoggizq.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2stdjuntv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2yoylbjpn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2bvuqrfnj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2kjmciunq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2upopdkrw.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fcwmelwt.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2axzmsrxk.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2cbilnpnk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2cthfozvw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2dykdblty.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2amcbgalc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2heffthuc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2iskdprii.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2innpqduz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2bvgtinxu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2xvkflqdn.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2ncexdwgc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2jlxyslmg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2bczfaxqh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2jfvgskzh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2gzusggne.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2vmgxlfev.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2pspvhnkp.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2esrphjpo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2qomvofoy.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2roccwise.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ljnsftck.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2ijyowtlm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tjljfsfj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2toeitxup.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2uxrzlrmc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2keuhojma.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2szqlwybc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2gjtzdxlw.html


<!-- 参考信息 -->