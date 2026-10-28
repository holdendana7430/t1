代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://hz.yanxiufei.cn/gtiznwsxzb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.daxiang520.top/gtmkflthed.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.guannengcc.top/gtetabtkzc.html

[D06] 数组长度
来源：http://hz.pycfn.com/gtkgkbvnbc.html

Py:   len(arr)
来源：http://hz.gzhubu.top/gtbgehtyob.html

PHP:  count($arr);
来源：http://hz.ppjwa.cn/gtvoikznia.html

JS:   arr.length
来源：http://hz.fengsongda.top/gtzbgnayjb.html

TS:   arr.length
来源：http://hz.xziqi.cn/gtfwnzkrid.html

Java: list.size();
来源：http://hz.andypj.xyz/gtayptdsnz.html

Go:   len(arr)
来源：http://hz.iojbl.cn/gtgalvnekl.html

Ruby: arr.length; arr.size
来源：http://hz.zdqjudy.top/gtfnnjtvpb.html

C#:   list.Count;
来源：http://hz.52xcode.cn/gtypfqppbo.html

[D07] 切片 / 取子数组
来源：http://hz.gogol.net.cn/gtgzenkxpt.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yj20258888.top/gtoztkuxac.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.shanyushiyangtech.top/gtkrdcmvfw.html

JS:   arr.slice(1, 4);
来源：http://hz.c1oappe.top/gttwdjfrti.html

TS:   arr.slice(1, 4);
来源：http://hz.jinghuilouyu.cn/gtwfyeqvmc.html

Java: list.subList(1, 4);
来源：http://hz.daria6918.cn/gtwhtltwpu.html

Go:   arr[1:4]
来源：http://hz.jyoumei.cn/gtbwymhtli.html

Ruby: arr[1, 3]
来源：http://hz.gotoacloud.top/gtahevtgfd.html

C#:   list.GetRange(1, 3);
来源：http://hz.yj202588.top/gtmjassbrz.html

[D08] 合并两个数组
来源：http://hz.wangdashe.top/gtblvcsnor.html

Py:   a + b;  a.extend(b)
来源：http://hz.cucudq.cn/gthvkouwcp.html

PHP:  array_merge($a, $b);
来源：http://hz.hywenlv.cn/gtxipmfbcp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.smart0.xyz/gtywurzguf.html

TS:   [...a, ...b];
来源：http://hz.zhiwuduotai.top/gtazmxurxn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.xuetiantiany.cn/gtrnejokxa.html

Go:   append(a, b...)
来源：http://hz.sufxvd.cn/gtvnppeysb.html

Ruby: a + b;  a.concat(b)
来源：http://hz.bjfxy.top/gtffoeigjj.html

C#:   a.Concat(b).ToList()
来源：http://hz.tanke756.top/gtbvlsbtff.html

[D09] 排序（升序）
来源：http://hz.yj202588.top/gtyqwansvr.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.redwolf501.top/gtnzjrtfei.html

PHP:  sort($arr);
来源：http://hz.aizwys.cn/gtprdphbch.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.jianghu66.top/gtpyzblduq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.shuidangran.top/gtcysidruq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.zhaomingkeji.xyz/gtpizfpebu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.fengsongda.top/gtqxhcfzcu.html

Ruby: arr.sort
来源：http://hz.yanxiufei.cn/gtpivbnzoc.html

C#:   list.Sort();
来源：http://hz.meibo888.top/gtiupdnvob.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.xuetiantiany.cn/gtsmtdtxdm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.hammf.cn/gtpthslumx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jinqigufen.top/gtxhyxpgvz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hysaishi.cn/gtgiatnqcj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.gotoacloud.top/gtqkivnttq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.aizwys.cn/gtjrcbglos.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yj202588.top/gtfegjqisq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.jianghu66.top/gtnfgheqjc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.redwolf501.top/gtstyozwse.html

[D11] 反转数组
来源：http://hz.ydjk.org.cn/gtbcfdvjfz.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.jlsjyb.cn/gtflhlamxr.html

PHP:  array_reverse($arr);
来源：http://hz.jinqigfzy.top/gtljxzeeff.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.svipenyu.cn/gtmqlffjgu.html

TS:   [...arr].reverse();
来源：http://hz.wangshuangyany.cn/gtqxxnjqex.html

Java: Collections.reverse(list);
来源：http://hz.yuxming.cn/gtosbslokl.html

Go:   slices.Reverse(arr)
来源：http://hz.gaohongyu789.top/gthxbouxqa.html

Ruby: arr.reverse
来源：http://hz.ywan-chungtsiang.top/gtracwkulu.html

C#:   list.Reverse();
来源：http://hz.yongpay.top/gtrlrkqnvr.html

[D12] 查找元素下标
来源：http://hz.hywenlv.cn/gtsjbsrfkk.html

Py:   arr.index(x);  x in arr
来源：http://hz.nanxuanxn.top/gtjacunayx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.hfpthk.cn/gtcuiakrdg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.xinyue.icu/gtsaghjxqd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.52xcode.cn/gttzeqiigh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.chenjidiqi.icu/gtvdvxemkx.html

Go:   slices.Index(arr, x)
来源：http://hz.hywenlv.cn/gtopnragzx.html

Ruby: arr.index(x)
来源：http://hz.kuanghao11.cn/gtzsjtdwcd.html

C#:   list.IndexOf(x);
来源：http://hz.smart0.xyz/gtfqncwjbd.html

[D13] 过滤（保留满足条件的）
来源：http://hz.cdnleiting.top/gtbayzvbyi.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.havefunace.top/gtsdwdanvm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.chenzaomai.com/gtefsyzstw.html

JS:   arr.filter(x => x > 3)
来源：http://hz.zhengqikj.top/gtnukgavlx.html

TS:   arr.filter(x => x > 3)
来源：http://hz.zycfv.cn/gtacekawha.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.gzhubu.top/gtfnpacnnp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yanxiufei.cn/gtovjwgjjo.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.haohaochexian.top/gtpzfxhlag.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.dashuyun.cn/gtoufcphus.html

[D14] 映射转换（每个元素变形）
来源：http://hz.52xcode.cn/gtkonmbsle.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.0kj1m.cn/gtjdxlqjmx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.316326.xyz/gtyhcwzdcx.html

JS:   arr.map(x => x * 2)
来源：http://hz.yj20258888.top/gtnuiqhxvm.html

TS:   arr.map(x => x * 2)
来源：http://hz.ywan-chungtsiang.top/gtimhastck.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.gaohongyu789.top/gtcpmyrhay.html

Go:   // 手写循环
来源：http://hz.sxryk.cn/gttwwhefpy.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.dianchejie.cn/gtkklvyhju.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.yongpay.top/gtcsvcrfmv.html

[D15] 去重
来源：http://hz.xuetiantiany.cn/gtjtlqwsnm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jlsjyb.cn/gtrjqtrard.html

PHP:  array_unique($arr);
来源：http://hz.xziqi.cn/gthpodzwzz.html

JS:   [...new Set(arr)]
来源：http://hz.haohaochexian.top/gtnaxaghuf.html

TS:   [...new Set(arr)]
来源：http://hz.shanyushiyangtech.top/gtgjrbomfe.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.guowangkeji.top/gtrpqklsen.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.wangdashe.top/gtravvbioz.html

Ruby: arr.uniq
来源：http://hz.iojbl.cn/gtrszfaoef.html

C#:   list.Distinct().ToList()
来源：http://hz.tianlin.xyz/gtohujaonw.html

[D16] 求和与平均值
来源：http://hz.cheryme.top/gtczuqxsqo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.shzxlz.cn/gtlgccttjg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.gogol.net.cn/gthpfqbvsu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.quarkkingdee.top/gtcblqyqew.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.fzhhl.top/gtbrncoroj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yuxming.cn/gtmmgramds.html

Go:   // 手写循环累加
来源：http://hz.ydjk.org.cn/gtspqyyalc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.nanxinkj.top/gtkyxtjapg.html

C#:   list.Sum();  list.Average()
来源：http://hz.hammf.cn/gtlokcjodv.html

[D17] 最大值与最小值
来源：http://hz.wangdashe.top/gtkwxbbdbh.html

Py:   max(arr);  min(arr)
来源：http://hz.cucudq.cn/gtedgoahnw.html

PHP:  max($arr);  min($arr);
来源：http://hz.daria6918.cn/gtwetaawpf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.cqqwz.cn/gtrixjhlle.html

TS:   Math.max(...arr);
来源：http://hz.zdqjudy.top/gtzxyzywgd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.feifeiyinyue.top/gtcwnjnuzs.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.mhx1999.top/gtqpoteuxr.html

Ruby: arr.max;  arr.min
来源：http://hz.zycfv.cn/gtjriodasq.html

C#:   list.Max();  list.Min()
来源：http://hz.shuidangran.top/gtrordyjqf.html

[D18] 扁平化嵌套数组
来源：http://hz.meibo888.top/gtqjcnajee.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.ybcxt.top/gtrapvfqck.html

PHP:  array_merge(...$nested);
来源：http://hz.andypj.xyz/gtkrpolawv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.cashguo.top/gthinpluff.html

TS:   nested.flat();
来源：http://hz.hfpthk.cn/gtqpnzqztv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.zhaomingkeji.xyz/gtaiobvlpd.html

Go:   // 手写双层循环
来源：http://hz.jianghu66.top/gtxvketgdq.html

Ruby: nested.flatten
来源：http://hz.zhengqikj.top/gtyocxleoz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.tian-w.cn/gtyvhkqopx.html

[D19] 按字段分组
来源：http://hz.shuidangran.top/gtwukxooks.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.feifeiyinyue.top/gtupzqirnu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.ivvv.top/gtrvlnyqro.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.tian-w.cn/gtdtxkjzlb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jinghuilouyu.cn/gtjzxwrdat.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.316326.xyz/gtnihqhttx.html

Go:   // 手写 map[string][]T
来源：http://hz.yonumen.top/gteleprrve.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.cheryme.top/gttgqfbmym.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.pycfn.com/gtjgfhvfym.html

[D20] 统计每个元素出现次数
来源：http://hz.birdmap.top/gtogxgzmzm.html

Py:   Counter(arr)
来源：http://hz.mhx1999.top/gtfeedsrtd.html

PHP:  array_count_values($arr);
来源：http://hz.9152youxi.cn/gtzofuezkv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hammf.cn/gtdeseseff.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.meibo888.top/gtfewtcowh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yvedp.cn/gtvqiyevjx.html

Go:   // 手写 map[T]int
来源：http://hz.smart0.xyz/gtbsbzgsox.html

Ruby: arr.tally
来源：http://hz.wangdashe.top/gtlwvlyxjr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.sufxvd.cn/gtryzbmuxw.html

[D21] 判断是否包含某元素
来源：http://hz.ivvv.top/gtdessmwam.html

Py:   x in arr
来源：http://hz.daxiang520.top/gtvwvgczpz.html

PHP:  in_array($x, $arr, true);
来源：http://hz.gzhubu.top/gtabkgctxh.html

JS:   arr.includes(x)
来源：http://hz.ywan-chungtsiang.top/gtksiucugl.html

TS:   arr.includes(x)
来源：http://hz.meibo888.top/gtlzzbogwo.html

Java: list.contains(x)
来源：http://hz.sxryk.cn/gtkmpttynf.html

Go:   slices.Contains(arr, x)
来源：http://hz.yueranfly.top/gteppfhcjk.html

Ruby: arr.include?(x)
来源：http://hz.jqgfzy.top/gtihkpezkp.html

C#:   list.Contains(x)
来源：http://hz.jinyuanbaomall.cn/gtoahqjywe.html

[D22] 复制数组（避免共享引用）
来源：http://hz.pycfn.com/gtuvpwsynl.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.xziqi.cn/gtaxevgiez.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.xziqi.cn/gtkaevctua.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.birdmap.top/gttnqntgft.html

TS:   [...arr];
来源：http://hz.cdnleiting.top/gtrplvirty.html

Java: new ArrayList<>(list);
来源：http://hz.shzxlz.cn/gtlswjyfeq.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.snrcjt.cn/gtepoefhmq.html

Ruby: arr.dup;  arr.clone
来源：http://hz.snrcjt.cn/gtvcjvjeid.html

C#:   new List<int>(list);
来源：http://hz.ppjwa.cn/gtwpvwdivt.html

[D23] reduce 累积计算
来源：http://hz.andypj.xyz/gtrzhligkf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jiagoushi.top/gtykvllscq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.jinyuanbaomall.cn/gtbnmyibgz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.andypj.xyz/gtyyqdkryl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.cheryme.top/gtgxczwrtf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.hywenlv.cn/gthvagjsyx.html

Go:   // 手写循环
来源：http://hz.ybcxt.top/gturofvobm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.wangdashe.top/gtcgrkphnu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.ydjk.org.cn/gtuainrhps.html

[D24] 字典 / Map 基本操作
来源：http://hz.sweek.top/gtyzplgwgv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.guannengcc.top/gtjfstudva.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.tanke756.top/gtjzqzvqwv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yonumen.top/gtpzgnpeph.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.hysaishi.cn/gtqruhwddc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.ydjk.org.cn/gtcnepliio.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.smart0.xyz/gtqufwzolu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.hnxiangtu.top/gthtghuxbv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.ehwqpu.com/gtvcggxqxc.html

[D25] Set 集合去重与交并差
来源：http://hz.316326.xyz/gtaddijkhw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.gotoacloud.top/gtcovsqhdi.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.kuanghao11.cn/gtvaagrxme.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.daxiang520.top/gtupjhdvbp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jqgfzy.top/gttxehtnau.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.nanxinkj.top/gtrxbxgnlp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.aizwys.cn/gthssermsg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.svipenyu.cn/gtdtcxgheb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.gzhubu.top/gtjrwcmwot.html

[D26] 数组转字符串
来源：http://hz.birdmap.top/gtjlhyhvhy.html

Py:   ", ".join(map(str, arr))
来源：http://hz.316326.xyz/gtyfccqfct.html

PHP:  implode(", ", $arr);
来源：http://hz.zhixingplan.top/gtptovakbh.html

JS:   arr.join(", ")
来源：http://hz.snrcjt.cn/gtxjyjmimv.html

TS:   arr.join(", ")
来源：http://hz.jlsjyb.cn/gtkhbsbexv.html

Java: String.join(", ", list)
来源：http://hz.ywan-chungtsiang.top/gtdhstbbmr.html

Go:   strings.Join(strs, ", ")
来源：http://hz.hywenlv.cn/gtzulaakyw.html

Ruby: arr.join(", ")
来源：http://hz.hysaishi.cn/gtvbanhnxx.html

C#:   string.Join(", ", list)
来源：http://hz.jinqigfzy.top/gtwdnbomym.html

================================================================================
来源：http://hz.haohaochexian.top/gtkdjjvyxo.html

E. 字符串处理
来源：http://hz.sweek.top/gtjnwmcumb.html

================================================================================
来源：http://hz.yanxiufei.cn/gtqfpwtmsy.html

[E01] 拼接字符串
来源：http://hz.jqgufenzy.top/gtsbafcpmi.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yj20258.top/gtagwrzgyg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.jyoumei.cn/gtfjkpwmhu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.haohaochexian.top/gtivmzufvl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.c1oappe.top/gtmlfvyzlu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.jinqigfzy.top/gtnilcbqxu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.jianghu66.top/gtwpvrbwyn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jqgfzy.top/gtszyxhdah.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.jiagoushi.top/gtotoextcj.html

[E02] 重复字符串
来源：http://hz.zdqjudy.top/gtnoardeij.html

Py:   "ab" * 3
来源：http://hz.hammf.cn/gtahcvhrwa.html

PHP:  str_repeat("ab", 3);
来源：http://hz.ehwqpu.com/gtrcggykvm.html

JS:   "ab".repeat(3)
来源：http://hz.smart0.xyz/gtxmwrzxzy.html

TS:   "ab".repeat(3)
来源：http://hz.jiagoushi.top/gtegocvndi.html

Java: "ab".repeat(3)
来源：http://hz.shangyingyoupin.top/gtkxuyhwvp.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.chenjidiqi.icu/gtsfebfdjy.html

Ruby: "ab" * 3
来源：http://hz.chenlongwang.top/gtfecxdykf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.chenjidiqi.icu/gtjgkkezcv.html

[E03] 截取子串
来源：http://hz.jianghu66.top/gtwfemljcs.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.fzhhl.top/gtlhapnunr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.9152youxi.cn/gtuqfvvich.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jianghu66.top/gtrazgfnfb.html

TS:   s.slice(1, 4)
来源：http://hz.hammf.cn/gtrxzaklia.html

Java: s.substring(1, 4)
来源：http://hz.cheryme.top/gtjoudszcs.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.feifeiyinyue.top/gtpxwmnhqf.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.jqgufenzy.top/gtgnojrnnf.html

C#:   s.Substring(1, 3)
来源：http://hz.daria6918.cn/gtafoqvqrx.html

[E04] 查找子串位置
来源：http://hz.sufxvd.cn/gtpghsyjuw.html

Py:   s.find("x");  s.index("x")
来源：http://hz.gzhubu.top/gtqgqltgcc.html

PHP:  strpos($s, "x");
来源：http://hz.shanyushiyangkeji.top/gtuyhevxja.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yj20258.top/gtnzcorbph.html

TS:   s.indexOf("x")
来源：http://hz.hammf.cn/gtozohpifl.html

Java: s.indexOf("x")
来源：http://hz.9152youxi.cn/gttjtyolhi.html

Go:   strings.Index(s, "x")
来源：http://hz.zhixingplan.top/gtxszgzdgs.html

Ruby: s.index("x")
来源：http://hz.yvedp.cn/gtblftvnvo.html

C#:   s.IndexOf("x")
来源：http://hz.shzxlz.cn/gtnwtirmkl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.shanyushiyangkeji.top/gtupcenytt.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.ybcxt.top/gtsvucbizf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.bjfxy.top/gtxsybuyam.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jinghuilouyu.cn/gtxofniubj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.andypj.xyz/gtlwigkjou.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.chenjidiqi.icu/gtxtrlpsnp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.zhiwuduotai.top/gtdkrwvynr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.xuanzx.com/gtahiseveu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.meibo888.top/gtlogyuhor.html

[E06] 替换子串
来源：http://hz.gotoacloud.top/gtaiivfopd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.gzhubu.top/gtzfseqixi.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.shzxlz.cn/gtttsedwaa.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.nanxinkj.top/gtzibisrjs.html

TS:   s.replaceAll("a", "b")
来源：http://hz.tianlin.xyz/gtozindubf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.pengpengdd.cyou/gtizyitpdt.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.cdnleiting.top/gtekotoids.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.zhoulong.xyz/gtrjrepgrk.html

C#:   s.Replace("a", "b")
来源：http://hz.zhengqikj.top/gtdqfrojkz.html

[E07] 按分隔符拆分
来源：http://hz.zhijiandao.cn/gtqvoqzvhu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.xylfe.cn/gtrqkxrzad.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.aibaodan.cn/gtnqbttjci.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.gotoacloud.top/gtigewevbw.html

TS:   s.split(",")
来源：http://hz.nanxuanxn.top/gthbxkysqw.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.wangshuangyany.cn/gtqywwwcnd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.daxiang520.top/gtelotdnvg.html

Ruby: s.split(",");  s.split
来源：http://hz.sysykeji.top/gtqvlqvbgq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.nanxinkj.top/gtymtwzvab.html

[E08] 数组按分隔符合并
来源：http://hz.gzhubu.top/gtlmsdrqst.html

Py:   ",".join(items)
来源：http://hz.zhoulong.xyz/gtcsskkygj.html

PHP:  implode(",", $items);
来源：http://hz.cashguo.top/gthcxwihpp.html

JS:   items.join(",")
来源：http://hz.hammf.cn/gtcbqhsajl.html

TS:   items.join(",")
来源：http://hz.cqqwz.cn/gtvylegibx.html

Java: String.join(",", items)
来源：http://hz.ywan-chungtsiang.top/gtdwaettrg.html

Go:   strings.Join(items, ",")
来源：http://hz.pengpengdd.cyou/gtekkrcquq.html

Ruby: items.join(",")
来源：http://hz.daxiang520.top/gtrpacmwng.html

C#:   string.Join(",", items)
来源：http://hz.hnxiangtu.top/gtdekjaxep.html

[E09] 去除所有空白字符
来源：http://hz.ppjwa.cn/gtatmhryyp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.snrcjt.cn/gtjpedvjpo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.xingfuxueyuan.xyz/gthoirgown.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.gaohongyu789.top/gtkbiatdna.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.nanxuanxn.top/gtvamedxdw.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jqgfzy.top/gtfoyboyar.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.sufxvd.cn/gtxlgrjxjq.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.feifeiyinyue.top/gthxwnoewh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.ppjwa.cn/gtxuolzsol.html

[E10] 左侧补零 / 定长填充
来源：http://hz.52xcode.cn/gtscgfoktr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.dianchejie.cn/gtojgbdsml.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.havefunace.top/gtfvphemwz.html

JS:   "7".padStart(3, "0")
来源：http://hz.52xcode.cn/gtmttyzqsi.html

TS:   "7".padStart(3, "0")
来源：http://hz.snrcjt.cn/gttahvdhba.html

Java: String.format("%03d", 7)
来源：http://hz.redwolf501.top/gtseumojqh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.fengsongda.top/gtbhkwbtac.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.jiagoushi.top/gtlqxpvxmp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.wangshuangyany.cn/gtlxegjhrt.html

[E11] 反转字符串
来源：http://hz.xylfe.cn/gtdzuhnvjs.html

Py:   s[::-1]
来源：http://hz.xylfe.cn/gtijwijglt.html

PHP:  strrev($s);
来源：http://hz.ppjwa.cn/gtiicjjftx.html

JS:   [...s].reverse().join("")
来源：http://hz.andypj.xyz/gtblerjefx.html

TS:   [...s].reverse().join("")
来源：http://hz.ehwqpu.com/gtxupmjzrm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jianghu66.top/gtqeowfjzo.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.tanke756.top/gtblkakqwe.html

Ruby: s.reverse
来源：http://hz.zhongyouzk.top/gtltodofvv.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yueranfly.top/gtucpxaphz.html

[E12] 统计某字符出现次数
来源：http://hz.aizwys.cn/gtkjcvjqdm.html

Py:   s.count("a")
来源：http://hz.hfpthk.cn/gtwnbzgqvd.html

PHP:  substr_count($s, "a");
来源：http://hz.daxiang520.top/gtupjnlypx.html

JS:   s.split("a").length - 1
来源：http://hz.birdmap.top/gtxuaunitx.html

TS:   s.split("a").length - 1
来源：http://hz.ivvv.top/gttgmifjge.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yonumen.top/gtapkugbus.html


<!-- 参考信息 -->