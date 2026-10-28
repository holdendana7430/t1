代发 wailian999

[D07] 切片 / 取子数组
来源：http://hz.bjfxy.top/gtneueatst.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.cdnleiting.top/gtwvcylpwn.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.nanxinkj.top/gtrkwybylj.html

JS:   arr.slice(1, 4);
来源：http://hz.sufxvd.cn/gtpoitwdjz.html

TS:   arr.slice(1, 4);
来源：http://hz.andypj.xyz/gtifrlcivq.html

Java: list.subList(1, 4);
来源：http://hz.gotoacloud.top/gtbgfcdbal.html

Go:   arr[1:4]
来源：http://hz.yongpay.top/gtbqurhbpb.html

Ruby: arr[1, 3]
来源：http://hz.zhiwuduotai.top/gtbofqcsyx.html

C#:   list.GetRange(1, 3);
来源：http://hz.jianghu66.top/gtjougzihh.html

[D08] 合并两个数组
来源：http://hz.yj20258.top/gthzmbeqsx.html

Py:   a + b;  a.extend(b)
来源：http://hz.havefunace.top/gtgnikblss.html

PHP:  array_merge($a, $b);
来源：http://hz.feifeiyinyue.top/gtjwdxvoso.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yj20258.top/gtumvlytzq.html

TS:   [...a, ...b];
来源：http://hz.hongshengwenyu.top/gtzrtkbpma.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yj20258.top/gtwtiromjb.html

Go:   append(a, b...)
来源：http://hz.xuanzx.com/gtalxjuckd.html

Ruby: a + b;  a.concat(b)
来源：http://hz.cucudq.cn/gtjtnwamyr.html

C#:   a.Concat(b).ToList()
来源：http://hz.hongshengwenyu.top/gtprwwcmch.html

[D09] 排序（升序）
来源：http://hz.ivvv.top/gtagqjifbq.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sxryk.cn/gtusuwzlfc.html

PHP:  sort($arr);
来源：http://hz.jinghuilouyu.cn/gtnzvifxyx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.jqgufenzy.top/gtrpnjacua.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yuanzhike.top/gtibzgvcsr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.andypj.xyz/gtkxnaygve.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.sufxvd.cn/gtkiljjpgw.html

Ruby: arr.sort
来源：http://hz.pengpengdd.cyou/gtdlxrhjyp.html

C#:   list.Sort();
来源：http://hz.hfpthk.cn/gtufcbjajh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zdqjudy.top/gtzzirkyfx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.ppjwa.cn/gtsecnmffm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.guowangkeji.top/gtuhssvynl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xylfe.cn/gtjyappvby.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.haohaochexian.top/gtpkfqjvar.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yuanzhike.top/gtoqtuyuta.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.shanyushiyangkeji.top/gtmmffgcwx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yonumen.top/gtqxmvytkm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.vqdsnc.cn/gtklxxljcr.html

[D11] 反转数组
来源：http://hz.hnxiangtu.top/gtcvuoqcrt.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.ppjwa.cn/gtypxnubno.html

PHP:  array_reverse($arr);
来源：http://hz.gogol.net.cn/gtnxemsuas.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.birdmap.top/gtwxzkgecv.html

TS:   [...arr].reverse();
来源：http://hz.c1oappe.top/gtptkqragt.html

Java: Collections.reverse(list);
来源：http://hz.yvedp.cn/gtsihpowmc.html

Go:   slices.Reverse(arr)
来源：http://hz.nwbrower.top/gtofszwgcx.html

Ruby: arr.reverse
来源：http://hz.cqqwz.cn/gtxjnswmkw.html

C#:   list.Reverse();
来源：http://hz.jinqigufen.top/gtdlvsdqqz.html

[D12] 查找元素下标
来源：http://hz.shangyingyoupin.top/gtykehckdu.html

Py:   arr.index(x);  x in arr
来源：http://hz.jqgfzy.top/gthyocebjt.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.dashuyun.cn/gtxllxtkeh.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.tanke756.top/gtkxxhmqda.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hywenlv.cn/gtnmtyudmo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.yueranfly.top/gtotvasngz.html

Go:   slices.Index(arr, x)
来源：http://hz.ywan-chungtsiang.top/gtcvymnoxb.html

Ruby: arr.index(x)
来源：http://hz.daria6918.cn/gtjmcpfmcw.html

C#:   list.IndexOf(x);
来源：http://hz.yuanzhike.top/gtpamtckwi.html

[D13] 过滤（保留满足条件的）
来源：http://hz.vqdsnc.cn/gtongbimpo.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.daxiang520.top/gtmejnccwk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yangfankeji.com/gtopllptmp.html

JS:   arr.filter(x => x > 3)
来源：http://hz.shuidangran.top/gtbcvbbeqo.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jqgufenzy.top/gtvibanlbd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.nanxinkj.top/gtvfhrygvz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yanxiufei.cn/gtfwpdtvgu.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.daxiang520.top/gtilfqymzr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.havefunace.top/gttydoaubo.html

[D14] 映射转换（每个元素变形）
来源：http://hz.ydjk.org.cn/gtuwblstya.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.sufxvd.cn/gtrspvmpoy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.shanyushiyangtech.top/gtgrlmwwxs.html

JS:   arr.map(x => x * 2)
来源：http://hz.nwbrower.top/gtgumbitok.html

TS:   arr.map(x => x * 2)
来源：http://hz.xinyue.icu/gtwwsgafxn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.feifeiyinyue.top/gtdrmtivrt.html

Go:   // 手写循环
来源：http://hz.0kj1m.cn/gtiwavfgku.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.jinqigufen.top/gtnatashlb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.ybcxt.top/gtcyjiefng.html

[D15] 去重
来源：http://hz.dashuyun.cn/gtgynohfpa.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.pengpengdd.cyou/gtlgwujzwf.html

PHP:  array_unique($arr);
来源：http://hz.redwolf501.top/gtscjbfpwm.html

JS:   [...new Set(arr)]
来源：http://hz.nwbrower.top/gtxmnkswwj.html

TS:   [...new Set(arr)]
来源：http://hz.shanyushiyangtech.top/gthesbgbcv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yanxiufei.cn/gtwrmyndnq.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.ppjwa.cn/gtgbzrutnb.html

Ruby: arr.uniq
来源：http://hz.guannengcc.top/gtcfxflrjd.html

C#:   list.Distinct().ToList()
来源：http://hz.zhaomingkeji.xyz/gttnjnryvb.html

[D16] 求和与平均值
来源：http://hz.bjfxy.top/gtgsstlgww.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.iojbl.cn/gtpyiiqylr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.zhaomingkeji.xyz/gtzdyeqtef.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yanxiufei.cn/gtfntdgwbf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.daxiang520.top/gtyyjgruzh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.zhoulong.xyz/gtzapkpewy.html

Go:   // 手写循环累加
来源：http://hz.ppjwa.cn/gtgrlgdkmr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.hammf.cn/gtmtkompyq.html

C#:   list.Sum();  list.Average()
来源：http://hz.cdnleiting.top/gtwsaokrcz.html

[D17] 最大值与最小值
来源：http://hz.cheryme.top/gthljvceua.html

Py:   max(arr);  min(arr)
来源：http://hz.pycfn.com/gtjfegtwnl.html

PHP:  max($arr);  min($arr);
来源：http://hz.wangdashe.top/gtofpwjinx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.jinyuanbaomall.cn/gtmilnchkz.html

TS:   Math.max(...arr);
来源：http://hz.gaohongyu789.top/gtpvclmioj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.mhx1999.top/gtcijmzcpu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.nanxinkj.top/gtuojdvfld.html

Ruby: arr.max;  arr.min
来源：http://hz.52xcode.cn/gtmbkpyzzl.html

C#:   list.Max();  list.Min()
来源：http://hz.andypj.xyz/gtwojgotga.html

[D18] 扁平化嵌套数组
来源：http://hz.ehwqpu.com/gtdxmkqcha.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yuanzhike.top/gtklftwdrm.html

PHP:  array_merge(...$nested);
来源：http://hz.hongshengwenyu.top/gtqcfwxpzi.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.guowangkeji.top/gtcnloprbk.html

TS:   nested.flat();
来源：http://hz.xuetiantiany.cn/gtucnpfuxk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.daxiang520.top/gtfxuhfhvx.html

Go:   // 手写双层循环
来源：http://hz.ehwqpu.com/gtdtbjrlfs.html

Ruby: nested.flatten
来源：http://hz.fzhhl.top/gttezyjvlx.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yonumen.top/gtqncukohq.html

[D19] 按字段分组
来源：http://hz.xinyue.icu/gtolhxzufg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.gzhubu.top/gthsxcxtgf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.dianchejie.cn/gtfdhniynh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.gzhubu.top/gttiptnxnd.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yongpay.top/gtigugwoyl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zhengqikj.top/gtgjuonmwu.html

Go:   // 手写 map[string][]T
来源：http://hz.hnxiangtu.top/gtvfluonzb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.gotoacloud.top/gtbxpqsucn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.shangyingyoupin.top/gtcivbdvlu.html

[D20] 统计每个元素出现次数
来源：http://hz.smart0.xyz/gtuzcjozpn.html

Py:   Counter(arr)
来源：http://hz.pengpengdd.cyou/gtaxbdbsdm.html

PHP:  array_count_values($arr);
来源：http://hz.gzhubu.top/gtwzwgrbrc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ivvv.top/gtwqdrrlon.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.smart0.xyz/gtldzgpyjq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.daria6918.cn/gtgtzhkzmp.html

Go:   // 手写 map[T]int
来源：http://hz.yuanzhike.top/gtfckmropt.html

Ruby: arr.tally
来源：http://hz.zhaomingkeji.xyz/gtptjxzfak.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.wangshuangyany.cn/gtpftcdwol.html

[D21] 判断是否包含某元素
来源：http://hz.zycfv.cn/gtlhctvwfi.html

Py:   x in arr
来源：http://hz.daria6918.cn/gtejloxvzk.html

PHP:  in_array($x, $arr, true);
来源：http://hz.snrcjt.cn/gtvglzkdsy.html

JS:   arr.includes(x)
来源：http://hz.sweek.top/gtfordjlcy.html

TS:   arr.includes(x)
来源：http://hz.ydzc1.top/gtncubxyeb.html

Java: list.contains(x)
来源：http://hz.cucudq.cn/gtgviexyze.html

Go:   slices.Contains(arr, x)
来源：http://hz.zhijiandao.cn/gtxaomlvoo.html

Ruby: arr.include?(x)
来源：http://hz.gotoacloud.top/gtvbzczcfi.html

C#:   list.Contains(x)
来源：http://hz.zdqjudy.top/gtxlhtpmgy.html

[D22] 复制数组（避免共享引用）
来源：http://hz.cheryme.top/gtdtplvpdm.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.zhongyouzk.top/gtgopnatai.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.gaohongyu789.top/gtuviybzoo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.mhx1999.top/gtsajqgvrl.html

TS:   [...arr];
来源：http://hz.hnxiangtu.top/gtjlzbqryh.html

Java: new ArrayList<>(list);
来源：http://hz.hnqzz.top/gtnggsygdn.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.zhijiandao.cn/gtemsssxcg.html

Ruby: arr.dup;  arr.clone
来源：http://hz.cashguo.top/gtisjklemf.html

C#:   new List<int>(list);
来源：http://hz.0kj1m.cn/gtrtamkyta.html

[D23] reduce 累积计算
来源：http://hz.kuanghao11.cn/gtjnxffjva.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jiagoushi.top/gtxovjaivb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.hongshengwenyu.top/gtvhvqkmbu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.birdmap.top/gtgjyxmqqk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.sysykeji.top/gtooplarkw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.svipenyu.cn/gtordjnigu.html

Go:   // 手写循环
来源：http://hz.ybcxt.top/gtsjbsykzr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.cucudq.cn/gteraodrdh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.hywenlv.cn/gtddgxnwjp.html

[D24] 字典 / Map 基本操作
来源：http://hz.jinqigufen.top/gtxiebmdid.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.daria6918.cn/gtimvqejwj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.xinyue.icu/gtnmneyyxd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.dashuyun.cn/gtxsmhnsch.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.shanyushiyangtech.top/gtzjduvkbj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.cashguo.top/gtgczdbvex.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.feifeiyinyue.top/gtuzfdkkyi.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.xylfe.cn/gtnkkofdwk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.kuanghao11.cn/gtxnviddww.html

[D25] Set 集合去重与交并差
来源：http://hz.sxryk.cn/gtkziebrqj.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.shanyushiyangkeji.top/gtpjhlfikp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.hnqzz.top/gtheqaofrs.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.hammf.cn/gthbwikwpz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.sxryk.cn/gtdwowvjlp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.zhixingplan.top/gtqwnsbihe.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yanxiufei.cn/gtmhyzzavc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.xingfuxueyuan.xyz/gtzrbshfvj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yonumen.top/gttggobdlh.html

[D26] 数组转字符串
来源：http://hz.cqqwz.cn/gtfmfrkmpm.html

Py:   ", ".join(map(str, arr))
来源：http://hz.havefunace.top/gtybzdmmfy.html

PHP:  implode(", ", $arr);
来源：http://hz.fengsongda.top/gtttlquooh.html

JS:   arr.join(", ")
来源：http://hz.tianlin.xyz/gthpvjsaan.html

TS:   arr.join(", ")
来源：http://hz.zhaomingkeji.xyz/gtvslkiujb.html

Java: String.join(", ", list)
来源：http://hz.daria6918.cn/gtvskqczae.html

Go:   strings.Join(strs, ", ")
来源：http://hz.birdmap.top/gtqtwznygo.html

Ruby: arr.join(", ")
来源：http://hz.sufxvd.cn/gtbinyvwbg.html

C#:   string.Join(", ", list)
来源：http://hz.0kj1m.cn/gtaptfenxm.html

================================================================================
来源：http://hz.yonumen.top/gtyoqvroih.html

E. 字符串处理
来源：http://hz.jianghu66.top/gtqyyfrjlj.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtrxdebtil.html

[E01] 拼接字符串
来源：http://hz.xinyue.icu/gtahxqqhod.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.sufxvd.cn/gtivccffje.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.nanxuanxn.top/gtlduqjfci.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.shzxlz.cn/gtljkpufhx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ywan-chungtsiang.top/gtlkesratt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.shuidangran.top/gtcqtunrff.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.jinyuanbaomall.cn/gtvwkdfogo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yongpay.top/gtcdjxheug.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.jinqigufen.top/gttthsrequ.html

[E02] 重复字符串
来源：http://hz.birdmap.top/gtrwceijws.html

Py:   "ab" * 3
来源：http://hz.cashguo.top/gtfugwvune.html

PHP:  str_repeat("ab", 3);
来源：http://hz.9152youxi.cn/gtnlapvrmq.html

JS:   "ab".repeat(3)
来源：http://hz.redwolf501.top/gtdcfjymbb.html

TS:   "ab".repeat(3)
来源：http://hz.dianchejie.cn/gtnprpjnsc.html

Java: "ab".repeat(3)
来源：http://hz.jiagoushi.top/gtecforszp.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.0kj1m.cn/gtkdghlcls.html

Ruby: "ab" * 3
来源：http://hz.yuanzhike.top/gtyaxzrpjn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.bjfxy.top/gteycrfjuy.html

[E03] 截取子串
来源：http://hz.svipenyu.cn/gtlkyypgcm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.hfpthk.cn/gtdnrwnocv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.ydzc1.top/gtxyohnklh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.bjfxy.top/gtqokyjyqr.html

TS:   s.slice(1, 4)
来源：http://hz.aizwys.cn/gtwuavfpem.html

Java: s.substring(1, 4)
来源：http://hz.ydjk.org.cn/gtmoezslhj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yuxming.cn/gtsshwtmok.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.xuetiantiany.cn/gtmjwvmvni.html

C#:   s.Substring(1, 3)
来源：http://hz.xuetiantiany.cn/gtdbxsalaa.html

[E04] 查找子串位置
来源：http://hz.xziqi.cn/gtxlzfmqyz.html

Py:   s.find("x");  s.index("x")
来源：http://hz.dashuyun.cn/gtpvjxcrju.html

PHP:  strpos($s, "x");
来源：http://hz.xziqi.cn/gtgmjqumoc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.pengpengdd.cyou/gtsmrswfzq.html

TS:   s.indexOf("x")
来源：http://hz.ppjwa.cn/gtdvitchgz.html

Java: s.indexOf("x")
来源：http://hz.ywan-chungtsiang.top/gthehfjvwn.html

Go:   strings.Index(s, "x")
来源：http://hz.chenzaomai.com/gtpsxczubq.html

Ruby: s.index("x")
来源：http://hz.andypj.xyz/gtzdrlqyne.html

C#:   s.IndexOf("x")
来源：http://hz.sufxvd.cn/gttufrltyj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.gaohongyu789.top/gtdlzkimxl.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.yueranfly.top/gtakkqtenn.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.dianchejie.cn/gtrigrnaec.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.kuanghao11.cn/gthqorympq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.jqgfzy.top/gtwywlsods.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.shuidangran.top/gtgiebbngh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.cucudq.cn/gtcwwsizto.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.feifeiyinyue.top/gtfbfaoqha.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.sweek.top/gttruvmbce.html

[E06] 替换子串
来源：http://hz.jianghu66.top/gtpirbvcor.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.guannengcc.top/gtqckbhdon.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.haohaochexian.top/gtzzzsjppi.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.gogol.net.cn/gtpdhjjfun.html

TS:   s.replaceAll("a", "b")
来源：http://hz.haohaochexian.top/gtdemmairl.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.gogol.net.cn/gthlusyurl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.zhixingplan.top/gtwcsesepc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.xuetiantiany.cn/gtozvfdjkv.html

C#:   s.Replace("a", "b")
来源：http://hz.cheryme.top/gtgtzcbelm.html

[E07] 按分隔符拆分
来源：http://hz.gotoacloud.top/gttsqrjyoo.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.kuanghao11.cn/gtgwxtfrgs.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.andypj.xyz/gtgfhamrou.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.jinghuilouyu.cn/gtvnlesoka.html

TS:   s.split(",")
来源：http://hz.cashguo.top/gtnbddvdyh.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.yj20258888.top/gtnepkvdhk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yuxming.cn/gtgkfxkbqm.html

Ruby: s.split(",");  s.split
来源：http://hz.guowangkeji.top/gtqhsjxius.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.hfpthk.cn/gtrmrtelmz.html

[E08] 数组按分隔符合并
来源：http://hz.sufxvd.cn/gtguphwnzs.html

Py:   ",".join(items)
来源：http://hz.zhijiandao.cn/gtgknubhio.html

PHP:  implode(",", $items);
来源：http://hz.gaohongyu789.top/gtpplpskld.html

JS:   items.join(",")
来源：http://hz.guannengcc.top/gtxmjwqhuh.html

TS:   items.join(",")
来源：http://hz.zhoulong.xyz/gtlnwtuvgv.html

Java: String.join(",", items)
来源：http://hz.redwolf501.top/gtykzxpdpf.html

Go:   strings.Join(items, ",")
来源：http://hz.nanxinkj.top/gtfnrazknl.html

Ruby: items.join(",")
来源：http://hz.yonumen.top/gtkhwfjbdu.html

C#:   string.Join(",", items)
来源：http://hz.hywenlv.cn/gtgzudvxgn.html

[E09] 去除所有空白字符
来源：http://hz.ydzc1.top/gtlhbkteuu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yj20258.top/gtwfzbqfey.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.hysaishi.cn/gtagaplucx.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.yongpay.top/gtkceootaw.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.sysykeji.top/gteepxfjqr.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.chenjidiqi.icu/gtpvcdosio.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.jqgufenzy.top/gtecgtcquf.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.zhiwuduotai.top/gtpqqavepj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.hammf.cn/gtwarhrkrd.html

[E10] 左侧补零 / 定长填充
来源：http://hz.ivvv.top/gtbgmyuuqs.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.smart0.xyz/gtglfklasu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.xziqi.cn/gtbtdpjtnt.html

JS:   "7".padStart(3, "0")
来源：http://hz.mhx1999.top/gtyqdgjkpr.html

TS:   "7".padStart(3, "0")
来源：http://hz.52xcode.cn/gtnmnenjjc.html

Java: String.format("%03d", 7)
来源：http://hz.sxryk.cn/gtdtsthoej.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yuanzhike.top/gtiwmyqzkx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.jlsjyb.cn/gtmcnarhbo.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.quarkkingdee.top/gteoitfebm.html

[E11] 反转字符串
来源：http://hz.yanxiufei.cn/gtseadsqgz.html

Py:   s[::-1]
来源：http://hz.jinyuanbaomall.cn/gtndsepvwg.html

PHP:  strrev($s);
来源：http://hz.gaohongyu789.top/gtrnmbvvzg.html

JS:   [...s].reverse().join("")
来源：http://hz.jlsjyb.cn/gtxbjmwocp.html

TS:   [...s].reverse().join("")
来源：http://hz.hongshengwenyu.top/gttlnjqryl.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.hysaishi.cn/gtbvodoeie.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.shanyushiyangkeji.top/gtfmcavbvx.html

Ruby: s.reverse
来源：http://hz.gotoacloud.top/gtqvrnfgyd.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.dianchejie.cn/gtwvlevmqo.html

[E12] 统计某字符出现次数
来源：http://hz.52xcode.cn/gtqflngvzb.html

Py:   s.count("a")
来源：http://hz.mhx1999.top/gtywnlhpcx.html

PHP:  substr_count($s, "a");
来源：http://hz.hysaishi.cn/gtrmjxyjpp.html

JS:   s.split("a").length - 1
来源：http://hz.yanxiufei.cn/gtxnlnibvk.html

TS:   s.split("a").length - 1
来源：http://hz.gaohongyu789.top/gtilinqimw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yuxming.cn/gtvpjzovdp.html

Go:   strings.Count(s, "a")
来源：http://hz.aizwys.cn/gtqaeitzma.html

Ruby: s.count("a")
来源：http://hz.haohaochexian.top/gtjqnuunsy.html

C#:   s.Count(c => c == 'a')
来源：http://hz.smart0.xyz/gtlnzrsmje.html

[E13] 逐字符遍历
来源：http://hz.zycfv.cn/gtwzocwcde.html

Py:   for ch in s: print(ch)
来源：http://hz.hammf.cn/gtyyclbczy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.tianlin.xyz/gtmtvqfjhc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.guowangkeji.top/gtcqzieidx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.dashuyun.cn/gtydlyfrmy.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.zhijiandao.cn/gtvlbvqaac.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jinyuanbaomall.cn/gtqggjjced.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.guannengcc.top/gttyhjhgxy.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.cqqwz.cn/gtqdkayvdv.html


<!-- 参考信息 -->