代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.aibaodan.cn/gtvnhcpzjw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.zycfv.cn/gtjyeyuezh.html

[D05] 访问与修改元素
来源：http://hz.daxiang520.top/gtdjudryur.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.smart0.xyz/gtlubdaucb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.quarkkingdee.top/gtxfwconzj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.zhengqikj.top/gtpgmkjqpi.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.quarkkingdee.top/gttiueqzpq.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zhiwuduotai.top/gtfgmkfaev.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jinqigufen.top/gtelvqcuan.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yj20258888.top/gtmmrzonou.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.zdqjudy.top/gttvxnuukq.html

[D06] 数组长度
来源：http://hz.zhixingplan.top/gtscldureq.html

Py:   len(arr)
来源：http://hz.nwbrower.top/gtvbhueshk.html

PHP:  count($arr);
来源：http://hz.zhoulong.xyz/gtmjuexgsx.html

JS:   arr.length
来源：http://hz.shzxlz.cn/gtcuonwscv.html

TS:   arr.length
来源：http://hz.yj202588.top/gtawmdclrw.html

Java: list.size();
来源：http://hz.jinyuanbaomall.cn/gtkdbcwtfl.html

Go:   len(arr)
来源：http://hz.cucudq.cn/gtepfxkood.html

Ruby: arr.length; arr.size
来源：http://hz.shangyingyoupin.top/gtiesufsbp.html

C#:   list.Count;
来源：http://hz.snrcjt.cn/gtevrfsyuu.html

[D07] 切片 / 取子数组
来源：http://hz.pengpengdd.cyou/gtibdarcai.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zhaomingkeji.xyz/gtxbydfswk.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zhengqikj.top/gtavnvfsay.html

JS:   arr.slice(1, 4);
来源：http://hz.kuanghao11.cn/gtvlyhelko.html

TS:   arr.slice(1, 4);
来源：http://hz.cucudq.cn/gtyfgbollv.html

Java: list.subList(1, 4);
来源：http://hz.nwbrower.top/gtmkpyxfrn.html

Go:   arr[1:4]
来源：http://hz.ppjwa.cn/gtauozqlqx.html

Ruby: arr[1, 3]
来源：http://hz.ydjk.org.cn/gtuynzdxfk.html

C#:   list.GetRange(1, 3);
来源：http://hz.pycfn.com/gtlgdimhhc.html

[D08] 合并两个数组
来源：http://hz.zdqjudy.top/gtaplpksdp.html

Py:   a + b;  a.extend(b)
来源：http://hz.316326.xyz/gturukjrdj.html

PHP:  array_merge($a, $b);
来源：http://hz.mhx1999.top/gtcubushwc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.xziqi.cn/gtzdrndqgi.html

TS:   [...a, ...b];
来源：http://hz.yj202588.top/gtkjmkqrpm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.gogol.net.cn/gtrqheqjog.html

Go:   append(a, b...)
来源：http://hz.quarkkingdee.top/gtbnycbajj.html

Ruby: a + b;  a.concat(b)
来源：http://hz.gzhubu.top/gtztkixlzi.html

C#:   a.Concat(b).ToList()
来源：http://hz.smart0.xyz/gtackfybbw.html

[D09] 排序（升序）
来源：http://hz.52xcode.cn/gtmrbkivib.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cheryme.top/gtjwlagjcq.html

PHP:  sort($arr);
来源：http://hz.redwolf501.top/gtjetffgdb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.quarkkingdee.top/gtpqlokfzq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.c1oappe.top/gtxvslzefe.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.ywan-chungtsiang.top/gtbdrqodyl.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yvedp.cn/gtkmjnrnzx.html

Ruby: arr.sort
来源：http://hz.zhaomingkeji.xyz/gtsssoxxrh.html

C#:   list.Sort();
来源：http://hz.gotoacloud.top/gtnctkktaj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.tianlin.xyz/gtssgcgbmx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.shangyingyoupin.top/gtazahwqhi.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yuxming.cn/gtfpunvwof.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yvedp.cn/gtnwflrmvh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yueranfly.top/gtsbctplsz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.ydzc1.top/gtyuirofzy.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.hammf.cn/gtuqbgkkph.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.52xcode.cn/gtkishvelp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.xingfuxueyuan.xyz/gtjsdifewt.html

[D11] 反转数组
来源：http://hz.jinqigufen.top/gtxcgnxexq.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.mhx1999.top/gtxuabozpc.html

PHP:  array_reverse($arr);
来源：http://hz.andypj.xyz/gtwvyugean.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.aibaodan.cn/gtwnxyijrm.html

TS:   [...arr].reverse();
来源：http://hz.zhijiandao.cn/gtnfkehpay.html

Java: Collections.reverse(list);
来源：http://hz.shanyushiyangtech.top/gtncgegeyr.html

Go:   slices.Reverse(arr)
来源：http://hz.birdmap.top/gtjnvmnhzb.html

Ruby: arr.reverse
来源：http://hz.feifeiyinyue.top/gtrezoyfih.html

C#:   list.Reverse();
来源：http://hz.xinyue.icu/gthzvhdaat.html

[D12] 查找元素下标
来源：http://hz.sufxvd.cn/gtzfmhuzre.html

Py:   arr.index(x);  x in arr
来源：http://hz.xylfe.cn/gtttueirfv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.redwolf501.top/gthdecnaug.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.tian-w.cn/gthhgehlke.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.cheryme.top/gtzdbkblbx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.mhx1999.top/gtpsgwwqus.html

Go:   slices.Index(arr, x)
来源：http://hz.ivvv.top/gttkngnrkh.html

Ruby: arr.index(x)
来源：http://hz.hnqzz.top/gtdqodqsvy.html

C#:   list.IndexOf(x);
来源：http://hz.cqqwz.cn/gteqncdhhp.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zhiwuduotai.top/gtwicjezqn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.hammf.cn/gtwgdqstlc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.316326.xyz/gtwajisilg.html

JS:   arr.filter(x => x > 3)
来源：http://hz.ywan-chungtsiang.top/gtupixfneb.html

TS:   arr.filter(x => x > 3)
来源：http://hz.nanxuanxn.top/gtlpfryeyq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.dashuyun.cn/gtavohjneb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jinyuanbaomall.cn/gtdfytjvnz.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.zhengqikj.top/gtvqripkwa.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.aizwys.cn/gtzxvywgpa.html

[D14] 映射转换（每个元素变形）
来源：http://hz.birdmap.top/gtmxxfumrp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.xuanzx.com/gtvfevxoeq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.meibo888.top/gtppeixhcc.html

JS:   arr.map(x => x * 2)
来源：http://hz.chenjidiqi.icu/gtbbatpecp.html

TS:   arr.map(x => x * 2)
来源：http://hz.9152youxi.cn/gtmtdkzodq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jqgufenzy.top/gtuzrzybda.html

Go:   // 手写循环
来源：http://hz.ivvv.top/gtpcpkcjxm.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.hfpthk.cn/gtyehbumcg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.chenzaomai.com/gtkbilfgux.html

[D15] 去重
来源：http://hz.daria6918.cn/gtehyruyxl.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.chenzaomai.com/gtaxpltxan.html

PHP:  array_unique($arr);
来源：http://hz.tanke756.top/gtpelzoxps.html

JS:   [...new Set(arr)]
来源：http://hz.hnxiangtu.top/gthlbtysrl.html

TS:   [...new Set(arr)]
来源：http://hz.xinyue.icu/gtlljeerlg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.ehwqpu.com/gtenugayfd.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yueranfly.top/gtyqnfgkfx.html

Ruby: arr.uniq
来源：http://hz.52xcode.cn/gtnmuzsxua.html

C#:   list.Distinct().ToList()
来源：http://hz.shangyingyoupin.top/gtmwdeuweo.html

[D16] 求和与平均值
来源：http://hz.yongpay.top/gtiyygsnto.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.aibaodan.cn/gtzvnujqnd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yuanzhike.top/gtpspliixy.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ybcxt.top/gtxzypmumk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.pycfn.com/gthjnsdcga.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.c1oappe.top/gtzdeepzzm.html

Go:   // 手写循环累加
来源：http://hz.ehwqpu.com/gtsdyoafhx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.svipenyu.cn/gtfqjhwwbj.html

C#:   list.Sum();  list.Average()
来源：http://hz.zhengqikj.top/gtdhgtanpz.html

[D17] 最大值与最小值
来源：http://hz.316326.xyz/gtcpvwsaum.html

Py:   max(arr);  min(arr)
来源：http://hz.xingfuxueyuan.xyz/gtkrxwrkwt.html

PHP:  max($arr);  min($arr);
来源：http://hz.kuanghao11.cn/gtyvfbcsqg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.zhongyouzk.top/gtwrveyxmh.html

TS:   Math.max(...arr);
来源：http://hz.316326.xyz/gtrzwpjyxh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.chenlongwang.top/gtqopgroey.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.guannengcc.top/gtexmmmciq.html

Ruby: arr.max;  arr.min
来源：http://hz.cucudq.cn/gtczfbujlt.html

C#:   list.Max();  list.Min()
来源：http://hz.gotoacloud.top/gtwscqkiag.html

[D18] 扁平化嵌套数组
来源：http://hz.cqqwz.cn/gtcftjiqoi.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.ybcxt.top/gtikholfcs.html

PHP:  array_merge(...$nested);
来源：http://hz.yuxming.cn/gtcvsotnwk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.sxryk.cn/gtekixuuer.html

TS:   nested.flat();
来源：http://hz.xuetiantiany.cn/gtmhyfyodx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.ywan-chungtsiang.top/gtnrcrmwqk.html

Go:   // 手写双层循环
来源：http://hz.shanyushiyangtech.top/gtinlghjkh.html

Ruby: nested.flatten
来源：http://hz.pengpengdd.cyou/gtlhvensis.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.gotoacloud.top/gtxgckacbd.html

[D19] 按字段分组
来源：http://hz.zycfv.cn/gtwjdqpmtl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.0kj1m.cn/gtpbofcalu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.redwolf501.top/gtvqujhqqm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yonumen.top/gtaftycobl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.guowangkeji.top/gtsrvedrcu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jinghuilouyu.cn/gtvkpoahve.html

Go:   // 手写 map[string][]T
来源：http://hz.zycfv.cn/gtghvgvcdc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.gaohongyu789.top/gtpxkacttr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.xziqi.cn/gtcqsmxwal.html

[D20] 统计每个元素出现次数
来源：http://hz.yj20258888.top/gteshbvgvi.html

Py:   Counter(arr)
来源：http://hz.yanxiufei.cn/gtnkpzhwys.html

PHP:  array_count_values($arr);
来源：http://hz.xuetiantiany.cn/gtsnnkfkip.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jlsjyb.cn/gtqbltnusc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yongpay.top/gtlxegelxt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.ydzc1.top/gtwjmvctmv.html

Go:   // 手写 map[T]int
来源：http://hz.jqgufenzy.top/gtfhyxlrkl.html

Ruby: arr.tally
来源：http://hz.cdnleiting.top/gtzywyapgh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.gzhubu.top/gtkstontjx.html

[D21] 判断是否包含某元素
来源：http://hz.yongpay.top/gtajrbvnrt.html

Py:   x in arr
来源：http://hz.yueranfly.top/gtnavzxhif.html

PHP:  in_array($x, $arr, true);
来源：http://hz.xylfe.cn/gtuqiyulhh.html

JS:   arr.includes(x)
来源：http://hz.cheryme.top/gtgjkxbmzm.html

TS:   arr.includes(x)
来源：http://hz.shuidangran.top/gtuufnexho.html

Java: list.contains(x)
来源：http://hz.mhx1999.top/gtifciqyop.html

Go:   slices.Contains(arr, x)
来源：http://hz.zhaomingkeji.xyz/gtbrwpalwz.html

Ruby: arr.include?(x)
来源：http://hz.xylfe.cn/gtudkearxa.html

C#:   list.Contains(x)
来源：http://hz.bjfxy.top/gtseerzgsh.html

[D22] 复制数组（避免共享引用）
来源：http://hz.sysykeji.top/gtczzwodlw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.svipenyu.cn/gthdpgshct.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.tanke756.top/gteoyzwife.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.kuanghao11.cn/gthbtijslo.html

TS:   [...arr];
来源：http://hz.aibaodan.cn/gtojprwvej.html

Java: new ArrayList<>(list);
来源：http://hz.svipenyu.cn/gtfnbzweku.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.nanxinkj.top/gtuujujkkv.html

Ruby: arr.dup;  arr.clone
来源：http://hz.cheryme.top/gtlihgqgzu.html

C#:   new List<int>(list);
来源：http://hz.snrcjt.cn/gtgvdduzbh.html

[D23] reduce 累积计算
来源：http://hz.0kj1m.cn/gtlynsdyat.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.xuanzx.com/gtcsvpjmvt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.fengsongda.top/gtptovtvhy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.haohaochexian.top/gtvlgaqoru.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.pengpengdd.cyou/gtweqbenho.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jinghuilouyu.cn/gtdlynizjx.html

Go:   // 手写循环
来源：http://hz.yj20258888.top/gtzubwewrg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.tianlin.xyz/gtqqmtaadg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.9152youxi.cn/gtkqwcpmtp.html

[D24] 字典 / Map 基本操作
来源：http://hz.guowangkeji.top/gtnlrnhivc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.vqdsnc.cn/gtcxmdnwub.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.hongshengwenyu.top/gtazznfbfn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.zhengqikj.top/gtkigjvblr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.0kj1m.cn/gtojifdomw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.cucudq.cn/gtuxjaodyo.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.guannengcc.top/gtekkzarpv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.chenlongwang.top/gtdnlhzwdj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zdqjudy.top/gtptgteugs.html

[D25] Set 集合去重与交并差
来源：http://hz.chenjidiqi.icu/gtklnvcdhf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zycfv.cn/gtfjopthun.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yonumen.top/gtbpobjzph.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.nanxuanxn.top/gtncjezknl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.ehwqpu.com/gtbblokbjf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.andypj.xyz/gtvyyfuhsm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.cashguo.top/gtbpiqjyun.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.hnxiangtu.top/gtbpmxjbtn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.jinqigufen.top/gtlaivdbyc.html

[D26] 数组转字符串
来源：http://hz.sweek.top/gtmlnwbrgj.html

Py:   ", ".join(map(str, arr))
来源：http://hz.cashguo.top/gtzsbhpsrj.html

PHP:  implode(", ", $arr);
来源：http://hz.9152youxi.cn/gtfutcoqlo.html

JS:   arr.join(", ")
来源：http://hz.pycfn.com/gtmuzwmdup.html

TS:   arr.join(", ")
来源：http://hz.tian-w.cn/gtatedpvff.html

Java: String.join(", ", list)
来源：http://hz.birdmap.top/gtpghprixf.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yvedp.cn/gtaihqwspz.html

Ruby: arr.join(", ")
来源：http://hz.bjfxy.top/gtbbihkgbr.html

C#:   string.Join(", ", list)
来源：http://hz.zhijiandao.cn/gtwbvsrsvl.html

================================================================================
来源：http://hz.yonumen.top/gtjjcdhpep.html

E. 字符串处理
来源：http://hz.yangfankeji.com/gtyssbbenw.html

================================================================================
来源：http://hz.zhongyouzk.top/gtigloxhqd.html

[E01] 拼接字符串
来源：http://hz.zdqjudy.top/gtwhxiyhfr.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.jinqigfzy.top/gtizxgrvdd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.shanyushiyangkeji.top/gtrndxmgqc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xziqi.cn/gtjctsoakf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yongpay.top/gtlwjnkvpe.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.nanxuanxn.top/gtaxwcmwgp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.chenlongwang.top/gtmxywyhrt.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.xuanzx.com/gtiydgmugg.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.chenjidiqi.icu/gtrjtgxrnm.html

[E02] 重复字符串
来源：http://hz.aibaodan.cn/gtwnnwkqxf.html

Py:   "ab" * 3
来源：http://hz.jiagoushi.top/gtdapllcsv.html

PHP:  str_repeat("ab", 3);
来源：http://hz.cashguo.top/gtstzezzhe.html

JS:   "ab".repeat(3)
来源：http://hz.52xcode.cn/gtfavohxlb.html

TS:   "ab".repeat(3)
来源：http://hz.shangyingyoupin.top/gtffqbpvjc.html

Java: "ab".repeat(3)
来源：http://hz.sysykeji.top/gtabppennz.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.xingfuxueyuan.xyz/gtytzarrfh.html

Ruby: "ab" * 3
来源：http://hz.shangyingyoupin.top/gtgzqvcymx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.hongshengwenyu.top/gtqzjeoudt.html

[E03] 截取子串
来源：http://hz.feifeiyinyue.top/gtssimgovq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.gogol.net.cn/gtsjogwdhp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.ppjwa.cn/gtshtlcsar.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.9152youxi.cn/gtzseorgft.html

TS:   s.slice(1, 4)
来源：http://hz.shanyushiyangkeji.top/gtqulazbye.html

Java: s.substring(1, 4)
来源：http://hz.yuxming.cn/gtctnanqjs.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yvedp.cn/gtcpcilzrw.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.gzhubu.top/gtqgukwznb.html

C#:   s.Substring(1, 3)
来源：http://hz.ppjwa.cn/gtynjjlafy.html

[E04] 查找子串位置
来源：http://hz.yuxming.cn/gtyerfggeu.html

Py:   s.find("x");  s.index("x")
来源：http://hz.xinyue.icu/gtnuiqeczx.html

PHP:  strpos($s, "x");
来源：http://hz.sufxvd.cn/gtnnmfxwwf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yj202588.top/gtdvwoxstn.html

TS:   s.indexOf("x")
来源：http://hz.chenjidiqi.icu/gtpdlbaydi.html

Java: s.indexOf("x")
来源：http://hz.snrcjt.cn/gtwkqfkszo.html

Go:   strings.Index(s, "x")
来源：http://hz.hywenlv.cn/gtwawailvt.html

Ruby: s.index("x")
来源：http://hz.shzxlz.cn/gtwzatgdal.html

C#:   s.IndexOf("x")
来源：http://hz.wangdashe.top/gtfzbcbsio.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.aizwys.cn/gtsjztambq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.pycfn.com/gtlhpmefgn.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.birdmap.top/gtogvjthcr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.tian-w.cn/gttlidsimh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.xinyue.icu/gtrrbvxdqk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yj20258.top/gtumgyltbu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.xuanzx.com/gtlduqbqlm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.hywenlv.cn/gtkkixuufa.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.hammf.cn/gtilanodyu.html

[E06] 替换子串
来源：http://hz.yuanzhike.top/gtqhvgygva.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.ivvv.top/gtzmxydzdl.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.ivvv.top/gtrjbfciso.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yonumen.top/gtavccpdsg.html

TS:   s.replaceAll("a", "b")
来源：http://hz.xuetiantiany.cn/gtclxqywca.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.9152youxi.cn/gtxbyydbzh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.zhengqikj.top/gtnudefidj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.chenlongwang.top/gtmpeolngl.html

C#:   s.Replace("a", "b")
来源：http://hz.dianchejie.cn/gtlpgmekvh.html

[E07] 按分隔符拆分
来源：http://hz.zhongyouzk.top/gtzgmoiujk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.cheryme.top/gtlfyjedoa.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yongpay.top/gtxqfsaojw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yuxming.cn/gtztfxzdie.html

TS:   s.split(",")
来源：http://hz.0kj1m.cn/gtovimpxoq.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.zhixingplan.top/gtxshhbxdc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yangfankeji.com/gtkfmcxazd.html

Ruby: s.split(",");  s.split
来源：http://hz.sufxvd.cn/gtwnenfpdd.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.aizwys.cn/gtpgmvozij.html

[E08] 数组按分隔符合并
来源：http://hz.tanke756.top/gtrbifilsp.html

Py:   ",".join(items)
来源：http://hz.tianlin.xyz/gterqcusdu.html

PHP:  implode(",", $items);
来源：http://hz.hnxiangtu.top/gtvdqbbqzz.html

JS:   items.join(",")
来源：http://hz.gogol.net.cn/gtdmlwhmlq.html

TS:   items.join(",")
来源：http://hz.zhiwuduotai.top/gtkooahgrl.html

Java: String.join(",", items)
来源：http://hz.jlsjyb.cn/gtrehjydzc.html

Go:   strings.Join(items, ",")
来源：http://hz.xuanzx.com/gtyxcmzdww.html

Ruby: items.join(",")
来源：http://hz.shanyushiyangkeji.top/gtpogrypcc.html

C#:   string.Join(",", items)
来源：http://hz.haohaochexian.top/gtwkracqoy.html

[E09] 去除所有空白字符
来源：http://hz.zhixingplan.top/gtosolbwdt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yanxiufei.cn/gttfqclhhw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.shanyushiyangtech.top/gtyxrwtshx.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.hfpthk.cn/gtmayweyww.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.fengsongda.top/gthgzobmcd.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.ivvv.top/gtxhdvsxbo.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.316326.xyz/gtsvjnxobm.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.chenzaomai.com/gtvcnvscxi.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.guannengcc.top/gtzvchcqtm.html

[E10] 左侧补零 / 定长填充
来源：http://hz.sxryk.cn/gttycowffg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.jinqigufen.top/gttzpsrduv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.dianchejie.cn/gtbdmvijod.html

JS:   "7".padStart(3, "0")
来源：http://hz.sufxvd.cn/gtwsjlgdhr.html

TS:   "7".padStart(3, "0")
来源：http://hz.guowangkeji.top/gtbmwonjls.html

Java: String.format("%03d", 7)
来源：http://hz.52xcode.cn/gtzljljkpz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.fengsongda.top/gtdjzcqwpd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.xylfe.cn/gtistzphul.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.gzhubu.top/gtfeuffktp.html

[E11] 反转字符串
来源：http://hz.sufxvd.cn/gtzhthvwqv.html

Py:   s[::-1]
来源：http://hz.nanxuanxn.top/gtuotnxryi.html

PHP:  strrev($s);
来源：http://hz.ywan-chungtsiang.top/gtcjmplkim.html

JS:   [...s].reverse().join("")
来源：http://hz.ehwqpu.com/gttenoncuc.html

TS:   [...s].reverse().join("")
来源：http://hz.zhongyouzk.top/gtdzkbirxa.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.gogol.net.cn/gtjozoctml.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yuxming.cn/gtrpftjvtw.html


<!-- 参考信息 -->