代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jlsjyb.cn/gtsamwtfre.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.ybcxt.top/gtfhggnder.html

JS:   arr.map(x => x * 2)
来源：http://hz.hammf.cn/gtvfezpake.html

TS:   arr.map(x => x * 2)
来源：http://hz.gaohongyu789.top/gtblyjzdvs.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.chenjidiqi.icu/gtbuwkbrmp.html

Go:   // 手写循环
来源：http://hz.jianghu66.top/gtpailfrey.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.ppjwa.cn/gtczfzltjg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.hysaishi.cn/gtrcenwgmv.html

[D15] 去重
来源：http://hz.yj202588.top/gtbdbealfd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.cdnleiting.top/gtnmtiwmju.html

PHP:  array_unique($arr);
来源：http://hz.smart0.xyz/gtuyilxcin.html

JS:   [...new Set(arr)]
来源：http://hz.cdnleiting.top/gtrncmeqjr.html

TS:   [...new Set(arr)]
来源：http://hz.shuidangran.top/gtacyirrlu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.guowangkeji.top/gtxqheuvhd.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yanxiufei.cn/gtahokvour.html

Ruby: arr.uniq
来源：http://hz.shuidangran.top/gtoprphxwq.html

C#:   list.Distinct().ToList()
来源：http://hz.zhengqikj.top/gtiuxqgddj.html

[D16] 求和与平均值
来源：http://hz.snrcjt.cn/gtdkihtqmv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.zhoulong.xyz/gtrmsrfdmz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.wangshuangyany.cn/gtlbbbyoqg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jqgfzy.top/gtqttvnkii.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.smart0.xyz/gtgbazohne.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.pengpengdd.cyou/gtbjlgpzth.html

Go:   // 手写循环累加
来源：http://hz.feifeiyinyue.top/gtajazbtnu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.sufxvd.cn/gtxusttfko.html

C#:   list.Sum();  list.Average()
来源：http://hz.chenjidiqi.icu/gthtswzkxe.html

[D17] 最大值与最小值
来源：http://hz.nanxuanxn.top/gtrrppkxhs.html

Py:   max(arr);  min(arr)
来源：http://hz.zhoulong.xyz/gtxabrwcel.html

PHP:  max($arr);  min($arr);
来源：http://hz.gzhubu.top/gtnfewwzvf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.chenzaomai.com/gttxmtcqvw.html

TS:   Math.max(...arr);
来源：http://hz.gogol.net.cn/gtouwwyzqp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.vqdsnc.cn/gtcuyjqdjn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.wangdashe.top/gtnraubuzo.html

Ruby: arr.max;  arr.min
来源：http://hz.ppjwa.cn/gtrxdoegcs.html

C#:   list.Max();  list.Min()
来源：http://hz.hfpthk.cn/gtsksiwwjo.html

[D18] 扁平化嵌套数组
来源：http://hz.zhixingplan.top/gtrggwzzut.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.daria6918.cn/gtlvjsmaso.html

PHP:  array_merge(...$nested);
来源：http://hz.chenjidiqi.icu/gtaqusnmtr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.chenzaomai.com/gtevlvkgyb.html

TS:   nested.flat();
来源：http://hz.yj20258.top/gtfwyonsql.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.jinqigufen.top/gtnjlpbmvq.html

Go:   // 手写双层循环
来源：http://hz.yuxming.cn/gtlwtclrqs.html

Ruby: nested.flatten
来源：http://hz.jyoumei.cn/gtisgvdyze.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.tanke756.top/gtzuixalzp.html

[D19] 按字段分组
来源：http://hz.xingfuxueyuan.xyz/gtppxordhr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.zhengqikj.top/gtkiggxucu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.zhengqikj.top/gtgrobhxon.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jinqigufen.top/gttiqyxwdp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.daria6918.cn/gtluuufjgo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.sysykeji.top/gtiptdqyfb.html

Go:   // 手写 map[string][]T
来源：http://hz.jinqigfzy.top/gtjlsydfrn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.hammf.cn/gtfoakpmjd.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.smart0.xyz/gttteleukd.html

[D20] 统计每个元素出现次数
来源：http://hz.9152youxi.cn/gtthmcwxzf.html

Py:   Counter(arr)
来源：http://hz.aizwys.cn/gtefezlpnu.html

PHP:  array_count_values($arr);
来源：http://hz.jlsjyb.cn/gtmkwbzcfs.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.dianchejie.cn/gtuofvsdso.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.snrcjt.cn/gtbkmfshmb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.c1oappe.top/gtfadadfso.html

Go:   // 手写 map[T]int
来源：http://hz.yj20258888.top/gtcmbbxbes.html

Ruby: arr.tally
来源：http://hz.zhiwuduotai.top/gtwazipseh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yuxming.cn/gtfxkbznxx.html

[D21] 判断是否包含某元素
来源：http://hz.xuanzx.com/gtnbgfkfyf.html

Py:   x in arr
来源：http://hz.kuanghao11.cn/gtpyttzszx.html

PHP:  in_array($x, $arr, true);
来源：http://hz.dashuyun.cn/gtmqgihcue.html

JS:   arr.includes(x)
来源：http://hz.cashguo.top/gtjngtsmou.html

TS:   arr.includes(x)
来源：http://hz.dianchejie.cn/gtchanurle.html

Java: list.contains(x)
来源：http://hz.ywan-chungtsiang.top/gtscgzvufj.html

Go:   slices.Contains(arr, x)
来源：http://hz.ivvv.top/gtyylgwfbc.html

Ruby: arr.include?(x)
来源：http://hz.nanxuanxn.top/gtecnzbjtn.html

C#:   list.Contains(x)
来源：http://hz.fengsongda.top/gtbrkahzim.html

[D22] 复制数组（避免共享引用）
来源：http://hz.yvedp.cn/gtopvrkpte.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.cdnleiting.top/gtjftwtiar.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.hywenlv.cn/gtlbuempia.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.xylfe.cn/gthbasjxqu.html

TS:   [...arr];
来源：http://hz.smart0.xyz/gtvggpjcut.html

Java: new ArrayList<>(list);
来源：http://hz.hysaishi.cn/gtwhxwwfom.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.shuidangran.top/gtrzkpobxp.html

Ruby: arr.dup;  arr.clone
来源：http://hz.shzxlz.cn/gtupptwmyz.html

C#:   new List<int>(list);
来源：http://hz.zdqjudy.top/gtyeupdgrd.html

[D23] reduce 累积计算
来源：http://hz.andypj.xyz/gtqvqvwghi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.pengpengdd.cyou/gtanlllmif.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.xziqi.cn/gtvpjrclxu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.nanxinkj.top/gtdkgyblro.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yj20258888.top/gtuorgwhqu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.zhixingplan.top/gtxxffoiqc.html

Go:   // 手写循环
来源：http://hz.52xcode.cn/gtmkkdxggr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.yueranfly.top/gtrxsifflc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yangfankeji.com/gtvghgrtok.html

[D24] 字典 / Map 基本操作
来源：http://hz.xylfe.cn/gtkrcqhbtq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.316326.xyz/gtvxwfdyhr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.316326.xyz/gtfyadqwrl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yj20258.top/gtuworevzx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.cqqwz.cn/gtnwowowrp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.xuetiantiany.cn/gtpzoattaa.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.hywenlv.cn/gtycrpuuhr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.shanyushiyangkeji.top/gtogzviyyo.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.gaohongyu789.top/gtzhxnfubt.html

[D25] Set 集合去重与交并差
来源：http://hz.guannengcc.top/gtvclwnvza.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yuanzhike.top/gtjnpfcuay.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.ybcxt.top/gtheeqevav.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yuanzhike.top/gtzgglmheo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jinqigufen.top/gtvkqnbumy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.xylfe.cn/gtpazocxmu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.zhaomingkeji.xyz/gtycxkcmtu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.tianlin.xyz/gtrbmrnjzf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.meibo888.top/gtisadvtzf.html

[D26] 数组转字符串
来源：http://hz.yuanzhike.top/gtfmsppxtl.html

Py:   ", ".join(map(str, arr))
来源：http://hz.cdnleiting.top/gtabucodbg.html

PHP:  implode(", ", $arr);
来源：http://hz.chenlongwang.top/gtspxzmqhz.html

JS:   arr.join(", ")
来源：http://hz.pengpengdd.cyou/gtfqxgaamq.html

TS:   arr.join(", ")
来源：http://hz.nwbrower.top/gtyxwckknj.html

Java: String.join(", ", list)
来源：http://hz.sxryk.cn/gtgiksuprg.html

Go:   strings.Join(strs, ", ")
来源：http://hz.hfpthk.cn/gtantjhayk.html

Ruby: arr.join(", ")
来源：http://hz.chenlongwang.top/gtgsuhzxjb.html

C#:   string.Join(", ", list)
来源：http://hz.0kj1m.cn/gtyvtcizdl.html

================================================================================
来源：http://hz.jinqigfzy.top/gtstpwgcws.html

E. 字符串处理
来源：http://hz.52xcode.cn/gtifdyxkok.html

================================================================================
来源：http://hz.jqgfzy.top/gtlwwofila.html

[E01] 拼接字符串
来源：http://hz.xziqi.cn/gtnqnxagoj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.ppjwa.cn/gtpmrnieog.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yanxiufei.cn/gtwfoghmkt.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.kuanghao11.cn/gtanhowfnt.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.sxryk.cn/gtuchgzrzq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.cqqwz.cn/gtwwinqjzh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yangfankeji.com/gtdneompas.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.zhongyouzk.top/gtumcjvrup.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.bjfxy.top/gtdiqlflbu.html

[E02] 重复字符串
来源：http://hz.hnxiangtu.top/gtujnhadyl.html

Py:   "ab" * 3
来源：http://hz.hammf.cn/gtlkyvhwtr.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yonumen.top/gtqrphtdqb.html

JS:   "ab".repeat(3)
来源：http://hz.ehwqpu.com/gtmdultene.html

TS:   "ab".repeat(3)
来源：http://hz.jlsjyb.cn/gtyqbkcmjj.html

Java: "ab".repeat(3)
来源：http://hz.dashuyun.cn/gtekxrtduo.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.aibaodan.cn/gtmuodutdg.html

Ruby: "ab" * 3
来源：http://hz.9152youxi.cn/gtyysxbevo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.hywenlv.cn/gtqbtzlgbt.html

[E03] 截取子串
来源：http://hz.xuanzx.com/gtntillwxl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.hfpthk.cn/gtshhfacgk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zhiwuduotai.top/gtfsozerpe.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.wangdashe.top/gtoccxouog.html

TS:   s.slice(1, 4)
来源：http://hz.xuetiantiany.cn/gtlwgkxvnl.html

Java: s.substring(1, 4)
来源：http://hz.0kj1m.cn/gtrvgkdqpi.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.guannengcc.top/gtdcowoxfe.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yonumen.top/gtbguctvjs.html

C#:   s.Substring(1, 3)
来源：http://hz.shzxlz.cn/gtscidtwfs.html

[E04] 查找子串位置
来源：http://hz.yonumen.top/gtnxxnjire.html

Py:   s.find("x");  s.index("x")
来源：http://hz.guowangkeji.top/gtdmsuxsjy.html

PHP:  strpos($s, "x");
来源：http://hz.zhongyouzk.top/gtitwrohln.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.hammf.cn/gtyuybhakq.html

TS:   s.indexOf("x")
来源：http://hz.pengpengdd.cyou/gtaxlkdegl.html

Java: s.indexOf("x")
来源：http://hz.ywan-chungtsiang.top/gtvkqolrtr.html

Go:   strings.Index(s, "x")
来源：http://hz.zhoulong.xyz/gtrmareimq.html

Ruby: s.index("x")
来源：http://hz.yuxming.cn/gteegxtofs.html

C#:   s.IndexOf("x")
来源：http://hz.cashguo.top/gtsgzxcqeo.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.cashguo.top/gtdgakdtrg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.xziqi.cn/gtsgkoevdx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.feifeiyinyue.top/gtokhmsahb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jiagoushi.top/gtilhtfhsd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.wangdashe.top/gtkykfayad.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yj20258.top/gthmzqaacf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.9152youxi.cn/gtfbfovnoo.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.yueranfly.top/gttvctzkvq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jyoumei.cn/gteuvzrpuw.html

[E06] 替换子串
来源：http://hz.daxiang520.top/gtxhkynqtf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.shzxlz.cn/gtlnqotvyx.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.tian-w.cn/gtgbpbgsml.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yanxiufei.cn/gtdpmqgjxt.html

TS:   s.replaceAll("a", "b")
来源：http://hz.yongpay.top/gtaktkmusc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jianghu66.top/gtetmmkker.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.ydzc1.top/gthwnipqpk.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.vqdsnc.cn/gtoyesmvon.html

C#:   s.Replace("a", "b")
来源：http://hz.zdqjudy.top/gtyewxdkpb.html

[E07] 按分隔符拆分
来源：http://hz.0kj1m.cn/gthoksenmw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.gogol.net.cn/gtvqblbtba.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.jinqigufen.top/gtxkwgrynx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yonumen.top/gtadyrgfbz.html

TS:   s.split(",")
来源：http://hz.ybcxt.top/gtkuxpqzna.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.zhongyouzk.top/gtawpsydwp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.sysykeji.top/gtjpzshtuk.html

Ruby: s.split(",");  s.split
来源：http://hz.shuidangran.top/gtxzscramk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.pycfn.com/gtpizucehl.html

[E08] 数组按分隔符合并
来源：http://hz.sweek.top/gtqqxadjcj.html

Py:   ",".join(items)
来源：http://hz.zhoulong.xyz/gtjlygepho.html

PHP:  implode(",", $items);
来源：http://hz.daxiang520.top/gtbmmnqsom.html

JS:   items.join(",")
来源：http://hz.kuanghao11.cn/gtokimulja.html

TS:   items.join(",")
来源：http://hz.jqgufenzy.top/gthbtqhmzs.html

Java: String.join(",", items)
来源：http://hz.ppjwa.cn/gtywyhjmyv.html

Go:   strings.Join(items, ",")
来源：http://hz.shzxlz.cn/gtrhjlbefu.html

Ruby: items.join(",")
来源：http://hz.ydjk.org.cn/gtpiiktxvw.html

C#:   string.Join(",", items)
来源：http://hz.yonumen.top/gtwohcvfcx.html

[E09] 去除所有空白字符
来源：http://hz.ydjk.org.cn/gttnscdmsk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.zhijiandao.cn/gtzinvpivl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.guowangkeji.top/gtopkprwzu.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.snrcjt.cn/gtonntbbnc.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.cdnleiting.top/gtnanwmpga.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.hongshengwenyu.top/gtpvlpanjo.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.ydjk.org.cn/gtwcctyaxy.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.cqqwz.cn/gtrwbdhdto.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.hammf.cn/gtzhafynso.html

[E10] 左侧补零 / 定长填充
来源：http://hz.ydzc1.top/gtpilzebqu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yvedp.cn/gtqczzaimm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.ivvv.top/gtnpgjetto.html

JS:   "7".padStart(3, "0")
来源：http://hz.nanxinkj.top/gtbzsxmskt.html

TS:   "7".padStart(3, "0")
来源：http://hz.chenzaomai.com/gtwrtfbfut.html

Java: String.format("%03d", 7)
来源：http://hz.yj20258888.top/gtcwsvfmag.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yuanzhike.top/gtuqmfkdrl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.gaohongyu789.top/gtkyceiaoh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.52xcode.cn/gtbciamkir.html

[E11] 反转字符串
来源：http://hz.tianlin.xyz/gtrgddtppx.html

Py:   s[::-1]
来源：http://hz.jinqigufen.top/gtpeyehecg.html

PHP:  strrev($s);
来源：http://hz.sufxvd.cn/gtcyucvbes.html

JS:   [...s].reverse().join("")
来源：http://hz.gotoacloud.top/gtmnccvjqg.html

TS:   [...s].reverse().join("")
来源：http://hz.svipenyu.cn/gtidgzunet.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.smart0.xyz/gtbyjvvzqm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.chenjidiqi.icu/gtzpadhfcf.html

Ruby: s.reverse
来源：http://hz.zdqjudy.top/gtrnjfwtye.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.wangshuangyany.cn/gtmryrqjgo.html

[E12] 统计某字符出现次数
来源：http://hz.hywenlv.cn/gtfvrzqwqq.html

Py:   s.count("a")
来源：http://hz.kuanghao11.cn/gtnkwsxgfn.html

PHP:  substr_count($s, "a");
来源：http://hz.ivvv.top/gthrkjkulh.html

JS:   s.split("a").length - 1
来源：http://hz.zdqjudy.top/gtldsouply.html

TS:   s.split("a").length - 1
来源：http://hz.shanyushiyangtech.top/gtwbberpku.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.andypj.xyz/gtfesrwtiq.html

Go:   strings.Count(s, "a")
来源：http://hz.andypj.xyz/gtyjkycrrr.html

Ruby: s.count("a")
来源：http://hz.wangdashe.top/gtjspuzudt.html

C#:   s.Count(c => c == 'a')
来源：http://hz.hongshengwenyu.top/gtzlmnkspa.html

[E13] 逐字符遍历
来源：http://hz.chenlongwang.top/gtnisrryyi.html

Py:   for ch in s: print(ch)
来源：http://hz.guowangkeji.top/gtyyzghwdt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.jinqigfzy.top/gtplgwnwlr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.daria6918.cn/gtchylpsfv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xuetiantiany.cn/gtmgqlanxa.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.sysykeji.top/gtqzgddvfa.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.xuetiantiany.cn/gtufwxokly.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.ivvv.top/gteiiglqke.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.hnqzz.top/gtdefljgpg.html

[E14] URL 编码与 Base64
来源：http://hz.guowangkeji.top/gtfxwqkhvk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jinqigfzy.top/gtkiwmbghb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.yvedp.cn/gtvcmwkavu.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.tianlin.xyz/gtfixzfbbs.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.zhiwuduotai.top/gtffbeshhw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.zhongyouzk.top/gtlrffazgq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.fzhhl.top/gtaemwatys.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.hysaishi.cn/gtkurblqqt.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.sweek.top/gtkkzmykvx.html

[E15] HTML 转义 / 反转义
来源：http://hz.zhoulong.xyz/gtpcimofmz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.shuidangran.top/gtbiiqpfwe.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.chenjidiqi.icu/gtofgivdhp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.iojbl.cn/gtfjdsvosn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.shuidangran.top/gtmtfnflzu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.dianchejie.cn/gtctvgvxph.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.pycfn.com/gtopkkycfu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.9152youxi.cn/gtvpkbjijm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.tian-w.cn/gtxhawzrst.html

[E16] 数字千分位
来源：http://hz.kuanghao11.cn/gtwqgxcvzd.html

Py:   f"{1234567:,}"
来源：http://hz.shanyushiyangtech.top/gthviltlkw.html

PHP:  number_format(1234567);
来源：http://hz.hammf.cn/gtszxykunc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.xziqi.cn/gtomwxpxws.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jqgufenzy.top/gttmahtrex.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.zhiwuduotai.top/gthiiiehmd.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yj202588.top/gtcqvktnri.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.tianlin.xyz/gtttzuxemg.html

C#:   1234567.ToString("N0")
来源：http://hz.gzhubu.top/gtyynjjptd.html

[E17] 首字母大写
来源：http://hz.shuidangran.top/gtzzlsznvd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.hnxiangtu.top/gtbhdbtvtt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.nanxinkj.top/gtmgjocseq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.chenlongwang.top/gtomzpvqnv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.snrcjt.cn/gtexyknwbv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.yangfankeji.com/gtwmafoety.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.redwolf501.top/gtcjgbdmyf.html

Ruby: s.capitalize
来源：http://hz.yongpay.top/gtdvofsrpg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.pengpengdd.cyou/gtyamcebfp.html

[E18] 模板占位符替换
来源：http://hz.andypj.xyz/gtwvsourgy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.zycfv.cn/gtpclcqhmm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.ppjwa.cn/gtaiegkrea.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.sxryk.cn/gtcnofgldv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhaomingkeji.xyz/gtiyfaqcpu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.tanke756.top/gtixhsaezb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.xingfuxueyuan.xyz/gtfvgzcxms.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.chenjidiqi.icu/gtwtenwtsz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.cdnleiting.top/gtblznscin.html

[E19] 多行文本按行拆分
来源：http://hz.meibo888.top/gtzgigqcxv.html

Py:   s.splitlines()
来源：http://hz.xuanzx.com/gttnivpdjy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.nanxuanxn.top/gtwntjsdrz.html

JS:   s.split(/\r?\n/)
来源：http://hz.xuetiantiany.cn/gtjeuezwcn.html

TS:   s.split(/\r?\n/)
来源：http://hz.gotoacloud.top/gthzyzwhzi.html

Java: s.lines().toList()
来源：http://hz.ivvv.top/gtsqsfoyay.html

Go:   strings.Split(s, "\n")
来源：http://hz.jinqigufen.top/gtugbhzepa.html

Ruby: s.lines
来源：http://hz.ybcxt.top/gtgnvmzwkk.html

C#:   s.Split('\n')
来源：http://hz.jinqigufen.top/gtqnzhjzye.html

[E20] 判断字符串是否为空
来源：http://hz.sysykeji.top/gtaokpienx.html

Py:   if not s:
来源：http://hz.zdqjudy.top/gtieadtins.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.316326.xyz/gtkdpksawq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.wangdashe.top/gtjsmwpngu.html

TS:   if (s === "") {}
来源：http://hz.pengpengdd.cyou/gtdmzmntfz.html

Java: if (s.isEmpty()) {}
来源：http://hz.ydjk.org.cn/gthnzifpao.html

Go:   if s == "" {}
来源：http://hz.nwbrower.top/gtpdcnadwm.html

Ruby: if s.empty?
来源：http://hz.jinqigfzy.top/gthkiicfnb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.yj20258888.top/gtcdimjbfa.html

[E21] 超长截断加省略号
来源：http://hz.shanyushiyangkeji.top/gtsrnlkmnd.html


<!-- 参考信息 -->