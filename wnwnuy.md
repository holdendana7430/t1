代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.c1oappe.top/gtnkgwfwih.html

C#:   list.Sum();  list.Average()
来源：http://hz.xylfe.cn/gtsiohqwto.html

[D17] 最大值与最小值
来源：http://hz.hnxiangtu.top/gtkpfnlkdi.html

Py:   max(arr);  min(arr)
来源：http://hz.jinqigufen.top/gtrrieldqw.html

PHP:  max($arr);  min($arr);
来源：http://hz.shzxlz.cn/gteqcxwjdg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.meibo888.top/gtezvpahqn.html

TS:   Math.max(...arr);
来源：http://hz.cashguo.top/gtxzdkbydr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.daxiang520.top/gtvqjgmeam.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.tian-w.cn/gtyxzxocbd.html

Ruby: arr.max;  arr.min
来源：http://hz.316326.xyz/gtcdxbzdgc.html

C#:   list.Max();  list.Min()
来源：http://hz.xuanzx.com/gtfdmcjens.html

[D18] 扁平化嵌套数组
来源：http://hz.snrcjt.cn/gtxlmdkqsc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.ehwqpu.com/gtylcxvvvx.html

PHP:  array_merge(...$nested);
来源：http://hz.ydzc1.top/gtrypovmhp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.hysaishi.cn/gtnoadnctv.html

TS:   nested.flat();
来源：http://hz.ppjwa.cn/gttvhcawsm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.tian-w.cn/gtjquebjtd.html

Go:   // 手写双层循环
来源：http://hz.yonumen.top/gtkzklaagj.html

Ruby: nested.flatten
来源：http://hz.xinyue.icu/gtxdbikhtm.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.wangshuangyany.cn/gtpfhlrfir.html

[D19] 按字段分组
来源：http://hz.kuanghao11.cn/gtcyuwkism.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.xinyue.icu/gtyyrqwwif.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.wangdashe.top/gtobbdpwgd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.snrcjt.cn/gthkhmjmbo.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.zhaomingkeji.xyz/gtppoonraz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.xylfe.cn/gticzypesy.html

Go:   // 手写 map[string][]T
来源：http://hz.smart0.xyz/gtnohndftr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.jinghuilouyu.cn/gthqsrkpqx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.gogol.net.cn/gtnlbozonp.html

[D20] 统计每个元素出现次数
来源：http://hz.jinghuilouyu.cn/gtkohneuvq.html

Py:   Counter(arr)
来源：http://hz.yuanzhike.top/gtbufyettg.html

PHP:  array_count_values($arr);
来源：http://hz.xingfuxueyuan.xyz/gtczvhtcrf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hywenlv.cn/gtzqggnuwq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.52xcode.cn/gtufobyvsr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.xziqi.cn/gtpaugjixr.html

Go:   // 手写 map[T]int
来源：http://hz.tanke756.top/gtqqsnzhnu.html

Ruby: arr.tally
来源：http://hz.jinqigfzy.top/gtwzfxozgp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.52xcode.cn/gtoqxcyirb.html

[D21] 判断是否包含某元素
来源：http://hz.yj20258888.top/gtfqsfdwrz.html

Py:   x in arr
来源：http://hz.yanxiufei.cn/gtririhfcw.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yj20258888.top/gtgwfntxug.html

JS:   arr.includes(x)
来源：http://hz.yanxiufei.cn/gtgqoorjfe.html

TS:   arr.includes(x)
来源：http://hz.yj20258888.top/gtknbzxann.html

Java: list.contains(x)
来源：http://hz.tianlin.xyz/gtdpobmydr.html

Go:   slices.Contains(arr, x)
来源：http://hz.nanxinkj.top/gtwuhvszhi.html

Ruby: arr.include?(x)
来源：http://hz.ydjk.org.cn/gtttbptdhl.html

C#:   list.Contains(x)
来源：http://hz.hysaishi.cn/gtqozwjkcf.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jiagoushi.top/gtfbngmfcw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.zycfv.cn/gtayuuwpmm.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.ywan-chungtsiang.top/gtqopucube.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.cdnleiting.top/gtxxpbfbad.html

TS:   [...arr];
来源：http://hz.tian-w.cn/gtzkomlbyz.html

Java: new ArrayList<>(list);
来源：http://hz.shanyushiyangtech.top/gtqyaqfrnz.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yj20258.top/gtvkcoqvyx.html

Ruby: arr.dup;  arr.clone
来源：http://hz.shanyushiyangtech.top/gtuunjpmyq.html

C#:   new List<int>(list);
来源：http://hz.aibaodan.cn/gtmfbkwsyw.html

[D23] reduce 累积计算
来源：http://hz.hnxiangtu.top/gtoqftauey.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.c1oappe.top/gtzedkjfwt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.jqgufenzy.top/gtwzrouwfm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.gotoacloud.top/gtqfvsayev.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.chenjidiqi.icu/gtilohbmkq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.zhengqikj.top/gtmikduotl.html

Go:   // 手写循环
来源：http://hz.yanxiufei.cn/gtvbkuqyok.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.kuanghao11.cn/gttnaicdhs.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jinqigufen.top/gtudyhipjp.html

[D24] 字典 / Map 基本操作
来源：http://hz.fengsongda.top/gtwnqalidi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.kuanghao11.cn/gtkjyzdqak.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.52xcode.cn/gtyrtacrkx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.guowangkeji.top/gtsgkesptm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.jinghuilouyu.cn/gtuhtcafvk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yuanzhike.top/gttruuogkd.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.jqgufenzy.top/gtnrqtwfgy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.yvedp.cn/gtjobdrjkn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.gotoacloud.top/gtetmjvolz.html

[D25] Set 集合去重与交并差
来源：http://hz.cheryme.top/gtvehycbfm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.cheryme.top/gtrofdnxts.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yj202588.top/gtiorzmddi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.dianchejie.cn/gtjrqyapcf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.zhongyouzk.top/gtbgnndeck.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.redwolf501.top/gtebbfjpjr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.hammf.cn/gtiimkbjgq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jianghu66.top/gtjkhpohpk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.hfpthk.cn/gtpquxriwe.html

[D26] 数组转字符串
来源：http://hz.sweek.top/gtlchqzxgl.html

Py:   ", ".join(map(str, arr))
来源：http://hz.xziqi.cn/gtxjcumfzh.html

PHP:  implode(", ", $arr);
来源：http://hz.cheryme.top/gtkpncwvhi.html

JS:   arr.join(", ")
来源：http://hz.jlsjyb.cn/gtsazjccms.html

TS:   arr.join(", ")
来源：http://hz.ybcxt.top/gtkgakqvrh.html

Java: String.join(", ", list)
来源：http://hz.zycfv.cn/gtzqkxydjh.html

Go:   strings.Join(strs, ", ")
来源：http://hz.zycfv.cn/gtbprclyfc.html

Ruby: arr.join(", ")
来源：http://hz.aizwys.cn/gtdmbjvwuv.html

C#:   string.Join(", ", list)
来源：http://hz.jqgfzy.top/gtphfeziux.html

================================================================================
来源：http://hz.andypj.xyz/gtgudnqlpc.html

E. 字符串处理
来源：http://hz.snrcjt.cn/gtjclasxdl.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtugwwwjgk.html

[E01] 拼接字符串
来源：http://hz.chenlongwang.top/gtbxcewadg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.guannengcc.top/gtxjubzvtw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.ywan-chungtsiang.top/gtdckovwfn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.tianlin.xyz/gtnoudaodb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.pycfn.com/gtkdhxvecw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.hfpthk.cn/gtapswmomx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.shzxlz.cn/gtfjjkfpqu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.ydzc1.top/gtciilwdxx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.jiagoushi.top/gtbegxewqs.html

[E02] 重复字符串
来源：http://hz.cheryme.top/gtzowjfpjh.html

Py:   "ab" * 3
来源：http://hz.wangshuangyany.cn/gtlbtzxcfq.html

PHP:  str_repeat("ab", 3);
来源：http://hz.svipenyu.cn/gtzawcbbhm.html

JS:   "ab".repeat(3)
来源：http://hz.jinghuilouyu.cn/gttmecnomf.html

TS:   "ab".repeat(3)
来源：http://hz.redwolf501.top/gtqiggqgmu.html

Java: "ab".repeat(3)
来源：http://hz.haohaochexian.top/gtgwfhnxjf.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.sysykeji.top/gtdfmdnpdl.html

Ruby: "ab" * 3
来源：http://hz.yj20258888.top/gtaxrhcxzr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.chenzaomai.com/gtcfxkmrgr.html

[E03] 截取子串
来源：http://hz.jinghuilouyu.cn/gtihjftofy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.zhaomingkeji.xyz/gtiqklejmg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.xylfe.cn/gtaijcibcn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.fengsongda.top/gtoorrmwrr.html

TS:   s.slice(1, 4)
来源：http://hz.ydzc1.top/gtnyjlvysd.html

Java: s.substring(1, 4)
来源：http://hz.shangyingyoupin.top/gtqchlfiyd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.tanke756.top/gtxqgetfpm.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.gaohongyu789.top/gtxuruuucj.html

C#:   s.Substring(1, 3)
来源：http://hz.chenjidiqi.icu/gthscficcz.html

[E04] 查找子串位置
来源：http://hz.redwolf501.top/gtwnfckgsn.html

Py:   s.find("x");  s.index("x")
来源：http://hz.xylfe.cn/gtpvabyydv.html

PHP:  strpos($s, "x");
来源：http://hz.ehwqpu.com/gthbrjbccu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.nwbrower.top/gtksigctic.html

TS:   s.indexOf("x")
来源：http://hz.shanyushiyangtech.top/gtmdjyztak.html

Java: s.indexOf("x")
来源：http://hz.jinyuanbaomall.cn/gtuasfdudm.html

Go:   strings.Index(s, "x")
来源：http://hz.ivvv.top/gteoqtktxb.html

Ruby: s.index("x")
来源：http://hz.ehwqpu.com/gtywplzprm.html

C#:   s.IndexOf("x")
来源：http://hz.ydzc1.top/gtrxhzzdtc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.jinghuilouyu.cn/gtnkjvejwr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.ppjwa.cn/gtphpwaakh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.aizwys.cn/gtkutfnzbz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.iojbl.cn/gtfigkvhtm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.kuanghao11.cn/gtzwgijtyp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.haohaochexian.top/gtfrxkekaz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.tianlin.xyz/gtaznhtfxi.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.ivvv.top/gttvhoccyo.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.smart0.xyz/gtpqgqwjok.html

[E06] 替换子串
来源：http://hz.cdnleiting.top/gteynsvrpm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jqgfzy.top/gtvefoxwwc.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.jianghu66.top/gtduudnxdy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.cheryme.top/gtfqhmnnyq.html

TS:   s.replaceAll("a", "b")
来源：http://hz.yuanzhike.top/gtgfmasxpv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xuetiantiany.cn/gtjbcfkqsm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.jyoumei.cn/gtuxqyeiyg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.gzhubu.top/gterarareu.html

C#:   s.Replace("a", "b")
来源：http://hz.xylfe.cn/gtsofjqrkh.html

[E07] 按分隔符拆分
来源：http://hz.aizwys.cn/gtijfdvrda.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jlsjyb.cn/gtkfxeewcq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.9152youxi.cn/gtcefdwice.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.xingfuxueyuan.xyz/gtsodmwxmz.html

TS:   s.split(",")
来源：http://hz.xuanzx.com/gtonobpftu.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.hysaishi.cn/gtmapifmtz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.hywenlv.cn/gtsvdfjeha.html

Ruby: s.split(",");  s.split
来源：http://hz.yongpay.top/gtrrzebuip.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.gogol.net.cn/gtfwpntthv.html

[E08] 数组按分隔符合并
来源：http://hz.cqqwz.cn/gtnsxibtgk.html

Py:   ",".join(items)
来源：http://hz.tian-w.cn/gtuicnddoc.html

PHP:  implode(",", $items);
来源：http://hz.jinqigfzy.top/gtshazvjpy.html

JS:   items.join(",")
来源：http://hz.yanxiufei.cn/gtupnyfoaf.html

TS:   items.join(",")
来源：http://hz.nwbrower.top/gtrzdfbato.html

Java: String.join(",", items)
来源：http://hz.pycfn.com/gtmhgcbhyu.html

Go:   strings.Join(items, ",")
来源：http://hz.zhengqikj.top/gtfwabjwzn.html

Ruby: items.join(",")
来源：http://hz.fengsongda.top/gtuhlscyuc.html

C#:   string.Join(",", items)
来源：http://hz.cqqwz.cn/gtsghvympb.html

[E09] 去除所有空白字符
来源：http://hz.hongshengwenyu.top/gtnuexxomt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.gotoacloud.top/gtlxttyubo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.hammf.cn/gtyopjxhqw.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.tian-w.cn/gtywvznvam.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.hfpthk.cn/gthbximhrk.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.shangyingyoupin.top/gtaormyvow.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.xingfuxueyuan.xyz/gtsnnaxens.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.jqgufenzy.top/gtwkgjmtgz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jinqigfzy.top/gtdubcxond.html

[E10] 左侧补零 / 定长填充
来源：http://hz.ydjk.org.cn/gteujwmewo.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.mhx1999.top/gtapepyisg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.shangyingyoupin.top/gtpqhmytsb.html

JS:   "7".padStart(3, "0")
来源：http://hz.daria6918.cn/gtfkrgknbh.html

TS:   "7".padStart(3, "0")
来源：http://hz.zhiwuduotai.top/gtgsbwpdqw.html

Java: String.format("%03d", 7)
来源：http://hz.shanyushiyangtech.top/gtsdllzecu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.0kj1m.cn/gtyhbpmcid.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.jinghuilouyu.cn/gteljfpicz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.daxiang520.top/gtecqprmrx.html

[E11] 反转字符串
来源：http://hz.guannengcc.top/gttkwgexlj.html

Py:   s[::-1]
来源：http://hz.jlsjyb.cn/gtorslgrtf.html

PHP:  strrev($s);
来源：http://hz.zhoulong.xyz/gtonjoqpmw.html

JS:   [...s].reverse().join("")
来源：http://hz.havefunace.top/gtxfpolmjq.html

TS:   [...s].reverse().join("")
来源：http://hz.ehwqpu.com/gtlmiwrdwh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.ydzc1.top/gtkpzdxwey.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.dashuyun.cn/gtmznbodxc.html

Ruby: s.reverse
来源：http://hz.zhiwuduotai.top/gtpjqmdyjn.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.hfpthk.cn/gtdxexjeet.html

[E12] 统计某字符出现次数
来源：http://hz.yangfankeji.com/gtvqpghiqf.html

Py:   s.count("a")
来源：http://hz.yj20258888.top/gtcubrrnih.html

PHP:  substr_count($s, "a");
来源：http://hz.jinqigfzy.top/gtdkfgwzga.html

JS:   s.split("a").length - 1
来源：http://hz.mhx1999.top/gtghnthmgl.html

TS:   s.split("a").length - 1
来源：http://hz.aibaodan.cn/gtyaepgeoh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.pengpengdd.cyou/gtfnerbsga.html

Go:   strings.Count(s, "a")
来源：http://hz.nanxinkj.top/gtpqewcyyr.html

Ruby: s.count("a")
来源：http://hz.zdqjudy.top/gtgjaohfgj.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yueranfly.top/gtbiibkiut.html

[E13] 逐字符遍历
来源：http://hz.nanxinkj.top/gttiitmqef.html

Py:   for ch in s: print(ch)
来源：http://hz.9152youxi.cn/gtjzfikikc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.zhengqikj.top/gtkexwccaz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.mhx1999.top/gtbasvetlj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yj202588.top/gtzplflaqe.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.aizwys.cn/gtweehoxok.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.tian-w.cn/gtwlqaemwn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.gaohongyu789.top/gtyjfjliqh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.xinyue.icu/gtgzhkauya.html

[E14] URL 编码与 Base64
来源：http://hz.guowangkeji.top/gtwkmansni.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.mhx1999.top/gtbhztlooo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.hysaishi.cn/gtuxuggfud.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yuxming.cn/gtjdmhgcrb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.guowangkeji.top/gtxhjpvila.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jinqigfzy.top/gtsbksoxug.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.gaohongyu789.top/gttpkxocbg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zhiwuduotai.top/gtgcfkjlsn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.daxiang520.top/gtjulfqdtp.html

[E15] HTML 转义 / 反转义
来源：http://hz.tanke756.top/gtzyjzzghd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.chenlongwang.top/gtzhlducwp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.hongshengwenyu.top/gtgjuyoqgr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yuanzhike.top/gtnsqsrlgd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.pycfn.com/gtvraidqej.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.guowangkeji.top/gtoyrxbfio.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.iojbl.cn/gtroqebadu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.ydzc1.top/gtukqxmrcz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.havefunace.top/gtqsbtckoq.html

[E16] 数字千分位
来源：http://hz.haohaochexian.top/gtlukjaade.html

Py:   f"{1234567:,}"
来源：http://hz.shangyingyoupin.top/gtshwilpgd.html

PHP:  number_format(1234567);
来源：http://hz.kuanghao11.cn/gtnlyqljfn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.havefunace.top/gtfrqgqjrb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yj20258.top/gtleegivmz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.ivvv.top/gtnpkmaotm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.nanxuanxn.top/gtvlaeykti.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.aibaodan.cn/gtlbftssyv.html

C#:   1234567.ToString("N0")
来源：http://hz.yuanzhike.top/gtcdotumdy.html

[E17] 首字母大写
来源：http://hz.tianlin.xyz/gtiaagmxhg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.tanke756.top/gtywqbktwc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jiagoushi.top/gtfktxddop.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ivvv.top/gtmxzwygua.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gogol.net.cn/gtvqoeqedr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.daxiang520.top/gtghvpbuue.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zhiwuduotai.top/gtfuwkubmj.html

Ruby: s.capitalize
来源：http://hz.yuanzhike.top/gtuzbezuqq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.birdmap.top/gtlbrrftgm.html

[E18] 模板占位符替换
来源：http://hz.jinyuanbaomall.cn/gtdggovrtg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.ybcxt.top/gtoeuawcge.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.vqdsnc.cn/gtlroudgqw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.fzhhl.top/gtnhtcerut.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.0kj1m.cn/gtybdgkauc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.pycfn.com/gtohvvnvwk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.wangdashe.top/gtyvvauony.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yuxming.cn/gtyfuaiayb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.aibaodan.cn/gtvsqfojxy.html

[E19] 多行文本按行拆分
来源：http://hz.yj20258888.top/gtgzfugbuj.html

Py:   s.splitlines()
来源：http://hz.cashguo.top/gtkhwqgpfe.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yanxiufei.cn/gtuylohxaw.html

JS:   s.split(/\r?\n/)
来源：http://hz.zdqjudy.top/gtocnswrsc.html

TS:   s.split(/\r?\n/)
来源：http://hz.pengpengdd.cyou/gttfimynhf.html

Java: s.lines().toList()
来源：http://hz.svipenyu.cn/gtcsrwtsyo.html

Go:   strings.Split(s, "\n")
来源：http://hz.shuidangran.top/gtihyuinmk.html

Ruby: s.lines
来源：http://hz.snrcjt.cn/gtnkouggea.html

C#:   s.Split('\n')
来源：http://hz.guowangkeji.top/gtbbrwvrdf.html

[E20] 判断字符串是否为空
来源：http://hz.daxiang520.top/gtnkchtpgq.html

Py:   if not s:
来源：http://hz.haohaochexian.top/gtdexhnozo.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.gotoacloud.top/gtzilpqwxf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.shzxlz.cn/gtkwauqgzj.html

TS:   if (s === "") {}
来源：http://hz.wangshuangyany.cn/gtycslslxs.html

Java: if (s.isEmpty()) {}
来源：http://hz.xinyue.icu/gtsxreipdw.html

Go:   if s == "" {}
来源：http://hz.c1oappe.top/gtcfmcwbzm.html

Ruby: if s.empty?
来源：http://hz.chenzaomai.com/gtwmjazsuq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.cqqwz.cn/gtcksbrzir.html

[E21] 超长截断加省略号
来源：http://hz.guannengcc.top/gtgedqiali.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.gzhubu.top/gtbwpgdxty.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.daxiang520.top/gtxofcuqzi.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.iojbl.cn/gtxoophicb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hfpthk.cn/gtciufylld.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.ywan-chungtsiang.top/gtdmwurlbw.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.xinyue.icu/gtnbssqlkd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.hnxiangtu.top/gtdyiybnzs.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.zhengqikj.top/gtvujkorrp.html

[E22] 字节长度与字符长度
来源：http://hz.quarkkingdee.top/gtollqurwf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.iojbl.cn/gthftvikvo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.wangdashe.top/gtwwgkjupi.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.vqdsnc.cn/gtixspvciv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.tianlin.xyz/gtcygmjqhh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.tianlin.xyz/gtlfxpxwuh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zycfv.cn/gttfewpwtm.html

Ruby: s.bytesize;  s.length
来源：http://hz.yj202588.top/gtoeetbjhh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yangfankeji.com/gtmwoirsrf.html

================================================================================
来源：http://hz.cdnleiting.top/gtytyqqvqq.html

F. 文件与目录
来源：http://hz.haohaochexian.top/gtgnhbwccn.html

================================================================================
来源：http://hz.sweek.top/gtvgmfwthb.html

[F01] 读取整个文件
来源：http://hz.52xcode.cn/gtsbkvceen.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.zdqjudy.top/gtgagdelya.html

PHP:  file_get_contents("a.txt");
来源：http://hz.chenjidiqi.icu/gtasabwqcb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.fzhhl.top/gtvbhynrsd.html


<!-- 参考信息 -->