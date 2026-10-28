代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.dashuyun.cn/gtpbjvgakn.html

TS:   arr.splice(0, 1);
来源：http://hz.yj20258.top/gtlqzawhbi.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.0kj1m.cn/gtymqonfyc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.316326.xyz/gtbaaemcdh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.shanyushiyangkeji.top/gttsokhsrw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.zhixingplan.top/gtmqjzfxws.html

[D05] 访问与修改元素
来源：http://hz.feifeiyinyue.top/gtenwloxid.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.quarkkingdee.top/gtzzmjzoez.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.gzhubu.top/gtudgopght.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.gzhubu.top/gtzoysmged.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.ppjwa.cn/gtensqzqxl.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jyoumei.cn/gtgqtirsqz.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.ybcxt.top/gtksdjelvr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zycfv.cn/gtzogjsauh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.52xcode.cn/gtspwtuugr.html

[D06] 数组长度
来源：http://hz.gaohongyu789.top/gtljnymoll.html

Py:   len(arr)
来源：http://hz.tanke756.top/gtwzpynsxb.html

PHP:  count($arr);
来源：http://hz.pycfn.com/gtfqnpbvkq.html

JS:   arr.length
来源：http://hz.xziqi.cn/gtmozybwue.html

TS:   arr.length
来源：http://hz.ehwqpu.com/gtdmjlzanj.html

Java: list.size();
来源：http://hz.yj20258.top/gtkjafhylw.html

Go:   len(arr)
来源：http://hz.jlsjyb.cn/gtweswziaf.html

Ruby: arr.length; arr.size
来源：http://hz.aizwys.cn/gtbindsrpq.html

C#:   list.Count;
来源：http://hz.ehwqpu.com/gtivtywrrk.html

[D07] 切片 / 取子数组
来源：http://hz.wangdashe.top/gtpuvbckxg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.gaohongyu789.top/gtnlmmepoo.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.dashuyun.cn/gtuhcpkdyv.html

JS:   arr.slice(1, 4);
来源：http://hz.cucudq.cn/gtpkdigfxd.html

TS:   arr.slice(1, 4);
来源：http://hz.ywan-chungtsiang.top/gtnxcjrrdx.html

Java: list.subList(1, 4);
来源：http://hz.yj202588.top/gteoowjkxf.html

Go:   arr[1:4]
来源：http://hz.jinyuanbaomall.cn/gtxpxqjzbk.html

Ruby: arr[1, 3]
来源：http://hz.andypj.xyz/gtgywitfvt.html

C#:   list.GetRange(1, 3);
来源：http://hz.bjfxy.top/gtxdlwthem.html

[D08] 合并两个数组
来源：http://hz.sufxvd.cn/gtvjkyroxc.html

Py:   a + b;  a.extend(b)
来源：http://hz.jianghu66.top/gtgouugvwq.html

PHP:  array_merge($a, $b);
来源：http://hz.guowangkeji.top/gtdacirsqh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.cheryme.top/gtszkqgfdy.html

TS:   [...a, ...b];
来源：http://hz.gaohongyu789.top/gtogkeutox.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.zhixingplan.top/gtbiutqfyi.html

Go:   append(a, b...)
来源：http://hz.havefunace.top/gtfzgqmzdg.html

Ruby: a + b;  a.concat(b)
来源：http://hz.jinghuilouyu.cn/gtdymoufvz.html

C#:   a.Concat(b).ToList()
来源：http://hz.xziqi.cn/gtjllsmzvr.html

[D09] 排序（升序）
来源：http://hz.nanxinkj.top/gtptyctmjp.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yj20258888.top/gtjkcfgnsv.html

PHP:  sort($arr);
来源：http://hz.chenjidiqi.icu/gtodfwltho.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yvedp.cn/gtieglwpve.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.zhengqikj.top/gtkwiadsvp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.xinyue.icu/gttijshivl.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.jinghuilouyu.cn/gtcfysagyx.html

Ruby: arr.sort
来源：http://hz.ppjwa.cn/gtaolaclcp.html

C#:   list.Sort();
来源：http://hz.xuetiantiany.cn/gtwfubmfeo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.jinghuilouyu.cn/gtoldficly.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yonumen.top/gtzybtmrwn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hysaishi.cn/gtutnixpij.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jqgufenzy.top/gtsiortksq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yj202588.top/gtjeqywuuw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.zycfv.cn/gthxqrawbf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.guannengcc.top/gtffmmkdsk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.dianchejie.cn/gtwxmwysft.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zycfv.cn/gtnjfdhbnr.html

[D11] 反转数组
来源：http://hz.yueranfly.top/gtksechdnb.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.aizwys.cn/gtdlmsbgcx.html

PHP:  array_reverse($arr);
来源：http://hz.cdnleiting.top/gtblqdsloz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.snrcjt.cn/gtoakryilq.html

TS:   [...arr].reverse();
来源：http://hz.birdmap.top/gtnieapwzk.html

Java: Collections.reverse(list);
来源：http://hz.gotoacloud.top/gtoymhlony.html

Go:   slices.Reverse(arr)
来源：http://hz.xylfe.cn/gtzfsnqjuf.html

Ruby: arr.reverse
来源：http://hz.dashuyun.cn/gtzuqiskfx.html

C#:   list.Reverse();
来源：http://hz.meibo888.top/gtmjherchq.html

[D12] 查找元素下标
来源：http://hz.jinqigufen.top/gtcanowjzg.html

Py:   arr.index(x);  x in arr
来源：http://hz.dashuyun.cn/gtytohjxaw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.xingfuxueyuan.xyz/gtvsttblsy.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zdqjudy.top/gtckeaptzp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jianghu66.top/gtqtqqwdxk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.ivvv.top/gtpeukkkhl.html

Go:   slices.Index(arr, x)
来源：http://hz.ydjk.org.cn/gtiyaaslfi.html

Ruby: arr.index(x)
来源：http://hz.daxiang520.top/gtxjdzcazj.html

C#:   list.IndexOf(x);
来源：http://hz.jqgfzy.top/gtkghuvybo.html

[D13] 过滤（保留满足条件的）
来源：http://hz.shangyingyoupin.top/gtsgyaibkk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.cheryme.top/gtxljpdcpv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.nanxinkj.top/gtgecelrbd.html

JS:   arr.filter(x => x > 3)
来源：http://hz.shangyingyoupin.top/gtxmtckhoc.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jyoumei.cn/gtenumkslf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.sxryk.cn/gtbxpocpus.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.aizwys.cn/gtubauwrey.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.yangfankeji.com/gtozivqqbt.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jqgfzy.top/gtxlkifzcr.html

[D14] 映射转换（每个元素变形）
来源：http://hz.hysaishi.cn/gtofihyxqy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.snrcjt.cn/gtjobluhhh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.chenjidiqi.icu/gtecaqemmg.html

JS:   arr.map(x => x * 2)
来源：http://hz.daxiang520.top/gtechgxkxh.html

TS:   arr.map(x => x * 2)
来源：http://hz.aibaodan.cn/gtswznjjqp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.wangshuangyany.cn/gtxntolmqv.html

Go:   // 手写循环
来源：http://hz.sxryk.cn/gtbxqdwija.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.vqdsnc.cn/gtkwtsagip.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.feifeiyinyue.top/gttfpvxcsb.html

[D15] 去重
来源：http://hz.hongshengwenyu.top/gtlnlmvjdt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.cheryme.top/gtnhvqvqrz.html

PHP:  array_unique($arr);
来源：http://hz.aibaodan.cn/gtjuynbswv.html

JS:   [...new Set(arr)]
来源：http://hz.316326.xyz/gtsqivpkps.html

TS:   [...new Set(arr)]
来源：http://hz.gogol.net.cn/gtjxmdhekj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.xuanzx.com/gtkblnsdrk.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.andypj.xyz/gtctexieko.html

Ruby: arr.uniq
来源：http://hz.ybcxt.top/gtqhmufbpg.html

C#:   list.Distinct().ToList()
来源：http://hz.9152youxi.cn/gtxsawnazt.html

[D16] 求和与平均值
来源：http://hz.yueranfly.top/gtkhymhvbq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.zhaomingkeji.xyz/gtxuhskrqu.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.zhiwuduotai.top/gtyzpcwfjk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinyuanbaomall.cn/gtcuctphep.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhengqikj.top/gtyvmoguwr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.shanyushiyangtech.top/gtvxzjyzbq.html

Go:   // 手写循环累加
来源：http://hz.jqgufenzy.top/gtfgrdwhtp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.birdmap.top/gtlfdylmpt.html

C#:   list.Sum();  list.Average()
来源：http://hz.hywenlv.cn/gtqljbwzns.html

[D17] 最大值与最小值
来源：http://hz.nwbrower.top/gtpmtjazhz.html

Py:   max(arr);  min(arr)
来源：http://hz.vqdsnc.cn/gtbrkxmxwf.html

PHP:  max($arr);  min($arr);
来源：http://hz.guowangkeji.top/gtzkghsmia.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.nwbrower.top/gtrmwwxmgb.html

TS:   Math.max(...arr);
来源：http://hz.shanyushiyangkeji.top/gtoqzxbxnm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.hywenlv.cn/gtsuogpyim.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.yj202588.top/gtnnensnjw.html

Ruby: arr.max;  arr.min
来源：http://hz.gogol.net.cn/gtspljrcuw.html

C#:   list.Max();  list.Min()
来源：http://hz.shanyushiyangkeji.top/gtiberwkug.html

[D18] 扁平化嵌套数组
来源：http://hz.zhoulong.xyz/gteeisrycf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.sxryk.cn/gtekutuuqc.html

PHP:  array_merge(...$nested);
来源：http://hz.guowangkeji.top/gttooklbgm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.hysaishi.cn/gtxywgrmxy.html

TS:   nested.flat();
来源：http://hz.tianlin.xyz/gtueuzcxqy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.tian-w.cn/gtxryopyoo.html

Go:   // 手写双层循环
来源：http://hz.gogol.net.cn/gtfuylqjvi.html

Ruby: nested.flatten
来源：http://hz.havefunace.top/gtpxwffijn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.aizwys.cn/gtanptdfnb.html

[D19] 按字段分组
来源：http://hz.yvedp.cn/gtihsqodto.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.aibaodan.cn/gtkutaqkoy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yueranfly.top/gtgrahlurh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yuxming.cn/gtypyidzcu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.pycfn.com/gtdhpwjlvb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.dianchejie.cn/gtdwputyir.html

Go:   // 手写 map[string][]T
来源：http://hz.shuidangran.top/gtrevuxrvy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.shzxlz.cn/gtzekafvln.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.zhijiandao.cn/gtnfcawnsk.html

[D20] 统计每个元素出现次数
来源：http://hz.shzxlz.cn/gtaskfxoow.html

Py:   Counter(arr)
来源：http://hz.316326.xyz/gtmurqvmwr.html

PHP:  array_count_values($arr);
来源：http://hz.ydjk.org.cn/gtjzbpdyvo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yanxiufei.cn/gtblehdywb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hammf.cn/gtqpmfkjwq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.shuidangran.top/gtswfuwrof.html

Go:   // 手写 map[T]int
来源：http://hz.xylfe.cn/gtjhsbzaxh.html

Ruby: arr.tally
来源：http://hz.smart0.xyz/gtsrhxjiio.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.ybcxt.top/gtflkccton.html

[D21] 判断是否包含某元素
来源：http://hz.jinqigfzy.top/gtddahwvbh.html

Py:   x in arr
来源：http://hz.jinghuilouyu.cn/gtdezviddl.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yj20258888.top/gtjezufkmc.html

JS:   arr.includes(x)
来源：http://hz.xuanzx.com/gtuxopalca.html

TS:   arr.includes(x)
来源：http://hz.tian-w.cn/gtdwisacok.html

Java: list.contains(x)
来源：http://hz.xziqi.cn/gtoxjletlj.html

Go:   slices.Contains(arr, x)
来源：http://hz.chenjidiqi.icu/gtxvonxdud.html

Ruby: arr.include?(x)
来源：http://hz.yj20258888.top/gtldngigab.html

C#:   list.Contains(x)
来源：http://hz.yangfankeji.com/gtlgbdhdce.html

[D22] 复制数组（避免共享引用）
来源：http://hz.andypj.xyz/gtejbhqycy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.dianchejie.cn/gtaklzpqdv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.jinyuanbaomall.cn/gtzsbcxoti.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.xingfuxueyuan.xyz/gtnzaxblwm.html

TS:   [...arr];
来源：http://hz.haohaochexian.top/gtindkqauf.html

Java: new ArrayList<>(list);
来源：http://hz.yuxming.cn/gtfqyaiabz.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.gaohongyu789.top/gtiuuqunvf.html

Ruby: arr.dup;  arr.clone
来源：http://hz.bjfxy.top/gtvmurqbif.html

C#:   new List<int>(list);
来源：http://hz.snrcjt.cn/gtlowlzwsy.html

[D23] reduce 累积计算
来源：http://hz.hywenlv.cn/gtnvwaaysk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.ydjk.org.cn/gtkkiarltn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.cashguo.top/gtgxlidipi.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.sufxvd.cn/gtcfsbebnc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yanxiufei.cn/gtozrwxzsw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jinqigfzy.top/gtpythnedp.html

Go:   // 手写循环
来源：http://hz.mhx1999.top/gtkgtczsyz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.andypj.xyz/gthqfjhmrl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.aizwys.cn/gtmdmjyznj.html

[D24] 字典 / Map 基本操作
来源：http://hz.yongpay.top/gtdmjqtots.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.ivvv.top/gtthatnkfh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.hfpthk.cn/gtxwreihxn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.aizwys.cn/gthfrknmir.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.zhiwuduotai.top/gtecomduku.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.hnxiangtu.top/gtwiotwwnv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.ivvv.top/gtwyryqwnk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jinqigufen.top/gtzcacjpiz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.nanxinkj.top/gtikkdzfav.html

[D25] Set 集合去重与交并差
来源：http://hz.sxryk.cn/gttsqloxes.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.birdmap.top/gtrjxvzzak.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.chenjidiqi.icu/gtmqvdxjel.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.zhengqikj.top/gtsjhvyndl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.nanxuanxn.top/gtazrgllzw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.havefunace.top/gtfpvtulyd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.hammf.cn/gtigpopwky.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yanxiufei.cn/gtqdraqath.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.daxiang520.top/gtsjzwbgum.html

[D26] 数组转字符串
来源：http://hz.snrcjt.cn/gtinseazal.html

Py:   ", ".join(map(str, arr))
来源：http://hz.tianlin.xyz/gtxfklxnjo.html

PHP:  implode(", ", $arr);
来源：http://hz.ivvv.top/gtrtasvasd.html

JS:   arr.join(", ")
来源：http://hz.cdnleiting.top/gtqarvwmwq.html

TS:   arr.join(", ")
来源：http://hz.jiagoushi.top/gtovodfzrp.html

Java: String.join(", ", list)
来源：http://hz.hongshengwenyu.top/gtpuqloiwj.html

Go:   strings.Join(strs, ", ")
来源：http://hz.daria6918.cn/gtymndyntm.html

Ruby: arr.join(", ")
来源：http://hz.xylfe.cn/gtzkzmdlpl.html

C#:   string.Join(", ", list)
来源：http://hz.zhixingplan.top/gtvwdfnmal.html

================================================================================
来源：http://hz.xinyue.icu/gtefyjxmri.html

E. 字符串处理
来源：http://hz.jyoumei.cn/gtznxmadwe.html

================================================================================
来源：http://hz.vqdsnc.cn/gtsmogsdgz.html

[E01] 拼接字符串
来源：http://hz.chenlongwang.top/gtfgvsoplh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.dianchejie.cn/gtymewiicp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.andypj.xyz/gtolmyecar.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.birdmap.top/gtlpdggqnw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xuanzx.com/gtlhpfiaaz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.fzhhl.top/gtjcklrjei.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.jianghu66.top/gtmreylvql.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.quarkkingdee.top/gthvwndsic.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zycfv.cn/gtujklyiye.html

[E02] 重复字符串
来源：http://hz.jinyuanbaomall.cn/gtgdzxwfsa.html

Py:   "ab" * 3
来源：http://hz.jlsjyb.cn/gtdokxahln.html

PHP:  str_repeat("ab", 3);
来源：http://hz.chenlongwang.top/gthbdwrlnl.html

JS:   "ab".repeat(3)
来源：http://hz.smart0.xyz/gtldkbaaxb.html

TS:   "ab".repeat(3)
来源：http://hz.nanxinkj.top/gtweatmtae.html

Java: "ab".repeat(3)
来源：http://hz.cashguo.top/gtorwnaqtk.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.shuidangran.top/gtezjairid.html

Ruby: "ab" * 3
来源：http://hz.fzhhl.top/gtpkgsczsr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.zhijiandao.cn/gtpjpyntzl.html

[E03] 截取子串
来源：http://hz.9152youxi.cn/gtwaggjdkk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.jianghu66.top/gtndcpluvb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.tanke756.top/gtsjkqfgke.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.chenlongwang.top/gtdltbhglf.html

TS:   s.slice(1, 4)
来源：http://hz.hfpthk.cn/gtryphiksz.html

Java: s.substring(1, 4)
来源：http://hz.birdmap.top/gtbnyycusw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.9152youxi.cn/gtkiucgdmh.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.shanyushiyangtech.top/gtqvakbooo.html

C#:   s.Substring(1, 3)
来源：http://hz.fzhhl.top/gtxgijoidb.html

[E04] 查找子串位置
来源：http://hz.ehwqpu.com/gtzaopwxeg.html

Py:   s.find("x");  s.index("x")
来源：http://hz.nanxinkj.top/gtnohvionw.html

PHP:  strpos($s, "x");
来源：http://hz.chenzaomai.com/gtzbjugpib.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.jiagoushi.top/gthrmwxurg.html

TS:   s.indexOf("x")
来源：http://hz.shuidangran.top/gtzghxnoar.html

Java: s.indexOf("x")
来源：http://hz.zhengqikj.top/gtbdrhegtk.html

Go:   strings.Index(s, "x")
来源：http://hz.kuanghao11.cn/gtiuvdkosu.html

Ruby: s.index("x")
来源：http://hz.nanxuanxn.top/gtjakzdjst.html

C#:   s.IndexOf("x")
来源：http://hz.snrcjt.cn/gtbhhlkrrm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.svipenyu.cn/gtzacgdefc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.yj20258.top/gtlmreicrm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zhaomingkeji.xyz/gtcrwsxkzk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.dianchejie.cn/gtjmcxcspz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.quarkkingdee.top/gtrzgrwnfy.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.iojbl.cn/gtzcpqvldp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.snrcjt.cn/gtdxnxlelf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.ybcxt.top/gtokamxizo.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.xingfuxueyuan.xyz/gtlnnhfwff.html

[E06] 替换子串
来源：http://hz.jinqigufen.top/gtoxyfaiqq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.wangshuangyany.cn/gtjonxyxcb.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.jqgufenzy.top/gtpbaqkwyo.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.haohaochexian.top/gtnfkchmzb.html

TS:   s.replaceAll("a", "b")
来源：http://hz.jianghu66.top/gtntngejpw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zycfv.cn/gtueyvqxtn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.shangyingyoupin.top/gtqjhmtxfc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.yj20258.top/gtsoxbbytj.html

C#:   s.Replace("a", "b")
来源：http://hz.gaohongyu789.top/gttbpifnqx.html

[E07] 按分隔符拆分
来源：http://hz.guannengcc.top/gtappxrawc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jqgfzy.top/gtksuvydnl.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.316326.xyz/gtulrjfdik.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.zhoulong.xyz/gtinohkuve.html

TS:   s.split(",")
来源：http://hz.yangfankeji.com/gtpqfymnby.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.shzxlz.cn/gtmjwijwul.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.xuanzx.com/gtgbyegogs.html

Ruby: s.split(",");  s.split
来源：http://hz.wangdashe.top/gtexxwcxbt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.iojbl.cn/gtfphwmjah.html

[E08] 数组按分隔符合并
来源：http://hz.aizwys.cn/gtegxneqib.html

Py:   ",".join(items)
来源：http://hz.yvedp.cn/gtuvrgspyh.html

PHP:  implode(",", $items);
来源：http://hz.zdqjudy.top/gtobvuzdis.html

JS:   items.join(",")
来源：http://hz.ydjk.org.cn/gtatpgwxpp.html

TS:   items.join(",")
来源：http://hz.yuanzhike.top/gtwdseoilw.html

Java: String.join(",", items)
来源：http://hz.jinghuilouyu.cn/gtzaauciiy.html

Go:   strings.Join(items, ",")
来源：http://hz.yongpay.top/gttqkvtxdg.html

Ruby: items.join(",")
来源：http://hz.ybcxt.top/gtmzbewrqt.html

C#:   string.Join(",", items)
来源：http://hz.snrcjt.cn/gtetpzvilj.html

[E09] 去除所有空白字符
来源：http://hz.birdmap.top/gtbistrwcl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.meibo888.top/gtmyjpztjl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.iojbl.cn/gtdkcvdogw.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.cucudq.cn/gtcqsafrls.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zhengqikj.top/gtqqrmktrk.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.xinyue.icu/gtjteqdggr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.bjfxy.top/gtsqijuvqg.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.dashuyun.cn/gtrmncrxeq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.andypj.xyz/gtykypmoxm.html

[E10] 左侧补零 / 定长填充
来源：http://hz.kuanghao11.cn/gtglgouflb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yuxming.cn/gtadsflgye.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.gaohongyu789.top/gtwbynftes.html

JS:   "7".padStart(3, "0")
来源：http://hz.jlsjyb.cn/gtulvvonkm.html

TS:   "7".padStart(3, "0")
来源：http://hz.nwbrower.top/gtxtsdzein.html

Java: String.format("%03d", 7)
来源：http://hz.xziqi.cn/gtwtinlxzm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.iojbl.cn/gtgjbxlmsq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.zhixingplan.top/gtpppxzzyt.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.quarkkingdee.top/gtlttdooqs.html

[E11] 反转字符串
来源：http://hz.aizwys.cn/gtzomjwuaz.html

Py:   s[::-1]
来源：http://hz.yonumen.top/gtivdtnuub.html

PHP:  strrev($s);
来源：http://hz.chenlongwang.top/gtubujckzp.html


<!-- 参考信息 -->