代发 wailian999

PHP:  sort($arr);
来源：http://hz.0kj1m.cn/gtbzbxrevf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.ppjwa.cn/gtuuxyusun.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.pengpengdd.cyou/gtqyaeqaua.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.52xcode.cn/gtlyaxklpd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.gzhubu.top/gtfxqhpnrm.html

Ruby: arr.sort
来源：http://hz.shanyushiyangkeji.top/gtkqialikm.html

C#:   list.Sort();
来源：http://hz.cqqwz.cn/gtlwjehvuv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.aibaodan.cn/gtofjrtwjc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yongpay.top/gtvuymqamx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yuxming.cn/gtjmwjbcec.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.gzhubu.top/gttqaeqmgx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.meibo888.top/gtazikvyep.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.shangyingyoupin.top/gtwpxgkujd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yj202588.top/gtuvxbsyqy.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.aibaodan.cn/gtnquihmsn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.pycfn.com/gtcvacrtms.html

[D11] 反转数组
来源：http://hz.jqgfzy.top/gtvujzymdt.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.aizwys.cn/gtdoarsqdr.html

PHP:  array_reverse($arr);
来源：http://hz.zhongyouzk.top/gteydfuage.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.tianlin.xyz/gtpjvmocck.html

TS:   [...arr].reverse();
来源：http://hz.guowangkeji.top/gtblopellb.html

Java: Collections.reverse(list);
来源：http://hz.yuanzhike.top/gtdawzjcfx.html

Go:   slices.Reverse(arr)
来源：http://hz.jqgfzy.top/gthtynulcq.html

Ruby: arr.reverse
来源：http://hz.xuanzx.com/gtekeqvwrc.html

C#:   list.Reverse();
来源：http://hz.hfpthk.cn/gtqiagoccu.html

[D12] 查找元素下标
来源：http://hz.jqgfzy.top/gtelclectj.html

Py:   arr.index(x);  x in arr
来源：http://hz.0kj1m.cn/gtdcuaajfz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.zhaomingkeji.xyz/gtvpjikeux.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.daria6918.cn/gtkmouopum.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yj20258.top/gtkgghmknv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.xingfuxueyuan.xyz/gtatykedsu.html

Go:   slices.Index(arr, x)
来源：http://hz.hammf.cn/gtctrydjrv.html

Ruby: arr.index(x)
来源：http://hz.fengsongda.top/gtcvyulxuv.html

C#:   list.IndexOf(x);
来源：http://hz.zhaomingkeji.xyz/gtclctaplq.html

[D13] 过滤（保留满足条件的）
来源：http://hz.ydjk.org.cn/gthkuepvso.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.hfpthk.cn/gtkljnlxzy.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.sxryk.cn/gtcaqbqhdh.html

JS:   arr.filter(x => x > 3)
来源：http://hz.yongpay.top/gteevhlagr.html

TS:   arr.filter(x => x > 3)
来源：http://hz.wangshuangyany.cn/gtxdpakzri.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.tian-w.cn/gtewppgylv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.mhx1999.top/gtyjpvopxf.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.xylfe.cn/gtndpbizrr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jyoumei.cn/gtxcrfhpyx.html

[D14] 映射转换（每个元素变形）
来源：http://hz.mhx1999.top/gtduzvycpw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.fzhhl.top/gtyicilxak.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.gotoacloud.top/gtlhsszbvt.html

JS:   arr.map(x => x * 2)
来源：http://hz.zycfv.cn/gttynhocba.html

TS:   arr.map(x => x * 2)
来源：http://hz.316326.xyz/gtjftzguhj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jqgfzy.top/gtfgjrhoub.html

Go:   // 手写循环
来源：http://hz.xuanzx.com/gtzoaxyaft.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.hfpthk.cn/gtuouicpeq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.zhixingplan.top/gtsnhjrtgd.html

[D15] 去重
来源：http://hz.ivvv.top/gtjohuotba.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.zhixingplan.top/gtwdqdgfpx.html

PHP:  array_unique($arr);
来源：http://hz.gogol.net.cn/gtjlmivbgs.html

JS:   [...new Set(arr)]
来源：http://hz.gogol.net.cn/gtdftrqljn.html

TS:   [...new Set(arr)]
来源：http://hz.zhiwuduotai.top/gtgergpvwl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.daxiang520.top/gtepeynwer.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.ivvv.top/gtptjgcfgp.html

Ruby: arr.uniq
来源：http://hz.andypj.xyz/gtlpembmui.html

C#:   list.Distinct().ToList()
来源：http://hz.jinqigfzy.top/gtttsvoncn.html

[D16] 求和与平均值
来源：http://hz.ybcxt.top/gtdkxlpiix.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.havefunace.top/gtothedvrl.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yongpay.top/gtjzhrrbff.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xingfuxueyuan.xyz/gtyisngsbb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.aibaodan.cn/gtherketse.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.kuanghao11.cn/gtbanrpfip.html

Go:   // 手写循环累加
来源：http://hz.iojbl.cn/gtkqbdthum.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.hnqzz.top/gttnywdwdk.html

C#:   list.Sum();  list.Average()
来源：http://hz.yj20258.top/gtuldpjfmn.html

[D17] 最大值与最小值
来源：http://hz.tianlin.xyz/gtxrmprizj.html

Py:   max(arr);  min(arr)
来源：http://hz.dianchejie.cn/gtirrnosen.html

PHP:  max($arr);  min($arr);
来源：http://hz.cheryme.top/gtziqtfhao.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.jyoumei.cn/gtrrnohlpj.html

TS:   Math.max(...arr);
来源：http://hz.shzxlz.cn/gtysfgrosb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.ywan-chungtsiang.top/gtkttbbltu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.gaohongyu789.top/gtytlvifmd.html

Ruby: arr.max;  arr.min
来源：http://hz.yongpay.top/gtkhrqpaxl.html

C#:   list.Max();  list.Min()
来源：http://hz.havefunace.top/gtknlhnymj.html

[D18] 扁平化嵌套数组
来源：http://hz.gaohongyu789.top/gtmelktjvb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zhiwuduotai.top/gtyqhshkkj.html

PHP:  array_merge(...$nested);
来源：http://hz.yvedp.cn/gtpllqlzeu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.gogol.net.cn/gtnwvwhqst.html

TS:   nested.flat();
来源：http://hz.cheryme.top/gtfgbpgmmi.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.zdqjudy.top/gtcxtiblml.html

Go:   // 手写双层循环
来源：http://hz.jqgfzy.top/gtdtauckut.html

Ruby: nested.flatten
来源：http://hz.ydjk.org.cn/gtoegkzhbz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.pycfn.com/gtesqawcrh.html

[D19] 按字段分组
来源：http://hz.hnxiangtu.top/gtdfkqcvtc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.shanyushiyangtech.top/gtkmivmhjt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.hongshengwenyu.top/gtdbhisinl.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.zhongyouzk.top/gtmzbrncvq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.chenjidiqi.icu/gtdipfofxf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yanxiufei.cn/gtohiqspbd.html

Go:   // 手写 map[string][]T
来源：http://hz.aizwys.cn/gtblgvxgrv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.jiagoushi.top/gtnlqxarhv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.9152youxi.cn/gtcugyvoya.html

[D20] 统计每个元素出现次数
来源：http://hz.ivvv.top/gtarehliuk.html

Py:   Counter(arr)
来源：http://hz.yueranfly.top/gtgyamdrdh.html

PHP:  array_count_values($arr);
来源：http://hz.daria6918.cn/gtgvovhyxa.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jqgfzy.top/gtdhgdpuzw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.sysykeji.top/gtpctzlapk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.xingfuxueyuan.xyz/gtdmhqtmbf.html

Go:   // 手写 map[T]int
来源：http://hz.ybcxt.top/gtkeoaznsl.html

Ruby: arr.tally
来源：http://hz.zhongyouzk.top/gtwkscarpf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.ehwqpu.com/gtiifsycjk.html

[D21] 判断是否包含某元素
来源：http://hz.jqgfzy.top/gttttnaghg.html

Py:   x in arr
来源：http://hz.aizwys.cn/gtxpkflzxc.html

PHP:  in_array($x, $arr, true);
来源：http://hz.zhoulong.xyz/gtyhsmfdig.html

JS:   arr.includes(x)
来源：http://hz.ybcxt.top/gterkaqohh.html

TS:   arr.includes(x)
来源：http://hz.tian-w.cn/gtmznwhpmp.html

Java: list.contains(x)
来源：http://hz.yangfankeji.com/gtuzbmefet.html

Go:   slices.Contains(arr, x)
来源：http://hz.yj20258888.top/gthjlzooxq.html

Ruby: arr.include?(x)
来源：http://hz.hfpthk.cn/gtejpdpxjc.html

C#:   list.Contains(x)
来源：http://hz.xziqi.cn/gtaawixcsm.html

[D22] 复制数组（避免共享引用）
来源：http://hz.aibaodan.cn/gtiqfnrpme.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.hysaishi.cn/gtvyyzsdbt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.aibaodan.cn/gttbcvlfsj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.wangdashe.top/gtuquwaaqj.html

TS:   [...arr];
来源：http://hz.zhoulong.xyz/gtiuvxacli.html

Java: new ArrayList<>(list);
来源：http://hz.yuxming.cn/gtbjzvsqet.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.tian-w.cn/gtsegdcnfb.html

Ruby: arr.dup;  arr.clone
来源：http://hz.hammf.cn/gtxnnafzei.html

C#:   new List<int>(list);
来源：http://hz.ivvv.top/gtghwdhkqh.html

[D23] reduce 累积计算
来源：http://hz.zhiwuduotai.top/gtouuajezd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.sweek.top/gtuiwuktze.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.ydzc1.top/gtrosbeilv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jyoumei.cn/gtvvyvlshv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.guannengcc.top/gtebwdcmjx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.mhx1999.top/gtffwuzgmq.html

Go:   // 手写循环
来源：http://hz.kuanghao11.cn/gtxwitojar.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.andypj.xyz/gtdokgglef.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.gzhubu.top/gtnqmcmgkd.html

[D24] 字典 / Map 基本操作
来源：http://hz.chenlongwang.top/gtqpdbezwo.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.yonumen.top/gtwnmyrvbn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.jinqigufen.top/gtbirjbeov.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.hammf.cn/gtqovdgflm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yonumen.top/gthfpwetvg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.hysaishi.cn/gtcpugjnur.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.52xcode.cn/gtdiwbjeuw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.9152youxi.cn/gtcifghgxu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.dianchejie.cn/gtbhbdcjfy.html

[D25] Set 集合去重与交并差
来源：http://hz.zhijiandao.cn/gtfwhzurii.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zhijiandao.cn/gtpbeeyaqw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jqgufenzy.top/gtwhpqreii.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.redwolf501.top/gtlgxebgzo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.xuanzx.com/gtusxjtflf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.sysykeji.top/gtnxmbwcez.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.ppjwa.cn/gtqbvvixuy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.chenlongwang.top/gtygcjugpz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.c1oappe.top/gtgcwumhti.html

[D26] 数组转字符串
来源：http://hz.yuxming.cn/gtouuecdff.html

Py:   ", ".join(map(str, arr))
来源：http://hz.dianchejie.cn/gtjiphdrfn.html

PHP:  implode(", ", $arr);
来源：http://hz.zycfv.cn/gtgravunzw.html

JS:   arr.join(", ")
来源：http://hz.chenlongwang.top/gththpwhaz.html

TS:   arr.join(", ")
来源：http://hz.feifeiyinyue.top/gtthmpnxsa.html

Java: String.join(", ", list)
来源：http://hz.kuanghao11.cn/gtuwksujed.html

Go:   strings.Join(strs, ", ")
来源：http://hz.ivvv.top/gtodbgylkf.html

Ruby: arr.join(", ")
来源：http://hz.chenjidiqi.icu/gtwkuvstik.html

C#:   string.Join(", ", list)
来源：http://hz.haohaochexian.top/gtlvgtgaoq.html

================================================================================
来源：http://hz.jqgfzy.top/gtbrbuowbx.html

E. 字符串处理
来源：http://hz.pycfn.com/gtkrtiqffe.html

================================================================================
来源：http://hz.hnxiangtu.top/gtlxmwqzze.html

[E01] 拼接字符串
来源：http://hz.guannengcc.top/gtneoopkzn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.cdnleiting.top/gtrdgmmgum.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.havefunace.top/gtxxelwmuf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zycfv.cn/gtkngasybe.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.pengpengdd.cyou/gtmxyfgrbf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.quarkkingdee.top/gtkflctonl.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.jqgufenzy.top/gtahwtscdd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yvedp.cn/gtmurplwha.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.cdnleiting.top/gtopellyqk.html

[E02] 重复字符串
来源：http://hz.jqgfzy.top/gtadcpqndz.html

Py:   "ab" * 3
来源：http://hz.shuidangran.top/gtjvyloqoy.html

PHP:  str_repeat("ab", 3);
来源：http://hz.quarkkingdee.top/gtumexnrbr.html

JS:   "ab".repeat(3)
来源：http://hz.feifeiyinyue.top/gtzbcmhcwb.html

TS:   "ab".repeat(3)
来源：http://hz.zdqjudy.top/gtnrlviiuh.html

Java: "ab".repeat(3)
来源：http://hz.ydzc1.top/gtnzryjvxc.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.tanke756.top/gtgeaosndj.html

Ruby: "ab" * 3
来源：http://hz.52xcode.cn/gtqfgjavmo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.sxryk.cn/gtvdnmngpc.html

[E03] 截取子串
来源：http://hz.tianlin.xyz/gtjjlotulp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.guowangkeji.top/gtdxccowny.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.redwolf501.top/gtchhsrphk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jinghuilouyu.cn/gtcduxrazw.html

TS:   s.slice(1, 4)
来源：http://hz.nanxuanxn.top/gtpehuallr.html

Java: s.substring(1, 4)
来源：http://hz.c1oappe.top/gtipgntkfq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.chenjidiqi.icu/gtsuxakwkm.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.feifeiyinyue.top/gtooqluxvf.html

C#:   s.Substring(1, 3)
来源：http://hz.zhoulong.xyz/gtmtjgrgpj.html

[E04] 查找子串位置
来源：http://hz.sysykeji.top/gtruhgqmwn.html

Py:   s.find("x");  s.index("x")
来源：http://hz.hywenlv.cn/gthnhsynqp.html

PHP:  strpos($s, "x");
来源：http://hz.bjfxy.top/gtzxlchbgx.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.chenzaomai.com/gtjljzstzq.html

TS:   s.indexOf("x")
来源：http://hz.smart0.xyz/gtkkoaxzgu.html

Java: s.indexOf("x")
来源：http://hz.0kj1m.cn/gtddyvytch.html

Go:   strings.Index(s, "x")
来源：http://hz.ehwqpu.com/gtnxelxutx.html

Ruby: s.index("x")
来源：http://hz.yuxming.cn/gtjklmxarp.html

C#:   s.IndexOf("x")
来源：http://hz.ppjwa.cn/gtohheszhe.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.hywenlv.cn/gtqhhraddl.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.xziqi.cn/gtrwecpshn.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.gogol.net.cn/gtcyewnlno.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jyoumei.cn/gtzsekucez.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.ydjk.org.cn/gttzpigthk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.dianchejie.cn/gtfswhubvw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.cheryme.top/gtqtlejgzt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.hnxiangtu.top/gtlucjczin.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.sysykeji.top/gtvspxzaag.html

[E06] 替换子串
来源：http://hz.smart0.xyz/gtsgagwgky.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jianghu66.top/gtfuiozzhb.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.ywan-chungtsiang.top/gtderqgdsf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hongshengwenyu.top/gtqjgsuwhz.html

TS:   s.replaceAll("a", "b")
来源：http://hz.yangfankeji.com/gtsoxvkxck.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.9152youxi.cn/gtmesixhrx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.shuidangran.top/gtxzvtgijz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.xinyue.icu/gteclzjsvt.html

C#:   s.Replace("a", "b")
来源：http://hz.yuxming.cn/gtmlrbfuzx.html

[E07] 按分隔符拆分
来源：http://hz.ppjwa.cn/gthsyxveoo.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.shanyushiyangkeji.top/gtvawmbuzq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.tian-w.cn/gthbcrdmsp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.ydjk.org.cn/gtxswqcigq.html

TS:   s.split(",")
来源：http://hz.yj202588.top/gtmbfdwlyz.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.ydzc1.top/gtsogxflzk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.jianghu66.top/gtrryxioow.html

Ruby: s.split(",");  s.split
来源：http://hz.jlsjyb.cn/gtpvtyzbyr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.iojbl.cn/gteohunhwk.html

[E08] 数组按分隔符合并
来源：http://hz.smart0.xyz/gttrcmrrky.html

Py:   ",".join(items)
来源：http://hz.shanyushiyangtech.top/gtfjthfjgq.html

PHP:  implode(",", $items);
来源：http://hz.guowangkeji.top/gtetwcbkfl.html

JS:   items.join(",")
来源：http://hz.kuanghao11.cn/gtlqqcqwqu.html

TS:   items.join(",")
来源：http://hz.feifeiyinyue.top/gtzazhurqt.html

Java: String.join(",", items)
来源：http://hz.meibo888.top/gtmwxgnqum.html

Go:   strings.Join(items, ",")
来源：http://hz.zhengqikj.top/gtypfixwkq.html

Ruby: items.join(",")
来源：http://hz.cqqwz.cn/gtuskbbhdn.html

C#:   string.Join(",", items)
来源：http://hz.zhaomingkeji.xyz/gtwrlzvzve.html

[E09] 去除所有空白字符
来源：http://hz.tanke756.top/gtqunadwmi.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.aibaodan.cn/gtfggisqim.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.jqgufenzy.top/gtbngztgtc.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.birdmap.top/gtluntfewk.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.nanxuanxn.top/gtgfzaxsxm.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.gzhubu.top/gtzudswbkx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.chenzaomai.com/gtyawahokm.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.jqgufenzy.top/gtvibivbde.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.yuanzhike.top/gtoylhwrol.html

[E10] 左侧补零 / 定长填充
来源：http://hz.jinqigfzy.top/gtkcvwtwyu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.jinghuilouyu.cn/gtgkurmswt.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.hnxiangtu.top/gthrkrjoxe.html

JS:   "7".padStart(3, "0")
来源：http://hz.cucudq.cn/gtowllitqv.html

TS:   "7".padStart(3, "0")
来源：http://hz.pycfn.com/gtyxvlhqbj.html

Java: String.format("%03d", 7)
来源：http://hz.yj20258888.top/gtcwheszpu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.tanke756.top/gtvoifhtex.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.vqdsnc.cn/gtsmtsqwxp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.zycfv.cn/gtmgrnugil.html

[E11] 反转字符串
来源：http://hz.zhaomingkeji.xyz/gtjjgaevlv.html

Py:   s[::-1]
来源：http://hz.shanyushiyangtech.top/gtuxwfewcy.html

PHP:  strrev($s);
来源：http://hz.zhiwuduotai.top/gtxwqbjqjc.html

JS:   [...s].reverse().join("")
来源：http://hz.hammf.cn/gtklpzhqzb.html

TS:   [...s].reverse().join("")
来源：http://hz.zhengqikj.top/gttcprnvpk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.zhiwuduotai.top/gtfqhcnpps.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.jinyuanbaomall.cn/gtnpzwidob.html

Ruby: s.reverse
来源：http://hz.c1oappe.top/gtguqgfapa.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.svipenyu.cn/gtfwyphgkw.html

[E12] 统计某字符出现次数
来源：http://hz.yuxming.cn/gtvzrykxdb.html

Py:   s.count("a")
来源：http://hz.snrcjt.cn/gtvmuaxswu.html

PHP:  substr_count($s, "a");
来源：http://hz.jinqigfzy.top/gtmpdkitja.html

JS:   s.split("a").length - 1
来源：http://hz.xingfuxueyuan.xyz/gtecjtmahh.html

TS:   s.split("a").length - 1
来源：http://hz.jinghuilouyu.cn/gtftgwwzdt.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.gaohongyu789.top/gtubugbdhm.html

Go:   strings.Count(s, "a")
来源：http://hz.feifeiyinyue.top/gthcvegyvg.html

Ruby: s.count("a")
来源：http://hz.zycfv.cn/gtzsifcdlw.html

C#:   s.Count(c => c == 'a')
来源：http://hz.sysykeji.top/gtrricvxkc.html

[E13] 逐字符遍历
来源：http://hz.hammf.cn/gtkfqeivfg.html

Py:   for ch in s: print(ch)
来源：http://hz.yuanzhike.top/gttxunoglm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.hnqzz.top/gtzdpagidc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xinyue.icu/gtjgbgwxzr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yj20258888.top/gthjvdsaqf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.jinyuanbaomall.cn/gthufifzyo.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jyoumei.cn/gtukvbqbcg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.sxryk.cn/gtbvycjlen.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.zhoulong.xyz/gtxhbmrckp.html

[E14] URL 编码与 Base64
来源：http://hz.hfpthk.cn/gthvrdywys.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.guannengcc.top/gtedtmhmek.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.hammf.cn/gtlsxwktfr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.ywan-chungtsiang.top/gthjfpnrvr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.gaohongyu789.top/gtrwjkwtfk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.dashuyun.cn/gtxnjzidef.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.aibaodan.cn/gtvahxwqsr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.svipenyu.cn/gtvnkwzxrf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zdqjudy.top/gtyvzhmgsw.html

[E15] HTML 转义 / 反转义
来源：http://hz.zhongyouzk.top/gtmsmmhdjn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.smart0.xyz/gtmtzyqtrf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jlsjyb.cn/gtwdwnahbg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.feifeiyinyue.top/gtwqhpdzbv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jinqigfzy.top/gtdojazajm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.ehwqpu.com/gtxrxnzzmu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.cheryme.top/gtbefffwbb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jinqigufen.top/gtzzzmenfu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.shangyingyoupin.top/gtspfzpkpe.html

[E16] 数字千分位
来源：http://hz.ehwqpu.com/gtyfzjotrf.html

Py:   f"{1234567:,}"
来源：http://hz.pengpengdd.cyou/gtrbhuvwxv.html


<!-- 参考信息 -->