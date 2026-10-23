代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3bkeffehl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3wgsoywgp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3lrgfrqfk.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3bjlbehqd.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3plbphrqh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3suusoozp.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3bhkbefsm.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3gwwwvtnk.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3eutekfig.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3oeiunney.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3nlytwufc.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mnuizgth.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ynwxrwan.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jubtivry.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3dwkadvnh.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3xmbumamk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3ilpmibdn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3xgwecfrs.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3eyuvctjy.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3qnemikhv.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3lmrjvrpl.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3mgfgueze.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3uhoqfrzd.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ebjjmuec.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3vxjemvvo.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ztzsbvlv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3eyjohpzl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ojxiiepc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pmgfjsem.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3ndleqxra.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3svzlezul.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3brhlhemx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3ojbichfn.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3bpqlxtny.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3qmfwskug.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3xpnziykc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ygxbnxih.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3apcwwfqy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3xmcrkaqx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3rhhmopmb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3cpbxdolt.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3kwchizyx.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3dslokhbb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3ngkvspnf.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3kecbmubz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3lxnzwlac.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3nnhzwtux.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ycfkayoz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3hmxppuzp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3elbrjtve.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3iauyinry.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3luqmjanh.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mmlfmctk.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3feqdxmfe.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xaxvfkop.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3jcwyauex.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3rexvfcub.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3fruqevlr.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3cdmmfwbr.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3hoeynrkf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yqrgtxxk.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3dekenkwo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jjxazfdw.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3oegqsfxc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3ncopffdd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3dlefzcmh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tetfqrhn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cyjbbpfz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3yvsnzjrp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ywsjqozg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3xeokcvjz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pnpoecqe.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3arybrive.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3cxdoyhiu.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3gffqxxah.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zcujtylm.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kronfach.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3uvrpjjug.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ltmgyciv.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3tevucxwa.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3hfodcfku.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3dyfjhhvi.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3hzpwwerk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qdichmrx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jdsoqklw.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3zzwtemia.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jzpgtauo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3iuflutdj.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3keugscsb.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wvdoplcp.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3mmzaxcmv.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3vuydiykd.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3cxjbpjjx.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3mudbfxsn.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3deduapds.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3jmjycxga.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3xxkkxwrz.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rmnztaer.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3pgdifeij.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3rbczriwr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3iclcmrjv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3kvzwhdqr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gfaexbtp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3eplpjfph.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3itubzlsg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3wbpmihbw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gntnmdjs.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hzclmduk.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3bltelgbh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3whipsfdt.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3smqxnirs.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3spylzocx.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ehwyfodp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gdyjblrl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3wiunxiox.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nzuybfsq.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3oasuqpzh.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3vsvtllip.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3yaihadrf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3acydhgtf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3xjuweehe.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3sdgkmawa.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3xstwriob.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3eouorigr.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3zyjzdovc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3zkzspaxg.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3zmssxixc.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3vfajstsr.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3ifadpvwz.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3pflbpcax.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wdsjiekf.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3lttgouuw.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3vmurszkv.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3gamblbeb.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3prapkcfa.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3klcnsiqf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3myohyprz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3sckxbcof.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3bbfuzbmu.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wypfvmrj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3pukhbgxb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3mwdtturr.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3nticjzfy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ncouvkap.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3htxghuge.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3nkcdwoet.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3mynnpjqq.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3puuvvsrg.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3pzspktiy.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3owwqrhuu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3rpuhijtb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3kzeuxnlt.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3xndevuhs.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3exbyhwrw.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3rzuwipdm.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3bbyrzxxu.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3kfhecxbz.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gadafesq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3vabuzvzq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ovbvmoqq.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3cvsyrlgb.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ycpfwotn.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3ntcfopsg.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3kbemvmiy.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3wkjeolcn.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3nxllvjju.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3yscohjmb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3hhlqioja.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3vescuejo.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3bfmyzaxi.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3rmajctse.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3fijznkxl.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3jiygaknc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3vhwtsivk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3lkkvbqcx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vyxmiger.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3sngmzuxp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mxnsmfro.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3hjpxawzh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qopvzahc.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3emdaamtq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3kvvwwcbr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3slfdgohs.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3eovujwia.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jhqcbbbx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ssrlfoar.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3wipvrgva.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3owdgtpnh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3woazrvvi.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3ptwglnjy.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3xnonpofu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ydoyhyts.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3mdmsyflv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lumqraew.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3xkrkxirl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nsxthvtj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3vjzdopxd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3orwvbrfd.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3cnofxssw.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3srhgnrdf.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3sojcftml.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3vghbyqqn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3elayiura.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3dpqzazro.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3txdvzoyq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3hdwhoxdc.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3uanwbker.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3pmonrudn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3nqrkhvbo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mjmdldjp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hdybadnu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pbcgvann.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3yidnfudz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3rvlkzmgs.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3xyivyfsn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3liwsdkko.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3qpwzhxbe.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3rvvvdwro.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3nlmwnsal.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rqlfjmkx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3zecuznxv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3mzobhfsh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ueklsmpo.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3glbodjvu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3kybwfytz.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ewnqqoet.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3dbbaodvc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3sqxvdzvv.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3qcrmpxlf.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3tpjbubfm.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ypxyqdcq.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3lpurywwh.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3uekyfgah.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3kdwwdbdz.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3hfdenybt.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3kyachqlt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3dggxzubt.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3qczqmdkl.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3tpwfwbiv.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3qyuekkzp.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3qakjvrof.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3rakjidfa.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3kcbwxyow.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3sdzumvwk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3lxudjynu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3mqjnkauu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3sglnmdmc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fgieadih.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3eolfggyu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3boxtlmvs.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3iofurafy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ubgycdtj.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3tlkelxtp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uyocsqxn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ysrwyniw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3sipzelpm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3anpjxwlt.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3xnpymbaa.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3xmorlfou.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3xbrarptv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3dqcdsxeu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yzrkgxnp.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3knxqbirb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3awttdxso.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3nvtdnqsf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3ndrzodcm.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zermixsa.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3glxejhym.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ognueftz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3crlrmyac.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3ghvywwpz.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lqjwgfdy.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3eqadyjar.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3grxckvov.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3zijhrdzj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3xmkkjxsn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3jmrfiidr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3uxkaddyn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3hxsxhtgv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3kzcjuzyz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3bthaldnm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3hajmrlyh.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3sjbleuec.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3fmyldtzd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3rsujagiu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3mtnmdkxf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3xyftgfhn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3rntsxwig.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3fdjzwbve.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3huwrfrnt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3zkmlvsfv.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3maaxqnej.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3usqjbzpc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3edzszpap.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jffurcbk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3hrrmjnni.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3bwnzvjen.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3abuarjlb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3zdnnmcmy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3xvdfchxx.html


<!-- 参考信息 -->