代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.gogol.net.cn/gtuuqeloti.html

TS:   [...a, ...b];
来源：http://hz.chenzaomai.com/gtzpvxwyub.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yuanzhike.top/gtblyxckkp.html

Go:   append(a, b...)
来源：http://hz.shangyingyoupin.top/gtlarvfzcv.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yueranfly.top/gtzriyjedw.html

C#:   a.Concat(b).ToList()
来源：http://hz.svipenyu.cn/gtxeibpilf.html

[D09] 排序（升序）
来源：http://hz.zhoulong.xyz/gtraywyumb.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sxryk.cn/gtpkibfjeh.html

PHP:  sort($arr);
来源：http://hz.jqgufenzy.top/gtvnazsmxu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.kuanghao11.cn/gtbdbktkxf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.meibo888.top/gtmaqjbkks.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.dashuyun.cn/gtdwvplzrq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.zdqjudy.top/gtxzxufqhw.html

Ruby: arr.sort
来源：http://hz.redwolf501.top/gtekkepdud.html

C#:   list.Sort();
来源：http://hz.zhiwuduotai.top/gtatdhlmkc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.chenzaomai.com/gtiyniikwt.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.svipenyu.cn/gtymllfwaq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.aibaodan.cn/gtyveprqlf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhaomingkeji.xyz/gtpfjptzyo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.aizwys.cn/gthsprkegu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yj20258888.top/gtfwjndogf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.andypj.xyz/gtbudoxijv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.xziqi.cn/gtyxqdmdbc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.hnxiangtu.top/gtvnkpfjpb.html

[D11] 反转数组
来源：http://hz.sysykeji.top/gtdwxyqvxp.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.bjfxy.top/gthwywrmrs.html

PHP:  array_reverse($arr);
来源：http://hz.yvedp.cn/gtfgdtyzxg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yonumen.top/gtynjvyymn.html

TS:   [...arr].reverse();
来源：http://hz.guannengcc.top/gtnsnrmxmh.html

Java: Collections.reverse(list);
来源：http://hz.gaohongyu789.top/gtieesjils.html

Go:   slices.Reverse(arr)
来源：http://hz.cucudq.cn/gtzvrxqhcu.html

Ruby: arr.reverse
来源：http://hz.shanyushiyangkeji.top/gtuktsvkve.html

C#:   list.Reverse();
来源：http://hz.cqqwz.cn/gtydprheii.html

[D12] 查找元素下标
来源：http://hz.9152youxi.cn/gtlbmlibfy.html

Py:   arr.index(x);  x in arr
来源：http://hz.jqgufenzy.top/gtvoyjzmdo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yuxming.cn/gtvqyvhlue.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.52xcode.cn/gtzndkpzoz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.meibo888.top/gtfamgsamp.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.52xcode.cn/gtuutfqbep.html

Go:   slices.Index(arr, x)
来源：http://hz.aibaodan.cn/gtctkswsre.html

Ruby: arr.index(x)
来源：http://hz.vqdsnc.cn/gtpesqhwdt.html

C#:   list.IndexOf(x);
来源：http://hz.pycfn.com/gtfohklirp.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jianghu66.top/gtkywskues.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.ehwqpu.com/gtgblcczbs.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.gogol.net.cn/gtmyeijpdh.html

JS:   arr.filter(x => x > 3)
来源：http://hz.quarkkingdee.top/gtvupotzam.html

TS:   arr.filter(x => x > 3)
来源：http://hz.zycfv.cn/gtimmznnvr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.ydjk.org.cn/gtdbwsrtsz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jinghuilouyu.cn/gtszbczhae.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.cqqwz.cn/gtjvnazpye.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.shanyushiyangtech.top/gtprhkumfx.html

[D14] 映射转换（每个元素变形）
来源：http://hz.zhixingplan.top/gtsvbzlupa.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.hongshengwenyu.top/gtxjhtnkap.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.c1oappe.top/gtheptutvq.html

JS:   arr.map(x => x * 2)
来源：http://hz.cashguo.top/gtzpqdomnx.html

TS:   arr.map(x => x * 2)
来源：http://hz.yueranfly.top/gtwnklhswe.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.chenlongwang.top/gtomotkymf.html

Go:   // 手写循环
来源：http://hz.fzhhl.top/gtuvxvrlxv.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.zdqjudy.top/gtlttgclot.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.zhongyouzk.top/gtijtzfurw.html

[D15] 去重
来源：http://hz.cdnleiting.top/gtkdciuqvf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jqgfzy.top/gtzanludtk.html

PHP:  array_unique($arr);
来源：http://hz.smart0.xyz/gtedpzghnr.html

JS:   [...new Set(arr)]
来源：http://hz.cucudq.cn/gtxebvcbyj.html

TS:   [...new Set(arr)]
来源：http://hz.52xcode.cn/gtbbbucrau.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.daxiang520.top/gtkicizdqi.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.tanke756.top/gtomprhatr.html

Ruby: arr.uniq
来源：http://hz.yj20258888.top/gtcqnomxiz.html

C#:   list.Distinct().ToList()
来源：http://hz.wangshuangyany.cn/gtdcvkkiim.html

[D16] 求和与平均值
来源：http://hz.jyoumei.cn/gtzyeehdmi.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.zhixingplan.top/gtwteyxvww.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.iojbl.cn/gtwikqkavm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.feifeiyinyue.top/gtdnejnmdc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.redwolf501.top/gtaanvvtsb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.jinghuilouyu.cn/gtbshwkhff.html

Go:   // 手写循环累加
来源：http://hz.tianlin.xyz/gtsfagkhgp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.fengsongda.top/gtjsdhcews.html

C#:   list.Sum();  list.Average()
来源：http://hz.bjfxy.top/gtajrvldwc.html

[D17] 最大值与最小值
来源：http://hz.yonumen.top/gtltalzzwy.html

Py:   max(arr);  min(arr)
来源：http://hz.jinyuanbaomall.cn/gtpfioxinw.html

PHP:  max($arr);  min($arr);
来源：http://hz.daria6918.cn/gtyuegcnkp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.aizwys.cn/gtgrustvil.html

TS:   Math.max(...arr);
来源：http://hz.jinyuanbaomall.cn/gtwyzlcewm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.0kj1m.cn/gtuvttngpa.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.tianlin.xyz/gthzqlxutj.html

Ruby: arr.max;  arr.min
来源：http://hz.hywenlv.cn/gttsdsxmuu.html

C#:   list.Max();  list.Min()
来源：http://hz.yueranfly.top/gtailozjny.html

[D18] 扁平化嵌套数组
来源：http://hz.hfpthk.cn/gtmkejnqqx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.hfpthk.cn/gtshwkaoez.html

PHP:  array_merge(...$nested);
来源：http://hz.birdmap.top/gtmsyyfnbb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.shanyushiyangkeji.top/gtfrhodnpf.html

TS:   nested.flat();
来源：http://hz.zhongyouzk.top/gtsrnyddqa.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.chenlongwang.top/gtjaenchsu.html

Go:   // 手写双层循环
来源：http://hz.nanxuanxn.top/gtdikwginh.html

Ruby: nested.flatten
来源：http://hz.hnxiangtu.top/gtymgxkuip.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yj202588.top/gtmtmcwujd.html

[D19] 按字段分组
来源：http://hz.zhoulong.xyz/gtgrgaxjyp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yangfankeji.com/gtaatdigzd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.xuanzx.com/gtatvqxmnb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.gzhubu.top/gtdfbsyhfo.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.ywan-chungtsiang.top/gtsytqgvcu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.fzhhl.top/gtxqdddrys.html

Go:   // 手写 map[string][]T
来源：http://hz.yuanzhike.top/gtulvqckpx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.ppjwa.cn/gtnhwufltx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.zhengqikj.top/gtjjwfibpe.html

[D20] 统计每个元素出现次数
来源：http://hz.pengpengdd.cyou/gtcopeyymn.html

Py:   Counter(arr)
来源：http://hz.redwolf501.top/gtaypjzakl.html

PHP:  array_count_values($arr);
来源：http://hz.yj20258.top/gtzdjzmkkx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhoulong.xyz/gtvodtxbjr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.mhx1999.top/gthwxeuszw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.hfpthk.cn/gtcvscgzue.html

Go:   // 手写 map[T]int
来源：http://hz.hnxiangtu.top/gtjevjsjqe.html

Ruby: arr.tally
来源：http://hz.yvedp.cn/gtrxvsxgci.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.dianchejie.cn/gtdypdfgip.html

[D21] 判断是否包含某元素
来源：http://hz.sxryk.cn/gtoypokrtd.html

Py:   x in arr
来源：http://hz.andypj.xyz/gtaefzbgdh.html

PHP:  in_array($x, $arr, true);
来源：http://hz.cheryme.top/gthexxuwbe.html

JS:   arr.includes(x)
来源：http://hz.daxiang520.top/gtcrfqrzvq.html

TS:   arr.includes(x)
来源：http://hz.hywenlv.cn/gtdxlnyygp.html

Java: list.contains(x)
来源：http://hz.jianghu66.top/gtcxaxsxis.html

Go:   slices.Contains(arr, x)
来源：http://hz.chenjidiqi.icu/gtteidmcgo.html

Ruby: arr.include?(x)
来源：http://hz.zhaomingkeji.xyz/gtjhhtaccy.html

C#:   list.Contains(x)
来源：http://hz.cheryme.top/gtuelannke.html

[D22] 复制数组（避免共享引用）
来源：http://hz.hnxiangtu.top/gtdvlgamwa.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.ydzc1.top/gtoaltvqxo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.redwolf501.top/gtvoclmlfu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.hnxiangtu.top/gtgjaftfik.html

TS:   [...arr];
来源：http://hz.jianghu66.top/gtqfnsuzvi.html

Java: new ArrayList<>(list);
来源：http://hz.quarkkingdee.top/gthbwfovut.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.ydzc1.top/gtokjmqbfc.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yj20258888.top/gtlsorqwij.html

C#:   new List<int>(list);
来源：http://hz.yj20258888.top/gtaixxjqvr.html

[D23] reduce 累积计算
来源：http://hz.aizwys.cn/gtkpnszhda.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.hywenlv.cn/gtkaapzche.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.daria6918.cn/gtcdapcfom.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.wangdashe.top/gttegramuk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hywenlv.cn/gtdqesthwc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.ydjk.org.cn/gtxojdtxza.html

Go:   // 手写循环
来源：http://hz.havefunace.top/gtjswifvtk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.0kj1m.cn/gtittjsbuh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.haohaochexian.top/gtemfrotnw.html

[D24] 字典 / Map 基本操作
来源：http://hz.yj202588.top/gtvufkggdk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.haohaochexian.top/gtohtnskpq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.shanyushiyangtech.top/gtjlivskgw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.chenjidiqi.icu/gtkjkhfdrq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.wangdashe.top/gtedurzecj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.ehwqpu.com/gteoqhztvm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.jianghu66.top/gtvwjhogww.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.shuidangran.top/gtyotfktkc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.xuetiantiany.cn/gtrihnqdsd.html

[D25] Set 集合去重与交并差
来源：http://hz.jinqigufen.top/gtcagornkv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yanxiufei.cn/gtacunqgfg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.shanyushiyangtech.top/gtqdnwocuj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.kuanghao11.cn/gtdnafkpss.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.zhongyouzk.top/gtxmrkcesz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.jiagoushi.top/gtcqsxhvri.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.guannengcc.top/gthynptrwo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.ywan-chungtsiang.top/gtezigcrin.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.feifeiyinyue.top/gtjaasdnbc.html

[D26] 数组转字符串
来源：http://hz.hysaishi.cn/gtqeosscid.html

Py:   ", ".join(map(str, arr))
来源：http://hz.pengpengdd.cyou/gtqryqnesk.html

PHP:  implode(", ", $arr);
来源：http://hz.yangfankeji.com/gtruxzzglp.html

JS:   arr.join(", ")
来源：http://hz.jinqigufen.top/gtrvkckqcv.html

TS:   arr.join(", ")
来源：http://hz.tianlin.xyz/gtzrzcdedx.html

Java: String.join(", ", list)
来源：http://hz.yongpay.top/gtldncgteq.html

Go:   strings.Join(strs, ", ")
来源：http://hz.gotoacloud.top/gtcenxfuri.html

Ruby: arr.join(", ")
来源：http://hz.zdqjudy.top/gtootnbsqe.html

C#:   string.Join(", ", list)
来源：http://hz.jinghuilouyu.cn/gtpuowmgfj.html

================================================================================
来源：http://hz.guannengcc.top/gtjmwzrbcc.html

E. 字符串处理
来源：http://hz.zhoulong.xyz/gtbvhkhyto.html

================================================================================
来源：http://hz.gzhubu.top/gtjumagwcp.html

[E01] 拼接字符串
来源：http://hz.nanxinkj.top/gtycztuppn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.nanxinkj.top/gtdbpqxuag.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.tian-w.cn/gtpemcgwjz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhengqikj.top/gtkmdojlcm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.nanxuanxn.top/gtxjxxpumq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.fengsongda.top/gtjnxyocpd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.316326.xyz/gtsjkdnapo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.wangshuangyany.cn/gtuikiysuf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.ybcxt.top/gtbpmlsspp.html

[E02] 重复字符串
来源：http://hz.9152youxi.cn/gtbnupaanc.html

Py:   "ab" * 3
来源：http://hz.ivvv.top/gthxacizeo.html

PHP:  str_repeat("ab", 3);
来源：http://hz.xylfe.cn/gtskuuqkpg.html

JS:   "ab".repeat(3)
来源：http://hz.yueranfly.top/gtgyugmvit.html

TS:   "ab".repeat(3)
来源：http://hz.c1oappe.top/gtsvpgsnqf.html

Java: "ab".repeat(3)
来源：http://hz.yuxming.cn/gtnkorcmtt.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.yangfankeji.com/gtddyxknkk.html

Ruby: "ab" * 3
来源：http://hz.tian-w.cn/gtdclwjnbq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.tanke756.top/gtgvugyaoh.html

[E03] 截取子串
来源：http://hz.yj202588.top/gtmviqojdu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.smart0.xyz/gtallscdit.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zycfv.cn/gturpmwqya.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jiagoushi.top/gtsiaefpkf.html

TS:   s.slice(1, 4)
来源：http://hz.xinyue.icu/gtbeeobinh.html

Java: s.substring(1, 4)
来源：http://hz.xuanzx.com/gteclbqrae.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.xylfe.cn/gtsjuxizfp.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.nwbrower.top/gtaqejqcuv.html

C#:   s.Substring(1, 3)
来源：http://hz.yongpay.top/gtwmgivwjx.html

[E04] 查找子串位置
来源：http://hz.jinghuilouyu.cn/gtnntygpsk.html

Py:   s.find("x");  s.index("x")
来源：http://hz.jiagoushi.top/gtzgdvjhto.html

PHP:  strpos($s, "x");
来源：http://hz.zhaomingkeji.xyz/gtyxeccuqe.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yanxiufei.cn/gtpdwugxur.html

TS:   s.indexOf("x")
来源：http://hz.xylfe.cn/gtauwyitcc.html

Java: s.indexOf("x")
来源：http://hz.hysaishi.cn/gthdfmcrrl.html

Go:   strings.Index(s, "x")
来源：http://hz.jlsjyb.cn/gtxcewrcnn.html

Ruby: s.index("x")
来源：http://hz.jqgfzy.top/gtxxhgikxk.html

C#:   s.IndexOf("x")
来源：http://hz.ydzc1.top/gtsfeyyqip.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.hongshengwenyu.top/gthocceyzr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.chenlongwang.top/gtylgvlnrr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.ydjk.org.cn/gthrqynkaw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhaomingkeji.xyz/gtgwqtsalo.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.yonumen.top/gtgvuzdqfy.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhiwuduotai.top/gtstfxpaom.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.shzxlz.cn/gtxyyqtmmi.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.daria6918.cn/gtobfixjcy.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.zhongyouzk.top/gtjobwprjy.html

[E06] 替换子串
来源：http://hz.jlsjyb.cn/gtctoxohxw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jiagoushi.top/gtqfpaquhj.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.316326.xyz/gtswuotsub.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hysaishi.cn/gtsymdlove.html

TS:   s.replaceAll("a", "b")
来源：http://hz.zhongyouzk.top/gtmijghgtb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xuanzx.com/gtpdlpuwgg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.svipenyu.cn/gttrthjssg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.tianlin.xyz/gtlqtvqkqg.html

C#:   s.Replace("a", "b")
来源：http://hz.pengpengdd.cyou/gtzbuhcdyw.html

[E07] 按分隔符拆分
来源：http://hz.ybcxt.top/gtkjbjiqrb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.zdqjudy.top/gtnxzncvly.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.aibaodan.cn/gtuobmkgxi.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.ppjwa.cn/gtmmuvwxuv.html

TS:   s.split(",")
来源：http://hz.316326.xyz/gtkqqgxfle.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.jinghuilouyu.cn/gtaftebtro.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yuanzhike.top/gtoeqbqgyd.html

Ruby: s.split(",");  s.split
来源：http://hz.guannengcc.top/gtxwsuueta.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.hfpthk.cn/gtexgdjtyl.html

[E08] 数组按分隔符合并
来源：http://hz.yonumen.top/gtmbrymldn.html

Py:   ",".join(items)
来源：http://hz.zhixingplan.top/gtmwaybrvn.html

PHP:  implode(",", $items);
来源：http://hz.pycfn.com/gtgflbecsf.html

JS:   items.join(",")
来源：http://hz.jinqigfzy.top/gtuextgcrf.html

TS:   items.join(",")
来源：http://hz.andypj.xyz/gtumegipsm.html

Java: String.join(",", items)
来源：http://hz.tanke756.top/gtavmhibjk.html

Go:   strings.Join(items, ",")
来源：http://hz.shangyingyoupin.top/gttzqlwcmh.html

Ruby: items.join(",")
来源：http://hz.xylfe.cn/gtftujpjyc.html

C#:   string.Join(",", items)
来源：http://hz.cashguo.top/gtzpaogibe.html

[E09] 去除所有空白字符
来源：http://hz.zycfv.cn/gttvyaghwp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.zhongyouzk.top/gtqhmxpbgl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.ydjk.org.cn/gtqyriaoah.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.yongpay.top/gtkgbchrqr.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.ybcxt.top/gtqldncbrg.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.aibaodan.cn/gtqpvytsyg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zhengqikj.top/gtqyyfwsvh.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.hnxiangtu.top/gtzhgievsg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.gogol.net.cn/gtwnyusgao.html

[E10] 左侧补零 / 定长填充
来源：http://hz.zhoulong.xyz/gtybsydhlt.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.hnxiangtu.top/gtvjorejel.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.daxiang520.top/gtfcpviawx.html

JS:   "7".padStart(3, "0")
来源：http://hz.jinyuanbaomall.cn/gtinlyrnxn.html

TS:   "7".padStart(3, "0")
来源：http://hz.birdmap.top/gtmeyxjvyo.html

Java: String.format("%03d", 7)
来源：http://hz.jinyuanbaomall.cn/gtmvpucsfw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.gotoacloud.top/gthysfqrlk.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.xingfuxueyuan.xyz/gtyrgqkwmn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.quarkkingdee.top/gtjuclkfpy.html

[E11] 反转字符串
来源：http://hz.andypj.xyz/gtlrjusfcc.html

Py:   s[::-1]
来源：http://hz.jiagoushi.top/gtqbsccqzc.html

PHP:  strrev($s);
来源：http://hz.guannengcc.top/gtzmyogldc.html

JS:   [...s].reverse().join("")
来源：http://hz.ppjwa.cn/gtwlsgneym.html

TS:   [...s].reverse().join("")
来源：http://hz.yonumen.top/gtwgzzwwvw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.daria6918.cn/gttrfjmxnp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.jiagoushi.top/gtgtdcbxay.html

Ruby: s.reverse
来源：http://hz.aibaodan.cn/gtlarbxqmq.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.wangdashe.top/gtetdmfovk.html

[E12] 统计某字符出现次数
来源：http://hz.xuetiantiany.cn/gtcljujbne.html

Py:   s.count("a")
来源：http://hz.chenjidiqi.icu/gtazrxkwdb.html

PHP:  substr_count($s, "a");
来源：http://hz.316326.xyz/gtwmeimgge.html

JS:   s.split("a").length - 1
来源：http://hz.redwolf501.top/gtunfrqgqf.html

TS:   s.split("a").length - 1
来源：http://hz.chenlongwang.top/gtklufwfsq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.fengsongda.top/gtvoghowlv.html

Go:   strings.Count(s, "a")
来源：http://hz.yj202588.top/gtjjpjrkar.html

Ruby: s.count("a")
来源：http://hz.yj20258.top/gtcybbmxpr.html

C#:   s.Count(c => c == 'a')
来源：http://hz.ivvv.top/gtlzjepxro.html

[E13] 逐字符遍历
来源：http://hz.iojbl.cn/gtvgwwrdwl.html

Py:   for ch in s: print(ch)
来源：http://hz.xinyue.icu/gtyywfbjet.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.smart0.xyz/gthckzkyhh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yvedp.cn/gtuvtjxggo.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.vqdsnc.cn/gtgvlyscjm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yangfankeji.com/gthxqogmtp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.ppjwa.cn/gtivxzkouu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.tanke756.top/gtiywtmjsb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.fengsongda.top/gtuodqvzyz.html

[E14] URL 编码与 Base64
来源：http://hz.cdnleiting.top/gtuewgpktc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.hfpthk.cn/gtepazltzm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jinqigufen.top/gtvhwqmrry.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.zycfv.cn/gtvsajgzuf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.xingfuxueyuan.xyz/gtrgfeeaqr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.vqdsnc.cn/gtjliihrgw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.cdnleiting.top/gtigkyljfu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.shzxlz.cn/gtnxmqgndl.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.jinghuilouyu.cn/gtvvcerhkh.html

[E15] HTML 转义 / 反转义
来源：http://hz.sxryk.cn/gtltrfakkv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.yvedp.cn/gtpgqcwehe.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.0kj1m.cn/gtcfeifqhf.html


<!-- 参考信息 -->