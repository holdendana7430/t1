代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.sufxvd.cn/gtwznvwvfa.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.fengsongda.top/gthgadcgjj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.zhengqikj.top/gtoarvwgvq.html

[D14] 映射转换（每个元素变形）
来源：http://hz.pycfn.com/gtltlziiob.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.52xcode.cn/gtyxmhngpm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yangfankeji.com/gtqjjduxkv.html

JS:   arr.map(x => x * 2)
来源：http://hz.xziqi.cn/gtcupdsiss.html

TS:   arr.map(x => x * 2)
来源：http://hz.feifeiyinyue.top/gttbrntgca.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.hywenlv.cn/gtqdmpebwt.html

Go:   // 手写循环
来源：http://hz.jianghu66.top/gtzfrcefhd.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.zhaomingkeji.xyz/gtnqczhurw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.tanke756.top/gtgqctfvck.html

[D15] 去重
来源：http://hz.chenzaomai.com/gtztjulaid.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.havefunace.top/gtkhyqnwhj.html

PHP:  array_unique($arr);
来源：http://hz.shzxlz.cn/gtyxuchxbk.html

JS:   [...new Set(arr)]
来源：http://hz.jiagoushi.top/gtwcaoeezx.html

TS:   [...new Set(arr)]
来源：http://hz.aizwys.cn/gtwnobxnsb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.xziqi.cn/gtxbqkorjl.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.zhengqikj.top/gtofgxdlmy.html

Ruby: arr.uniq
来源：http://hz.tanke756.top/gtauybxpyz.html

C#:   list.Distinct().ToList()
来源：http://hz.guannengcc.top/gthiehshcu.html

[D16] 求和与平均值
来源：http://hz.yj20258888.top/gtbrdmdlza.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.hongshengwenyu.top/gtxcldysnp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.ehwqpu.com/gtaeovykpq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhengqikj.top/gtixdfrvxz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jlsjyb.cn/gtcofwgfjg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.gzhubu.top/gtnknalmlo.html

Go:   // 手写循环累加
来源：http://hz.ybcxt.top/gtttdtkkvs.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.jyoumei.cn/gtesscufqw.html

C#:   list.Sum();  list.Average()
来源：http://hz.yj202588.top/gtclkzduoh.html

[D17] 最大值与最小值
来源：http://hz.daxiang520.top/gtflxwajjf.html

Py:   max(arr);  min(arr)
来源：http://hz.daxiang520.top/gtzgrevhpw.html

PHP:  max($arr);  min($arr);
来源：http://hz.shangyingyoupin.top/gtabqndocs.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.guowangkeji.top/gtsvwlgchl.html

TS:   Math.max(...arr);
来源：http://hz.ywan-chungtsiang.top/gtfibixbku.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.ppjwa.cn/gtplmxvheb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.yonumen.top/gtkofyuxoc.html

Ruby: arr.max;  arr.min
来源：http://hz.tian-w.cn/gtvyvhdecg.html

C#:   list.Max();  list.Min()
来源：http://hz.zhaomingkeji.xyz/gtepqbdfxf.html

[D18] 扁平化嵌套数组
来源：http://hz.hywenlv.cn/gtcalxbqpy.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.feifeiyinyue.top/gtxqvhdbfp.html

PHP:  array_merge(...$nested);
来源：http://hz.jyoumei.cn/gtxydxxcho.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.sxryk.cn/gtxknijgfx.html

TS:   nested.flat();
来源：http://hz.daria6918.cn/gtybmcpbok.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.zhengqikj.top/gtehqdbvqm.html

Go:   // 手写双层循环
来源：http://hz.dashuyun.cn/gtgnrpekgc.html

Ruby: nested.flatten
来源：http://hz.bjfxy.top/gtjsvxtvxt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.fengsongda.top/gtgtulhbsi.html

[D19] 按字段分组
来源：http://hz.shanyushiyangtech.top/gthrufnvjy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.nanxinkj.top/gtbuqepxkw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.fzhhl.top/gtvpdxbjut.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.hnxiangtu.top/gtbprvnqkv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.cashguo.top/gtbqxfyczj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yongpay.top/gteqeguijc.html

Go:   // 手写 map[string][]T
来源：http://hz.sweek.top/gtkshanbfs.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.yj202588.top/gtzsurtdnt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.smart0.xyz/gtzybyxbip.html

[D20] 统计每个元素出现次数
来源：http://hz.yangfankeji.com/gtgfnblnqb.html

Py:   Counter(arr)
来源：http://hz.mhx1999.top/gtapxlvrhh.html

PHP:  array_count_values($arr);
来源：http://hz.hysaishi.cn/gtbbvklwqq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.sxryk.cn/gtilsysndi.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jinqigufen.top/gtfgdxvgxk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.hywenlv.cn/gtsjhmuctv.html

Go:   // 手写 map[T]int
来源：http://hz.ydzc1.top/gtkwsgfwhu.html

Ruby: arr.tally
来源：http://hz.ybcxt.top/gtcbnqxkax.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.gogol.net.cn/gtgxxangtx.html

[D21] 判断是否包含某元素
来源：http://hz.hnqzz.top/gtjwmmqodc.html

Py:   x in arr
来源：http://hz.sxryk.cn/gtscdkfdas.html

PHP:  in_array($x, $arr, true);
来源：http://hz.zhijiandao.cn/gtqlzixmwu.html

JS:   arr.includes(x)
来源：http://hz.ehwqpu.com/gtfxpeqhbm.html

TS:   arr.includes(x)
来源：http://hz.xingfuxueyuan.xyz/gtbdlcasdn.html

Java: list.contains(x)
来源：http://hz.dashuyun.cn/gtjrmderfc.html

Go:   slices.Contains(arr, x)
来源：http://hz.ywan-chungtsiang.top/gtbrlnfdgb.html

Ruby: arr.include?(x)
来源：http://hz.316326.xyz/gtoabcymjy.html

C#:   list.Contains(x)
来源：http://hz.andypj.xyz/gtgoylpjpn.html

[D22] 复制数组（避免共享引用）
来源：http://hz.xinyue.icu/gtajqyygsr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.smart0.xyz/gttjjcuipc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.shangyingyoupin.top/gtsteknoqo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.haohaochexian.top/gtsepukumj.html

TS:   [...arr];
来源：http://hz.chenjidiqi.icu/gtrxqgcbmw.html

Java: new ArrayList<>(list);
来源：http://hz.birdmap.top/gtvinhnocb.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.iojbl.cn/gtohbvvwfn.html

Ruby: arr.dup;  arr.clone
来源：http://hz.gaohongyu789.top/gtsgdxtkau.html

C#:   new List<int>(list);
来源：http://hz.andypj.xyz/gtdfwkzjcc.html

[D23] reduce 累积计算
来源：http://hz.jyoumei.cn/gtxpfeejta.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.nanxinkj.top/gtujvfjgkg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.sxryk.cn/gtgpfcstcy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ybcxt.top/gtelmakvar.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jyoumei.cn/gtuzuktsmw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jqgfzy.top/gtalskqhah.html

Go:   // 手写循环
来源：http://hz.birdmap.top/gtrfycbcpa.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.yj20258.top/gtimtriuga.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.chenlongwang.top/gtzzrjnuur.html

[D24] 字典 / Map 基本操作
来源：http://hz.jianghu66.top/gtatdxftad.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.hfpthk.cn/gtmjgtyzqw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.tanke756.top/gtwthdaihv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.sxryk.cn/gtpvsmuric.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yangfankeji.com/gtmvwfclsh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.shzxlz.cn/gtsrpqzukx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.fzhhl.top/gtrrxcocto.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.fzhhl.top/gteyecnbzk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.pengpengdd.cyou/gtpdzkahip.html

[D25] Set 集合去重与交并差
来源：http://hz.yj20258.top/gtgupcujfb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zhaomingkeji.xyz/gtljesgjpb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yuanzhike.top/gtqwhokeec.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.snrcjt.cn/gtgsxwdffv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.ywan-chungtsiang.top/gteeipscia.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.jinyuanbaomall.cn/gtkdnposru.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.hywenlv.cn/gtprhgyfvq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yuxming.cn/gtfvwsqsne.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.316326.xyz/gtglfxjdca.html

[D26] 数组转字符串
来源：http://hz.guowangkeji.top/gtkayuztoo.html

Py:   ", ".join(map(str, arr))
来源：http://hz.sweek.top/gtvralxuxw.html

PHP:  implode(", ", $arr);
来源：http://hz.cucudq.cn/gtmzllwysl.html

JS:   arr.join(", ")
来源：http://hz.gogol.net.cn/gtvfxphvqu.html

TS:   arr.join(", ")
来源：http://hz.kuanghao11.cn/gtdomiwbox.html

Java: String.join(", ", list)
来源：http://hz.ppjwa.cn/gtfkkvhpct.html

Go:   strings.Join(strs, ", ")
来源：http://hz.svipenyu.cn/gttbyliqdp.html

Ruby: arr.join(", ")
来源：http://hz.andypj.xyz/gthkgfmpcr.html

C#:   string.Join(", ", list)
来源：http://hz.smart0.xyz/gtdhrixsfo.html

================================================================================
来源：http://hz.ydjk.org.cn/gtdskmfbzj.html

E. 字符串处理
来源：http://hz.hnxiangtu.top/gtupxlmqbc.html

================================================================================
来源：http://hz.nanxuanxn.top/gtcghiythg.html

[E01] 拼接字符串
来源：http://hz.cqqwz.cn/gtxlqneodu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yj20258.top/gtqjalvtqm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.hfpthk.cn/gtqplrkpri.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yanxiufei.cn/gtvkjahsus.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ivvv.top/gtbhbgrtmk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.jinqigfzy.top/gtqfldscts.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.nwbrower.top/gtkvpgnzyc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yueranfly.top/gtruanfbpy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.ywan-chungtsiang.top/gtkqrieqkz.html

[E02] 重复字符串
来源：http://hz.yueranfly.top/gtavgwoprj.html

Py:   "ab" * 3
来源：http://hz.cucudq.cn/gtwtyygdwi.html

PHP:  str_repeat("ab", 3);
来源：http://hz.xuetiantiany.cn/gtkjcqetcb.html

JS:   "ab".repeat(3)
来源：http://hz.jlsjyb.cn/gtzgbnksup.html

TS:   "ab".repeat(3)
来源：http://hz.yvedp.cn/gtvevuztcx.html

Java: "ab".repeat(3)
来源：http://hz.tian-w.cn/gtokrvkjdn.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.chenlongwang.top/gtujdavdik.html

Ruby: "ab" * 3
来源：http://hz.yj20258.top/gtravxupwh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.aizwys.cn/gtfnfwjvmz.html

[E03] 截取子串
来源：http://hz.zycfv.cn/gtoqcmulsv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.snrcjt.cn/gthwsnawyp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.hnqzz.top/gtjjmzwpmo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yuanzhike.top/gtsbrzetwf.html

TS:   s.slice(1, 4)
来源：http://hz.yvedp.cn/gtyhycijks.html

Java: s.substring(1, 4)
来源：http://hz.hnqzz.top/gtgjltbzmk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yuxming.cn/gtaaamduyr.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.guannengcc.top/gtvanuwzqz.html

C#:   s.Substring(1, 3)
来源：http://hz.pycfn.com/gtzcrligtg.html

[E04] 查找子串位置
来源：http://hz.gaohongyu789.top/gtrcksmyyf.html

Py:   s.find("x");  s.index("x")
来源：http://hz.sufxvd.cn/gtkroyxafi.html

PHP:  strpos($s, "x");
来源：http://hz.guannengcc.top/gtytordyxa.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.jqgufenzy.top/gtjxidbnkj.html

TS:   s.indexOf("x")
来源：http://hz.shangyingyoupin.top/gtkngxbjfk.html

Java: s.indexOf("x")
来源：http://hz.hongshengwenyu.top/gtccbknpua.html

Go:   strings.Index(s, "x")
来源：http://hz.ybcxt.top/gtyybjwslp.html

Ruby: s.index("x")
来源：http://hz.hongshengwenyu.top/gtpkwgvfmq.html

C#:   s.IndexOf("x")
来源：http://hz.xingfuxueyuan.xyz/gtqfmiajrd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.fzhhl.top/gtowiaesyd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.dianchejie.cn/gtswcjpxlo.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.yueranfly.top/gtjecllxhe.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.daxiang520.top/gtklpwzijn.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.guannengcc.top/gthdocietg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.cucudq.cn/gtrzmyatyt.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.yueranfly.top/gttsnmqpzf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.zhijiandao.cn/gtpfitozif.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.shangyingyoupin.top/gtxrezrlew.html

[E06] 替换子串
来源：http://hz.xinyue.icu/gtgzvzrjyo.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.hywenlv.cn/gtxzzidkyg.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.aibaodan.cn/gtwwxhsovl.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.mhx1999.top/gtoscmwcqb.html

TS:   s.replaceAll("a", "b")
来源：http://hz.chenzaomai.com/gtofqvcpaj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.wangdashe.top/gtrgokylab.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.zhaomingkeji.xyz/gtyhmomjwr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.snrcjt.cn/gtupbtzfrj.html

C#:   s.Replace("a", "b")
来源：http://hz.zhoulong.xyz/gtkijknish.html

[E07] 按分隔符拆分
来源：http://hz.jinqigfzy.top/gtsfbjmmev.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yongpay.top/gtsrqjagip.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.nanxinkj.top/gtngcgygji.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.andypj.xyz/gtwnjazdcv.html

TS:   s.split(",")
来源：http://hz.hfpthk.cn/gthcyyqfhl.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.shanyushiyangtech.top/gtxizrdqjb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.havefunace.top/gtafhypcwy.html

Ruby: s.split(",");  s.split
来源：http://hz.yj202588.top/gtwuzlmtny.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.zhongyouzk.top/gtblyrrcoc.html

[E08] 数组按分隔符合并
来源：http://hz.smart0.xyz/gtfvkhzfry.html

Py:   ",".join(items)
来源：http://hz.fengsongda.top/gtwhnwowty.html

PHP:  implode(",", $items);
来源：http://hz.bjfxy.top/gtqsvlrruo.html

JS:   items.join(",")
来源：http://hz.shanyushiyangtech.top/gtcrsnrzbk.html

TS:   items.join(",")
来源：http://hz.fzhhl.top/gtrslnpyfa.html

Java: String.join(",", items)
来源：http://hz.xinyue.icu/gtpuaesfzl.html

Go:   strings.Join(items, ",")
来源：http://hz.wangshuangyany.cn/gtbxuqvkne.html

Ruby: items.join(",")
来源：http://hz.guannengcc.top/gteorrvjcr.html

C#:   string.Join(",", items)
来源：http://hz.hfpthk.cn/gtxghqkaec.html

[E09] 去除所有空白字符
来源：http://hz.jqgufenzy.top/gtvijqzkqn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yj20258.top/gtnxikqutc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.shangyingyoupin.top/gtonscsica.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.dianchejie.cn/gtvkzxoqul.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.xylfe.cn/gtxksgjcdf.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.wangshuangyany.cn/gtbqtpdrts.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.jinqigfzy.top/gtoizeslvt.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.52xcode.cn/gtykhxwzcg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.cashguo.top/gtxbeebtwa.html

[E10] 左侧补零 / 定长填充
来源：http://hz.ivvv.top/gtordxdryt.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.gzhubu.top/gthrphdbxo.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.c1oappe.top/gtyyvirlms.html

JS:   "7".padStart(3, "0")
来源：http://hz.xinyue.icu/gthxqytcki.html

TS:   "7".padStart(3, "0")
来源：http://hz.ywan-chungtsiang.top/gtxnixgtvu.html

Java: String.format("%03d", 7)
来源：http://hz.gogol.net.cn/gtjmzfunxu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.zhixingplan.top/gtnakpotmf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.kuanghao11.cn/gtisirycyf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.bjfxy.top/gtcfnwcpqc.html

[E11] 反转字符串
来源：http://hz.gaohongyu789.top/gtgzvjrtht.html

Py:   s[::-1]
来源：http://hz.birdmap.top/gtqwjngapv.html

PHP:  strrev($s);
来源：http://hz.xuanzx.com/gthwrbvzjx.html

JS:   [...s].reverse().join("")
来源：http://hz.pengpengdd.cyou/gtdjewwlay.html

TS:   [...s].reverse().join("")
来源：http://hz.xylfe.cn/gtdgwcxnpu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.0kj1m.cn/gtukbvessf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.jlsjyb.cn/gtbcwozbup.html

Ruby: s.reverse
来源：http://hz.hywenlv.cn/gtcuvirbfo.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.daxiang520.top/gthxlsghmw.html

[E12] 统计某字符出现次数
来源：http://hz.ybcxt.top/gtapehmnwf.html

Py:   s.count("a")
来源：http://hz.zhongyouzk.top/gtsgpadbeu.html

PHP:  substr_count($s, "a");
来源：http://hz.yongpay.top/gtwpjxwbee.html

JS:   s.split("a").length - 1
来源：http://hz.daria6918.cn/gtiwlqpely.html

TS:   s.split("a").length - 1
来源：http://hz.aibaodan.cn/gtxceohodi.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.nwbrower.top/gthtqnyneq.html

Go:   strings.Count(s, "a")
来源：http://hz.zhijiandao.cn/gtyjjwrcle.html

Ruby: s.count("a")
来源：http://hz.yj20258.top/gtakgufvoj.html

C#:   s.Count(c => c == 'a')
来源：http://hz.pengpengdd.cyou/gtvbrkeehd.html

[E13] 逐字符遍历
来源：http://hz.sxryk.cn/gtxdirbuwu.html

Py:   for ch in s: print(ch)
来源：http://hz.jyoumei.cn/gtzepfnjnk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.daria6918.cn/gtyrduccqu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.havefunace.top/gtbcplhnys.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jlsjyb.cn/gtdtzbzqpk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.xuanzx.com/gttresljxr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.smart0.xyz/gtovqcduwz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.andypj.xyz/gtobkdmzxb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.zhixingplan.top/gtmtzyeqnq.html

[E14] URL 编码与 Base64
来源：http://hz.zhoulong.xyz/gtrdexovcg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yj20258888.top/gtqfipteed.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.wangshuangyany.cn/gtzygtdhwv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.cashguo.top/gthkogelnt.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.guannengcc.top/gtcapxxbxf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.snrcjt.cn/gtpryyozkx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.zhengqikj.top/gtoafakgqe.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.ivvv.top/gtzdtsuyxk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zhixingplan.top/gtkdyxekhf.html

[E15] HTML 转义 / 反转义
来源：http://hz.daria6918.cn/gtgpfnpmty.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.hysaishi.cn/gtegosbcud.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.tanke756.top/gtrmaazpgy.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.kuanghao11.cn/gtnmqpwbfc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.dashuyun.cn/gtvhhhhbwc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.ybcxt.top/gtlapxnbgm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.ydzc1.top/gttpoxyrzi.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.nanxinkj.top/gtqiciaugs.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.birdmap.top/gtkyowaipv.html

[E16] 数字千分位
来源：http://hz.chenjidiqi.icu/gtslbtlfai.html

Py:   f"{1234567:,}"
来源：http://hz.xylfe.cn/gtpybiioky.html

PHP:  number_format(1234567);
来源：http://hz.daria6918.cn/gtduyhnyqi.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.snrcjt.cn/gtkfcvtvag.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.0kj1m.cn/gtcjmzxsga.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.gogol.net.cn/gtdpmscafn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.hammf.cn/gtqjxjwkva.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yj20258888.top/gtwrhxhsri.html

C#:   1234567.ToString("N0")
来源：http://hz.shuidangran.top/gttmsluigc.html

[E17] 首字母大写
来源：http://hz.feifeiyinyue.top/gtisoggrln.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.quarkkingdee.top/gtglxmxtiq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.gaohongyu789.top/gtdprxmkec.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sxryk.cn/gtdqlanzap.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jinqigufen.top/gteyzahnym.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jyoumei.cn/gtfrsnceyd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.hysaishi.cn/gtlhilniut.html

Ruby: s.capitalize
来源：http://hz.yj202588.top/gtqxavhpma.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.chenjidiqi.icu/gthmbnvygc.html

[E18] 模板占位符替换
来源：http://hz.ybcxt.top/gtrlkjwczc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.haohaochexian.top/gtbplcdrcm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.feifeiyinyue.top/gttpigzict.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jinqigufen.top/gtpwnpavfx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.0kj1m.cn/gteasfwtkt.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.chenlongwang.top/gtuwmynbcm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.sufxvd.cn/gtenvybump.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.c1oappe.top/gtznynvswf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.chenzaomai.com/gtuobymyfp.html

[E19] 多行文本按行拆分
来源：http://hz.gotoacloud.top/gtagbzrssm.html

Py:   s.splitlines()
来源：http://hz.gaohongyu789.top/gtvhsfpsgv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.chenzaomai.com/gtkmlliuvw.html

JS:   s.split(/\r?\n/)
来源：http://hz.chenlongwang.top/gtulkyioae.html

TS:   s.split(/\r?\n/)
来源：http://hz.zycfv.cn/gtmatgzxse.html

Java: s.lines().toList()
来源：http://hz.jqgfzy.top/gtmgrmgqeq.html

Go:   strings.Split(s, "\n")
来源：http://hz.yongpay.top/gtbgiyfxyr.html

Ruby: s.lines
来源：http://hz.xylfe.cn/gtanzmbqus.html

C#:   s.Split('\n')
来源：http://hz.chenzaomai.com/gtketgkpmg.html

[E20] 判断字符串是否为空
来源：http://hz.redwolf501.top/gtqormwmyb.html

Py:   if not s:
来源：http://hz.jianghu66.top/gtkbvlbbtj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.quarkkingdee.top/gtpzirqxch.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.hnxiangtu.top/gtikambflb.html

TS:   if (s === "") {}
来源：http://hz.zhijiandao.cn/gtnlxkdmjz.html

Java: if (s.isEmpty()) {}
来源：http://hz.xuetiantiany.cn/gtqtchphrz.html


<!-- 参考信息 -->