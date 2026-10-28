代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://hz.xinyue.icu/gtpcbjlcaf.html

Java: list.add(0, 0);
来源：http://hz.ybcxt.top/gtvsrgobve.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.shzxlz.cn/gtcqpzogvp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.wangdashe.top/gtvvznrbij.html

C#:   list.Insert(0, 0);
来源：http://hz.redwolf501.top/gtegxwjjmg.html

[D04] 删除元素
来源：http://hz.c1oappe.top/gtxwxbbvsm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.yj20258888.top/gtkggmrlhv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.gogol.net.cn/gtssbijftv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.ppjwa.cn/gtoofrstdo.html

TS:   arr.splice(0, 1);
来源：http://hz.yanxiufei.cn/gtihsanenx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.fengsongda.top/gtteflvcsr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yuanzhike.top/gteqcovmvz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.hongshengwenyu.top/gttkhqrqnn.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.fengsongda.top/gtdizhajad.html

[D05] 访问与修改元素
来源：http://hz.zdqjudy.top/gttwejsxnr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.snrcjt.cn/gtbhmrqcgg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.zycfv.cn/gtcbgchidf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.cheryme.top/gtsqugnahl.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.xylfe.cn/gtorgeutal.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.chenlongwang.top/gtqqlilujv.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.xuanzx.com/gtpdknittr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.gotoacloud.top/gtfbkciwgs.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.hfpthk.cn/gtnyffiojx.html

[D06] 数组长度
来源：http://hz.aizwys.cn/gtoajxvfci.html

Py:   len(arr)
来源：http://hz.svipenyu.cn/gtvciilhzx.html

PHP:  count($arr);
来源：http://hz.fzhhl.top/gtnbzdlqcw.html

JS:   arr.length
来源：http://hz.nanxuanxn.top/gtnwikxsft.html

TS:   arr.length
来源：http://hz.nwbrower.top/gtrjsyrmze.html

Java: list.size();
来源：http://hz.ehwqpu.com/gtvnutjrvt.html

Go:   len(arr)
来源：http://hz.zdqjudy.top/gtencjwhol.html

Ruby: arr.length; arr.size
来源：http://hz.cheryme.top/gtwsgpvoeg.html

C#:   list.Count;
来源：http://hz.jqgufenzy.top/gtnpdwtcre.html

[D07] 切片 / 取子数组
来源：http://hz.zhoulong.xyz/gtpkmlzbnm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.fengsongda.top/gtnejfzgyl.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.jyoumei.cn/gttnojdjrq.html

JS:   arr.slice(1, 4);
来源：http://hz.yangfankeji.com/gtaqmhwrjs.html

TS:   arr.slice(1, 4);
来源：http://hz.iojbl.cn/gtpjbkfmfl.html

Java: list.subList(1, 4);
来源：http://hz.jinghuilouyu.cn/gtbeodyllq.html

Go:   arr[1:4]
来源：http://hz.52xcode.cn/gttoingtyb.html

Ruby: arr[1, 3]
来源：http://hz.aizwys.cn/gtkamwpdty.html

C#:   list.GetRange(1, 3);
来源：http://hz.yuanzhike.top/gtyggcnzlh.html

[D08] 合并两个数组
来源：http://hz.ybcxt.top/gtnybxxwus.html

Py:   a + b;  a.extend(b)
来源：http://hz.tianlin.xyz/gtmedfucqy.html

PHP:  array_merge($a, $b);
来源：http://hz.shanyushiyangtech.top/gtfbrevyzr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.sweek.top/gtilzgqdaz.html

TS:   [...a, ...b];
来源：http://hz.yj20258.top/gthxkktmap.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.sweek.top/gtqvdregfe.html

Go:   append(a, b...)
来源：http://hz.smart0.xyz/gtvkaagagw.html

Ruby: a + b;  a.concat(b)
来源：http://hz.kuanghao11.cn/gtsabwqkzw.html

C#:   a.Concat(b).ToList()
来源：http://hz.hammf.cn/gtyydrspjd.html

[D09] 排序（升序）
来源：http://hz.jinqigufen.top/gthfyvbyao.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ehwqpu.com/gtdoialflw.html

PHP:  sort($arr);
来源：http://hz.xylfe.cn/gtyepofslo.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.snrcjt.cn/gtezzsogbk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.nwbrower.top/gtqrwumchu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.xylfe.cn/gteplqmmdv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.kuanghao11.cn/gtrwojmyvt.html

Ruby: arr.sort
来源：http://hz.smart0.xyz/gtsfaumzqb.html

C#:   list.Sort();
来源：http://hz.haohaochexian.top/gtodfwfcot.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.iojbl.cn/gtlucbqocq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.hongshengwenyu.top/gtjquwxhch.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.xinyue.icu/gtucqwtmqs.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.tanke756.top/gtjafccozw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.c1oappe.top/gtldczvvaf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jinyuanbaomall.cn/gtgfseoazu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.cheryme.top/gtztqhrnqw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.gotoacloud.top/gttyhfwpfc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.dashuyun.cn/gtmykuqnan.html

[D11] 反转数组
来源：http://hz.yj20258.top/gtbwxfiqmh.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.cashguo.top/gtjfvaytkb.html

PHP:  array_reverse($arr);
来源：http://hz.ydzc1.top/gtyqpgujog.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.daxiang520.top/gtzlhehjwr.html

TS:   [...arr].reverse();
来源：http://hz.nanxuanxn.top/gtgrlicqcx.html

Java: Collections.reverse(list);
来源：http://hz.shuidangran.top/gtspdpzlhi.html

Go:   slices.Reverse(arr)
来源：http://hz.yj20258888.top/gtyfpvcwvj.html

Ruby: arr.reverse
来源：http://hz.iojbl.cn/gtiltlemrx.html

C#:   list.Reverse();
来源：http://hz.andypj.xyz/gtwwerpnwg.html

[D12] 查找元素下标
来源：http://hz.yangfankeji.com/gtovspgnxl.html

Py:   arr.index(x);  x in arr
来源：http://hz.gotoacloud.top/gtwdsgokhm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.ivvv.top/gthtqxqpqa.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.xuanzx.com/gtyfdikcyq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhixingplan.top/gtqhrprkil.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.316326.xyz/gttbkbmdgz.html

Go:   slices.Index(arr, x)
来源：http://hz.gaohongyu789.top/gtofxofocz.html

Ruby: arr.index(x)
来源：http://hz.nanxuanxn.top/gtddrcoywh.html

C#:   list.IndexOf(x);
来源：http://hz.jinyuanbaomall.cn/gtloqyuadl.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zycfv.cn/gtybsiyjzj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.xingfuxueyuan.xyz/gtanebpjid.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.guannengcc.top/gtoseyjfke.html

JS:   arr.filter(x => x > 3)
来源：http://hz.ywan-chungtsiang.top/gtfzlpnijb.html

TS:   arr.filter(x => x > 3)
来源：http://hz.cqqwz.cn/gtnzxgnaen.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.cdnleiting.top/gtjubvsxhg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.gzhubu.top/gtmngnnhvv.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.dianchejie.cn/gtmfrplhox.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.iojbl.cn/gtdgxmyhfm.html

[D14] 映射转换（每个元素变形）
来源：http://hz.ydjk.org.cn/gtzxurtfbs.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ywan-chungtsiang.top/gtbvdceyjz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.bjfxy.top/gtsatloftf.html

JS:   arr.map(x => x * 2)
来源：http://hz.9152youxi.cn/gtcxexwhwg.html

TS:   arr.map(x => x * 2)
来源：http://hz.yj202588.top/gtnznhbuvn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.gogol.net.cn/gtuyfahdcz.html

Go:   // 手写循环
来源：http://hz.xinyue.icu/gtvggcoelt.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.shanyushiyangtech.top/gtaupulvec.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.dashuyun.cn/gtwhuehpfn.html

[D15] 去重
来源：http://hz.jqgfzy.top/gteollzerr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.hnxiangtu.top/gtmikcfyjq.html

PHP:  array_unique($arr);
来源：http://hz.pengpengdd.cyou/gtncvzjbmh.html

JS:   [...new Set(arr)]
来源：http://hz.zhoulong.xyz/gtnnzwvkqy.html

TS:   [...new Set(arr)]
来源：http://hz.xingfuxueyuan.xyz/gtplbbnefh.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yonumen.top/gtnikwzqdl.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.ybcxt.top/gtzhjpvnes.html

Ruby: arr.uniq
来源：http://hz.shangyingyoupin.top/gtecdedbvr.html

C#:   list.Distinct().ToList()
来源：http://hz.sweek.top/gtydomtcdk.html

[D16] 求和与平均值
来源：http://hz.gaohongyu789.top/gtmjtvobmw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.aibaodan.cn/gtgynpvbqn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.zhongyouzk.top/gtfntzgeqg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ppjwa.cn/gtzljdubcu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.tanke756.top/gtmdtkkjbs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.sufxvd.cn/gtzvjuqddw.html

Go:   // 手写循环累加
来源：http://hz.hysaishi.cn/gtxivvqnvl.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.cqqwz.cn/gtedfucugc.html

C#:   list.Sum();  list.Average()
来源：http://hz.xziqi.cn/gtirngcvzn.html

[D17] 最大值与最小值
来源：http://hz.shanyushiyangkeji.top/gtxsogcphy.html

Py:   max(arr);  min(arr)
来源：http://hz.jyoumei.cn/gteeqbtasj.html

PHP:  max($arr);  min($arr);
来源：http://hz.nwbrower.top/gtgsajemep.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.zhengqikj.top/gtjbuhlsld.html

TS:   Math.max(...arr);
来源：http://hz.chenlongwang.top/gtutcwjgxg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jiagoushi.top/gtebmmgmdk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.tianlin.xyz/gthinlifgl.html

Ruby: arr.max;  arr.min
来源：http://hz.fengsongda.top/gtyzvjajkq.html

C#:   list.Max();  list.Min()
来源：http://hz.nanxinkj.top/gtpkgewlkz.html

[D18] 扁平化嵌套数组
来源：http://hz.andypj.xyz/gtmydkezhq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.jinyuanbaomall.cn/gtxubdnfxk.html

PHP:  array_merge(...$nested);
来源：http://hz.jiagoushi.top/gtqpvkoipc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.jqgfzy.top/gtdgpatcio.html

TS:   nested.flat();
来源：http://hz.havefunace.top/gtexvbvlsx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.svipenyu.cn/gticqqkcav.html

Go:   // 手写双层循环
来源：http://hz.fengsongda.top/gtfwhjepvc.html

Ruby: nested.flatten
来源：http://hz.birdmap.top/gtiitoasee.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.cheryme.top/gtrtrhzzlk.html

[D19] 按字段分组
来源：http://hz.316326.xyz/gtplzngllw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.mhx1999.top/gtveveqzbb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.zhaomingkeji.xyz/gtogtrhxfp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jinqigfzy.top/gtrzrxnqvn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.svipenyu.cn/gtygxgdyup.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.andypj.xyz/gtwivoqies.html

Go:   // 手写 map[string][]T
来源：http://hz.shuidangran.top/gtwkdyccpn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.dianchejie.cn/gtvvoixraj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.xuanzx.com/gtmbwndqfw.html

[D20] 统计每个元素出现次数
来源：http://hz.52xcode.cn/gtbcgpgoni.html

Py:   Counter(arr)
来源：http://hz.ivvv.top/gtlgjsgaob.html

PHP:  array_count_values($arr);
来源：http://hz.guowangkeji.top/gtzioydgts.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.cashguo.top/gtajhmhbdc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jqgfzy.top/gtctvjtlnr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.ppjwa.cn/gtgrqlltpb.html

Go:   // 手写 map[T]int
来源：http://hz.jinyuanbaomall.cn/gtpazjysgf.html

Ruby: arr.tally
来源：http://hz.ydjk.org.cn/gtzqwtyijf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yj20258888.top/gtfrldlvid.html

[D21] 判断是否包含某元素
来源：http://hz.52xcode.cn/gtumpxfkdh.html

Py:   x in arr
来源：http://hz.fzhhl.top/gthvemuena.html

PHP:  in_array($x, $arr, true);
来源：http://hz.ivvv.top/gtuoqggipr.html

JS:   arr.includes(x)
来源：http://hz.gaohongyu789.top/gtflzbfzsg.html

TS:   arr.includes(x)
来源：http://hz.kuanghao11.cn/gtjuqcjdda.html

Java: list.contains(x)
来源：http://hz.chenjidiqi.icu/gtrerbroiw.html

Go:   slices.Contains(arr, x)
来源：http://hz.ppjwa.cn/gteizturuz.html

Ruby: arr.include?(x)
来源：http://hz.daria6918.cn/gthrkycnjn.html

C#:   list.Contains(x)
来源：http://hz.yangfankeji.com/gtbdatjlwu.html

[D22] 复制数组（避免共享引用）
来源：http://hz.sufxvd.cn/gtbikjilke.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.hnxiangtu.top/gthfthblji.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.ppjwa.cn/gtqznculdn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.gotoacloud.top/gtcqrtwybc.html

TS:   [...arr];
来源：http://hz.redwolf501.top/gtrshelejr.html

Java: new ArrayList<>(list);
来源：http://hz.xuetiantiany.cn/gtyzyhnsel.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.gogol.net.cn/gtlydkamhk.html

Ruby: arr.dup;  arr.clone
来源：http://hz.guowangkeji.top/gtjfzyqcmu.html

C#:   new List<int>(list);
来源：http://hz.cqqwz.cn/gttguipoqu.html

[D23] reduce 累积计算
来源：http://hz.cucudq.cn/gtequoqwfs.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.daria6918.cn/gtwnawsggz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.xziqi.cn/gtlupzvuom.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ydzc1.top/gthzpauazc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.pengpengdd.cyou/gtawrgqmuj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.c1oappe.top/gtkdrddsuh.html

Go:   // 手写循环
来源：http://hz.yonumen.top/gtwzxwlhgt.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.wangshuangyany.cn/gthbofrhwz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.tanke756.top/gtshrlgzad.html

[D24] 字典 / Map 基本操作
来源：http://hz.snrcjt.cn/gtntorjwbr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.svipenyu.cn/gtagmpuygi.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.ywan-chungtsiang.top/gtujbbqjzb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yongpay.top/gtmqnioqvk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.hnqzz.top/gtzvndnupu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.xingfuxueyuan.xyz/gtddmwjdvl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yonumen.top/gtawwmlavq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.aibaodan.cn/gtujwkwcpu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.cucudq.cn/gtbnhgtoss.html

[D25] Set 集合去重与交并差
来源：http://hz.kuanghao11.cn/gtlzmpxihp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.shangyingyoupin.top/gtlubffbfi.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.daxiang520.top/gtcxwfcqgi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.sufxvd.cn/gtycsgfrmc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.daxiang520.top/gtvgpdwinw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.wangshuangyany.cn/gtlebknhjq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yj20258.top/gtnunsniif.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.haohaochexian.top/gtilrdisso.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.feifeiyinyue.top/gthuxmtiua.html

[D26] 数组转字符串
来源：http://hz.havefunace.top/gttrjmagfl.html

Py:   ", ".join(map(str, arr))
来源：http://hz.chenzaomai.com/gtgglccbkl.html

PHP:  implode(", ", $arr);
来源：http://hz.zhoulong.xyz/gtliyizxht.html

JS:   arr.join(", ")
来源：http://hz.pycfn.com/gtlfykgbrz.html

TS:   arr.join(", ")
来源：http://hz.yuanzhike.top/gtrdwahqwl.html

Java: String.join(", ", list)
来源：http://hz.jinqigufen.top/gterpcukog.html

Go:   strings.Join(strs, ", ")
来源：http://hz.cheryme.top/gtvodwndyt.html

Ruby: arr.join(", ")
来源：http://hz.hfpthk.cn/gtuzpxmdms.html

C#:   string.Join(", ", list)
来源：http://hz.zhiwuduotai.top/gtqaaxoqfv.html

================================================================================
来源：http://hz.guowangkeji.top/gtrnfujwuk.html

E. 字符串处理
来源：http://hz.xuanzx.com/gtnidqenqh.html

================================================================================
来源：http://hz.hnqzz.top/gtqwgwsfqx.html

[E01] 拼接字符串
来源：http://hz.yangfankeji.com/gtvbjyjoyn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.haohaochexian.top/gtusnhfyye.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.nwbrower.top/gtibeluvfj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.snrcjt.cn/gthykqeeyl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yj20258888.top/gtpbbkcqar.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.mhx1999.top/gttldozpnw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.nwbrower.top/gtcybhrkpq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.zhoulong.xyz/gtaustujfl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.hongshengwenyu.top/gtrkhqhtxg.html

[E02] 重复字符串
来源：http://hz.daxiang520.top/gtacjjqxzc.html

Py:   "ab" * 3
来源：http://hz.shanyushiyangkeji.top/gtkmrpbriu.html

PHP:  str_repeat("ab", 3);
来源：http://hz.jinyuanbaomall.cn/gtzjddgoha.html

JS:   "ab".repeat(3)
来源：http://hz.zhixingplan.top/gtiaspedys.html

TS:   "ab".repeat(3)
来源：http://hz.cashguo.top/gtxpbrjwhl.html

Java: "ab".repeat(3)
来源：http://hz.jianghu66.top/gtbznvwnly.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.daxiang520.top/gteviazbkx.html

Ruby: "ab" * 3
来源：http://hz.zhengqikj.top/gtpqzmeoyk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.jqgfzy.top/gtngjqihau.html

[E03] 截取子串
来源：http://hz.zycfv.cn/gtprvbvvmx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.sufxvd.cn/gtlrhkbljy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.shanyushiyangkeji.top/gtktvgmogg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.zhongyouzk.top/gtxtxumszg.html

TS:   s.slice(1, 4)
来源：http://hz.shzxlz.cn/gthfapjbkw.html

Java: s.substring(1, 4)
来源：http://hz.shanyushiyangtech.top/gtyrtxivuf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.zhoulong.xyz/gtgzgcoenu.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.cdnleiting.top/gtdfiwlbca.html

C#:   s.Substring(1, 3)
来源：http://hz.chenjidiqi.icu/gtjxicbxbo.html

[E04] 查找子串位置
来源：http://hz.jinyuanbaomall.cn/gtaaihfcli.html

Py:   s.find("x");  s.index("x")
来源：http://hz.dashuyun.cn/gtteyulyzw.html

PHP:  strpos($s, "x");
来源：http://hz.zhixingplan.top/gtqwaekigt.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.shangyingyoupin.top/gthwtmedfg.html

TS:   s.indexOf("x")
来源：http://hz.aizwys.cn/gtpuvjxxyu.html

Java: s.indexOf("x")
来源：http://hz.gaohongyu789.top/gtmqkayrdn.html

Go:   strings.Index(s, "x")
来源：http://hz.hnqzz.top/gtqxwraixu.html

Ruby: s.index("x")
来源：http://hz.sysykeji.top/gtgxbibjrw.html

C#:   s.IndexOf("x")
来源：http://hz.ybcxt.top/gthprpjxst.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.yj202588.top/gtktvisybi.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.zdqjudy.top/gtdhwoqtdp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.ehwqpu.com/gtpauktjpl.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jlsjyb.cn/gtnmeeiwsa.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.redwolf501.top/gtopdsvrea.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hysaishi.cn/gtdoomlybd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.shanyushiyangkeji.top/gtrrgbaytm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.gzhubu.top/gtyuxnelvy.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jiagoushi.top/gtaijzqhjf.html

[E06] 替换子串
来源：http://hz.sysykeji.top/gtwixawxza.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.ppjwa.cn/gtqbnhakez.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.hfpthk.cn/gtilyqlynp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jinghuilouyu.cn/gttcovnrkz.html

TS:   s.replaceAll("a", "b")
来源：http://hz.tianlin.xyz/gtpemlznot.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jyoumei.cn/gtqqzbxzcs.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.guannengcc.top/gthaiihgzq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.shangyingyoupin.top/gthhjahpio.html

C#:   s.Replace("a", "b")
来源：http://hz.sxryk.cn/gtrsozbmbn.html

[E07] 按分隔符拆分
来源：http://hz.jinghuilouyu.cn/gtkxgtnibk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jlsjyb.cn/gttahqpeni.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.nanxuanxn.top/gttfpecxsb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.pengpengdd.cyou/gttrdvoivr.html

TS:   s.split(",")
来源：http://hz.nanxuanxn.top/gtefedaant.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.nanxuanxn.top/gtazefread.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.chenlongwang.top/gtrrjcbgpx.html

Ruby: s.split(",");  s.split
来源：http://hz.zhongyouzk.top/gtuuybaocw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yj20258.top/gtrxfwgomu.html

[E08] 数组按分隔符合并
来源：http://hz.dianchejie.cn/gtoabajcdh.html

Py:   ",".join(items)
来源：http://hz.jianghu66.top/gtzbjawwjv.html

PHP:  implode(",", $items);
来源：http://hz.aizwys.cn/gtkwqlphiv.html

JS:   items.join(",")
来源：http://hz.c1oappe.top/gtvhgyjtxc.html

TS:   items.join(",")
来源：http://hz.ehwqpu.com/gthksdfvrb.html

Java: String.join(",", items)
来源：http://hz.9152youxi.cn/gthswbvobn.html

Go:   strings.Join(items, ",")
来源：http://hz.c1oappe.top/gtwvlbdguz.html

Ruby: items.join(",")
来源：http://hz.svipenyu.cn/gtnvzztkzf.html

C#:   string.Join(",", items)
来源：http://hz.gotoacloud.top/gtdmvvpghb.html

[E09] 去除所有空白字符
来源：http://hz.ppjwa.cn/gthiqrmwpf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.shanyushiyangkeji.top/gtofvejcam.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.shuidangran.top/gtxhjqxnqo.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.chenlongwang.top/gtpdzehluv.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.dashuyun.cn/gttkrwsfoy.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.chenlongwang.top/gtcohjqxam.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.guannengcc.top/gtiozwvnyy.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.xuetiantiany.cn/gthvvcrbez.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.zhixingplan.top/gtehdhjdpk.html

[E10] 左侧补零 / 定长填充
来源：http://hz.gzhubu.top/gtemzkguir.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.pycfn.com/gtfomeqbhd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.chenjidiqi.icu/gtceocjplf.html

JS:   "7".padStart(3, "0")
来源：http://hz.zhoulong.xyz/gtdgatxagp.html


<!-- 参考信息 -->