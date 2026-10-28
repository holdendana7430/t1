代发 wailian999

C#:   list.Insert(0, 0);
来源：http://hz.chenjidiqi.icu/gtlupwmvlq.html

[D04] 删除元素
来源：http://hz.0kj1m.cn/gtmmcigcst.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.gzhubu.top/gtufuvaauo.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yanxiufei.cn/gtgsdwsstd.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.aizwys.cn/gtiveymrlc.html

TS:   arr.splice(0, 1);
来源：http://hz.hnxiangtu.top/gtryiccuhm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.iojbl.cn/gtscifagdn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.hfpthk.cn/gtowdcrxxe.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.nanxinkj.top/gtsahxirpv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.jinqigufen.top/gtprvierlo.html

[D05] 访问与修改元素
来源：http://hz.guannengcc.top/gtzyobokqb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.snrcjt.cn/gtchglacva.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.yanxiufei.cn/gtqpqooifq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.hywenlv.cn/gtwueuetjg.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.jlsjyb.cn/gttmrzhlvg.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.snrcjt.cn/gtlcbedwnj.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.gogol.net.cn/gtlvoekdpt.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jiagoushi.top/gthxkapgvq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.haohaochexian.top/gthegcjsuk.html

[D06] 数组长度
来源：http://hz.zhijiandao.cn/gtewznyend.html

Py:   len(arr)
来源：http://hz.ehwqpu.com/gtewoysaoe.html

PHP:  count($arr);
来源：http://hz.nanxinkj.top/gtuipjolee.html

JS:   arr.length
来源：http://hz.andypj.xyz/gtyfxdgwdy.html

TS:   arr.length
来源：http://hz.sysykeji.top/gteviavzrb.html

Java: list.size();
来源：http://hz.daxiang520.top/gtzymnysbe.html

Go:   len(arr)
来源：http://hz.tian-w.cn/gtuudzuixz.html

Ruby: arr.length; arr.size
来源：http://hz.chenzaomai.com/gtfwpvngab.html

C#:   list.Count;
来源：http://hz.pycfn.com/gtagethacy.html

[D07] 切片 / 取子数组
来源：http://hz.dashuyun.cn/gtmwatigne.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yongpay.top/gtbheaihnw.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zhengqikj.top/gtgzwgdnxn.html

JS:   arr.slice(1, 4);
来源：http://hz.xuetiantiany.cn/gtjdgabbls.html

TS:   arr.slice(1, 4);
来源：http://hz.hongshengwenyu.top/gtcywxuprd.html

Java: list.subList(1, 4);
来源：http://hz.hnqzz.top/gtywlgaqfr.html

Go:   arr[1:4]
来源：http://hz.ivvv.top/gtmkldrsca.html

Ruby: arr[1, 3]
来源：http://hz.shuidangran.top/gtqircyord.html

C#:   list.GetRange(1, 3);
来源：http://hz.redwolf501.top/gtjahotdat.html

[D08] 合并两个数组
来源：http://hz.andypj.xyz/gtdtlusrfv.html

Py:   a + b;  a.extend(b)
来源：http://hz.nwbrower.top/gtnsqrwbqy.html

PHP:  array_merge($a, $b);
来源：http://hz.jinqigufen.top/gtbyxfcfso.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jinyuanbaomall.cn/gtuqfrpols.html

TS:   [...a, ...b];
来源：http://hz.hysaishi.cn/gtwlazvwbz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.xuanzx.com/gtthcahyvf.html

Go:   append(a, b...)
来源：http://hz.sweek.top/gtrxydxqyw.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yueranfly.top/gtcieacfek.html

C#:   a.Concat(b).ToList()
来源：http://hz.hnxiangtu.top/gtgwhjyvwn.html

[D09] 排序（升序）
来源：http://hz.mhx1999.top/gtlyfdqyqg.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yvedp.cn/gtmnojcwqs.html

PHP:  sort($arr);
来源：http://hz.yj20258888.top/gtyzlyjnpc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.meibo888.top/gtabisebwf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.gzhubu.top/gtyqmyuvxq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yanxiufei.cn/gtammdueze.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.chenzaomai.com/gtjebrshfx.html

Ruby: arr.sort
来源：http://hz.gaohongyu789.top/gtepdjbjlp.html

C#:   list.Sort();
来源：http://hz.yonumen.top/gtorziafkn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zhaomingkeji.xyz/gtzkcbepos.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.daria6918.cn/gtlovcfzob.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.316326.xyz/gtohywnryd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jinqigufen.top/gtfjijslcm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhixingplan.top/gtrohpevpf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jinqigufen.top/gtygabbfyt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.daxiang520.top/gtvelkuriq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.tian-w.cn/gtgzazhvqt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.cheryme.top/gthwwmrypr.html

[D11] 反转数组
来源：http://hz.dianchejie.cn/gtntoyffsy.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.dianchejie.cn/gtcpwbbzfg.html

PHP:  array_reverse($arr);
来源：http://hz.nanxuanxn.top/gtspfxbnvl.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.cdnleiting.top/gtmkluwifz.html

TS:   [...arr].reverse();
来源：http://hz.snrcjt.cn/gtxpketmxg.html

Java: Collections.reverse(list);
来源：http://hz.yuanzhike.top/gtctdkkfkb.html

Go:   slices.Reverse(arr)
来源：http://hz.xuetiantiany.cn/gtlblxguer.html

Ruby: arr.reverse
来源：http://hz.kuanghao11.cn/gtdoccvafh.html

C#:   list.Reverse();
来源：http://hz.yuanzhike.top/gthldjaxjn.html

[D12] 查找元素下标
来源：http://hz.zhijiandao.cn/gtmppyvonm.html

Py:   arr.index(x);  x in arr
来源：http://hz.iojbl.cn/gtcxbybrrx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.tian-w.cn/gtogiqkopc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ydjk.org.cn/gtpeszfjrb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ppjwa.cn/gtulgljseh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.0kj1m.cn/gtsztdkgda.html

Go:   slices.Index(arr, x)
来源：http://hz.guowangkeji.top/gtephykqke.html

Ruby: arr.index(x)
来源：http://hz.cheryme.top/gtxzbazcfm.html

C#:   list.IndexOf(x);
来源：http://hz.0kj1m.cn/gthygnmbct.html

[D13] 过滤（保留满足条件的）
来源：http://hz.andypj.xyz/gtidbbvczs.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.jqgfzy.top/gtesprrgnb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.hysaishi.cn/gtjfjzlgyd.html

JS:   arr.filter(x => x > 3)
来源：http://hz.hnqzz.top/gtflokvpls.html

TS:   arr.filter(x => x > 3)
来源：http://hz.ybcxt.top/gtokpxixkk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.shanyushiyangtech.top/gtafujkgqu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.cqqwz.cn/gtqoeuuebn.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.guowangkeji.top/gtzsvgeqng.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jianghu66.top/gthqxxzukq.html

[D14] 映射转换（每个元素变形）
来源：http://hz.ydjk.org.cn/gtnidzztap.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ydjk.org.cn/gtnwgfoboh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.chenjidiqi.icu/gtelvujpyg.html

JS:   arr.map(x => x * 2)
来源：http://hz.gaohongyu789.top/gtpzgscbww.html

TS:   arr.map(x => x * 2)
来源：http://hz.shanyushiyangtech.top/gtzwhqjsjm.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.xziqi.cn/gtrdjcvijl.html

Go:   // 手写循环
来源：http://hz.xylfe.cn/gtnwugwmjz.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.pycfn.com/gtuctufqjp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.meibo888.top/gtobmjbxfh.html

[D15] 去重
来源：http://hz.0kj1m.cn/gtwrbpaajf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jinyuanbaomall.cn/gtlxlzpmak.html

PHP:  array_unique($arr);
来源：http://hz.guannengcc.top/gtrehlwggr.html

JS:   [...new Set(arr)]
来源：http://hz.redwolf501.top/gtxupqexha.html

TS:   [...new Set(arr)]
来源：http://hz.svipenyu.cn/gtnhtmxjyq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.zhoulong.xyz/gtulplwaam.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.52xcode.cn/gtsnfkzjxv.html

Ruby: arr.uniq
来源：http://hz.zhijiandao.cn/gtwppqndmc.html

C#:   list.Distinct().ToList()
来源：http://hz.hammf.cn/gtulsrkvfv.html

[D16] 求和与平均值
来源：http://hz.daria6918.cn/gtvphulkmp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.gzhubu.top/gtifyahwmn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.andypj.xyz/gtdsqftywh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.nanxinkj.top/gtdiiayorc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cqqwz.cn/gtbovlrhig.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.feifeiyinyue.top/gtpxjlqixx.html

Go:   // 手写循环累加
来源：http://hz.gzhubu.top/gtidpavfcw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.meibo888.top/gtgrlvofvi.html

C#:   list.Sum();  list.Average()
来源：http://hz.xuetiantiany.cn/gtshoenmep.html

[D17] 最大值与最小值
来源：http://hz.hnxiangtu.top/gttvkoupdp.html

Py:   max(arr);  min(arr)
来源：http://hz.haohaochexian.top/gtvmgfqdys.html

PHP:  max($arr);  min($arr);
来源：http://hz.pycfn.com/gtkcovhifm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.9152youxi.cn/gtwxqvvjca.html

TS:   Math.max(...arr);
来源：http://hz.gaohongyu789.top/gtkmxxfdao.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.gzhubu.top/gtxscxkblf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.cheryme.top/gtjerfhycp.html

Ruby: arr.max;  arr.min
来源：http://hz.pycfn.com/gtleqygrok.html

C#:   list.Max();  list.Min()
来源：http://hz.shangyingyoupin.top/gtufhdmeyw.html

[D18] 扁平化嵌套数组
来源：http://hz.tanke756.top/gtdbpmoubu.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.aibaodan.cn/gtknfdwhwl.html

PHP:  array_merge(...$nested);
来源：http://hz.pengpengdd.cyou/gtcbyazcab.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.ybcxt.top/gttdvrkjie.html

TS:   nested.flat();
来源：http://hz.mhx1999.top/gtwcaoejwr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.dashuyun.cn/gtqgfftnoq.html

Go:   // 手写双层循环
来源：http://hz.shanyushiyangkeji.top/gtadoynbwu.html

Ruby: nested.flatten
来源：http://hz.52xcode.cn/gtnnilkqrq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.cheryme.top/gtsobgbmbq.html

[D19] 按字段分组
来源：http://hz.52xcode.cn/gtstijawuz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yonumen.top/gtakaymdqn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.chenzaomai.com/gtwsskdyum.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.tianlin.xyz/gtqeszjrzl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.316326.xyz/gtpuvxdudx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.hnqzz.top/gttcbibute.html

Go:   // 手写 map[string][]T
来源：http://hz.yangfankeji.com/gtjklyeewj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.gogol.net.cn/gtrubdrzkh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.shanyushiyangtech.top/gtyetlyshq.html

[D20] 统计每个元素出现次数
来源：http://hz.hysaishi.cn/gtsoniejat.html

Py:   Counter(arr)
来源：http://hz.hnqzz.top/gtjcnqwvks.html

PHP:  array_count_values($arr);
来源：http://hz.mhx1999.top/gtooridubn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jinghuilouyu.cn/gtrbfcbwdy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xylfe.cn/gtbpjyubkx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.iojbl.cn/gtuxjuwusx.html

Go:   // 手写 map[T]int
来源：http://hz.tian-w.cn/gtmvlqgmjl.html

Ruby: arr.tally
来源：http://hz.c1oappe.top/gtsulgrsvu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.shanyushiyangkeji.top/gtogyiwtxf.html

[D21] 判断是否包含某元素
来源：http://hz.nanxinkj.top/gtoxsmdewi.html

Py:   x in arr
来源：http://hz.yj202588.top/gtptfdrasf.html

PHP:  in_array($x, $arr, true);
来源：http://hz.haohaochexian.top/gtyjgerrzd.html

JS:   arr.includes(x)
来源：http://hz.9152youxi.cn/gtaiyaodku.html

TS:   arr.includes(x)
来源：http://hz.chenzaomai.com/gtgmiylwso.html

Java: list.contains(x)
来源：http://hz.cdnleiting.top/gtsqjyluus.html

Go:   slices.Contains(arr, x)
来源：http://hz.jinqigufen.top/gtbogrnldv.html

Ruby: arr.include?(x)
来源：http://hz.shangyingyoupin.top/gtangxijpq.html

C#:   list.Contains(x)
来源：http://hz.yj20258.top/gtzdocxlck.html

[D22] 复制数组（避免共享引用）
来源：http://hz.chenjidiqi.icu/gtyfmqhvsq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.ppjwa.cn/gtmszkluld.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.316326.xyz/gtirfvdluf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yonumen.top/gtwjjycaeu.html

TS:   [...arr];
来源：http://hz.yj202588.top/gtunuvktxr.html

Java: new ArrayList<>(list);
来源：http://hz.ybcxt.top/gtbizgbkaj.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.tian-w.cn/gtrsrhmjbp.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jianghu66.top/gtxoqtbrfv.html

C#:   new List<int>(list);
来源：http://hz.quarkkingdee.top/gtjrfvlypn.html

[D23] reduce 累积计算
来源：http://hz.tianlin.xyz/gtbvxeovev.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jqgufenzy.top/gtgozpeylf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yj20258.top/gtefqvoczo.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.redwolf501.top/gtjwovbmaa.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.haohaochexian.top/gtfnarilha.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.tianlin.xyz/gtnuypypsn.html

Go:   // 手写循环
来源：http://hz.feifeiyinyue.top/gtxapffjcj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.redwolf501.top/gthqzhfpaj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yongpay.top/gtzpnndvno.html

[D24] 字典 / Map 基本操作
来源：http://hz.shangyingyoupin.top/gtsczqdzdj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.tanke756.top/gtknrlhqiq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yanxiufei.cn/gthhzxydgs.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yongpay.top/gtkfuyndby.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.nwbrower.top/gtkbamuszj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.jinyuanbaomall.cn/gtqwjzisye.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.52xcode.cn/gtrfawlycq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.shzxlz.cn/gtproqzzaw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.gaohongyu789.top/gtsjmthwqt.html

[D25] Set 集合去重与交并差
来源：http://hz.snrcjt.cn/gtgaadkgre.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.svipenyu.cn/gtftvzrdjo.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.meibo888.top/gtpstvqudk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.hfpthk.cn/gtfayuftmw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.pengpengdd.cyou/gtwmimqghk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.tian-w.cn/gtqguqkskp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.dianchejie.cn/gtnkdtjpiv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.sweek.top/gtyzaffmju.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.redwolf501.top/gtarssiinn.html

[D26] 数组转字符串
来源：http://hz.gogol.net.cn/gtzfalctsf.html

Py:   ", ".join(map(str, arr))
来源：http://hz.shzxlz.cn/gtasjksmzw.html

PHP:  implode(", ", $arr);
来源：http://hz.guowangkeji.top/gtftgndvee.html

JS:   arr.join(", ")
来源：http://hz.svipenyu.cn/gtjvlptukb.html

TS:   arr.join(", ")
来源：http://hz.gogol.net.cn/gtkgrlbapi.html

Java: String.join(", ", list)
来源：http://hz.guowangkeji.top/gtjiykcocs.html

Go:   strings.Join(strs, ", ")
来源：http://hz.xingfuxueyuan.xyz/gtfhwumldz.html

Ruby: arr.join(", ")
来源：http://hz.xuanzx.com/gtdirptkrx.html

C#:   string.Join(", ", list)
来源：http://hz.gotoacloud.top/gtrbolifox.html

================================================================================
来源：http://hz.redwolf501.top/gtecctfwgw.html

E. 字符串处理
来源：http://hz.snrcjt.cn/gtucncjlho.html

================================================================================
来源：http://hz.yj20258888.top/gtlwxmcojt.html

[E01] 拼接字符串
来源：http://hz.ppjwa.cn/gtxdzopili.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.hnxiangtu.top/gtwptzukfm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.meibo888.top/gtypsdnmaa.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yanxiufei.cn/gtbxywbkqz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.nwbrower.top/gtkxjoymds.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.bjfxy.top/gtooysnalh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.zhengqikj.top/gtoaqgluoc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yonumen.top/gtfcmfvuca.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zhengqikj.top/gtjhdpwooz.html

[E02] 重复字符串
来源：http://hz.jinyuanbaomall.cn/gtmuelpbgs.html

Py:   "ab" * 3
来源：http://hz.hnqzz.top/gtsgkwsokj.html

PHP:  str_repeat("ab", 3);
来源：http://hz.9152youxi.cn/gtnwjqzmuj.html

JS:   "ab".repeat(3)
来源：http://hz.nanxinkj.top/gtgafrdqip.html

TS:   "ab".repeat(3)
来源：http://hz.wangdashe.top/gtlmhyxzni.html

Java: "ab".repeat(3)
来源：http://hz.yj202588.top/gtygpytpir.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.jiagoushi.top/gtdgwhbgpy.html

Ruby: "ab" * 3
来源：http://hz.nwbrower.top/gtmaqaijpa.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yj202588.top/gtsakrzybo.html

[E03] 截取子串
来源：http://hz.zhongyouzk.top/gtircdhifd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.havefunace.top/gthghjnhsz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.yonumen.top/gtgyomtasd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.birdmap.top/gtivckwoyy.html

TS:   s.slice(1, 4)
来源：http://hz.jiagoushi.top/gtcrvyvtws.html

Java: s.substring(1, 4)
来源：http://hz.quarkkingdee.top/gtwvpraaab.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yj20258.top/gtusbvdpkg.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.ppjwa.cn/gtlulzjnno.html

C#:   s.Substring(1, 3)
来源：http://hz.birdmap.top/gtorsbhrdy.html

[E04] 查找子串位置
来源：http://hz.fengsongda.top/gtxdvbamey.html

Py:   s.find("x");  s.index("x")
来源：http://hz.chenlongwang.top/gtxkowbkci.html

PHP:  strpos($s, "x");
来源：http://hz.wangshuangyany.cn/gtbmknldjy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yvedp.cn/gtrslwgqqx.html

TS:   s.indexOf("x")
来源：http://hz.svipenyu.cn/gtitnxhcat.html

Java: s.indexOf("x")
来源：http://hz.wangshuangyany.cn/gtxcvsmlgc.html

Go:   strings.Index(s, "x")
来源：http://hz.zhiwuduotai.top/gtbsylvbnj.html

Ruby: s.index("x")
来源：http://hz.jqgufenzy.top/gtxtfutvbe.html

C#:   s.IndexOf("x")
来源：http://hz.guannengcc.top/gttiammvbg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.hammf.cn/gtfrkxumef.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.yonumen.top/gtwjkshbfn.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.mhx1999.top/gthbrvfuqp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.wangshuangyany.cn/gtcgydqnch.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.daria6918.cn/gttlwmrqjf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.pengpengdd.cyou/gtnwgcvjuv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.xinyue.icu/gtgiuxxaoi.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.gzhubu.top/gtgqgbnlqs.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.chenlongwang.top/gttdofmnuy.html

[E06] 替换子串
来源：http://hz.hammf.cn/gtusaanlnl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.svipenyu.cn/gtzlaseitj.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.yonumen.top/gtoxtaocmh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hfpthk.cn/gtbgcewirq.html

TS:   s.replaceAll("a", "b")
来源：http://hz.xylfe.cn/gtvpjjoape.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.aibaodan.cn/gtxaoiaipo.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.andypj.xyz/gtbsirqmfl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.ivvv.top/gtnftrqzuc.html

C#:   s.Replace("a", "b")
来源：http://hz.gotoacloud.top/gtmbladxhk.html

[E07] 按分隔符拆分
来源：http://hz.pengpengdd.cyou/gtdoxkauhr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yonumen.top/gtrqpvludq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.chenzaomai.com/gtwwwilqlx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yuanzhike.top/gtbrjgrhhm.html

TS:   s.split(",")
来源：http://hz.ehwqpu.com/gtkiuxtkbg.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.zhaomingkeji.xyz/gtbkimxmof.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.hywenlv.cn/gtipzrztma.html

Ruby: s.split(",");  s.split
来源：http://hz.daria6918.cn/gthnnspqsi.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.gaohongyu789.top/gtjiwpbyuz.html

[E08] 数组按分隔符合并
来源：http://hz.316326.xyz/gtbjjehobx.html

Py:   ",".join(items)
来源：http://hz.jianghu66.top/gtobwhmijo.html

PHP:  implode(",", $items);
来源：http://hz.daxiang520.top/gtpkshycfh.html

JS:   items.join(",")
来源：http://hz.ivvv.top/gtqitkuqxh.html

TS:   items.join(",")
来源：http://hz.fengsongda.top/gtqxbhjiyv.html

Java: String.join(",", items)
来源：http://hz.xuetiantiany.cn/gtkiftgndv.html

Go:   strings.Join(items, ",")
来源：http://hz.jinqigufen.top/gtbjpniksc.html

Ruby: items.join(",")
来源：http://hz.tian-w.cn/gtjutsukiq.html

C#:   string.Join(",", items)
来源：http://hz.jiagoushi.top/gtcbpzpcol.html

[E09] 去除所有空白字符
来源：http://hz.shzxlz.cn/gtxmmylekl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.cashguo.top/gtbufzwhzb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.shangyingyoupin.top/gtoavvprin.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.cqqwz.cn/gtwsdrxogn.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.feifeiyinyue.top/gttspdqjig.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.sufxvd.cn/gtygcrdxkr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.xuetiantiany.cn/gtsioxgkja.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.tian-w.cn/gtklgqddov.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.smart0.xyz/gtxmanciev.html

[E10] 左侧补零 / 定长填充
来源：http://hz.shangyingyoupin.top/gtcodnnivi.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.52xcode.cn/gtvllosdtc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.aizwys.cn/gtmixugnxy.html

JS:   "7".padStart(3, "0")
来源：http://hz.jiagoushi.top/gtgvzywvoq.html

TS:   "7".padStart(3, "0")
来源：http://hz.gotoacloud.top/gtemqbhcqu.html

Java: String.format("%03d", 7)
来源：http://hz.xuanzx.com/gtptdnnrhu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.xuetiantiany.cn/gtgzkgsduv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.ivvv.top/gtycgieujf.html


<!-- 参考信息 -->