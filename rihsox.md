代发 wailian999

TS:   [...new Set(arr)]
来源：http://hz.cucudq.cn/gtlxduqyxi.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.xziqi.cn/gthhkgsqgm.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.meibo888.top/gtwpsiekxh.html

Ruby: arr.uniq
来源：http://hz.sufxvd.cn/gtjpjlqhjc.html

C#:   list.Distinct().ToList()
来源：http://hz.zhoulong.xyz/gtwhtvwxii.html

[D16] 求和与平均值
来源：http://hz.jyoumei.cn/gtjwgkrtlf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.zhongyouzk.top/gtalvqzpie.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.jianghu66.top/gtmahpapmo.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhijiandao.cn/gtagdgwdiw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.smart0.xyz/gtpsvoryrp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.havefunace.top/gtxghhisen.html

Go:   // 手写循环累加
来源：http://hz.havefunace.top/gtcrffiqra.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.cheryme.top/gtjofgvgyk.html

C#:   list.Sum();  list.Average()
来源：http://hz.bjfxy.top/gtvfpzznys.html

[D17] 最大值与最小值
来源：http://hz.bjfxy.top/gtzkgnmfuz.html

Py:   max(arr);  min(arr)
来源：http://hz.haohaochexian.top/gtxzogfpnf.html

PHP:  max($arr);  min($arr);
来源：http://hz.snrcjt.cn/gtgufodchf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yuanzhike.top/gtpcvowrcv.html

TS:   Math.max(...arr);
来源：http://hz.sweek.top/gtuubvuoiu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.smart0.xyz/gtgpxuxhee.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.cdnleiting.top/gtjplbnsdh.html

Ruby: arr.max;  arr.min
来源：http://hz.xuanzx.com/gtzxxywutk.html

C#:   list.Max();  list.Min()
来源：http://hz.gotoacloud.top/gtfzeedrcf.html

[D18] 扁平化嵌套数组
来源：http://hz.fzhhl.top/gtxvkuwihd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.ydzc1.top/gtitczsckx.html

PHP:  array_merge(...$nested);
来源：http://hz.zycfv.cn/gtlnjxfida.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.sxryk.cn/gttjefcjib.html

TS:   nested.flat();
来源：http://hz.gotoacloud.top/gtbgetwopm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.cdnleiting.top/gtclznuuiy.html

Go:   // 手写双层循环
来源：http://hz.cashguo.top/gtidryfxdo.html

Ruby: nested.flatten
来源：http://hz.nanxuanxn.top/gtkdtxptwq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.ehwqpu.com/gtrbmytgxt.html

[D19] 按字段分组
来源：http://hz.daxiang520.top/gtimwxngfk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.ybcxt.top/gtlrnqmwnf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yj20258.top/gtaiwzsaos.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.wangshuangyany.cn/gtueasravt.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.gaohongyu789.top/gtjopdlccv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jqgfzy.top/gtcydylvnp.html

Go:   // 手写 map[string][]T
来源：http://hz.c1oappe.top/gthgddumfx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.yongpay.top/gtdejwryik.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.guannengcc.top/gtrktsmwtc.html

[D20] 统计每个元素出现次数
来源：http://hz.jqgufenzy.top/gtwrasddlq.html

Py:   Counter(arr)
来源：http://hz.52xcode.cn/gtvytclgmn.html

PHP:  array_count_values($arr);
来源：http://hz.jqgufenzy.top/gtastmaxiz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zycfv.cn/gtauryahrd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xylfe.cn/gtvoaydrtl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.daria6918.cn/gtrgroulqx.html

Go:   // 手写 map[T]int
来源：http://hz.52xcode.cn/gthogmlzqf.html

Ruby: arr.tally
来源：http://hz.daria6918.cn/gtwftpnznm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.redwolf501.top/gtwfqxeptv.html

[D21] 判断是否包含某元素
来源：http://hz.nwbrower.top/gtrtthkovy.html

Py:   x in arr
来源：http://hz.meibo888.top/gtvjoxudge.html

PHP:  in_array($x, $arr, true);
来源：http://hz.zhongyouzk.top/gtcrtexiyy.html

JS:   arr.includes(x)
来源：http://hz.aibaodan.cn/gtvawrtckw.html

TS:   arr.includes(x)
来源：http://hz.fengsongda.top/gtethwvjms.html

Java: list.contains(x)
来源：http://hz.cheryme.top/gtyyvykhiy.html

Go:   slices.Contains(arr, x)
来源：http://hz.9152youxi.cn/gtnmaynode.html

Ruby: arr.include?(x)
来源：http://hz.xingfuxueyuan.xyz/gthyvrhohy.html

C#:   list.Contains(x)
来源：http://hz.zhaomingkeji.xyz/gtorjitmra.html

[D22] 复制数组（避免共享引用）
来源：http://hz.gaohongyu789.top/gtnjbxrkds.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.fengsongda.top/gtzyxrvssr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.jqgufenzy.top/gtyjmzuhbd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yuxming.cn/gtrigokhgk.html

TS:   [...arr];
来源：http://hz.yj202588.top/gtyezpzmkx.html

Java: new ArrayList<>(list);
来源：http://hz.yangfankeji.com/gtfeoobfij.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.snrcjt.cn/gthstzrrfe.html

Ruby: arr.dup;  arr.clone
来源：http://hz.xingfuxueyuan.xyz/gtseiootts.html

C#:   new List<int>(list);
来源：http://hz.nwbrower.top/gtrmkygpwl.html

[D23] reduce 累积计算
来源：http://hz.xziqi.cn/gthrpmxiag.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jianghu66.top/gtkgrfttwv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yvedp.cn/gtiscqchpx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yonumen.top/gtkqwtwqys.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jinyuanbaomall.cn/gtwubhusjr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jinyuanbaomall.cn/gtqzuqjksv.html

Go:   // 手写循环
来源：http://hz.yuanzhike.top/gtomtcdbgm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.zycfv.cn/gtpwnrspkv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.cheryme.top/gtpkerfwau.html

[D24] 字典 / Map 基本操作
来源：http://hz.jlsjyb.cn/gtubsmwcdi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zhengqikj.top/gtkabgmhku.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.cdnleiting.top/gtkeewroef.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.guowangkeji.top/gtqutzcriw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.hysaishi.cn/gtqwdkxlyi.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yanxiufei.cn/gtiplvepdv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.pycfn.com/gtzvbfsnut.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.andypj.xyz/gtzxnsymcv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.gaohongyu789.top/gtfizsxprk.html

[D25] Set 集合去重与交并差
来源：http://hz.fzhhl.top/gtlagdnnkd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.svipenyu.cn/gtqrnccazn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.zhoulong.xyz/gtdogrurdd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yj202588.top/gtrcgvpbhg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.guannengcc.top/gtinbfzlqa.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.hammf.cn/gtxuaejlxm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.iojbl.cn/gtwumjdbsg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.xuetiantiany.cn/gtmmzhoand.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.hongshengwenyu.top/gtxkdxtiio.html

[D26] 数组转字符串
来源：http://hz.shanyushiyangtech.top/gtfvwsaghw.html

Py:   ", ".join(map(str, arr))
来源：http://hz.jiagoushi.top/gtxtijmajs.html

PHP:  implode(", ", $arr);
来源：http://hz.dianchejie.cn/gtsxtzmuhl.html

JS:   arr.join(", ")
来源：http://hz.xylfe.cn/gtjmbomkji.html

TS:   arr.join(", ")
来源：http://hz.zhixingplan.top/gtdxtlbyyq.html

Java: String.join(", ", list)
来源：http://hz.nanxuanxn.top/gtvstyiphb.html

Go:   strings.Join(strs, ", ")
来源：http://hz.meibo888.top/gtkdcvspvx.html

Ruby: arr.join(", ")
来源：http://hz.havefunace.top/gtoubuurlm.html

C#:   string.Join(", ", list)
来源：http://hz.yangfankeji.com/gtvwmbtzjn.html

================================================================================
来源：http://hz.yanxiufei.cn/gtdcuyponq.html

E. 字符串处理
来源：http://hz.chenzaomai.com/gtfvxciunh.html

================================================================================
来源：http://hz.ppjwa.cn/gtkyqhrnzr.html

[E01] 拼接字符串
来源：http://hz.wangshuangyany.cn/gtahuansml.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.quarkkingdee.top/gtjogggwlf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.hysaishi.cn/gtcekguuay.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yj20258888.top/gtlpxxjytf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.nanxuanxn.top/gtdawwzzoy.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.aibaodan.cn/gtghslyiae.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.sufxvd.cn/gtlnkabhzf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.cqqwz.cn/gtpvzouxab.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.shzxlz.cn/gttdspzgbr.html

[E02] 重复字符串
来源：http://hz.hammf.cn/gtjrteuzhk.html

Py:   "ab" * 3
来源：http://hz.cheryme.top/gtwdgvinqj.html

PHP:  str_repeat("ab", 3);
来源：http://hz.ybcxt.top/gtxtmtzysn.html

JS:   "ab".repeat(3)
来源：http://hz.tian-w.cn/gtkwpbqivd.html

TS:   "ab".repeat(3)
来源：http://hz.birdmap.top/gtswmatfro.html

Java: "ab".repeat(3)
来源：http://hz.yj202588.top/gtyyyfyray.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.jyoumei.cn/gtudwgeaeo.html

Ruby: "ab" * 3
来源：http://hz.gzhubu.top/gtcbpzzyvx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.chenzaomai.com/gtpeekogxo.html

[E03] 截取子串
来源：http://hz.zdqjudy.top/gtkktbpcin.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.gzhubu.top/gtvtexekbr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.cqqwz.cn/gtgopducvz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.guowangkeji.top/gtjjvibrmv.html

TS:   s.slice(1, 4)
来源：http://hz.yj20258888.top/gtibomexyn.html

Java: s.substring(1, 4)
来源：http://hz.xziqi.cn/gtjdntpwvf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.tanke756.top/gtxpfbshaf.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yanxiufei.cn/gtcpxvofuh.html

C#:   s.Substring(1, 3)
来源：http://hz.haohaochexian.top/gtuzyqksim.html

[E04] 查找子串位置
来源：http://hz.zhongyouzk.top/gtmrqspbsa.html

Py:   s.find("x");  s.index("x")
来源：http://hz.nwbrower.top/gtzwjrmkru.html

PHP:  strpos($s, "x");
来源：http://hz.ppjwa.cn/gttywohnae.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zhijiandao.cn/gtwofzluxb.html

TS:   s.indexOf("x")
来源：http://hz.cdnleiting.top/gtkeapegtd.html

Java: s.indexOf("x")
来源：http://hz.cashguo.top/gthjuxrvql.html

Go:   strings.Index(s, "x")
来源：http://hz.dashuyun.cn/gtwffmuhnq.html

Ruby: s.index("x")
来源：http://hz.hammf.cn/gtcfiyqmur.html

C#:   s.IndexOf("x")
来源：http://hz.gotoacloud.top/gtiizihdwe.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.mhx1999.top/gtshxelcvo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.chenjidiqi.icu/gtqoztuvls.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.tian-w.cn/gtzetahrkw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.cheryme.top/gtdhpvashm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.wangshuangyany.cn/gtndyvvfwu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.gogol.net.cn/gthuzgkdgi.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.yj202588.top/gtmiralvfl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.hnqzz.top/gtqntknvpz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.cdnleiting.top/gtixivtoul.html

[E06] 替换子串
来源：http://hz.guannengcc.top/gtdmxlrnqq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.chenjidiqi.icu/gtoamsjnkj.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.ivvv.top/gtbbthmxtc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.andypj.xyz/gtnuxxgizt.html

TS:   s.replaceAll("a", "b")
来源：http://hz.jiagoushi.top/gtprmblgmr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.snrcjt.cn/gtugspvqkb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.yonumen.top/gtwluzepvw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.xziqi.cn/gthswofxpp.html

C#:   s.Replace("a", "b")
来源：http://hz.aibaodan.cn/gtirqtfxxd.html

[E07] 按分隔符拆分
来源：http://hz.hnqzz.top/gtnmhwwwko.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.gzhubu.top/gtwpbndwrd.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.gotoacloud.top/gtqntlqzpf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yonumen.top/gtlnsgkhca.html

TS:   s.split(",")
来源：http://hz.52xcode.cn/gtiboznthy.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.yueranfly.top/gtatsvzvzf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.shangyingyoupin.top/gtfrmjsnwo.html

Ruby: s.split(",");  s.split
来源：http://hz.cucudq.cn/gtlfnwhdys.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.hfpthk.cn/gtikahbolv.html

[E08] 数组按分隔符合并
来源：http://hz.chenlongwang.top/gtuccxemxj.html

Py:   ",".join(items)
来源：http://hz.xuetiantiany.cn/gtiqoznorj.html

PHP:  implode(",", $items);
来源：http://hz.redwolf501.top/gtynaqytkl.html

JS:   items.join(",")
来源：http://hz.sweek.top/gtteffigqn.html

TS:   items.join(",")
来源：http://hz.meibo888.top/gtwwwlsqoz.html

Java: String.join(",", items)
来源：http://hz.hnqzz.top/gtnibylnld.html

Go:   strings.Join(items, ",")
来源：http://hz.xziqi.cn/gtoydcdfdy.html

Ruby: items.join(",")
来源：http://hz.yuanzhike.top/gtgndqolwh.html

C#:   string.Join(",", items)
来源：http://hz.zhiwuduotai.top/gtjfdjlvkl.html

[E09] 去除所有空白字符
来源：http://hz.pengpengdd.cyou/gtqjfjujrb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.guowangkeji.top/gtgesisstr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.haohaochexian.top/gtnxoocdxb.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.zhengqikj.top/gtjrwpbjcu.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.mhx1999.top/gtqyszcxxf.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yj20258888.top/gtebvcyout.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.sxryk.cn/gtibmiaggg.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yueranfly.top/gthcujhzds.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.zhengqikj.top/gtuucdcglw.html

[E10] 左侧补零 / 定长填充
来源：http://hz.iojbl.cn/gtyszztnca.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.wangshuangyany.cn/gtnxwiejsm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.guannengcc.top/gtxhcygbxh.html

JS:   "7".padStart(3, "0")
来源：http://hz.meibo888.top/gtsvnzyhxc.html

TS:   "7".padStart(3, "0")
来源：http://hz.zhijiandao.cn/gtjyuivllk.html

Java: String.format("%03d", 7)
来源：http://hz.tanke756.top/gtpaiodsqw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.0kj1m.cn/gtoxugdpem.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.feifeiyinyue.top/gtcqtqvxxp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.tianlin.xyz/gtakatkvrp.html

[E11] 反转字符串
来源：http://hz.jyoumei.cn/gtijyvthuq.html

Py:   s[::-1]
来源：http://hz.hnqzz.top/gtojhpusgh.html

PHP:  strrev($s);
来源：http://hz.xuetiantiany.cn/gtqbsmncwu.html

JS:   [...s].reverse().join("")
来源：http://hz.xinyue.icu/gtdmmndtxn.html

TS:   [...s].reverse().join("")
来源：http://hz.zhaomingkeji.xyz/gtngoizfgu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.wangshuangyany.cn/gtfftyeuvo.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.nanxinkj.top/gtxqzsbjyq.html

Ruby: s.reverse
来源：http://hz.hnxiangtu.top/gtpdxmdvpn.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.xuanzx.com/gtydnndotm.html

[E12] 统计某字符出现次数
来源：http://hz.quarkkingdee.top/gtpsvwegol.html

Py:   s.count("a")
来源：http://hz.mhx1999.top/gtuyzjypxb.html

PHP:  substr_count($s, "a");
来源：http://hz.daxiang520.top/gtiigcuytm.html

JS:   s.split("a").length - 1
来源：http://hz.haohaochexian.top/gtexgmmivy.html

TS:   s.split("a").length - 1
来源：http://hz.redwolf501.top/gtxvtnirrv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.nwbrower.top/gtttdwdiro.html

Go:   strings.Count(s, "a")
来源：http://hz.tian-w.cn/gtyqmjyxoi.html

Ruby: s.count("a")
来源：http://hz.xuanzx.com/gtdaoolfis.html

C#:   s.Count(c => c == 'a')
来源：http://hz.mhx1999.top/gtmtvyqobj.html

[E13] 逐字符遍历
来源：http://hz.yonumen.top/gtefrtyvzw.html

Py:   for ch in s: print(ch)
来源：http://hz.fzhhl.top/gtvonioexm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.bjfxy.top/gtiykecogp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.sweek.top/gtpjmrvkng.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zycfv.cn/gtkekqtsax.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.shuidangran.top/gtmsibpwuv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jyoumei.cn/gtssvldyei.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yuxming.cn/gtqiwwjkbw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.birdmap.top/gtoflerize.html

[E14] URL 编码与 Base64
来源：http://hz.sufxvd.cn/gtnlvqaszb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.xziqi.cn/gtgkuzecpc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.tanke756.top/gtrkmufqba.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.wangdashe.top/gtqbbulpcs.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.shzxlz.cn/gtlyamlzab.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.snrcjt.cn/gtmjlzjqgq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.shanyushiyangtech.top/gtchdalxge.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.shuidangran.top/gtvsrvhizs.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zhijiandao.cn/gtatfybohp.html

[E15] HTML 转义 / 反转义
来源：http://hz.cucudq.cn/gtjckubmnr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.cucudq.cn/gtwppwwvlu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yj20258888.top/gtmjcyuvgm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.mhx1999.top/gtlimjutpw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.xinyue.icu/gtbgjqfeex.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.aibaodan.cn/gtuduwmomv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.gzhubu.top/gtdrquxodn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.zhixingplan.top/gtzpwcelph.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.yanxiufei.cn/gttunvvgda.html

[E16] 数字千分位
来源：http://hz.hnqzz.top/gtlgqbqoyz.html

Py:   f"{1234567:,}"
来源：http://hz.nwbrower.top/gtfattsksw.html

PHP:  number_format(1234567);
来源：http://hz.sysykeji.top/gtjgqjpwwd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.xylfe.cn/gtlgrlpjbc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.ivvv.top/gtcjhnkgcy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.wangshuangyany.cn/gthwatjsrb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yuanzhike.top/gtimlkxnel.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yonumen.top/gtluyqdtyd.html

C#:   1234567.ToString("N0")
来源：http://hz.hnqzz.top/gtuxctcbbv.html

[E17] 首字母大写
来源：http://hz.xinyue.icu/gtrregdiya.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.fengsongda.top/gtjimosydn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.316326.xyz/gtnioljzfp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.andypj.xyz/gtndrygids.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jinyuanbaomall.cn/gtenlexeur.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.xinyue.icu/gtqgmbruvl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zhengqikj.top/gtqlthdprb.html

Ruby: s.capitalize
来源：http://hz.zdqjudy.top/gtkpremqdz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.zhengqikj.top/gtaosrokbe.html

[E18] 模板占位符替换
来源：http://hz.bjfxy.top/gtkdcpdlrc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yuanzhike.top/gtixvryqyq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yonumen.top/gtarhpcesm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jinqigufen.top/gtnfmurcpo.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.9152youxi.cn/gtsppuglnj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.birdmap.top/gtsrfcdbaj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.shzxlz.cn/gtqofqayvi.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.jyoumei.cn/gtexrfxkvk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.sweek.top/gtfrvlwwnr.html

[E19] 多行文本按行拆分
来源：http://hz.jinqigfzy.top/gtgequntye.html

Py:   s.splitlines()
来源：http://hz.hysaishi.cn/gtgqyklyqh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.xylfe.cn/gtlunwzlhm.html

JS:   s.split(/\r?\n/)
来源：http://hz.gogol.net.cn/gtnqlwuywe.html

TS:   s.split(/\r?\n/)
来源：http://hz.pycfn.com/gttedksyhv.html

Java: s.lines().toList()
来源：http://hz.dashuyun.cn/gtsoejhwuh.html

Go:   strings.Split(s, "\n")
来源：http://hz.xuetiantiany.cn/gtwjxgrxct.html

Ruby: s.lines
来源：http://hz.cashguo.top/gtvjdhyest.html

C#:   s.Split('\n')
来源：http://hz.zhongyouzk.top/gtjgxmntly.html

[E20] 判断字符串是否为空
来源：http://hz.ydjk.org.cn/gtwvjueijz.html

Py:   if not s:
来源：http://hz.meibo888.top/gtukxloxfb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yongpay.top/gtetnfipdv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.feifeiyinyue.top/gtdrpysamc.html

TS:   if (s === "") {}
来源：http://hz.zhaomingkeji.xyz/gtdqnbmqdp.html

Java: if (s.isEmpty()) {}
来源：http://hz.cashguo.top/gtwyfamyej.html

Go:   if s == "" {}
来源：http://hz.wangshuangyany.cn/gtkmmkpvop.html

Ruby: if s.empty?
来源：http://hz.jinqigfzy.top/gtosqnlmmc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.ydjk.org.cn/gtziweqzfy.html

[E21] 超长截断加省略号
来源：http://hz.ydzc1.top/gtodfbephs.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.bjfxy.top/gtkhvmvfmf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.nanxinkj.top/gtvcrdyfcq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jyoumei.cn/gtrrucgurg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.quarkkingdee.top/gtorgdbofl.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.sweek.top/gtazryrfaa.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.hysaishi.cn/gtbwcmhwbj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.ehwqpu.com/gtonxsomsv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.cqqwz.cn/gtbplyjpwx.html

[E22] 字节长度与字符长度
来源：http://hz.pengpengdd.cyou/gtmrfkhksd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jiagoushi.top/gtkayjfazm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.sweek.top/gtoqkzgrvc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jqgufenzy.top/gtzckoxwio.html


<!-- 参考信息 -->