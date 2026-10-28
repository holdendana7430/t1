代发 wailian999

[D15] 去重
来源：http://hz.dianchejie.cn/gthyqcuntd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.hongshengwenyu.top/gtjyuwgedm.html

PHP:  array_unique($arr);
来源：http://hz.daxiang520.top/gtiwdqnuow.html

JS:   [...new Set(arr)]
来源：http://hz.tianlin.xyz/gtzdnlbuwm.html

TS:   [...new Set(arr)]
来源：http://hz.xuetiantiany.cn/gtiojwfcpi.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.hysaishi.cn/gttoqacvyl.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.hnqzz.top/gtwaozczyo.html

Ruby: arr.uniq
来源：http://hz.yueranfly.top/gtidxyshko.html

C#:   list.Distinct().ToList()
来源：http://hz.xingfuxueyuan.xyz/gttvfcjyds.html

[D16] 求和与平均值
来源：http://hz.xuetiantiany.cn/gtyipngxux.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.bjfxy.top/gtjzqwxxrz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.shzxlz.cn/gtocrqmhbo.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.52xcode.cn/gtgikemedj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.dianchejie.cn/gtmdqkxstv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.zhongyouzk.top/gtgmxrtayt.html

Go:   // 手写循环累加
来源：http://hz.yj20258888.top/gtuzcnugel.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.chenzaomai.com/gthqejtysi.html

C#:   list.Sum();  list.Average()
来源：http://hz.xylfe.cn/gtlykbqvrm.html

[D17] 最大值与最小值
来源：http://hz.daria6918.cn/gtfbdzhrri.html

Py:   max(arr);  min(arr)
来源：http://hz.ybcxt.top/gtbqjoaehe.html

PHP:  max($arr);  min($arr);
来源：http://hz.shanyushiyangkeji.top/gtchjqfytf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.shzxlz.cn/gtfgnoolvg.html

TS:   Math.max(...arr);
来源：http://hz.zycfv.cn/gtzusqlmnm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.guowangkeji.top/gthnoziocj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hysaishi.cn/gtfwdunkmg.html

Ruby: arr.max;  arr.min
来源：http://hz.zdqjudy.top/gtpspvhcnq.html

C#:   list.Max();  list.Min()
来源：http://hz.jianghu66.top/gtqlnlvazs.html

[D18] 扁平化嵌套数组
来源：http://hz.xuetiantiany.cn/gtapeffbkq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.shzxlz.cn/gtemgocqej.html

PHP:  array_merge(...$nested);
来源：http://hz.guowangkeji.top/gtqtdmvskz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yj202588.top/gtvskauoge.html

TS:   nested.flat();
来源：http://hz.shanyushiyangkeji.top/gtunzxjflu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.jyoumei.cn/gtjsrygcgl.html

Go:   // 手写双层循环
来源：http://hz.yuxming.cn/gtvajxqgwx.html

Ruby: nested.flatten
来源：http://hz.cucudq.cn/gtbvrhnjhw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.nanxuanxn.top/gtalwknqog.html

[D19] 按字段分组
来源：http://hz.tianlin.xyz/gtmphsnrrr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.quarkkingdee.top/gtlhuxnwgs.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.cheryme.top/gtctyihkfm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jinyuanbaomall.cn/gtkjojauqo.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.ehwqpu.com/gtfxclperm.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.daxiang520.top/gtaslbmgcc.html

Go:   // 手写 map[string][]T
来源：http://hz.yvedp.cn/gtewcmthme.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.snrcjt.cn/gtpasnramd.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.ivvv.top/gtdglaacph.html

[D20] 统计每个元素出现次数
来源：http://hz.hysaishi.cn/gtbebpcauf.html

Py:   Counter(arr)
来源：http://hz.jyoumei.cn/gtafxouzrv.html

PHP:  array_count_values($arr);
来源：http://hz.aizwys.cn/gtptdhvlyz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.daxiang520.top/gttuvugzlt.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.haohaochexian.top/gtlijrrnwv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.ydzc1.top/gtxhpwdbww.html

Go:   // 手写 map[T]int
来源：http://hz.hnqzz.top/gtpuruhamn.html

Ruby: arr.tally
来源：http://hz.xuetiantiany.cn/gtatybyuey.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.sweek.top/gtezltddtn.html

[D21] 判断是否包含某元素
来源：http://hz.shzxlz.cn/gtccddpdqx.html

Py:   x in arr
来源：http://hz.bjfxy.top/gthnrsrfym.html

PHP:  in_array($x, $arr, true);
来源：http://hz.zhengqikj.top/gtfxfxfvcq.html

JS:   arr.includes(x)
来源：http://hz.hnqzz.top/gtvozgushp.html

TS:   arr.includes(x)
来源：http://hz.cdnleiting.top/gtgsplxmmo.html

Java: list.contains(x)
来源：http://hz.hysaishi.cn/gtldnpqwwn.html

Go:   slices.Contains(arr, x)
来源：http://hz.sweek.top/gtdvcynjwz.html

Ruby: arr.include?(x)
来源：http://hz.zhixingplan.top/gtnuajulfc.html

C#:   list.Contains(x)
来源：http://hz.sweek.top/gtoosgumus.html

[D22] 复制数组（避免共享引用）
来源：http://hz.chenjidiqi.icu/gtbxcmcowy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.hywenlv.cn/gtwobyeast.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.zdqjudy.top/gttdflwkax.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yuxming.cn/gtzdcigdjr.html

TS:   [...arr];
来源：http://hz.sxryk.cn/gtyrnrslcu.html

Java: new ArrayList<>(list);
来源：http://hz.yj202588.top/gtsjtptyzc.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jinghuilouyu.cn/gtczkqelmo.html

Ruby: arr.dup;  arr.clone
来源：http://hz.daria6918.cn/gtdmghprle.html

C#:   new List<int>(list);
来源：http://hz.yj20258888.top/gtrpmayhss.html

[D23] reduce 累积计算
来源：http://hz.ehwqpu.com/gttxogeygp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.shanyushiyangkeji.top/gtprvjrufg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.pycfn.com/gtntmqthrb.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.0kj1m.cn/gtbmjujuhw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jlsjyb.cn/gtgsvwggwi.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.mhx1999.top/gtxhmwbzhs.html

Go:   // 手写循环
来源：http://hz.tian-w.cn/gtrmcrtjpt.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.cdnleiting.top/gtqvgwxufo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.nanxinkj.top/gtosaqqaed.html

[D24] 字典 / Map 基本操作
来源：http://hz.shangyingyoupin.top/gtcgbictke.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.ywan-chungtsiang.top/gtppejgirr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.zhengqikj.top/gtjqnxmddt.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yueranfly.top/gthzvubljy.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.zhengqikj.top/gtdhzwekdn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.hammf.cn/gtassaeiwd.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.bjfxy.top/gtdvxsegey.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.sweek.top/gtepugwylx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.hysaishi.cn/gttzmvpiar.html

[D25] Set 集合去重与交并差
来源：http://hz.svipenyu.cn/gtgshtvvbn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.gogol.net.cn/gtmixeynaj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.cdnleiting.top/gtvxupvrlf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.c1oappe.top/gtmlisjtbn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.cucudq.cn/gtqsheycjp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.jianghu66.top/gtlfditaig.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.jinqigfzy.top/gtfhjjzstv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.shangyingyoupin.top/gtmlncebiq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.birdmap.top/gtryqzaqtd.html

[D26] 数组转字符串
来源：http://hz.ppjwa.cn/gtvtlmixkf.html

Py:   ", ".join(map(str, arr))
来源：http://hz.xinyue.icu/gtigyqhhsn.html

PHP:  implode(", ", $arr);
来源：http://hz.xinyue.icu/gtqvymsoon.html

JS:   arr.join(", ")
来源：http://hz.snrcjt.cn/gtupaoyzyv.html

TS:   arr.join(", ")
来源：http://hz.ywan-chungtsiang.top/gtlvrzshhv.html

Java: String.join(", ", list)
来源：http://hz.svipenyu.cn/gtillzvbxl.html

Go:   strings.Join(strs, ", ")
来源：http://hz.nanxuanxn.top/gtbgeibpuy.html

Ruby: arr.join(", ")
来源：http://hz.xuetiantiany.cn/gtlxsjefxo.html

C#:   string.Join(", ", list)
来源：http://hz.hysaishi.cn/gttvgevdek.html

================================================================================
来源：http://hz.hfpthk.cn/gthuqdkxub.html

E. 字符串处理
来源：http://hz.zhixingplan.top/gtmeutjlxf.html

================================================================================
来源：http://hz.52xcode.cn/gtzpptifsz.html

[E01] 拼接字符串
来源：http://hz.yangfankeji.com/gtfjacpcyz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.sxryk.cn/gtubbrhduf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.mhx1999.top/gtxgqhidlo.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhaomingkeji.xyz/gtpdrkobdu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jqgfzy.top/gtfyiqsidz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.chenlongwang.top/gtxrmegscd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.shzxlz.cn/gtlvnhipux.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.hnxiangtu.top/gtigheyevq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.tian-w.cn/gtyzfdifti.html

[E02] 重复字符串
来源：http://hz.cucudq.cn/gtzibawrnd.html

Py:   "ab" * 3
来源：http://hz.gotoacloud.top/gtrnnylbqh.html

PHP:  str_repeat("ab", 3);
来源：http://hz.jinqigfzy.top/gtugylvdzb.html

JS:   "ab".repeat(3)
来源：http://hz.aibaodan.cn/gtvqafreru.html

TS:   "ab".repeat(3)
来源：http://hz.hnxiangtu.top/gtfekdnmze.html

Java: "ab".repeat(3)
来源：http://hz.9152youxi.cn/gtyudmyzzd.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.yanxiufei.cn/gtxeimurmp.html

Ruby: "ab" * 3
来源：http://hz.gaohongyu789.top/gtngrokowp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.dashuyun.cn/gtluktjvbw.html

[E03] 截取子串
来源：http://hz.zhengqikj.top/gtetwrfabz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.daxiang520.top/gtlwssubzu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.dianchejie.cn/gtvcxfqfyi.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jianghu66.top/gtthxbkilh.html

TS:   s.slice(1, 4)
来源：http://hz.jyoumei.cn/gtujpjjnkr.html

Java: s.substring(1, 4)
来源：http://hz.zhixingplan.top/gteoqtvpva.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.nanxuanxn.top/gtfmugmmma.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.havefunace.top/gtzjhcyrcm.html

C#:   s.Substring(1, 3)
来源：http://hz.pycfn.com/gtngvfnfdh.html

[E04] 查找子串位置
来源：http://hz.snrcjt.cn/gtzpehrwmw.html

Py:   s.find("x");  s.index("x")
来源：http://hz.xinyue.icu/gtyggvvmui.html

PHP:  strpos($s, "x");
来源：http://hz.shuidangran.top/gtqmaiswkx.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.cdnleiting.top/gttsbyhcdc.html

TS:   s.indexOf("x")
来源：http://hz.zhixingplan.top/gtjrmcakhu.html

Java: s.indexOf("x")
来源：http://hz.sweek.top/gtkdsjwjlp.html

Go:   strings.Index(s, "x")
来源：http://hz.jyoumei.cn/gtqtucwsos.html

Ruby: s.index("x")
来源：http://hz.ydzc1.top/gtcgtpgeos.html

C#:   s.IndexOf("x")
来源：http://hz.cucudq.cn/gtgbegmygj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.pengpengdd.cyou/gtghllspsn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.meibo888.top/gtggdhshxj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.daxiang520.top/gtgieayvnn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.iojbl.cn/gtvsvgcmcx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.nanxinkj.top/gtsbfhltnj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jiagoushi.top/gtutyslmel.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.jinghuilouyu.cn/gtrtdezrhh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.gotoacloud.top/gtymvsrvzp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yongpay.top/gtvghwglfv.html

[E06] 替换子串
来源：http://hz.zhijiandao.cn/gtwgywygmn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.havefunace.top/gtfgladdle.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.zhoulong.xyz/gtgbfaeceb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhengqikj.top/gtqorhhdrj.html

TS:   s.replaceAll("a", "b")
来源：http://hz.mhx1999.top/gtzsfnolgf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.meibo888.top/gteumcrryg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.daria6918.cn/gtdkaysaus.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.316326.xyz/gtmwbyiums.html

C#:   s.Replace("a", "b")
来源：http://hz.jinyuanbaomall.cn/gtybnpcjsi.html

[E07] 按分隔符拆分
来源：http://hz.havefunace.top/gtrlqfxaal.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.sweek.top/gtmtdxbulw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yuxming.cn/gturblzbjf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.birdmap.top/gtqavsofrq.html

TS:   s.split(",")
来源：http://hz.sweek.top/gtctvblxbe.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.cucudq.cn/gtjskkmaet.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.zhijiandao.cn/gtvuqzxbxe.html

Ruby: s.split(",");  s.split
来源：http://hz.chenjidiqi.icu/gtyykcfztb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.cdnleiting.top/gtgoymarua.html

[E08] 数组按分隔符合并
来源：http://hz.kuanghao11.cn/gtflkrtruk.html

Py:   ",".join(items)
来源：http://hz.hnqzz.top/gteetbbeci.html

PHP:  implode(",", $items);
来源：http://hz.bjfxy.top/gtwvejcmgn.html

JS:   items.join(",")
来源：http://hz.meibo888.top/gtfwcxckjz.html

TS:   items.join(",")
来源：http://hz.zhoulong.xyz/gtylzlycek.html

Java: String.join(",", items)
来源：http://hz.havefunace.top/gtbeucnyjc.html

Go:   strings.Join(items, ",")
来源：http://hz.tianlin.xyz/gtkoovswnx.html

Ruby: items.join(",")
来源：http://hz.fengsongda.top/gtdrburlzt.html

C#:   string.Join(",", items)
来源：http://hz.9152youxi.cn/gtrowtmmmi.html

[E09] 去除所有空白字符
来源：http://hz.havefunace.top/gtwynzadrx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.quarkkingdee.top/gtwqpxhkzc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.snrcjt.cn/gtpdfkphly.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.xziqi.cn/gtozjedbeb.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.52xcode.cn/gtfgvommmb.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.9152youxi.cn/gtwvltcgau.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.mhx1999.top/gtyhyizuap.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.hammf.cn/gtfemwgwom.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.redwolf501.top/gtqntmrlln.html

[E10] 左侧补零 / 定长填充
来源：http://hz.jianghu66.top/gtcrcpfuft.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.jqgufenzy.top/gtuhljwsez.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.daxiang520.top/gthtsfgfku.html

JS:   "7".padStart(3, "0")
来源：http://hz.yangfankeji.com/gtgukvnmvk.html

TS:   "7".padStart(3, "0")
来源：http://hz.ehwqpu.com/gtznfhmmpa.html

Java: String.format("%03d", 7)
来源：http://hz.ydzc1.top/gtsulmvuxu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.haohaochexian.top/gtufmrbgnp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.chenzaomai.com/gtdtqqlvrl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.0kj1m.cn/gtmbdhdmen.html

[E11] 反转字符串
来源：http://hz.wangshuangyany.cn/gtifevgnfs.html

Py:   s[::-1]
来源：http://hz.fengsongda.top/gtcodapppg.html

PHP:  strrev($s);
来源：http://hz.shanyushiyangkeji.top/gtnafsnqjf.html

JS:   [...s].reverse().join("")
来源：http://hz.ppjwa.cn/gtqybqzkku.html

TS:   [...s].reverse().join("")
来源：http://hz.ppjwa.cn/gtewvneues.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.dianchejie.cn/gtexnknmrc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.jianghu66.top/gtszyynfwv.html

Ruby: s.reverse
来源：http://hz.dashuyun.cn/gthcamucsx.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.fengsongda.top/gtejzdcyru.html

[E12] 统计某字符出现次数
来源：http://hz.quarkkingdee.top/gtojhjlzuq.html

Py:   s.count("a")
来源：http://hz.ehwqpu.com/gtllhanvie.html

PHP:  substr_count($s, "a");
来源：http://hz.ydjk.org.cn/gtetpoycsm.html

JS:   s.split("a").length - 1
来源：http://hz.yongpay.top/gttxjchygn.html

TS:   s.split("a").length - 1
来源：http://hz.jqgufenzy.top/gteixtxhvj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.haohaochexian.top/gtwqikcqat.html

Go:   strings.Count(s, "a")
来源：http://hz.shangyingyoupin.top/gtjagcgmsv.html

Ruby: s.count("a")
来源：http://hz.zhaomingkeji.xyz/gtlqvauzkn.html

C#:   s.Count(c => c == 'a')
来源：http://hz.cdnleiting.top/gtnwexczrx.html

[E13] 逐字符遍历
来源：http://hz.haohaochexian.top/gthdkonmla.html

Py:   for ch in s: print(ch)
来源：http://hz.xuanzx.com/gtuzjofoym.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.nanxuanxn.top/gtplunatay.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhixingplan.top/gtikrvucfw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.316326.xyz/gtgcbculew.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.shzxlz.cn/gtlnxfrzug.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.ehwqpu.com/gtkumunxjl.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yuxming.cn/gtuprealxk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.yvedp.cn/gtxjrgfivs.html

[E14] URL 编码与 Base64
来源：http://hz.yonumen.top/gtcxnoxyju.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.chenjidiqi.icu/gtrwiugoeh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.ppjwa.cn/gtazvufkjy.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.tian-w.cn/gtlfudlibz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.aizwys.cn/gtolgjigag.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yvedp.cn/gtvbbmnlcd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.shanyushiyangkeji.top/gtfdlcsqyc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.nwbrower.top/gtjgrvfhdc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zhijiandao.cn/gttdyxjxfx.html

[E15] HTML 转义 / 反转义
来源：http://hz.dianchejie.cn/gtalnkrnea.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.hammf.cn/gtouxjtjsh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.tian-w.cn/gtvefblcnp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.fengsongda.top/gtzifwwiat.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yongpay.top/gtuqucunwe.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.zhixingplan.top/gtnrdypldt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.zhengqikj.top/gtxlccqioq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.hywenlv.cn/gtcobkxtjm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.redwolf501.top/gtvbmeuhwf.html

[E16] 数字千分位
来源：http://hz.52xcode.cn/gtobneexoj.html

Py:   f"{1234567:,}"
来源：http://hz.cashguo.top/gtuscwmcls.html

PHP:  number_format(1234567);
来源：http://hz.xuetiantiany.cn/gtxdtzzxcv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.snrcjt.cn/gtlzbwupan.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jinghuilouyu.cn/gtidvgwqbu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jinqigufen.top/gthimcxayg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.sysykeji.top/gtjrsamvjm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.cashguo.top/gttgxcwelu.html

C#:   1234567.ToString("N0")
来源：http://hz.jqgfzy.top/gtkitlqkyc.html

[E17] 首字母大写
来源：http://hz.jinqigufen.top/gtrnvexnld.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.svipenyu.cn/gtwgabkpyv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.0kj1m.cn/gtpczduoll.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sufxvd.cn/gtvinahrdw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.9152youxi.cn/gtnlcslcys.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.wangdashe.top/gtqaywngak.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.snrcjt.cn/gtpvxaxnxl.html

Ruby: s.capitalize
来源：http://hz.xuetiantiany.cn/gtdgobpynr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.fengsongda.top/gtagcbkiqt.html

[E18] 模板占位符替换
来源：http://hz.svipenyu.cn/gtyqtzfeyf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.quarkkingdee.top/gtxcygwjor.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.chenlongwang.top/gtfjtgydax.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.zycfv.cn/gttixelvie.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.ywan-chungtsiang.top/gtdkibqtqs.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.mhx1999.top/gthsqgaatv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.cqqwz.cn/gthqipqmiq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.cheryme.top/gtaoiprzyg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.9152youxi.cn/gtbidbqxwz.html

[E19] 多行文本按行拆分
来源：http://hz.zhaomingkeji.xyz/gtnrbshszf.html

Py:   s.splitlines()
来源：http://hz.pycfn.com/gtyckhtbfi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.zdqjudy.top/gtlkbuwlld.html

JS:   s.split(/\r?\n/)
来源：http://hz.cucudq.cn/gtperczbsj.html

TS:   s.split(/\r?\n/)
来源：http://hz.zhiwuduotai.top/gtajbmrqyt.html

Java: s.lines().toList()
来源：http://hz.wangdashe.top/gttvndqgnx.html

Go:   strings.Split(s, "\n")
来源：http://hz.andypj.xyz/gtpdvwuxxl.html

Ruby: s.lines
来源：http://hz.9152youxi.cn/gtrbqbiwaq.html

C#:   s.Split('\n')
来源：http://hz.ydzc1.top/gtoefaftqj.html

[E20] 判断字符串是否为空
来源：http://hz.andypj.xyz/gtncwbicul.html

Py:   if not s:
来源：http://hz.yuanzhike.top/gtejwawkix.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.ybcxt.top/gtnogszjfq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yuxming.cn/gtpiztxett.html

TS:   if (s === "") {}
来源：http://hz.vqdsnc.cn/gtdqlxdyoh.html

Java: if (s.isEmpty()) {}
来源：http://hz.nwbrower.top/gteetbimdv.html

Go:   if s == "" {}
来源：http://hz.dianchejie.cn/gtshlerbqb.html

Ruby: if s.empty?
来源：http://hz.cqqwz.cn/gtuwauuvno.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.meibo888.top/gtaagbgvzu.html

[E21] 超长截断加省略号
来源：http://hz.yanxiufei.cn/gtezxsgvth.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.cashguo.top/gtnmarjhhd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.shanyushiyangtech.top/gtpntmoabi.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jyoumei.cn/gtnjdgmlxd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.wangshuangyany.cn/gtbdctzobn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.chenlongwang.top/gtcgkbbrbz.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.hywenlv.cn/gttgybmvsi.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jlsjyb.cn/gtmlyukoco.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yueranfly.top/gtcwvubcae.html


<!-- 参考信息 -->