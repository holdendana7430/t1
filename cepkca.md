代发 wailian999

C#:   list.Distinct().ToList()
来源：http://hz.xinyue.icu/gtahrtjzcu.html

[D16] 求和与平均值
来源：http://hz.cashguo.top/gtkgpvuchq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.ehwqpu.com/gtdexpuiuj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.gogol.net.cn/gtdptdtuoh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.chenjidiqi.icu/gtsgbnpffo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinqigufen.top/gtzdvyxfpc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.gzhubu.top/gthzkfaihw.html

Go:   // 手写循环累加
来源：http://hz.hfpthk.cn/gtbrqoifzg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.hnxiangtu.top/gtojtithku.html

C#:   list.Sum();  list.Average()
来源：http://hz.iojbl.cn/gtpxtqykqq.html

[D17] 最大值与最小值
来源：http://hz.0kj1m.cn/gtdjdqyvsh.html

Py:   max(arr);  min(arr)
来源：http://hz.hongshengwenyu.top/gtyheudaml.html

PHP:  max($arr);  min($arr);
来源：http://hz.fzhhl.top/gtaaaqcxla.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.gaohongyu789.top/gtedabzhtf.html

TS:   Math.max(...arr);
来源：http://hz.hnqzz.top/gtrqttxlzm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yj20258.top/gtnrfszmhg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.cqqwz.cn/gtbquhzmsw.html

Ruby: arr.max;  arr.min
来源：http://hz.xziqi.cn/gtxypvfgck.html

C#:   list.Max();  list.Min()
来源：http://hz.dashuyun.cn/gtzkbzpbxl.html

[D18] 扁平化嵌套数组
来源：http://hz.haohaochexian.top/gtilgaiagv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.chenjidiqi.icu/gtgjdmolad.html

PHP:  array_merge(...$nested);
来源：http://hz.redwolf501.top/gtvxoxibvo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.zhijiandao.cn/gtmfasunze.html

TS:   nested.flat();
来源：http://hz.xylfe.cn/gtoyekrfph.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.xingfuxueyuan.xyz/gtinoqznel.html

Go:   // 手写双层循环
来源：http://hz.xziqi.cn/gtbxbqxyhc.html

Ruby: nested.flatten
来源：http://hz.jqgufenzy.top/gtcvgeqcan.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yueranfly.top/gtaqrdhtyi.html

[D19] 按字段分组
来源：http://hz.52xcode.cn/gtxhhaumvt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.zdqjudy.top/gttbturlns.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jqgufenzy.top/gtfxdsfpng.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.vqdsnc.cn/gtdgipzlfv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.zycfv.cn/gtyzkicjtk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.c1oappe.top/gtmtfxessf.html

Go:   // 手写 map[string][]T
来源：http://hz.andypj.xyz/gtspfgkdjt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.fengsongda.top/gtuubfdhth.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.ydzc1.top/gtjfiqisqw.html

[D20] 统计每个元素出现次数
来源：http://hz.zdqjudy.top/gtksmrybtm.html

Py:   Counter(arr)
来源：http://hz.jianghu66.top/gtmhpvcjuh.html

PHP:  array_count_values($arr);
来源：http://hz.cheryme.top/gtwqlrjiqn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.sweek.top/gtlamijldr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jiagoushi.top/gtfdvpfvob.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jinghuilouyu.cn/gtpxcwveue.html

Go:   // 手写 map[T]int
来源：http://hz.zdqjudy.top/gtttfyebcp.html

Ruby: arr.tally
来源：http://hz.shangyingyoupin.top/gtkqdziljb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.chenlongwang.top/gtfytreuyf.html

[D21] 判断是否包含某元素
来源：http://hz.havefunace.top/gtnugafpam.html

Py:   x in arr
来源：http://hz.zycfv.cn/gtqfztmtrs.html

PHP:  in_array($x, $arr, true);
来源：http://hz.hnqzz.top/gtmkltgqgi.html

JS:   arr.includes(x)
来源：http://hz.cashguo.top/gtkvsxpazi.html

TS:   arr.includes(x)
来源：http://hz.jianghu66.top/gtazxxdswv.html

Java: list.contains(x)
来源：http://hz.chenlongwang.top/gtqxzskbjo.html

Go:   slices.Contains(arr, x)
来源：http://hz.jqgfzy.top/gtouxjqxnp.html

Ruby: arr.include?(x)
来源：http://hz.yangfankeji.com/gtcfomytvo.html

C#:   list.Contains(x)
来源：http://hz.shuidangran.top/gtyffqqlhg.html

[D22] 复制数组（避免共享引用）
来源：http://hz.cucudq.cn/gteyxjiwtp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.shzxlz.cn/gtifgkcnso.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yangfankeji.com/gtbfeckkkw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.bjfxy.top/gtkhxhfsyb.html

TS:   [...arr];
来源：http://hz.feifeiyinyue.top/gtrxuxqdme.html

Java: new ArrayList<>(list);
来源：http://hz.yuanzhike.top/gtdwcahgby.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.hnqzz.top/gtmabdkjfw.html

Ruby: arr.dup;  arr.clone
来源：http://hz.sufxvd.cn/gthgrgaiad.html

C#:   new List<int>(list);
来源：http://hz.jqgufenzy.top/gtehoebpew.html

[D23] reduce 累积计算
来源：http://hz.andypj.xyz/gtxglzdptz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jinqigufen.top/gtbqbilxyf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.jyoumei.cn/gtyyuxahmc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.0kj1m.cn/gtjjsgevgc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ydzc1.top/gtwdnmwkeq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jlsjyb.cn/gtbsqvryhx.html

Go:   // 手写循环
来源：http://hz.jqgfzy.top/gtmagpgvjp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.yj20258.top/gtevhxjxxz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jyoumei.cn/gtfpcupkqr.html

[D24] 字典 / Map 基本操作
来源：http://hz.iojbl.cn/gtoejwmcbm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.mhx1999.top/gtrwiussij.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.pengpengdd.cyou/gtgsjphpim.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yvedp.cn/gtanzwlolf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.jqgfzy.top/gtlhesepvn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.zhijiandao.cn/gtgtnmnxzt.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.nwbrower.top/gtsxiqfiau.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.xylfe.cn/gtsjuzcyun.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.hongshengwenyu.top/gtpnjvelgv.html

[D25] Set 集合去重与交并差
来源：http://hz.yueranfly.top/gtofkzyqjc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.hammf.cn/gtwmjktxco.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.hongshengwenyu.top/gtsvfwncjs.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.ehwqpu.com/gtfejgmzcp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.mhx1999.top/gtxqqhpawv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yongpay.top/gtlwaefwcq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.zycfv.cn/gtkwocgkzn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.cqqwz.cn/gtlqliteto.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.zhaomingkeji.xyz/gtwsrnsbfi.html

[D26] 数组转字符串
来源：http://hz.chenzaomai.com/gtdhrszgvh.html

Py:   ", ".join(map(str, arr))
来源：http://hz.yonumen.top/gtscpdqjnt.html

PHP:  implode(", ", $arr);
来源：http://hz.jiagoushi.top/gtsiqvypqf.html

JS:   arr.join(", ")
来源：http://hz.redwolf501.top/gtljbzmluj.html

TS:   arr.join(", ")
来源：http://hz.shanyushiyangkeji.top/gtkwyimqgx.html

Java: String.join(", ", list)
来源：http://hz.hfpthk.cn/gtuvrrkvvy.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yongpay.top/gtxisncpko.html

Ruby: arr.join(", ")
来源：http://hz.sufxvd.cn/gtjucxyipv.html

C#:   string.Join(", ", list)
来源：http://hz.jinqigufen.top/gtbqctxyfa.html

================================================================================
来源：http://hz.cheryme.top/gtslrkynef.html

E. 字符串处理
来源：http://hz.cdnleiting.top/gtafjgomov.html

================================================================================
来源：http://hz.jqgufenzy.top/gtizmrxfgo.html

[E01] 拼接字符串
来源：http://hz.birdmap.top/gtafaafnhl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.cheryme.top/gtbgietnos.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.jqgufenzy.top/gtkykmhype.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.chenzaomai.com/gtbjkarkjj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhengqikj.top/gtracfxgfk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.ppjwa.cn/gtlitdrerd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.mhx1999.top/gtyczsgwza.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jianghu66.top/gtvpxtarjz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zhoulong.xyz/gtuiktlioa.html

[E02] 重复字符串
来源：http://hz.xingfuxueyuan.xyz/gtnoyzkkup.html

Py:   "ab" * 3
来源：http://hz.snrcjt.cn/gtuvfdnxzp.html

PHP:  str_repeat("ab", 3);
来源：http://hz.wangdashe.top/gtkbvvwhdr.html

JS:   "ab".repeat(3)
来源：http://hz.zhongyouzk.top/gtobfktdxe.html

TS:   "ab".repeat(3)
来源：http://hz.cqqwz.cn/gteajjwnpg.html

Java: "ab".repeat(3)
来源：http://hz.pycfn.com/gtiwxqvfuz.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.bjfxy.top/gtlniblfyj.html

Ruby: "ab" * 3
来源：http://hz.gogol.net.cn/gtlgafulsg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.redwolf501.top/gtwqemewui.html

[E03] 截取子串
来源：http://hz.iojbl.cn/gtpwlejzcc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.zhongyouzk.top/gtykwqorza.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.pengpengdd.cyou/gtkadximus.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.aizwys.cn/gtncjmmzes.html

TS:   s.slice(1, 4)
来源：http://hz.feifeiyinyue.top/gtwbzjaftc.html

Java: s.substring(1, 4)
来源：http://hz.yanxiufei.cn/gtwspqofnx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.xylfe.cn/gtedavcorx.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.chenjidiqi.icu/gtfayncbjj.html

C#:   s.Substring(1, 3)
来源：http://hz.snrcjt.cn/gtnfjkwvln.html

[E04] 查找子串位置
来源：http://hz.shangyingyoupin.top/gtfjvoaocn.html

Py:   s.find("x");  s.index("x")
来源：http://hz.tian-w.cn/gtfrekpzfh.html

PHP:  strpos($s, "x");
来源：http://hz.sweek.top/gtzmviyrhg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.cdnleiting.top/gtjvfmuurv.html

TS:   s.indexOf("x")
来源：http://hz.zycfv.cn/gtlrmkewok.html

Java: s.indexOf("x")
来源：http://hz.tian-w.cn/gtoxplooum.html

Go:   strings.Index(s, "x")
来源：http://hz.pycfn.com/gtgdvcmfrl.html

Ruby: s.index("x")
来源：http://hz.birdmap.top/gtnlojtkkj.html

C#:   s.IndexOf("x")
来源：http://hz.daria6918.cn/gthfimpyqc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.yj202588.top/gtrszeltwf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.shanyushiyangtech.top/gtzpcbgvyr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.sysykeji.top/gtjdtirxon.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.cashguo.top/gtdiggxqaj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.jyoumei.cn/gtyldaznqc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.xziqi.cn/gtptogvucu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.316326.xyz/gtnedhusjs.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.shangyingyoupin.top/gtuxuisoom.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.meibo888.top/gtmmakfshe.html

[E06] 替换子串
来源：http://hz.xylfe.cn/gtuoiimfaw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.vqdsnc.cn/gtrfnxezqt.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.hysaishi.cn/gtcarkqvzx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.shuidangran.top/gtbkcxwsfa.html

TS:   s.replaceAll("a", "b")
来源：http://hz.c1oappe.top/gtfcodflqu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.iojbl.cn/gtpbirxrgs.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.gogol.net.cn/gtdckspjwx.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.316326.xyz/gtuojhyuok.html

C#:   s.Replace("a", "b")
来源：http://hz.dashuyun.cn/gtsretdacg.html

[E07] 按分隔符拆分
来源：http://hz.jqgfzy.top/gtjsoczsym.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.shangyingyoupin.top/gtlrmrumyl.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.tian-w.cn/gtniomyqgs.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.hnxiangtu.top/gtxkcvcxxb.html

TS:   s.split(",")
来源：http://hz.wangshuangyany.cn/gtiossktdx.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.cucudq.cn/gtjnpnyvih.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yonumen.top/gthbvblajf.html

Ruby: s.split(",");  s.split
来源：http://hz.jlsjyb.cn/gtbmwqjmgy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.tanke756.top/gtoruzjxwy.html

[E08] 数组按分隔符合并
来源：http://hz.tianlin.xyz/gtndfbvdwy.html

Py:   ",".join(items)
来源：http://hz.cucudq.cn/gtgwwyhwhh.html

PHP:  implode(",", $items);
来源：http://hz.vqdsnc.cn/gtnxzzwyhv.html

JS:   items.join(",")
来源：http://hz.jqgufenzy.top/gtztqslfku.html

TS:   items.join(",")
来源：http://hz.fzhhl.top/gtcaedsfau.html

Java: String.join(",", items)
来源：http://hz.jlsjyb.cn/gtrddaiquw.html

Go:   strings.Join(items, ",")
来源：http://hz.shanyushiyangtech.top/gtedwhmiii.html

Ruby: items.join(",")
来源：http://hz.yueranfly.top/gtewonjgqo.html

C#:   string.Join(",", items)
来源：http://hz.yj20258.top/gtnbjognak.html

[E09] 去除所有空白字符
来源：http://hz.jyoumei.cn/gtbchozxoy.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yvedp.cn/gtofrallkm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.jinqigfzy.top/gtkaespsgh.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.shuidangran.top/gttbrhgwkj.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.nanxinkj.top/gtqwdpsxjy.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yangfankeji.com/gtapudxvwb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.pycfn.com/gtgunaiepv.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.nwbrower.top/gtxcxcbtmz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.fengsongda.top/gtbkgrjeuc.html

[E10] 左侧补零 / 定长填充
来源：http://hz.ppjwa.cn/gthgzqjmcf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.ybcxt.top/gterhuwsxm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.gotoacloud.top/gtxifoqxxq.html

JS:   "7".padStart(3, "0")
来源：http://hz.nanxinkj.top/gtoyqfxdvg.html

TS:   "7".padStart(3, "0")
来源：http://hz.hongshengwenyu.top/gthtgtjzaj.html

Java: String.format("%03d", 7)
来源：http://hz.sxryk.cn/gtzgrbqurh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.tianlin.xyz/gtoeobaefb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.andypj.xyz/gtndhwtfoe.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.hysaishi.cn/gtjvpizclg.html

[E11] 反转字符串
来源：http://hz.kuanghao11.cn/gtedditelm.html

Py:   s[::-1]
来源：http://hz.zhengqikj.top/gtormgrlxv.html

PHP:  strrev($s);
来源：http://hz.yuanzhike.top/gtmpofupnr.html

JS:   [...s].reverse().join("")
来源：http://hz.hfpthk.cn/gtoyzekwhe.html

TS:   [...s].reverse().join("")
来源：http://hz.c1oappe.top/gtczpyocsw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.shanyushiyangkeji.top/gtcvjstiwd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.xuetiantiany.cn/gtxruzslcw.html

Ruby: s.reverse
来源：http://hz.ybcxt.top/gthbpxsmmt.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.xylfe.cn/gtpjnzxpmx.html

[E12] 统计某字符出现次数
来源：http://hz.daxiang520.top/gtxwmwzhkb.html

Py:   s.count("a")
来源：http://hz.shanyushiyangkeji.top/gthsjvlyvb.html

PHP:  substr_count($s, "a");
来源：http://hz.yonumen.top/gtcknmbixg.html

JS:   s.split("a").length - 1
来源：http://hz.dashuyun.cn/gtnfnuokkg.html

TS:   s.split("a").length - 1
来源：http://hz.daria6918.cn/gthhysyzci.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.cheryme.top/gtgqgueqfe.html

Go:   strings.Count(s, "a")
来源：http://hz.pycfn.com/gtxsdgysmu.html

Ruby: s.count("a")
来源：http://hz.zdqjudy.top/gtigfiwysn.html

C#:   s.Count(c => c == 'a')
来源：http://hz.xuetiantiany.cn/gttzfpoqqf.html

[E13] 逐字符遍历
来源：http://hz.0kj1m.cn/gtvqvmonxa.html

Py:   for ch in s: print(ch)
来源：http://hz.xinyue.icu/gteeaolibd.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yueranfly.top/gtlqvrenfq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xziqi.cn/gtjaukdhot.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hywenlv.cn/gtmjjegowx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.zycfv.cn/gtjcnkkrqa.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.xingfuxueyuan.xyz/gtfvvpdzjk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yuxming.cn/gteczatvsh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.dianchejie.cn/gtaptrwgmm.html

[E14] URL 编码与 Base64
来源：http://hz.xuanzx.com/gtsgrxegro.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jqgufenzy.top/gtnogxbcxu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.aizwys.cn/gtrtmmtbaz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yangfankeji.com/gtjfmdiytl.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.zhengqikj.top/gtdjxxxkhp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.dashuyun.cn/gtfribjpry.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.smart0.xyz/gtocqhwfzi.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.xziqi.cn/gtxrschrcq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.ppjwa.cn/gtkfhenixd.html

[E15] HTML 转义 / 反转义
来源：http://hz.iojbl.cn/gtqbgcpped.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.fengsongda.top/gtbgfcmzlm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yongpay.top/gttkebupxl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.nwbrower.top/gtoamepnus.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.zhixingplan.top/gtrazydjie.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yj20258.top/gtmjlfjpak.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.sysykeji.top/gtaqznywfn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.guowangkeji.top/gtmxlcvhbb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.xuanzx.com/gtdgaafzzp.html

[E16] 数字千分位
来源：http://hz.jqgfzy.top/gtqkiksakq.html

Py:   f"{1234567:,}"
来源：http://hz.ydzc1.top/gtnvtplbgi.html

PHP:  number_format(1234567);
来源：http://hz.smart0.xyz/gtlyttdqik.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.daria6918.cn/gtgzgxgmyu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.cashguo.top/gtqimaeume.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.bjfxy.top/gthwgkopai.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.sysykeji.top/gtlluiapfl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.smart0.xyz/gtxsqwmuse.html

C#:   1234567.ToString("N0")
来源：http://hz.jyoumei.cn/gtsoouraqs.html

[E17] 首字母大写
来源：http://hz.yonumen.top/gtsbzkrisn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.xuetiantiany.cn/gtbcjgktxl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.tanke756.top/gtcalkrpab.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hammf.cn/gtjdlhccyh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.9152youxi.cn/gtdpvyiozf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.xuetiantiany.cn/gtcyblilvd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.yuanzhike.top/gtcnaajmdv.html

Ruby: s.capitalize
来源：http://hz.hywenlv.cn/gtdfbdpviu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yanxiufei.cn/gtbgchsinv.html

[E18] 模板占位符替换
来源：http://hz.vqdsnc.cn/gtcgohayhn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.gogol.net.cn/gtzxuuyhsw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.aibaodan.cn/gtpqhxjvpt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.snrcjt.cn/gtlhjjgvlr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.haohaochexian.top/gtphabsjaw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.guowangkeji.top/gtaxwhojhe.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.chenjidiqi.icu/gtenqzigjv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.nanxuanxn.top/gtprubbhkg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.ppjwa.cn/gtszvhbylx.html

[E19] 多行文本按行拆分
来源：http://hz.aizwys.cn/gtzdbmkdzr.html

Py:   s.splitlines()
来源：http://hz.zhongyouzk.top/gtebidfpii.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.gzhubu.top/gtpdjszves.html

JS:   s.split(/\r?\n/)
来源：http://hz.fzhhl.top/gtabsvviix.html

TS:   s.split(/\r?\n/)
来源：http://hz.hfpthk.cn/gtiecjtnvh.html

Java: s.lines().toList()
来源：http://hz.yuanzhike.top/gtntidqwls.html

Go:   strings.Split(s, "\n")
来源：http://hz.52xcode.cn/gttzzctacc.html

Ruby: s.lines
来源：http://hz.zhengqikj.top/gtiidbkwem.html

C#:   s.Split('\n')
来源：http://hz.ppjwa.cn/gtzwssynlr.html

[E20] 判断字符串是否为空
来源：http://hz.tianlin.xyz/gtyodnkzrh.html

Py:   if not s:
来源：http://hz.xuetiantiany.cn/gtpfttlkti.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.shzxlz.cn/gtmxtcaycc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.wangshuangyany.cn/gtwdfakbuc.html

TS:   if (s === "") {}
来源：http://hz.tanke756.top/gthxamsdls.html

Java: if (s.isEmpty()) {}
来源：http://hz.yj202588.top/gtgkoltrcu.html

Go:   if s == "" {}
来源：http://hz.xziqi.cn/gtreyrwpbu.html

Ruby: if s.empty?
来源：http://hz.cdnleiting.top/gttteaoabu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.chenlongwang.top/gtqijihurr.html

[E21] 超长截断加省略号
来源：http://hz.jianghu66.top/gteswyzmec.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.xingfuxueyuan.xyz/gtkvpzamin.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yj20258888.top/gtlzbyasqd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhongyouzk.top/gttuchzwhg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.tian-w.cn/gtfpordtda.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jinqigufen.top/gtngbzfkho.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.dashuyun.cn/gtwynroipd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.sweek.top/gtihszswtb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.meibo888.top/gtekhnrtqq.html

[E22] 字节长度与字符长度
来源：http://hz.xinyue.icu/gtyibljypp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.nanxinkj.top/gtvhsfjxoc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xuetiantiany.cn/gtrhljbgpt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.kuanghao11.cn/gtucydnjtd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.guowangkeji.top/gtchmnunkh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.nanxuanxn.top/gtrxalbrem.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.hammf.cn/gtkebnwpru.html

Ruby: s.bytesize;  s.length
来源：http://hz.dianchejie.cn/gtdlmhrgul.html


<!-- 参考信息 -->