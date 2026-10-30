代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.hesvh.cn/Article/details/gczwipkxv.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.zdbjq.cn/Article/details/gtmnqqfbc.sHtML

Py:   Counter(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gweswckox.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.zdbjq.cn/Article/details/gnkppvrbr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gcnuqenvy.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gplunevpr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.zdbjq.cn/Article/details/gbfshboqm.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.hesvh.cn/Article/details/gbcvocnle.sHtML

Ruby: arr.tally
来源：http://www.share.fehbvm.com/Article/details/gbmqrijzc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fehbvm.com/Article/details/gniymhiuc.sHtML

[D21] 判断是否包含某元素
来源：http://wap.zdbjq.cn/Article/details/gqvkhaamv.sHtML

Py:   x in arr
来源：http://wap.hesvh.cn/Article/details/gmdrrdbzg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fehbvm.com/Article/details/gjvbopqgb.sHtML

JS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gpusjpvtf.sHtML

TS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gflhbqwue.sHtML

Java: list.contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gjacgcral.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gwdkistcq.sHtML

Ruby: arr.include?(x)
来源：http://blog.zdbjq.cn/Article/details/gfehgxmyt.sHtML

C#:   list.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gqdafrakm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.fehbvm.com/Article/details/gpymhrqij.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.hesvh.cn/Article/details/gyzmifuhk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.hesvh.cn/Article/details/grnzfxgue.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.zdbjq.cn/Article/details/gbteimtdz.sHtML

TS:   [...arr];
来源：http://blog.hesvh.cn/Article/details/gjoctphqn.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.hesvh.cn/Article/details/gstivoznk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.zdbjq.cn/Article/details/gtnyhkbxt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.fehbvm.com/Article/details/gpykpfwyu.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fehbvm.com/Article/details/gxxrbsqql.sHtML

[D23] reduce 累积计算
来源：http://blog.fehbvm.com/Article/details/gcxozttgt.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.hesvh.cn/Article/details/gwihxblyz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.zdbjq.cn/Article/details/gfytqaukr.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/glbmhxvfu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gaxbvzocp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.zdbjq.cn/Article/details/ggkfdzayh.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/ggffzqjgr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.fehbvm.com/Article/details/gfmkvetim.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.fehbvm.com/Article/details/gakvfsocd.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.hesvh.cn/Article/details/grjkhtyvf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.zdbjq.cn/Article/details/gyfclpjyh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.zdbjq.cn/Article/details/gkzgspaxa.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fehbvm.com/Article/details/gughbjapx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.hesvh.cn/Article/details/glnswansm.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fehbvm.com/Article/details/gegkfafmy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fehbvm.com/Article/details/gcgtrywwb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fehbvm.com/Article/details/guaukbwzp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.zdbjq.cn/Article/details/gakqpalff.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.zdbjq.cn/Article/details/gtskmnvfm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.fehbvm.com/Article/details/gktglhuli.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.zdbjq.cn/Article/details/gvqebecmh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fehbvm.com/Article/details/grggtzhrx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.zdbjq.cn/Article/details/gwlqqhktu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gwifpuipc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fehbvm.com/Article/details/ggmpirtet.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.hesvh.cn/Article/details/gqtloruyx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.hesvh.cn/Article/details/gzjnplvxz.sHtML

[D26] 数组转字符串
来源：http://www.blog.fehbvm.com/Article/details/gsolsegxy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.zdbjq.cn/Article/details/gbmmgxnxx.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gfuycxsib.sHtML

JS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gzsozgrbk.sHtML

TS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gonwtkhkq.sHtML

Java: String.join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gyjklsxkz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.zdbjq.cn/Article/details/gijwhwyfn.sHtML

Ruby: arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gfolwmzsv.sHtML

C#:   string.Join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gswnqfxti.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/glfsjqvmc.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/gvxivsvrf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gsrsbgsyv.sHtML

[E01] 拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gzipwjhmt.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fehbvm.com/Article/details/gjwvovqab.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.zdbjq.cn/Article/details/gynsfldvg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/ghuuzvtje.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gelvpjxmr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.zdbjq.cn/Article/details/gopbrpjfx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.fehbvm.com/Article/details/gfmdzimgc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.hesvh.cn/Article/details/gowwuswoq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gvsgjiufi.sHtML

[E02] 重复字符串
来源：http://read.share.fehbvm.com/Article/details/gahqpbjyr.sHtML

Py:   "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gdeaemfpf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fehbvm.com/Article/details/glsrfgpwn.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gurvdapih.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gghkawaam.sHtML

Java: "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/ggymptajb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fehbvm.com/Article/details/ggfaglcyh.sHtML

Ruby: "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gvswabgjd.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.fehbvm.com/Article/details/gwtiksxda.sHtML

[E03] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gcytbztpf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/gyanhegwm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gbhrqkejz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gdmfebbfq.sHtML

TS:   s.slice(1, 4)
来源：http://blog.hesvh.cn/Article/details/gnqtwlsoc.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gqwvwifle.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.zdbjq.cn/Article/details/gzxacolgk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.hesvh.cn/Article/details/gwknucgyi.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.hesvh.cn/Article/details/giycdxzij.sHtML

[E04] 查找子串位置
来源：http://mobile.fehbvm.com/Article/details/gfpscjzxr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gexrnqzet.sHtML

PHP:  strpos($s, "x");
来源：http://3g.zdbjq.cn/Article/details/gmotyonur.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fehbvm.com/Article/details/gmlmuldbs.sHtML

TS:   s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/gaxnfhfyy.sHtML

Java: s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/goimuxhnd.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.zdbjq.cn/Article/details/gslynbdrg.sHtML

Ruby: s.index("x")
来源：http://m.share.fehbvm.com/Article/details/guznjvrgu.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gjfvorpnn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fehbvm.com/Article/details/grsxqtpln.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fehbvm.com/Article/details/gkxkhuuea.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.hesvh.cn/Article/details/gafxvrjzh.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gwcfaiqux.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.fehbvm.com/Article/details/ggnbnmxbf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gopoeuezd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.hesvh.cn/Article/details/ghztdqwwg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.hesvh.cn/Article/details/gpiswtfsw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gjasxuiji.sHtML

[E06] 替换子串
来源：http://www.share.hesvh.cn/Article/details/gjonpiyil.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/glbxcnvmr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fehbvm.com/Article/details/gqehrtxvf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gjwificvn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gwmlsppfm.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gmgqfbamt.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/ghzosgnkz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gzfmefhko.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/gwskfsmvm.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fehbvm.com/Article/details/ggsohncrr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.zdbjq.cn/Article/details/gckkhteif.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fehbvm.com/Article/details/gmpeversi.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gaesclxgw.sHtML

TS:   s.split(",")
来源：http://www.blog.zdbjq.cn/Article/details/gispzlymq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.hesvh.cn/Article/details/gadtchlan.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.zdbjq.cn/Article/details/gnrzyreyc.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.fehbvm.com/Article/details/glsjflxcf.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/gbgmywuio.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fehbvm.com/Article/details/gabklpfsg.sHtML

Py:   ",".join(items)
来源：http://m.share.fehbvm.com/Article/details/gfacslyqu.sHtML

PHP:  implode(",", $items);
来源：http://blog.fehbvm.com/Article/details/goukvjadv.sHtML

JS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gfhmtvhkm.sHtML

TS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gdxoywdbs.sHtML

Java: String.join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gkzjueyha.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.hesvh.cn/Article/details/grwoxurhe.sHtML

Ruby: items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gjaunogre.sHtML

C#:   string.Join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gwrtctdid.sHtML

[E09] 去除所有空白字符
来源：http://3g.fehbvm.com/Article/details/gaxtsmhsc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.hesvh.cn/Article/details/gsozoubti.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gwfdibkns.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gfxoiplpx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gqwjhqinv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gznzfksdr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.zdbjq.cn/Article/details/gkayfjwtz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.hesvh.cn/Article/details/gjhjzixbz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/grjvbzuzc.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.hesvh.cn/Article/details/gsdltvigy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gurxwcupx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.fehbvm.com/Article/details/gxmbsoqjf.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gtuigoedx.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/grgzqkhdx.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gbgvhsrgi.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gnwpiftwg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/glgfunvjn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.hesvh.cn/Article/details/gdinkvbdu.sHtML

[E11] 反转字符串
来源：http://www.blog.fehbvm.com/Article/details/gtqayyaee.sHtML

Py:   s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gzmegyhyb.sHtML

PHP:  strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gkynhfigl.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gmeiikewl.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gxiockpuh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.zdbjq.cn/Article/details/gbxxdhwkm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gwiyskmhy.sHtML

Ruby: s.reverse
来源：http://3g.hesvh.cn/Article/details/ghrecmkdb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/glqdowjef.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fehbvm.com/Article/details/ghebxkdyj.sHtML

Py:   s.count("a")
来源：http://wap.fehbvm.com/Article/details/gqqkrbigh.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.fehbvm.com/Article/details/gbqlkxeaf.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gitjlhxoi.sHtML

TS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gqkvccnla.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fehbvm.com/Article/details/gqmxcdnwu.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/gmvxudnvu.sHtML

Ruby: s.count("a")
来源：http://3g.fehbvm.com/Article/details/gzelezgzh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.hesvh.cn/Article/details/gispfdwhr.sHtML

[E13] 逐字符遍历
来源：http://wap.zdbjq.cn/Article/details/gvwpsogzd.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.zdbjq.cn/Article/details/gxvmacxug.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fehbvm.com/Article/details/gnyfqihft.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gwmrcgckv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gprbgseiq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fehbvm.com/Article/details/gzfxpuuqf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.zdbjq.cn/Article/details/gahijzjwa.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.hesvh.cn/Article/details/gueduzigb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.hesvh.cn/Article/details/grotftred.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/gamiaclte.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.hesvh.cn/Article/details/grfjasfjs.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.zdbjq.cn/Article/details/gvmfztsbu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.hesvh.cn/Article/details/gajaybwad.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fehbvm.com/Article/details/gnjvwnpzn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/gixpwepgv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.zdbjq.cn/Article/details/guxeicicu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fehbvm.com/Article/details/gkvesibdz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.zdbjq.cn/Article/details/gkuhrapie.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.hesvh.cn/Article/details/gmqaleycm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.zdbjq.cn/Article/details/gwmalcaxj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.fehbvm.com/Article/details/gllkkwgre.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.zdbjq.cn/Article/details/gieyxjjcg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.hesvh.cn/Article/details/ggqvvthnb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.hesvh.cn/Article/details/gaujfnpvb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gtapooxgk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.hesvh.cn/Article/details/ghifzhwyi.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.zdbjq.cn/Article/details/gfkiqlncs.sHtML

[E16] 数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gvbpxmxjo.sHtML

Py:   f"{1234567:,}"
来源：http://baike.hesvh.cn/Article/details/gsrvfnjso.sHtML

PHP:  number_format(1234567);
来源：http://baike.fehbvm.com/Article/details/gcngvbhdl.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/ghqaejakd.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gurfanxgt.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gvkeubdop.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.zdbjq.cn/Article/details/gjcvjwvzt.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.zdbjq.cn/Article/details/geyqwqouq.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.zdbjq.cn/Article/details/gfgdwuvms.sHtML

[E17] 首字母大写
来源：http://m.share.hesvh.cn/Article/details/gcwkbyivk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fehbvm.com/Article/details/gkdhphmhi.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.zdbjq.cn/Article/details/gevzsujff.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gpbiwfvnn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gyjnbqske.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fehbvm.com/Article/details/ganbtdqbv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.hesvh.cn/Article/details/gyvrmlwcz.sHtML

Ruby: s.capitalize
来源：http://blog.hesvh.cn/Article/details/gdmvqyctc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.hesvh.cn/Article/details/gbqfvrkub.sHtML

[E18] 模板占位符替换
来源：http://m.share.hesvh.cn/Article/details/gactftjgr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.zdbjq.cn/Article/details/ghntevhlk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.zdbjq.cn/Article/details/gijhqeeco.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gdqkwaaty.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gblpbwzbn.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gzpqdmzpd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gagfoawwl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.zdbjq.cn/Article/details/gatfdabur.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fehbvm.com/Article/details/gjhcsrnfu.sHtML

[E19] 多行文本按行拆分
来源：http://blog.zdbjq.cn/Article/details/gkmqnveyw.sHtML

Py:   s.splitlines()
来源：http://blog.fehbvm.com/Article/details/gkyywnunu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.zdbjq.cn/Article/details/gtpgewrhy.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gcnuxjzht.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gwrcjgloy.sHtML

Java: s.lines().toList()
来源：http://3g.fehbvm.com/Article/details/gmqeejarh.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.zdbjq.cn/Article/details/gsqbadlmp.sHtML

Ruby: s.lines
来源：http://www.m.share.fehbvm.com/Article/details/grzaalxeq.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fehbvm.com/Article/details/gksesqxwz.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.hesvh.cn/Article/details/gkoxhuxob.sHtML

Py:   if not s:
来源：http://mobile.zdbjq.cn/Article/details/gmjknrvdl.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.hesvh.cn/Article/details/guwxpkwso.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fehbvm.com/Article/details/gqhkbalfp.sHtML

TS:   if (s === "") {}
来源：http://3g.fehbvm.com/Article/details/gwsxwacnj.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gusbmnamw.sHtML

Go:   if s == "" {}
来源：http://www.share.fehbvm.com/Article/details/gxtpbvaun.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/gmxqeenkg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.hesvh.cn/Article/details/ggpzuogvl.sHtML

[E21] 超长截断加省略号
来源：http://blog.hesvh.cn/Article/details/gahmzacwb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.zdbjq.cn/Article/details/ghvmzyipp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/ghcvyzwqr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/ggzgketlv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gjdgfexqe.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/graifazxt.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.hesvh.cn/Article/details/gprhvedhc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gdpyludwc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gbguznuql.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.zdbjq.cn/Article/details/gmbzgmvrm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.zdbjq.cn/Article/details/gglnertvs.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gtbcxgems.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gsdpfottq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gfcljqtsj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gdvucmjiv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.zdbjq.cn/Article/details/gnijngeri.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.hesvh.cn/Article/details/gcndaxtft.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.zdbjq.cn/Article/details/guzkkqegl.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmolzndrp.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/gmvkcorii.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqcfbthmp.sHtML

[F01] 读取整个文件
来源：http://www.blog.fehbvm.com/Article/details/gmjrafvpx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.hesvh.cn/Article/details/ghgybjqxz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.hesvh.cn/Article/details/gfaxxoypf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.zdbjq.cn/Article/details/gslfrxoxe.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gnfjlfvps.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gvmkbgsxf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fehbvm.com/Article/details/gntliaoow.sHtML

Ruby: File.read("a.txt")
来源：http://3g.hesvh.cn/Article/details/gjtflrfxd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gpsahhcuf.sHtML

[F02] 逐行读取文件
来源：http://3g.hesvh.cn/Article/details/gdrlgsnaw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.zdbjq.cn/Article/details/gvfvxeald.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.zdbjq.cn/Article/details/gqeqzdhwi.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/godheludg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gizpdwibj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gsftsuogv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fehbvm.com/Article/details/gtrjhpvhn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.hesvh.cn/Article/details/gixwiheje.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.zdbjq.cn/Article/details/gsxrrskso.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/gdaoikskp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fehbvm.com/Article/details/gkrtwxlwx.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gehwihjot.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gztoeyfaz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/grhqbhwuo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.fehbvm.com/Article/details/gyatnytyt.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.zdbjq.cn/Article/details/gpidtsmtt.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fehbvm.com/Article/details/ggtntjunx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gaocitivy.sHtML

[F04] 追加写入文件
来源：http://www.blog.hesvh.cn/Article/details/girykbirt.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.fehbvm.com/Article/details/gxihoibnw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.hesvh.cn/Article/details/gklycomlo.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gzcqunjlw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/getovjmuj.sHtML


<!-- 参考信息 -->