代发 wailian999

[D07] 切片 / 取子数组
来源：http://hz.zhengqikj.top/gtsefvykor.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.pengpengdd.cyou/gtsgendlzw.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zdqjudy.top/gtowsocizx.html

JS:   arr.slice(1, 4);
来源：http://hz.zhaomingkeji.xyz/gtbiookoqt.html

TS:   arr.slice(1, 4);
来源：http://hz.kuanghao11.cn/gtqhslzbli.html

Java: list.subList(1, 4);
来源：http://hz.pycfn.com/gtxgxktsjl.html

Go:   arr[1:4]
来源：http://hz.yuxming.cn/gtcwepcpos.html

Ruby: arr[1, 3]
来源：http://hz.cqqwz.cn/gtyegnredo.html

C#:   list.GetRange(1, 3);
来源：http://hz.jianghu66.top/gtsviddapw.html

[D08] 合并两个数组
来源：http://hz.ehwqpu.com/gtvcczoqsw.html

Py:   a + b;  a.extend(b)
来源：http://hz.xuetiantiany.cn/gtqtehgfgs.html

PHP:  array_merge($a, $b);
来源：http://hz.sufxvd.cn/gtiruiwdhd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jinyuanbaomall.cn/gtuawdzbzd.html

TS:   [...a, ...b];
来源：http://hz.shanyushiyangkeji.top/gtnxmxharx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.cucudq.cn/gtmyvmqriv.html

Go:   append(a, b...)
来源：http://hz.sxryk.cn/gtyzzmdxha.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yj202588.top/gtgjnkkrsd.html

C#:   a.Concat(b).ToList()
来源：http://hz.haohaochexian.top/gtfhjtqees.html

[D09] 排序（升序）
来源：http://hz.nwbrower.top/gtorewoebe.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jyoumei.cn/gtqyuyhxdv.html

PHP:  sort($arr);
来源：http://hz.jinghuilouyu.cn/gtacahxwgi.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.xylfe.cn/gtbdlmicby.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.sysykeji.top/gtbhuawxmi.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.jinghuilouyu.cn/gteraexdku.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.xuetiantiany.cn/gtgvcotoqw.html

Ruby: arr.sort
来源：http://hz.ppjwa.cn/gtjtmtfynf.html

C#:   list.Sort();
来源：http://hz.jinyuanbaomall.cn/gthljgklid.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.hywenlv.cn/gtcfhjrwtg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zhoulong.xyz/gtwahxyjcm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.fzhhl.top/gtphaqqgnr.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yj20258.top/gtqrjzclac.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhiwuduotai.top/gtqodglrgu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.dianchejie.cn/gtlgygsjod.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.ybcxt.top/gtyiavmaut.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.chenlongwang.top/gttjzejjbb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.shangyingyoupin.top/gtauyreymc.html

[D11] 反转数组
来源：http://hz.quarkkingdee.top/gtutmwaptz.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.zycfv.cn/gtoapskzpn.html

PHP:  array_reverse($arr);
来源：http://hz.daxiang520.top/gttvvuewvg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.quarkkingdee.top/gtvpsqwmbq.html

TS:   [...arr].reverse();
来源：http://hz.xylfe.cn/gthfwscknp.html

Java: Collections.reverse(list);
来源：http://hz.snrcjt.cn/gtuccodkyg.html

Go:   slices.Reverse(arr)
来源：http://hz.pycfn.com/gtbzxdagoa.html

Ruby: arr.reverse
来源：http://hz.hnxiangtu.top/gtpkhinkau.html

C#:   list.Reverse();
来源：http://hz.jiagoushi.top/gtolgztbag.html

[D12] 查找元素下标
来源：http://hz.aizwys.cn/gtxsctyezh.html

Py:   arr.index(x);  x in arr
来源：http://hz.redwolf501.top/gtbekcydss.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.nanxuanxn.top/gthiptgpje.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.redwolf501.top/gtcqpfdlww.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yueranfly.top/gtipwbrzfq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.xuetiantiany.cn/gtciogntqx.html

Go:   slices.Index(arr, x)
来源：http://hz.sysykeji.top/gtilyakpsi.html

Ruby: arr.index(x)
来源：http://hz.zhengqikj.top/gtxfjvkzqx.html

C#:   list.IndexOf(x);
来源：http://hz.feifeiyinyue.top/gtjgaywvdh.html

[D13] 过滤（保留满足条件的）
来源：http://hz.gzhubu.top/gtzozcknto.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.yj20258888.top/gtycimokja.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.smart0.xyz/gtltncegyg.html

JS:   arr.filter(x => x > 3)
来源：http://hz.zhengqikj.top/gtcxjjzjnt.html

TS:   arr.filter(x => x > 3)
来源：http://hz.zhaomingkeji.xyz/gtrruufzlv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.pycfn.com/gtmmmripfp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.haohaochexian.top/gtdiuucwpp.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.dashuyun.cn/gtoewnsjwl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.zhengqikj.top/gtxcagzfnt.html

[D14] 映射转换（每个元素变形）
来源：http://hz.wangshuangyany.cn/gtdlbnsqyl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.shangyingyoupin.top/gtqdgcfvko.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.sweek.top/gtfruziuww.html

JS:   arr.map(x => x * 2)
来源：http://hz.nanxinkj.top/gtpzxjrqls.html

TS:   arr.map(x => x * 2)
来源：http://hz.chenzaomai.com/gttufacqeb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.kuanghao11.cn/gtcgrwlutw.html

Go:   // 手写循环
来源：http://hz.52xcode.cn/gtmyalhhtp.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.cqqwz.cn/gtpuydofia.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.aizwys.cn/gttltddldb.html

[D15] 去重
来源：http://hz.fzhhl.top/gtiwnblpjk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.cucudq.cn/gtgkzbvjof.html

PHP:  array_unique($arr);
来源：http://hz.redwolf501.top/gtczfjncei.html

JS:   [...new Set(arr)]
来源：http://hz.tianlin.xyz/gtohldzury.html

TS:   [...new Set(arr)]
来源：http://hz.zhengqikj.top/gtjtlefkvv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jinghuilouyu.cn/gtguybijhv.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.aibaodan.cn/gtpnlyesbd.html

Ruby: arr.uniq
来源：http://hz.cashguo.top/gtvjdltksv.html

C#:   list.Distinct().ToList()
来源：http://hz.zhaomingkeji.xyz/gteyalhzan.html

[D16] 求和与平均值
来源：http://hz.cucudq.cn/gtqtcithzy.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.ywan-chungtsiang.top/gtklvywbbb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.chenzaomai.com/gtrrdkazis.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.wangshuangyany.cn/gttnttvrld.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xylfe.cn/gtbjnesauc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.meibo888.top/gtypucaazi.html

Go:   // 手写循环累加
来源：http://hz.chenjidiqi.icu/gthpqxvmua.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.iojbl.cn/gtkvjxoakl.html

C#:   list.Sum();  list.Average()
来源：http://hz.zhengqikj.top/gtehzhsdqn.html

[D17] 最大值与最小值
来源：http://hz.nwbrower.top/gtmadsnnaa.html

Py:   max(arr);  min(arr)
来源：http://hz.yangfankeji.com/gtfrlaebjl.html

PHP:  max($arr);  min($arr);
来源：http://hz.pengpengdd.cyou/gthaxmrnhw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yuanzhike.top/gtbhpiujke.html

TS:   Math.max(...arr);
来源：http://hz.316326.xyz/gthhbxkkgm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jianghu66.top/gtzwpkqrgd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.yj20258.top/gtnxgxrvyu.html

Ruby: arr.max;  arr.min
来源：http://hz.c1oappe.top/gtndhoqzxi.html

C#:   list.Max();  list.Min()
来源：http://hz.ppjwa.cn/gtxikcimnh.html

[D18] 扁平化嵌套数组
来源：http://hz.hammf.cn/gtipmjlpbq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.meibo888.top/gthqbodvdg.html

PHP:  array_merge(...$nested);
来源：http://hz.sweek.top/gtfunvhtwp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.havefunace.top/gtszypuoto.html

TS:   nested.flat();
来源：http://hz.dianchejie.cn/gttgnwjdpc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.zhijiandao.cn/gtxndstqsb.html

Go:   // 手写双层循环
来源：http://hz.zhengqikj.top/gthsobgfbw.html

Ruby: nested.flatten
来源：http://hz.xuetiantiany.cn/gtwurhnljz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yongpay.top/gtfvbigmtc.html

[D19] 按字段分组
来源：http://hz.birdmap.top/gtrxofwhns.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.gotoacloud.top/gtkbccxqkd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.ywan-chungtsiang.top/gtlpnqloef.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yj202588.top/gtwpdvydem.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.zhixingplan.top/gtkujhgyae.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.ivvv.top/gtrigaxhbn.html

Go:   // 手写 map[string][]T
来源：http://hz.fengsongda.top/gtrbbqksqd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.cashguo.top/gtrxyhfshc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.shanyushiyangkeji.top/gtkeapzdcu.html

[D20] 统计每个元素出现次数
来源：http://hz.smart0.xyz/gtjqsupagc.html

Py:   Counter(arr)
来源：http://hz.haohaochexian.top/gtaeqwfgvq.html

PHP:  array_count_values($arr);
来源：http://hz.chenlongwang.top/gtzzcxlowf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhixingplan.top/gttuhefimn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hnqzz.top/gtfklueqiy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.shanyushiyangkeji.top/gtfuavondq.html

Go:   // 手写 map[T]int
来源：http://hz.cdnleiting.top/gtqdzickec.html

Ruby: arr.tally
来源：http://hz.gaohongyu789.top/gtbvnqyife.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.gotoacloud.top/gtjruhuoec.html

[D21] 判断是否包含某元素
来源：http://hz.shzxlz.cn/gtakswxqxb.html

Py:   x in arr
来源：http://hz.ivvv.top/gteojrbmpj.html

PHP:  in_array($x, $arr, true);
来源：http://hz.tian-w.cn/gthxskiqac.html

JS:   arr.includes(x)
来源：http://hz.ppjwa.cn/gtkjsugszl.html

TS:   arr.includes(x)
来源：http://hz.yanxiufei.cn/gtaeafyevz.html

Java: list.contains(x)
来源：http://hz.jqgufenzy.top/gtmwlxosit.html

Go:   slices.Contains(arr, x)
来源：http://hz.yj20258.top/gtyrqmojpg.html

Ruby: arr.include?(x)
来源：http://hz.chenlongwang.top/gtsktmbszz.html

C#:   list.Contains(x)
来源：http://hz.316326.xyz/gtpawvuhts.html

[D22] 复制数组（避免共享引用）
来源：http://hz.cqqwz.cn/gtthsuumiq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yuxming.cn/gthyxpgpsv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.feifeiyinyue.top/gthcvkchvv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.0kj1m.cn/gtinrkcckc.html

TS:   [...arr];
来源：http://hz.shangyingyoupin.top/gthaiacmam.html

Java: new ArrayList<>(list);
来源：http://hz.9152youxi.cn/gtcrdhsohx.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.chenzaomai.com/gtlzjnmpre.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zhongyouzk.top/gtxqltdoja.html

C#:   new List<int>(list);
来源：http://hz.cdnleiting.top/gtiqdcpkbo.html

[D23] reduce 累积计算
来源：http://hz.gogol.net.cn/gtmispzchh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.9152youxi.cn/gtfciutnnt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.sufxvd.cn/gtakyjlrgi.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.9152youxi.cn/gtchgqaapv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.nanxuanxn.top/gtanbnrgif.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jlsjyb.cn/gtwkobngot.html

Go:   // 手写循环
来源：http://hz.0kj1m.cn/gtjvguvxqm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.xingfuxueyuan.xyz/gtnlnwuift.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yj20258.top/gtxygbwxlp.html

[D24] 字典 / Map 基本操作
来源：http://hz.nanxinkj.top/gtslygaruf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.sxryk.cn/gteyqgxjfe.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.jyoumei.cn/gtnnesiutb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jlsjyb.cn/gtageizlrf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.ybcxt.top/gtkedgzsjr.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.jinghuilouyu.cn/gtzcjvbxnj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yangfankeji.com/gtcmkfhlod.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.mhx1999.top/gtawmyizjm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.daria6918.cn/gtsowiadbb.html

[D25] Set 集合去重与交并差
来源：http://hz.sufxvd.cn/gtlixclazc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.ydzc1.top/gtzlgysuyw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.svipenyu.cn/gtpsandncr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.zhiwuduotai.top/gtrahurbgf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.ydjk.org.cn/gtrblsxkuy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.kuanghao11.cn/gtxkgiuazw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.shanyushiyangtech.top/gtxbvniwsq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.svipenyu.cn/gttbxkgthe.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.cucudq.cn/gtvkxqheip.html

[D26] 数组转字符串
来源：http://hz.pycfn.com/gtovttkcsa.html

Py:   ", ".join(map(str, arr))
来源：http://hz.gotoacloud.top/gtlgldycpj.html

PHP:  implode(", ", $arr);
来源：http://hz.shangyingyoupin.top/gtybqkrzuj.html

JS:   arr.join(", ")
来源：http://hz.52xcode.cn/gtodvfzbal.html

TS:   arr.join(", ")
来源：http://hz.hfpthk.cn/gtozhvsksz.html

Java: String.join(", ", list)
来源：http://hz.ydzc1.top/gtcqhfyqwf.html

Go:   strings.Join(strs, ", ")
来源：http://hz.cucudq.cn/gtmqcgdlhj.html

Ruby: arr.join(", ")
来源：http://hz.jianghu66.top/gtcbqdarmi.html

C#:   string.Join(", ", list)
来源：http://hz.jqgufenzy.top/gtqomrucjm.html

================================================================================
来源：http://hz.jlsjyb.cn/gtjqvvzekm.html

E. 字符串处理
来源：http://hz.xylfe.cn/gtkqnsicoq.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gttogcjrtk.html

[E01] 拼接字符串
来源：http://hz.daria6918.cn/gtgfcsdeeu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.xingfuxueyuan.xyz/gtmushamfh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.ivvv.top/gtdyknnzqv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.birdmap.top/gtndzdwpvy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.sufxvd.cn/gtwyylxklr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.cashguo.top/gthxjziwma.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.ehwqpu.com/gtkvjoyjkj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yuanzhike.top/gtyfhudpzh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.xziqi.cn/gtefpfucfo.html

[E02] 重复字符串
来源：http://hz.zhengqikj.top/gtbtdzwhjb.html

Py:   "ab" * 3
来源：http://hz.zhixingplan.top/gtskwsdpvp.html

PHP:  str_repeat("ab", 3);
来源：http://hz.ydjk.org.cn/gtyiywydqm.html

JS:   "ab".repeat(3)
来源：http://hz.sweek.top/gtdlkedshx.html

TS:   "ab".repeat(3)
来源：http://hz.ydzc1.top/gtwnaumgun.html

Java: "ab".repeat(3)
来源：http://hz.yj202588.top/gtdvrpsqxp.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.aibaodan.cn/gtyubtmiaf.html

Ruby: "ab" * 3
来源：http://hz.shuidangran.top/gtianwqeft.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.snrcjt.cn/gtnmaeqqzr.html

[E03] 截取子串
来源：http://hz.nanxinkj.top/gtwhgcgcad.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yueranfly.top/gtsrnvtlyf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zhoulong.xyz/gtzempsydn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.c1oappe.top/gtgfrcqkqs.html

TS:   s.slice(1, 4)
来源：http://hz.fengsongda.top/gtfzpgsacz.html

Java: s.substring(1, 4)
来源：http://hz.9152youxi.cn/gthtjngpjv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yonumen.top/gtxurlwdmw.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.shanyushiyangkeji.top/gtkvbecemj.html

C#:   s.Substring(1, 3)
来源：http://hz.jinqigufen.top/gtrlarpojt.html

[E04] 查找子串位置
来源：http://hz.zhijiandao.cn/gtpyrxdezo.html

Py:   s.find("x");  s.index("x")
来源：http://hz.jyoumei.cn/gtedpitqit.html

PHP:  strpos($s, "x");
来源：http://hz.daxiang520.top/gtuvmibxjs.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zhongyouzk.top/gtpntesbhs.html

TS:   s.indexOf("x")
来源：http://hz.nanxinkj.top/gtcnywdprd.html

Java: s.indexOf("x")
来源：http://hz.svipenyu.cn/gtdtihqyoo.html

Go:   strings.Index(s, "x")
来源：http://hz.shangyingyoupin.top/gtqehnfunv.html

Ruby: s.index("x")
来源：http://hz.zycfv.cn/gtuygasskc.html

C#:   s.IndexOf("x")
来源：http://hz.jlsjyb.cn/gtnchbqsff.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.sxryk.cn/gtslbhakvx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.ivvv.top/gtvdayjozl.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.52xcode.cn/gtmitlzxxd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.shuidangran.top/gtrmrxvvsk.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.guannengcc.top/gtyftdpvnn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhoulong.xyz/gtbxwpxbnx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.hfpthk.cn/gtdbwoppxt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.sweek.top/gtectxhpvd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.xinyue.icu/gtrpuqbziq.html

[E06] 替换子串
来源：http://hz.sxryk.cn/gtlnvtfwet.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.bjfxy.top/gtmfydcekr.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.hongshengwenyu.top/gtyvaxmxms.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhoulong.xyz/gtkzsrchng.html

TS:   s.replaceAll("a", "b")
来源：http://hz.jqgufenzy.top/gthwwzwqdl.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xuanzx.com/gttpakvtji.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.chenzaomai.com/gtoqltgvgr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.gzhubu.top/gtocakqxua.html

C#:   s.Replace("a", "b")
来源：http://hz.sxryk.cn/gtmdmhfqho.html

[E07] 按分隔符拆分
来源：http://hz.ppjwa.cn/gtwtmqmgwj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.dianchejie.cn/gtssceheiq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yj20258.top/gtdtyqloqr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.meibo888.top/gttoxanrhz.html

TS:   s.split(",")
来源：http://hz.xuetiantiany.cn/gtsfqrbuoz.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.cucudq.cn/gtwwlpykje.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.mhx1999.top/gthcgjrjay.html

Ruby: s.split(",");  s.split
来源：http://hz.xuanzx.com/gtixgutzbp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.gzhubu.top/gtysppmder.html

[E08] 数组按分隔符合并
来源：http://hz.xylfe.cn/gtcaabhysd.html

Py:   ",".join(items)
来源：http://hz.yongpay.top/gtmbfeoghv.html

PHP:  implode(",", $items);
来源：http://hz.yueranfly.top/gtfekidcme.html

JS:   items.join(",")
来源：http://hz.shanyushiyangkeji.top/gtggzkwzwo.html

TS:   items.join(",")
来源：http://hz.shanyushiyangtech.top/gtfpjnuqgw.html

Java: String.join(",", items)
来源：http://hz.chenlongwang.top/gtzyxnnhhj.html

Go:   strings.Join(items, ",")
来源：http://hz.jinghuilouyu.cn/gtlsrohzsz.html

Ruby: items.join(",")
来源：http://hz.bjfxy.top/gtuabspalv.html

C#:   string.Join(",", items)
来源：http://hz.shanyushiyangkeji.top/gtmlnjsypf.html

[E09] 去除所有空白字符
来源：http://hz.shuidangran.top/gtguvagjbx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.shuidangran.top/gtjnywbdjv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.guannengcc.top/gthuokulvh.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.pengpengdd.cyou/gtqpeeadqp.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.shzxlz.cn/gtjhvlvkls.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.daria6918.cn/gtbuthdgsz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.shanyushiyangtech.top/gtweuggbwo.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.snrcjt.cn/gtuxuhwyac.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.hongshengwenyu.top/gtwovzhtid.html

[E10] 左侧补零 / 定长填充
来源：http://hz.yvedp.cn/gtcepzsgxc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.iojbl.cn/gtfzuzczqx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.jinqigufen.top/gtehgtqvqz.html

JS:   "7".padStart(3, "0")
来源：http://hz.jyoumei.cn/gtqtnkraaf.html

TS:   "7".padStart(3, "0")
来源：http://hz.gotoacloud.top/gtphfgyxnt.html

Java: String.format("%03d", 7)
来源：http://hz.jqgufenzy.top/gtckgwyruh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.xuetiantiany.cn/gtbassxxsr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.ydzc1.top/gtmbfgwqyb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.gaohongyu789.top/gtprsbeexl.html

[E11] 反转字符串
来源：http://hz.yvedp.cn/gtdoncpnts.html

Py:   s[::-1]
来源：http://hz.hysaishi.cn/gtdqrlvuqd.html

PHP:  strrev($s);
来源：http://hz.jiagoushi.top/gtcatjnfiq.html

JS:   [...s].reverse().join("")
来源：http://hz.zhaomingkeji.xyz/gtjsmzvyxd.html

TS:   [...s].reverse().join("")
来源：http://hz.jqgfzy.top/gthppbhafs.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jiagoushi.top/gttwpcbusv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.xuetiantiany.cn/gtpoutkjek.html

Ruby: s.reverse
来源：http://hz.redwolf501.top/gtzqxnrpfq.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.c1oappe.top/gtuxjldony.html

[E12] 统计某字符出现次数
来源：http://hz.hysaishi.cn/gtzgpqxfam.html

Py:   s.count("a")
来源：http://hz.andypj.xyz/gtzqjgenuz.html

PHP:  substr_count($s, "a");
来源：http://hz.zhaomingkeji.xyz/gttlgsettd.html

JS:   s.split("a").length - 1
来源：http://hz.nwbrower.top/gtyjzquiyn.html

TS:   s.split("a").length - 1
来源：http://hz.0kj1m.cn/gttrtmbbsj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.fengsongda.top/gtukfosxab.html

Go:   strings.Count(s, "a")
来源：http://hz.chenlongwang.top/gtpysndkns.html

Ruby: s.count("a")
来源：http://hz.pengpengdd.cyou/gtdlrhfhoo.html

C#:   s.Count(c => c == 'a')
来源：http://hz.ywan-chungtsiang.top/gtfzgrwfxv.html

[E13] 逐字符遍历
来源：http://hz.tianlin.xyz/gttkehuiyj.html

Py:   for ch in s: print(ch)
来源：http://hz.hysaishi.cn/gtplsonwrv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.52xcode.cn/gtkootjaxe.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.nanxuanxn.top/gtpwvnvrqq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.52xcode.cn/gtxktwbgjx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.gaohongyu789.top/gtncpkwjup.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.feifeiyinyue.top/gtfyeecpva.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.shanyushiyangtech.top/gtbqmmbvwv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.aibaodan.cn/gtwngriwds.html


<!-- 参考信息 -->