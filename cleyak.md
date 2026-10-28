代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.aibaodan.cn/gtzdzpnwrr.html

TS:   arr.splice(0, 1);
来源：http://hz.zhaomingkeji.xyz/gtrwagjwep.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.tian-w.cn/gtetecagln.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.zhiwuduotai.top/gtgpowcqcn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.wangdashe.top/gtksznvmtu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.feifeiyinyue.top/gtlsrzivaw.html

[D05] 访问与修改元素
来源：http://hz.jinqigfzy.top/gtsnzbphme.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yongpay.top/gtvkqptsye.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.sxryk.cn/gtdejrbkju.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.aibaodan.cn/gtunetswnf.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yonumen.top/gtgtmanoft.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yj202588.top/gtdjydezaq.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.aizwys.cn/gtudfznrkn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.fzhhl.top/gtdybyciuo.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yueranfly.top/gtegnffsxz.html

[D06] 数组长度
来源：http://hz.ivvv.top/gtwgkbaymw.html

Py:   len(arr)
来源：http://hz.xinyue.icu/gttlhlsfms.html

PHP:  count($arr);
来源：http://hz.zhaomingkeji.xyz/gtdwvrgown.html

JS:   arr.length
来源：http://hz.bjfxy.top/gtxpkwowmw.html

TS:   arr.length
来源：http://hz.quarkkingdee.top/gtntwcneuy.html

Java: list.size();
来源：http://hz.hnqzz.top/gtderuqkje.html

Go:   len(arr)
来源：http://hz.pengpengdd.cyou/gtnufgecps.html

Ruby: arr.length; arr.size
来源：http://hz.xuetiantiany.cn/gtwpywyifr.html

C#:   list.Count;
来源：http://hz.hnxiangtu.top/gtycsouasz.html

[D07] 切片 / 取子数组
来源：http://hz.0kj1m.cn/gtyvnmvtdh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.ywan-chungtsiang.top/gtaiprhoce.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.9152youxi.cn/gtrykrqbar.html

JS:   arr.slice(1, 4);
来源：http://hz.xziqi.cn/gtcbxjpdwt.html

TS:   arr.slice(1, 4);
来源：http://hz.gogol.net.cn/gtjgvrcofx.html

Java: list.subList(1, 4);
来源：http://hz.cucudq.cn/gtnrfbkuzd.html

Go:   arr[1:4]
来源：http://hz.ppjwa.cn/gtcadegcup.html

Ruby: arr[1, 3]
来源：http://hz.cashguo.top/gtldihqdno.html

C#:   list.GetRange(1, 3);
来源：http://hz.yangfankeji.com/gtjqeaweds.html

[D08] 合并两个数组
来源：http://hz.chenlongwang.top/gtornrounj.html

Py:   a + b;  a.extend(b)
来源：http://hz.snrcjt.cn/gtfuvcgtwh.html

PHP:  array_merge($a, $b);
来源：http://hz.guowangkeji.top/gthzqmwnae.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.tian-w.cn/gtgrybsitc.html

TS:   [...a, ...b];
来源：http://hz.chenzaomai.com/gtxcaufkum.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.shanyushiyangtech.top/gtdfvgfeif.html

Go:   append(a, b...)
来源：http://hz.chenlongwang.top/gtsesjgbje.html

Ruby: a + b;  a.concat(b)
来源：http://hz.shuidangran.top/gtkomffepg.html

C#:   a.Concat(b).ToList()
来源：http://hz.pengpengdd.cyou/gthkzxnkvp.html

[D09] 排序（升序）
来源：http://hz.hfpthk.cn/gtaazvffho.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yonumen.top/gtopnbzsgo.html

PHP:  sort($arr);
来源：http://hz.birdmap.top/gtfnivzpfq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.0kj1m.cn/gthjmbixdz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.xylfe.cn/gtqwvalecr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.guowangkeji.top/gtzcywkfxd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yj20258888.top/gtyoizcaar.html

Ruby: arr.sort
来源：http://hz.zhaomingkeji.xyz/gtnhyonckx.html

C#:   list.Sort();
来源：http://hz.zhixingplan.top/gtfzfifyni.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.vqdsnc.cn/gtpfjiwxrj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.sysykeji.top/gtutscewin.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.iojbl.cn/gtdqolqyya.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.vqdsnc.cn/gthjnerlgb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.dashuyun.cn/gtzhdqjbtb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.wangshuangyany.cn/gtgbtgncic.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.chenzaomai.com/gtdmquzqeb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.zhiwuduotai.top/gtxfmpwcrn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zhixingplan.top/gtmwsayeqv.html

[D11] 反转数组
来源：http://hz.yj20258888.top/gtqkhlnbnv.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.guannengcc.top/gtadutkfml.html

PHP:  array_reverse($arr);
来源：http://hz.gotoacloud.top/gtzkboawjq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.zhoulong.xyz/gtyibmpojg.html

TS:   [...arr].reverse();
来源：http://hz.yonumen.top/gtbsejvvnv.html

Java: Collections.reverse(list);
来源：http://hz.zhixingplan.top/gtbgllaoph.html

Go:   slices.Reverse(arr)
来源：http://hz.smart0.xyz/gtmfzkzocv.html

Ruby: arr.reverse
来源：http://hz.ivvv.top/gtehemroqm.html

C#:   list.Reverse();
来源：http://hz.pycfn.com/gtylradnma.html

[D12] 查找元素下标
来源：http://hz.yanxiufei.cn/gtlpnqscac.html

Py:   arr.index(x);  x in arr
来源：http://hz.jqgufenzy.top/gtdsxvnlhm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yangfankeji.com/gthpzcldwr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.wangshuangyany.cn/gtbofzavsx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhongyouzk.top/gtxcfqjpqk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.cucudq.cn/gtafulzdkk.html

Go:   slices.Index(arr, x)
来源：http://hz.chenlongwang.top/gttcmykfwm.html

Ruby: arr.index(x)
来源：http://hz.hammf.cn/gtopblhpdq.html

C#:   list.IndexOf(x);
来源：http://hz.cucudq.cn/gtocmmzbfn.html

[D13] 过滤（保留满足条件的）
来源：http://hz.ydzc1.top/gtnnzztdug.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.hnxiangtu.top/gtqtgoaqpk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.ywan-chungtsiang.top/gtwfyhodmu.html

JS:   arr.filter(x => x > 3)
来源：http://hz.xziqi.cn/gtkbpbfsts.html

TS:   arr.filter(x => x > 3)
来源：http://hz.fzhhl.top/gtqylazidr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.andypj.xyz/gttkbvxucb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.sxryk.cn/gthfxbynyz.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.gotoacloud.top/gtgwcrfqmc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.xuetiantiany.cn/gtowalbpjf.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yanxiufei.cn/gtduangfrt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.cheryme.top/gtwgjpyejy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.jqgufenzy.top/gtnizthgyx.html

JS:   arr.map(x => x * 2)
来源：http://hz.redwolf501.top/gtqsckbcca.html

TS:   arr.map(x => x * 2)
来源：http://hz.cheryme.top/gtezuzznfs.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.tianlin.xyz/gtfkuhehwx.html

Go:   // 手写循环
来源：http://hz.yongpay.top/gtsotvecty.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.hysaishi.cn/gtwqhaqrzc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.birdmap.top/gthmxrhemt.html

[D15] 去重
来源：http://hz.jinqigfzy.top/gtxjymjzth.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.smart0.xyz/gtmdcbnpha.html

PHP:  array_unique($arr);
来源：http://hz.sweek.top/gtscbvynro.html

JS:   [...new Set(arr)]
来源：http://hz.cheryme.top/gtespployq.html

TS:   [...new Set(arr)]
来源：http://hz.smart0.xyz/gtzzmajgsb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.snrcjt.cn/gtrvnbpdut.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.xuanzx.com/gtjtfnrpox.html

Ruby: arr.uniq
来源：http://hz.fengsongda.top/gtuutxkawy.html

C#:   list.Distinct().ToList()
来源：http://hz.jqgfzy.top/gtgbljumwa.html

[D16] 求和与平均值
来源：http://hz.yangfankeji.com/gtsnmzulyg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.xziqi.cn/gtsojnyssa.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.svipenyu.cn/gtchkcihvv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yuanzhike.top/gtnaorxkht.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cucudq.cn/gtkxiedcag.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.quarkkingdee.top/gtymkmvpdn.html

Go:   // 手写循环累加
来源：http://hz.pengpengdd.cyou/gtuirxqotb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.hfpthk.cn/gtooexfkxs.html

C#:   list.Sum();  list.Average()
来源：http://hz.nanxuanxn.top/gtjecnjdrc.html

[D17] 最大值与最小值
来源：http://hz.pengpengdd.cyou/gtdsfokzmk.html

Py:   max(arr);  min(arr)
来源：http://hz.bjfxy.top/gtxvsnxvms.html

PHP:  max($arr);  min($arr);
来源：http://hz.pengpengdd.cyou/gtkiogyiqb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.zhengqikj.top/gtjheilgrj.html

TS:   Math.max(...arr);
来源：http://hz.aizwys.cn/gtnriaipmt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jiagoushi.top/gtecdpwumz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.sxryk.cn/gtxcypyabb.html

Ruby: arr.max;  arr.min
来源：http://hz.zhiwuduotai.top/gtxfcmnlqt.html

C#:   list.Max();  list.Min()
来源：http://hz.vqdsnc.cn/gtfzsjvjpq.html

[D18] 扁平化嵌套数组
来源：http://hz.ydjk.org.cn/gttbwkbbeo.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.xziqi.cn/gtdrffcfvx.html

PHP:  array_merge(...$nested);
来源：http://hz.jyoumei.cn/gtzlxiqlvu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.zhengqikj.top/gtjspabbof.html

TS:   nested.flat();
来源：http://hz.tanke756.top/gtlveiznal.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.sufxvd.cn/gtktopqmka.html

Go:   // 手写双层循环
来源：http://hz.fengsongda.top/gtjyuahfeu.html

Ruby: nested.flatten
来源：http://hz.zhongyouzk.top/gtqtborwnj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.ywan-chungtsiang.top/gtnkcxkntv.html

[D19] 按字段分组
来源：http://hz.guannengcc.top/gtddyzjqjr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.ppjwa.cn/gtgwaezsfy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.zdqjudy.top/gtffaunpxq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.daria6918.cn/gtmmqzzefk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.cqqwz.cn/gtkzcjqqek.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yangfankeji.com/gtngxwkdhv.html

Go:   // 手写 map[string][]T
来源：http://hz.guannengcc.top/gtmvkosena.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.c1oappe.top/gtlrrreigr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.ydzc1.top/gtuobopqtq.html

[D20] 统计每个元素出现次数
来源：http://hz.cqqwz.cn/gtumpfimkn.html

Py:   Counter(arr)
来源：http://hz.yj20258888.top/gttjduufth.html

PHP:  array_count_values($arr);
来源：http://hz.hnxiangtu.top/gtwiubnjjm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.feifeiyinyue.top/gtxlxuplkw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.nanxuanxn.top/gtvmnlshdz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.meibo888.top/gtxgboomng.html

Go:   // 手写 map[T]int
来源：http://hz.jlsjyb.cn/gtfoneiksv.html

Ruby: arr.tally
来源：http://hz.meibo888.top/gtwsiphesy.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.cheryme.top/gtuetgaxzd.html

[D21] 判断是否包含某元素
来源：http://hz.zdqjudy.top/gtdxlpvueq.html

Py:   x in arr
来源：http://hz.zhixingplan.top/gtubxkmoqs.html

PHP:  in_array($x, $arr, true);
来源：http://hz.cashguo.top/gtmyuksmzy.html

JS:   arr.includes(x)
来源：http://hz.jyoumei.cn/gtuneiacfp.html

TS:   arr.includes(x)
来源：http://hz.hywenlv.cn/gtqyszbnrl.html

Java: list.contains(x)
来源：http://hz.yuanzhike.top/gtecogrggw.html

Go:   slices.Contains(arr, x)
来源：http://hz.ehwqpu.com/gtnvvifgzg.html

Ruby: arr.include?(x)
来源：http://hz.c1oappe.top/gtmgoiqapl.html

C#:   list.Contains(x)
来源：http://hz.0kj1m.cn/gtmiokjpos.html

[D22] 复制数组（避免共享引用）
来源：http://hz.ywan-chungtsiang.top/gtqptbcdav.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yonumen.top/gtrunbkolt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.xingfuxueyuan.xyz/gtnfhgohnq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.nanxuanxn.top/gtubwabzrh.html

TS:   [...arr];
来源：http://hz.wangshuangyany.cn/gtwsuwwhfx.html

Java: new ArrayList<>(list);
来源：http://hz.chenlongwang.top/gtklgbtwcc.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.chenzaomai.com/gtkqtoftwt.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yangfankeji.com/gtmskhexaz.html

C#:   new List<int>(list);
来源：http://hz.havefunace.top/gtferciyck.html

[D23] reduce 累积计算
来源：http://hz.zhixingplan.top/gtuscevsmv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yuxming.cn/gtwgwnyjgp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.chenjidiqi.icu/gtpeftmtes.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ppjwa.cn/gtkmjwqvkg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xuanzx.com/gtqrgsmbqc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.52xcode.cn/gtpsdmwtjj.html

Go:   // 手写循环
来源：http://hz.chenzaomai.com/gtrmbdgpjk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.cucudq.cn/gtluhajqgu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.hongshengwenyu.top/gtsnxunxfp.html

[D24] 字典 / Map 基本操作
来源：http://hz.guowangkeji.top/gtcspjgwge.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.iojbl.cn/gtcwbjblek.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yuanzhike.top/gtmmzkstwa.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.316326.xyz/gtohmghuwv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.shangyingyoupin.top/gtyacpemxi.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.zdqjudy.top/gtqhsnqehs.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.zhaomingkeji.xyz/gtouyuoovj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.shangyingyoupin.top/gttyxyeoyn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zycfv.cn/gtpmwffwmz.html

[D25] Set 集合去重与交并差
来源：http://hz.cdnleiting.top/gtzqggttql.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.gogol.net.cn/gtkkdgpvub.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.guowangkeji.top/gteupfrwny.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.nanxuanxn.top/gtvjixyuxt.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.316326.xyz/gtiepkpnap.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.vqdsnc.cn/gtxozarpzh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.xziqi.cn/gtktyprbga.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.daxiang520.top/gtqvfcteyj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.bjfxy.top/gtspatphfb.html

[D26] 数组转字符串
来源：http://hz.zhixingplan.top/gtdzabzkso.html

Py:   ", ".join(map(str, arr))
来源：http://hz.ehwqpu.com/gtcdngggne.html

PHP:  implode(", ", $arr);
来源：http://hz.yuxming.cn/gtnowrvkyc.html

JS:   arr.join(", ")
来源：http://hz.daxiang520.top/gtezhwrcha.html

TS:   arr.join(", ")
来源：http://hz.wangshuangyany.cn/gtpciekhcw.html

Java: String.join(", ", list)
来源：http://hz.cheryme.top/gtvzhkardi.html

Go:   strings.Join(strs, ", ")
来源：http://hz.gaohongyu789.top/gtdkcpedeb.html

Ruby: arr.join(", ")
来源：http://hz.c1oappe.top/gtnuspdiha.html

C#:   string.Join(", ", list)
来源：http://hz.gaohongyu789.top/gtrlsfyijs.html

================================================================================
来源：http://hz.chenzaomai.com/gtsvylufej.html

E. 字符串处理
来源：http://hz.9152youxi.cn/gtlsclyqnx.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtehhslgci.html

[E01] 拼接字符串
来源：http://hz.birdmap.top/gtmdipzmlo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yongpay.top/gthrewbill.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.shangyingyoupin.top/gtwcobnnyx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.chenzaomai.com/gtfvkvgwwy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hfpthk.cn/gtfrlmbhvz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.ydzc1.top/gtrsdtrbfr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.chenzaomai.com/gtigvspygx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.ppjwa.cn/gthtsfkrqx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.shuidangran.top/gtbokqutod.html

[E02] 重复字符串
来源：http://hz.316326.xyz/gtqyxqfinx.html

Py:   "ab" * 3
来源：http://hz.zhaomingkeji.xyz/gtoggsiife.html

PHP:  str_repeat("ab", 3);
来源：http://hz.daria6918.cn/gtrtxqgfsh.html

JS:   "ab".repeat(3)
来源：http://hz.yvedp.cn/gtowxzqdve.html

TS:   "ab".repeat(3)
来源：http://hz.hammf.cn/gtudxrkqlt.html

Java: "ab".repeat(3)
来源：http://hz.316326.xyz/gtkeejvgnu.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.feifeiyinyue.top/gtgpfbsjgo.html

Ruby: "ab" * 3
来源：http://hz.chenjidiqi.icu/gtwuoxcggd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.zhixingplan.top/gtwbrcgfxd.html

[E03] 截取子串
来源：http://hz.9152youxi.cn/gtaqroqpyh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.zhongyouzk.top/gtncmeatgs.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.birdmap.top/gtlnvzhgnl.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.hongshengwenyu.top/gtuvjemlka.html

TS:   s.slice(1, 4)
来源：http://hz.chenlongwang.top/gtkbnfndbn.html

Java: s.substring(1, 4)
来源：http://hz.xuanzx.com/gtfuykhbsa.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.xuetiantiany.cn/gtzotqxbzz.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.snrcjt.cn/gtzwpsugly.html

C#:   s.Substring(1, 3)
来源：http://hz.gzhubu.top/gtorjldryh.html

[E04] 查找子串位置
来源：http://hz.jinyuanbaomall.cn/gtfhxkjghp.html

Py:   s.find("x");  s.index("x")
来源：http://hz.nanxuanxn.top/gtijamtkng.html

PHP:  strpos($s, "x");
来源：http://hz.ivvv.top/gtdxvlggwx.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.meibo888.top/gtkhiuketi.html

TS:   s.indexOf("x")
来源：http://hz.cqqwz.cn/gtzuklvnii.html

Java: s.indexOf("x")
来源：http://hz.zhiwuduotai.top/gtucfdqbzd.html

Go:   strings.Index(s, "x")
来源：http://hz.tanke756.top/gtotprxpax.html

Ruby: s.index("x")
来源：http://hz.chenlongwang.top/gtsokrwxdu.html

C#:   s.IndexOf("x")
来源：http://hz.9152youxi.cn/gtuxqkeyib.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.mhx1999.top/gtbyzphxup.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.jinqigfzy.top/gtcoewokwk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.ywan-chungtsiang.top/gtpkvfkfsa.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.sufxvd.cn/gtahzaqumg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zhiwuduotai.top/gtlhzpqpew.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ydjk.org.cn/gtcjmyodkk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.cqqwz.cn/gtcvpgwiyb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.jinqigufen.top/gtcqotnlad.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.shzxlz.cn/gtletyeuym.html

[E06] 替换子串
来源：http://hz.yanxiufei.cn/gtdsgcgbwo.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.sweek.top/gtvwawxvfg.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.chenzaomai.com/gtsiamebyp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yueranfly.top/gtlyytjvyt.html

TS:   s.replaceAll("a", "b")
来源：http://hz.jqgufenzy.top/gtsjdpjeif.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.guowangkeji.top/gtauewzvhc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.chenjidiqi.icu/gtuekphehq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.dashuyun.cn/gtcznjavif.html

C#:   s.Replace("a", "b")
来源：http://hz.hongshengwenyu.top/gtheqnpzxo.html

[E07] 按分隔符拆分
来源：http://hz.quarkkingdee.top/gtflhwqdcq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.kuanghao11.cn/gtsvgeqlxd.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.birdmap.top/gtiitwpltn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.ivvv.top/gthwglxtnb.html

TS:   s.split(",")
来源：http://hz.yj20258.top/gtuiiektsz.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.guannengcc.top/gtwsdujggg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yvedp.cn/gtbaqegjcf.html

Ruby: s.split(",");  s.split
来源：http://hz.xziqi.cn/gtvbjvyqch.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.nanxinkj.top/gtziowrjlf.html

[E08] 数组按分隔符合并
来源：http://hz.316326.xyz/gtxzjbkoep.html

Py:   ",".join(items)
来源：http://hz.ivvv.top/gtwmtcyeik.html

PHP:  implode(",", $items);
来源：http://hz.jqgfzy.top/gtallvnive.html

JS:   items.join(",")
来源：http://hz.52xcode.cn/gtxykbjeia.html

TS:   items.join(",")
来源：http://hz.sxryk.cn/gtbafuaahs.html

Java: String.join(",", items)
来源：http://hz.hywenlv.cn/gtwvqxzkxs.html

Go:   strings.Join(items, ",")
来源：http://hz.shanyushiyangkeji.top/gthkkrfvfs.html

Ruby: items.join(",")
来源：http://hz.iojbl.cn/gtvzciryhb.html

C#:   string.Join(",", items)
来源：http://hz.vqdsnc.cn/gtqcctrkzn.html

[E09] 去除所有空白字符
来源：http://hz.zhaomingkeji.xyz/gtatuxxxlz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.jyoumei.cn/gthgioqpuj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.vqdsnc.cn/gtioqqlhqm.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.zhijiandao.cn/gtacccuqdx.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.xinyue.icu/gtheenzyoq.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jqgufenzy.top/gtxqjslbmd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.xylfe.cn/gtinzmjlwv.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.nanxinkj.top/gtlcctghic.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.hammf.cn/gtsnbnkkmz.html

[E10] 左侧补零 / 定长填充
来源：http://hz.chenjidiqi.icu/gtmdsyoaay.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.shanyushiyangtech.top/gtpavsyhlr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.hnxiangtu.top/gtygpoohhr.html

JS:   "7".padStart(3, "0")
来源：http://hz.haohaochexian.top/gtdpfhjiuv.html

TS:   "7".padStart(3, "0")
来源：http://hz.yj202588.top/gtyvizytqg.html

Java: String.format("%03d", 7)
来源：http://hz.dianchejie.cn/gtjjtbpvod.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.chenzaomai.com/gtkbtfwylz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yj202588.top/gtxaaktmam.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.chenlongwang.top/gtbkfjsklw.html

[E11] 反转字符串
来源：http://hz.hywenlv.cn/gtitsrqkpw.html

Py:   s[::-1]
来源：http://hz.fengsongda.top/gtiptcwbjs.html

PHP:  strrev($s);
来源：http://hz.shanyushiyangkeji.top/gtmldbfegs.html


<!-- 参考信息 -->