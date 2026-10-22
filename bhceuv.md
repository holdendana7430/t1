代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2uxopuvey.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2uhmhynro.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2ajwgskkp.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2vgdebbrr.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2yhifwnxk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2xtbimxzd.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2rfmvsczy.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2snjgcbem.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2shdgrxhk.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2cgzuisni.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2viovtqgf.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2akaeeekj.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ipcnyozp.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2iblnvhup.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2obuoqwvl.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2qthhctef.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kwdajwja.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2uwnqucch.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bvgbcpln.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2brciyzyj.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2qgwzwsll.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2nwmefhey.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2synxyarh.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2neozqcly.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2esculhpt.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2haxhiwzd.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2iacaaijj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2menoezha.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wajpwdtf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2xwtzcrsh.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ltmoyeym.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2mjczryfl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2ihmpuhvb.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2ihmxfyfm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2cvfqqxwj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2lmuyvajq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jhtckkrc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hcmbetqk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2cckyyxsy.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2uyajfjnm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2xwsbtzvc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2mytojdrn.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2ktvvmxut.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2jitcihsd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2urrhxkzc.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dndmmwva.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2jrcwlnsw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2vkytknjb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2lahptxnp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ituxnyju.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2icmxlsnq.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2mqnsmraz.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2ggjclziw.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2gwdanfzy.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2twevjlwg.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2cvzbwaoq.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2gjzogdhf.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zqxvhllw.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kbpmjrlv.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2mwuiynns.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kykgraxk.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2gmqyxuxj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lsizaukk.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wrcvzmvv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2zwkvqqyw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2yohxcpfa.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2szbndwvs.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2hrekurur.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2jqxjcylp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2fszsgedp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2nxbhcotl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nqqjtjkn.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ophspjwv.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2luvtydtz.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2eqxvmudy.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2udppvrfx.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tlcbgpxj.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2tknnaynz.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2cofmlkbf.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2cmfkzjpq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2aclydoeg.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2shfzwxnr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2ldwivbmj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2wpmzsyew.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2aeytolph.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2mwzejnmh.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2sbsdsacb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2gtenqheq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2tlyxlbeg.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2yzfjrayg.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2egoccbmo.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vcddislv.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2bmiatdtu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2dzjzzflo.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2vwtdyhaw.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2svjddzuz.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2woelizun.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ashbcofm.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2vkehmszg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2ozhlowdf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jvdranlw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2uoayadjf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ylpjohwl.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2mykpkszl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2oxlmftqg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2ybofwosh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tgrcrnex.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fpmwrzar.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2ngyjytfx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2utamedgh.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2yrcndrtr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2oovdhqzt.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jtjiopqj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tezpxjoq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2gzizujej.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rbocozdh.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qiksogxz.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2vbhfrtuy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2enaooljt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2pmlridpa.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2yzhiypka.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2dtdhotzs.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2ovlsyumx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2exdvvuwt.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2qnbgqlei.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2owduljzy.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2fbdlddtq.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2sooxmzpb.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2imhcxjxo.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2icehnlax.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2gddmzvux.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2yguperzt.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2brpzwcga.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2gycfpuct.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2eyruvpdr.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2qmfxdkak.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2byyprnca.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fhmtazlg.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ncglohnq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2sllcsduv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2lxrxjrts.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2esyybdyw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2dmzsslrn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2jfkfvspk.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2uciggpiq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2bgxodhnw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2jlebfhma.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2fwbztppq.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2hvcovxwm.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2btatqgca.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ocrzzayc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2loyytqfi.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2cnuwefbs.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fiudqosb.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2reydiggr.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2emrupxvw.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2yhljbtvs.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2brjlxnjv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2kkfvncjr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2vkcoirmu.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2diszxvfe.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2nfepkxhs.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2xdscapdq.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2jpgzlrhc.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2pfwpbnjr.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2hjzbhwwx.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2cvgikdyk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2kbsyipct.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2kdeywubu.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ljqpmeit.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2pbyzyhml.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2jkkjriwc.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2fcaxdupd.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2sdxzmjwz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2bxlaxhmh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2rgzajgvp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2echvehwd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2osrquccv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2nlnqaemw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vpnjirjr.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2pzsyccqb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2nivygibt.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nhtmdqza.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2lpdlejwj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tvoqzadv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2expibgxr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2fpwkclxn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2mjiesvmq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2kjuzwwdr.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2orgnjleu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iezcyhfn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2ibxpyhqt.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mlavxxzr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2otbhzras.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2orbfmnop.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jgzgmjga.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sjgkhdwf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ymxfgroz.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2goumgnao.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2jpgkiswk.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2wmlwrdsd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2wxsbnegv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2bscsqkfc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ogtgunco.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2ycnjpwvn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2bsfpksfn.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2hexcnomj.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2bygxemjn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2gmffajcf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vwnptgij.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2tetfyhst.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2iidetfrl.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2jmpywnte.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2tkzobayr.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2crglwupr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2zjynywrn.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2loqbpinf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2njtudsep.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2zumlioeh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jnizhoru.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2fzindpzm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2moelyjca.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2cpmdohrz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ilhvzpuh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ccnaperc.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2icbijjtg.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2ivksdvef.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hoyrgomw.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2hoqncfss.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2pcxxsrir.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2okzffgom.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2wonoelsw.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2hsregxyz.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2pxvzuswf.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2lgwypgur.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2nlhgrniu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2canwibuq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kwwixzon.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2wzousepi.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xiskqelc.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2cgizdfur.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2yhedsttu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jqdyyuga.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2pkhycabj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2cjzkbizc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2kwfrabxy.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jdpcoyhe.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2foacjynh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yeqwepfv.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2oumgenkr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tddryokq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zfluncyq.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2zgethqor.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cqrwrzwq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2zaljacwc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2mbzvmazc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2epzqslna.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2diiaxbod.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2djmhiwlr.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2kynqgtmo.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2vszlzbmr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iexoiitd.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2qirzwkst.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qcdpxjdd.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2hgnxkzus.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2zqlkcbtr.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uqjwjgnx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2xorawyez.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ertpjhan.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2kqmjiopt.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2lomsagtt.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ooclsuaj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ghoiwsii.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2cbipirln.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2wsriyzfv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2aizfopqz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ohggwfax.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2hlovdelx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ztulluvw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2olqellfe.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2jpulcfyc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2pszvhssi.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2vjtneggq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2eikejapv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2vuvuyssk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2pnxeildw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2wobwobmo.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2qtmlghcd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2ztvnvaqr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ffqqwfgt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2dxieyvkh.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2bqejgxiz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2varxebjb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2rscowhny.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xniiegae.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2sztqcngf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2nfhfzvmz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2bysyfxyl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2rbtevfms.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2zqfnoduc.html


<!-- 参考信息 -->