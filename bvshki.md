代发 wailian999

C#:   list.Distinct().ToList()
来源：http://hz.jlsjyb.cn/gtpvzltczj.html

[D16] 求和与平均值
来源：http://hz.ppjwa.cn/gtkjyzxajb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jinqigufen.top/gtplhvcheu.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.chenzaomai.com/gtlveefecb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.pycfn.com/gtsrazrlwj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yanxiufei.cn/gtyhpcyyca.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.jinyuanbaomall.cn/gtylwvarzv.html

Go:   // 手写循环累加
来源：http://hz.chenlongwang.top/gtbwnuaxgf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.chenzaomai.com/gtzlaekeen.html

C#:   list.Sum();  list.Average()
来源：http://hz.kuanghao11.cn/gtkyguxnqy.html

[D17] 最大值与最小值
来源：http://hz.zycfv.cn/gtwzuxoyns.html

Py:   max(arr);  min(arr)
来源：http://hz.vqdsnc.cn/gtexwmbeov.html

PHP:  max($arr);  min($arr);
来源：http://hz.kuanghao11.cn/gthsrysbyx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.xziqi.cn/gtvarudifw.html

TS:   Math.max(...arr);
来源：http://hz.smart0.xyz/gthhzmkrmm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.xuanzx.com/gtheytfsny.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jiagoushi.top/gtvtymzgrv.html

Ruby: arr.max;  arr.min
来源：http://hz.gzhubu.top/gttgbnkjul.html

C#:   list.Max();  list.Min()
来源：http://hz.ppjwa.cn/gtadthneai.html

[D18] 扁平化嵌套数组
来源：http://hz.yueranfly.top/gttnkywbax.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.jiagoushi.top/gtbqyqpcmv.html

PHP:  array_merge(...$nested);
来源：http://hz.ybcxt.top/gtsntgvghn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.xinyue.icu/gtauwmxiur.html

TS:   nested.flat();
来源：http://hz.jyoumei.cn/gtfuaxlvll.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.nanxuanxn.top/gtkukpoigl.html

Go:   // 手写双层循环
来源：http://hz.tian-w.cn/gtogqhlnij.html

Ruby: nested.flatten
来源：http://hz.jianghu66.top/gtjccgxoic.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.ehwqpu.com/gtclpgujgb.html

[D19] 按字段分组
来源：http://hz.jinqigufen.top/gtyazjcemb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.cucudq.cn/gtzejesjbd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jianghu66.top/gtujjojvsx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jlsjyb.cn/gtrbctqnxm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.shzxlz.cn/gtlyqdxycn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yueranfly.top/gtfkouvllp.html

Go:   // 手写 map[string][]T
来源：http://hz.bjfxy.top/gtyoaqnliw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.shangyingyoupin.top/gtrypxellr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yonumen.top/gthpijsmvg.html

[D20] 统计每个元素出现次数
来源：http://hz.ppjwa.cn/gthbxxapnn.html

Py:   Counter(arr)
来源：http://hz.fengsongda.top/gthjacxhzg.html

PHP:  array_count_values($arr);
来源：http://hz.shzxlz.cn/gtehhijnnj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xinyue.icu/gthztrobms.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.andypj.xyz/gtbgmnncir.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.fzhhl.top/gtputemrbb.html

Go:   // 手写 map[T]int
来源：http://hz.gzhubu.top/gtxoybctoq.html

Ruby: arr.tally
来源：http://hz.yj20258888.top/gtizhltlhh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.zhiwuduotai.top/gtjhqiceeo.html

[D21] 判断是否包含某元素
来源：http://hz.jyoumei.cn/gtkcdlybyg.html

Py:   x in arr
来源：http://hz.yj202588.top/gtradwmoft.html

PHP:  in_array($x, $arr, true);
来源：http://hz.xinyue.icu/gtwnkkxixe.html

JS:   arr.includes(x)
来源：http://hz.guowangkeji.top/gtftvxuhfd.html

TS:   arr.includes(x)
来源：http://hz.cqqwz.cn/gtbeumtjjz.html

Java: list.contains(x)
来源：http://hz.iojbl.cn/gtpzpaizzl.html

Go:   slices.Contains(arr, x)
来源：http://hz.xingfuxueyuan.xyz/gtytmcqqks.html

Ruby: arr.include?(x)
来源：http://hz.yj202588.top/gtzeaceyen.html

C#:   list.Contains(x)
来源：http://hz.jinyuanbaomall.cn/gteqkbetdi.html

[D22] 复制数组（避免共享引用）
来源：http://hz.tianlin.xyz/gtkvqrapbp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.ehwqpu.com/gtozlwvezd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.aizwys.cn/gtqprpjapy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.cheryme.top/gtjfgzoigh.html

TS:   [...arr];
来源：http://hz.jinqigfzy.top/gtizxhdxzk.html

Java: new ArrayList<>(list);
来源：http://hz.fengsongda.top/gtgazfwxst.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.dashuyun.cn/gtfdeqievk.html

Ruby: arr.dup;  arr.clone
来源：http://hz.daria6918.cn/gtzxnqbdde.html

C#:   new List<int>(list);
来源：http://hz.zhiwuduotai.top/gtztnfwkbk.html

[D23] reduce 累积计算
来源：http://hz.ivvv.top/gtjqcmvgei.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.mhx1999.top/gtcmkortyv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.ywan-chungtsiang.top/gtdpyljjkb.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.snrcjt.cn/gtabwdtzrd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yueranfly.top/gtoheefylm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jinyuanbaomall.cn/gtfkvqjwew.html

Go:   // 手写循环
来源：http://hz.c1oappe.top/gtffbydagj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.xuanzx.com/gtwaontsae.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.redwolf501.top/gtrjosgjuc.html

[D24] 字典 / Map 基本操作
来源：http://hz.zhixingplan.top/gtjlwjdudj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.yangfankeji.com/gtqtuxqsvr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.ehwqpu.com/gtntvtlvfc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.c1oappe.top/gtiupngexd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.dashuyun.cn/gtoppqjdlw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.tianlin.xyz/gtahbvatla.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.zhixingplan.top/gtgadvdwtj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.gotoacloud.top/gtdovdkkji.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.mhx1999.top/gtslyolcds.html

[D25] Set 集合去重与交并差
来源：http://hz.yangfankeji.com/gtkepdwuql.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zhaomingkeji.xyz/gtlzabngfk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.nanxinkj.top/gtqqdxbtfa.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.zhixingplan.top/gtttvvsrch.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.snrcjt.cn/gtlamhuugv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.chenzaomai.com/gttfcfvcib.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.wangdashe.top/gtmbvowwsg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jinghuilouyu.cn/gtmqjyngyp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.fzhhl.top/gtxptsnxtl.html

[D26] 数组转字符串
来源：http://hz.zycfv.cn/gtlaryuwjt.html

Py:   ", ".join(map(str, arr))
来源：http://hz.yj20258888.top/gtxlqtpwbt.html

PHP:  implode(", ", $arr);
来源：http://hz.yj20258888.top/gtxauwenrw.html

JS:   arr.join(", ")
来源：http://hz.yj20258888.top/gtgwfscctm.html

TS:   arr.join(", ")
来源：http://hz.andypj.xyz/gtuedtkhea.html

Java: String.join(", ", list)
来源：http://hz.shzxlz.cn/gtcdilcoyo.html

Go:   strings.Join(strs, ", ")
来源：http://hz.jiagoushi.top/gtaduyfhks.html

Ruby: arr.join(", ")
来源：http://hz.nwbrower.top/gtrjflvodv.html

C#:   string.Join(", ", list)
来源：http://hz.ydjk.org.cn/gtsvqbgjvb.html

================================================================================
来源：http://hz.cheryme.top/gthggnruoa.html

E. 字符串处理
来源：http://hz.cqqwz.cn/gtnlxnrexg.html

================================================================================
来源：http://hz.daxiang520.top/gtvrqiyyju.html

[E01] 拼接字符串
来源：http://hz.yj20258888.top/gtpmzbapkm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.shzxlz.cn/gtkqclropu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.sweek.top/gttlsklyih.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.snrcjt.cn/gtlymwbbxx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jqgufenzy.top/gtjhyoappz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.daxiang520.top/gtqyvncvyt.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.xuetiantiany.cn/gtaxoyvpwy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.pengpengdd.cyou/gtobzptugu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.guowangkeji.top/gtwnmkxloi.html

[E02] 重复字符串
来源：http://hz.sysykeji.top/gtxrkegykk.html

Py:   "ab" * 3
来源：http://hz.daria6918.cn/gtgxnutjlb.html

PHP:  str_repeat("ab", 3);
来源：http://hz.shangyingyoupin.top/gtbngfglij.html

JS:   "ab".repeat(3)
来源：http://hz.ivvv.top/gtngtjyphf.html

TS:   "ab".repeat(3)
来源：http://hz.0kj1m.cn/gtvpwctetg.html

Java: "ab".repeat(3)
来源：http://hz.chenjidiqi.icu/gtcmkiuimz.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.meibo888.top/gtvwpywvpb.html

Ruby: "ab" * 3
来源：http://hz.daria6918.cn/gtklnseibs.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.zhijiandao.cn/gtdsnkhigz.html

[E03] 截取子串
来源：http://hz.havefunace.top/gttqllwwuc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yonumen.top/gtmcdfuxbj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.xuetiantiany.cn/gtbhcnspos.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.aizwys.cn/gtwghavkit.html

TS:   s.slice(1, 4)
来源：http://hz.aizwys.cn/gtytrlenmx.html

Java: s.substring(1, 4)
来源：http://hz.cucudq.cn/gttvpnnpci.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.xziqi.cn/gththhrqvq.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.shangyingyoupin.top/gtyyztontp.html

C#:   s.Substring(1, 3)
来源：http://hz.gogol.net.cn/gthkffsijg.html

[E04] 查找子串位置
来源：http://hz.zhongyouzk.top/gtmndzaypq.html

Py:   s.find("x");  s.index("x")
来源：http://hz.zhoulong.xyz/gtzdpezxaj.html

PHP:  strpos($s, "x");
来源：http://hz.meibo888.top/gtbwhbsbul.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yangfankeji.com/gtmxdahonv.html

TS:   s.indexOf("x")
来源：http://hz.fengsongda.top/gtjztkxcva.html

Java: s.indexOf("x")
来源：http://hz.zhaomingkeji.xyz/gtrercqrfj.html

Go:   strings.Index(s, "x")
来源：http://hz.jinghuilouyu.cn/gtfqehswpm.html

Ruby: s.index("x")
来源：http://hz.snrcjt.cn/gtemsacuia.html

C#:   s.IndexOf("x")
来源：http://hz.shuidangran.top/gtetvdvcmb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.guowangkeji.top/gtjwvfgmzf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.zhaomingkeji.xyz/gtpcgaphjx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.snrcjt.cn/gtxytjgdhx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.birdmap.top/gtyifbkaat.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.hongshengwenyu.top/gtmzjbnlpg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jyoumei.cn/gtjzzfkucs.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.quarkkingdee.top/gtfmkrzzhs.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.daria6918.cn/gtkiutjijs.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.chenlongwang.top/gtdquzrizq.html

[E06] 替换子串
来源：http://hz.smart0.xyz/gtyfrxgyyf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.nwbrower.top/gtslsvjqmd.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.shanyushiyangtech.top/gtqbisocgn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.sxryk.cn/gtdbdlwpdk.html

TS:   s.replaceAll("a", "b")
来源：http://hz.zhijiandao.cn/gtlrnrkgon.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xinyue.icu/gtanlqoyji.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.zdqjudy.top/gtampaimwp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.yvedp.cn/gtkhfmaesv.html

C#:   s.Replace("a", "b")
来源：http://hz.shzxlz.cn/gttzxjgali.html

[E07] 按分隔符拆分
来源：http://hz.zhijiandao.cn/gtmkjdmlbs.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.zhaomingkeji.xyz/gtdzspukac.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.cashguo.top/gtaakclnsn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.sysykeji.top/gtvuoawudq.html

TS:   s.split(",")
来源：http://hz.gogol.net.cn/gtvddpiccs.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.shzxlz.cn/gtfpivnpjm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.vqdsnc.cn/gtzbbhjcom.html

Ruby: s.split(",");  s.split
来源：http://hz.yj20258888.top/gtogetldqn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.zhaomingkeji.xyz/gtcmjsnakd.html

[E08] 数组按分隔符合并
来源：http://hz.ybcxt.top/gtfskslkmi.html

Py:   ",".join(items)
来源：http://hz.gotoacloud.top/gtuekeaiwf.html

PHP:  implode(",", $items);
来源：http://hz.hongshengwenyu.top/gtkgpjwvqo.html

JS:   items.join(",")
来源：http://hz.tianlin.xyz/gtfwmgesvh.html

TS:   items.join(",")
来源：http://hz.fzhhl.top/gtsxvhgpvo.html

Java: String.join(",", items)
来源：http://hz.xylfe.cn/gtbxckcbcw.html

Go:   strings.Join(items, ",")
来源：http://hz.aizwys.cn/gtymutaelw.html

Ruby: items.join(",")
来源：http://hz.ehwqpu.com/gtsexxgmkb.html

C#:   string.Join(",", items)
来源：http://hz.aibaodan.cn/gtvmeznfgz.html

[E09] 去除所有空白字符
来源：http://hz.yueranfly.top/gtyksvlouy.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yj202588.top/gthfegyxun.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.sweek.top/gttcmlvveb.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.sysykeji.top/gtdyfjsiej.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.xinyue.icu/gtolhuybfe.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.ybcxt.top/gthytbcbel.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.ydjk.org.cn/gtxydcpecy.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.pycfn.com/gtvhmhhbns.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.xinyue.icu/gtoqgiymaj.html

[E10] 左侧补零 / 定长填充
来源：http://hz.cucudq.cn/gtivizyauu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.bjfxy.top/gtihcowimo.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.andypj.xyz/gtopkcgqrp.html

JS:   "7".padStart(3, "0")
来源：http://hz.daria6918.cn/gtwcmvsodb.html

TS:   "7".padStart(3, "0")
来源：http://hz.dashuyun.cn/gtoonjqovv.html

Java: String.format("%03d", 7)
来源：http://hz.xuetiantiany.cn/gtxlyrnikf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.hongshengwenyu.top/gtdkvnlani.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.zdqjudy.top/gtyztqbdvt.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.yueranfly.top/gtovinhajz.html

[E11] 反转字符串
来源：http://hz.shangyingyoupin.top/gtydbgcyoq.html

Py:   s[::-1]
来源：http://hz.nwbrower.top/gteovzjywl.html

PHP:  strrev($s);
来源：http://hz.tianlin.xyz/gtjpqxvbhf.html

JS:   [...s].reverse().join("")
来源：http://hz.zhoulong.xyz/gtpwwcqjyt.html

TS:   [...s].reverse().join("")
来源：http://hz.yj202588.top/gtlylqwtih.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yj20258.top/gtvkydlofg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yueranfly.top/gtdvwoyrsq.html

Ruby: s.reverse
来源：http://hz.9152youxi.cn/gtbecbqhjo.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.andypj.xyz/gtcjmplwhs.html

[E12] 统计某字符出现次数
来源：http://hz.316326.xyz/gtwcofcqky.html

Py:   s.count("a")
来源：http://hz.aizwys.cn/gtmevlwdwu.html

PHP:  substr_count($s, "a");
来源：http://hz.sufxvd.cn/gtjzoiwgmp.html

JS:   s.split("a").length - 1
来源：http://hz.haohaochexian.top/gtwvujjyhc.html

TS:   s.split("a").length - 1
来源：http://hz.gaohongyu789.top/gtrgpywpgj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.dashuyun.cn/gtcaxzdfpu.html

Go:   strings.Count(s, "a")
来源：http://hz.daria6918.cn/gtnpirhplu.html

Ruby: s.count("a")
来源：http://hz.52xcode.cn/gtbvaciwup.html

C#:   s.Count(c => c == 'a')
来源：http://hz.ybcxt.top/gthfxafuhm.html

[E13] 逐字符遍历
来源：http://hz.haohaochexian.top/gtcpkpncnm.html

Py:   for ch in s: print(ch)
来源：http://hz.svipenyu.cn/gtghxxlgzg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.c1oappe.top/gtslfpaciy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.wangshuangyany.cn/gtzcptwoan.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jinyuanbaomall.cn/gtcwnscpey.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.shanyushiyangkeji.top/gtigvnbeho.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jyoumei.cn/gtumtuwhvx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.aizwys.cn/gtlkoazxju.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.guannengcc.top/gtdgrrekol.html

[E14] URL 编码与 Base64
来源：http://hz.hnxiangtu.top/gtmmoupsaa.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.zhoulong.xyz/gtlwcpdweh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.shzxlz.cn/gtpomvvdcd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.wangshuangyany.cn/gtdewsdrsk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.fengsongda.top/gtyxrsxjcx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.tanke756.top/gtxqekqkjb.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.52xcode.cn/gtuzqmjjcz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.yanxiufei.cn/gtoczkecgq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.andypj.xyz/gtcqbtygzw.html

[E15] HTML 转义 / 反转义
来源：http://hz.yuanzhike.top/gthfhynawp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.hysaishi.cn/gtlrfowawh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yanxiufei.cn/gtrloybwuw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.ydjk.org.cn/gtbajuvile.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jianghu66.top/gtrzwkvbrt.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.hysaishi.cn/gtymnygefq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.svipenyu.cn/gthbqgtwuz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.shzxlz.cn/gtvazmhhdp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.gaohongyu789.top/gtmgvqcqmt.html

[E16] 数字千分位
来源：http://hz.xylfe.cn/gtusjqarxk.html

Py:   f"{1234567:,}"
来源：http://hz.jqgfzy.top/gtvtuqljjz.html

PHP:  number_format(1234567);
来源：http://hz.ydjk.org.cn/gtwbvxebed.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.c1oappe.top/gtrtjyogvb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.nwbrower.top/gtriypucbg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.gzhubu.top/gtgtlayksf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.0kj1m.cn/gturvqtthx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.ydzc1.top/gtkfdfzpcr.html

C#:   1234567.ToString("N0")
来源：http://hz.ywan-chungtsiang.top/gtkxoyriyu.html

[E17] 首字母大写
来源：http://hz.wangshuangyany.cn/gttcrionwy.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.chenjidiqi.icu/gtiwvqmufx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.zhongyouzk.top/gtcxzhlpuk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.c1oappe.top/gtcnaoowxp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hnxiangtu.top/gttvvwfvpq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.316326.xyz/gtmiqoodyt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.shzxlz.cn/gtcslpuguf.html

Ruby: s.capitalize
来源：http://hz.hysaishi.cn/gtcnfgplrl.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.gotoacloud.top/gtcjdzfzak.html

[E18] 模板占位符替换
来源：http://hz.aibaodan.cn/gtaefdrczq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.c1oappe.top/gtopqsbyef.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.c1oappe.top/gtfuxgwwwi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yanxiufei.cn/gtyhxbxmot.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.tianlin.xyz/gtlbuasowy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.ydzc1.top/gtrnohlhgt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.snrcjt.cn/gtkfcbhbqj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.c1oappe.top/gtynxqttsm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.mhx1999.top/gtztosbxfy.html

[E19] 多行文本按行拆分
来源：http://hz.guowangkeji.top/gtutgkyuhg.html

Py:   s.splitlines()
来源：http://hz.zdqjudy.top/gtcoqrnhuh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.zhongyouzk.top/gtywspkrxg.html

JS:   s.split(/\r?\n/)
来源：http://hz.ywan-chungtsiang.top/gtscklkbds.html

TS:   s.split(/\r?\n/)
来源：http://hz.yanxiufei.cn/gtrsudydqf.html

Java: s.lines().toList()
来源：http://hz.guowangkeji.top/gtletzsyly.html

Go:   strings.Split(s, "\n")
来源：http://hz.ywan-chungtsiang.top/gtxeqrxzab.html

Ruby: s.lines
来源：http://hz.tian-w.cn/gteguikmjq.html

C#:   s.Split('\n')
来源：http://hz.cdnleiting.top/gtlrixhaok.html

[E20] 判断字符串是否为空
来源：http://hz.hammf.cn/gttglnsmdq.html

Py:   if not s:
来源：http://hz.ivvv.top/gtuyhqhbdc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.fzhhl.top/gtroajxstz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.ybcxt.top/gtusaytuyy.html

TS:   if (s === "") {}
来源：http://hz.mhx1999.top/gtknoasemr.html

Java: if (s.isEmpty()) {}
来源：http://hz.yonumen.top/gtlgitmgoq.html

Go:   if s == "" {}
来源：http://hz.yuxming.cn/gttsnofcfs.html

Ruby: if s.empty?
来源：http://hz.guowangkeji.top/gtwyjvxbds.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.zhengqikj.top/gtefbwfziz.html

[E21] 超长截断加省略号
来源：http://hz.bjfxy.top/gtmctwwntu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.c1oappe.top/gtzcbryqke.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.xingfuxueyuan.xyz/gtjxoskcix.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jqgufenzy.top/gtfpdnncuo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jqgfzy.top/gtfoijtewh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jqgfzy.top/gtmivgmjmn.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.aibaodan.cn/gtsgwmdark.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.daria6918.cn/gtzccdfxkb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yueranfly.top/gtsyrxaudu.html

[E22] 字节长度与字符长度
来源：http://hz.c1oappe.top/gtjzahdsvg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.gzhubu.top/gtsclsapjw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.fzhhl.top/gtpjiyqlkc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.52xcode.cn/gtsxiwadsj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.tianlin.xyz/gtiwmvagyq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yj202588.top/gtucfnzasv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.dianchejie.cn/gtmdlghedt.html

Ruby: s.bytesize;  s.length
来源：http://hz.smart0.xyz/gtcxtzoesl.html


<!-- 参考信息 -->