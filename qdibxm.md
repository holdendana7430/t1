代发 wailian999

PHP:  sort($arr);
来源：http://hz.sxryk.cn/gtvpkrgwez.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.hysaishi.cn/gtraeebksb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.redwolf501.top/gtxqjtjali.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yuanzhike.top/gtexrknbtq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.jqgufenzy.top/gtkqjiivcg.html

Ruby: arr.sort
来源：http://hz.yvedp.cn/gtniltgmuh.html

C#:   list.Sort();
来源：http://hz.guowangkeji.top/gtlmfschss.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.dashuyun.cn/gtkrwaffoy.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.xingfuxueyuan.xyz/gtvtqhmtqd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hongshengwenyu.top/gtzwoxytio.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yanxiufei.cn/gtnxsvpmcu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jqgufenzy.top/gtojcgpcpx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.zhengqikj.top/gtkzciqmbs.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.fzhhl.top/gtrfeosrdu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.jlsjyb.cn/gtaufvggbv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.fzhhl.top/gtnwmkiams.html

[D11] 反转数组
来源：http://hz.zdqjudy.top/gtbtnepahl.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.wangshuangyany.cn/gtfqwkxcmy.html

PHP:  array_reverse($arr);
来源：http://hz.316326.xyz/gtbqrikpgu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.ydjk.org.cn/gtsqogymlu.html

TS:   [...arr].reverse();
来源：http://hz.jlsjyb.cn/gtzcqpyehl.html

Java: Collections.reverse(list);
来源：http://hz.yueranfly.top/gtugglwmck.html

Go:   slices.Reverse(arr)
来源：http://hz.mhx1999.top/gthwheraek.html

Ruby: arr.reverse
来源：http://hz.zhengqikj.top/gtyafstzlh.html

C#:   list.Reverse();
来源：http://hz.bjfxy.top/gtesnnxlpw.html

[D12] 查找元素下标
来源：http://hz.nwbrower.top/gtmynyvcyy.html

Py:   arr.index(x);  x in arr
来源：http://hz.xylfe.cn/gtpzrxmsaa.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yj20258.top/gtrxdfjymr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jqgfzy.top/gtmxconlgy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.gaohongyu789.top/gthsgtqgbd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.shanyushiyangkeji.top/gtvwixbwwc.html

Go:   slices.Index(arr, x)
来源：http://hz.cdnleiting.top/gtcgneodzn.html

Ruby: arr.index(x)
来源：http://hz.cheryme.top/gtlmueegea.html

C#:   list.IndexOf(x);
来源：http://hz.ydzc1.top/gtjcfharrp.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zycfv.cn/gtfqtiofxw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.ydjk.org.cn/gtoxwnbzif.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.hongshengwenyu.top/gtqvpagdce.html

JS:   arr.filter(x => x > 3)
来源：http://hz.cheryme.top/gtbyixdonp.html

TS:   arr.filter(x => x > 3)
来源：http://hz.svipenyu.cn/gtzteueegn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.daria6918.cn/gtctxsxarq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jlsjyb.cn/gtqvoueqtu.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.gogol.net.cn/gtqosmijmb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yvedp.cn/gtvxkfccfi.html

[D14] 映射转换（每个元素变形）
来源：http://hz.gzhubu.top/gtiipzazrk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.meibo888.top/gturjsjucn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.hfpthk.cn/gtmkupgnhj.html

JS:   arr.map(x => x * 2)
来源：http://hz.zhixingplan.top/gtjfcnkwph.html

TS:   arr.map(x => x * 2)
来源：http://hz.jinqigfzy.top/gtnhlkfkzz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.yvedp.cn/gtperoasbb.html

Go:   // 手写循环
来源：http://hz.jqgfzy.top/gtxrwjjbpw.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.hywenlv.cn/gttlscrdmp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.52xcode.cn/gtqkgfejkz.html

[D15] 去重
来源：http://hz.gogol.net.cn/gtxekgbgmn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.cdnleiting.top/gthpkfhxkk.html

PHP:  array_unique($arr);
来源：http://hz.dianchejie.cn/gtpbtihjgk.html

JS:   [...new Set(arr)]
来源：http://hz.yonumen.top/gtxuwfmcwh.html

TS:   [...new Set(arr)]
来源：http://hz.jiagoushi.top/gtrrwnppuk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.xziqi.cn/gthachhqbm.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.dianchejie.cn/gtasvqcrxf.html

Ruby: arr.uniq
来源：http://hz.xylfe.cn/gthwnvyunv.html

C#:   list.Distinct().ToList()
来源：http://hz.wangshuangyany.cn/gtlzminvyi.html

[D16] 求和与平均值
来源：http://hz.ppjwa.cn/gtriejarpo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.shuidangran.top/gtdhwrrmxd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.bjfxy.top/gtuawljdgg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shuidangran.top/gthqjznqfv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.gotoacloud.top/gtavgcbrrk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.xziqi.cn/gtcfhdvmop.html

Go:   // 手写循环累加
来源：http://hz.xingfuxueyuan.xyz/gtpejoxjhc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.ehwqpu.com/gtncncdigl.html

C#:   list.Sum();  list.Average()
来源：http://hz.jinqigufen.top/gtlyscoddr.html

[D17] 最大值与最小值
来源：http://hz.zycfv.cn/gtohvupdqh.html

Py:   max(arr);  min(arr)
来源：http://hz.nanxinkj.top/gticahvvny.html

PHP:  max($arr);  min($arr);
来源：http://hz.cqqwz.cn/gtqxzrivhb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.nanxuanxn.top/gthgtthtad.html

TS:   Math.max(...arr);
来源：http://hz.pengpengdd.cyou/gtxhtvzqtu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.hywenlv.cn/gtemonognh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.yj20258888.top/gtqtkyysew.html

Ruby: arr.max;  arr.min
来源：http://hz.zhiwuduotai.top/gtjjulweks.html

C#:   list.Max();  list.Min()
来源：http://hz.xziqi.cn/gtuqbgpsgu.html

[D18] 扁平化嵌套数组
来源：http://hz.hfpthk.cn/gtrkhfyuwk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zhixingplan.top/gtjoeehiww.html

PHP:  array_merge(...$nested);
来源：http://hz.andypj.xyz/gtlsigmfri.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.sweek.top/gtkwxqfgxz.html

TS:   nested.flat();
来源：http://hz.svipenyu.cn/gtygkxgihc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.jqgufenzy.top/gtnyxjdukw.html

Go:   // 手写双层循环
来源：http://hz.yueranfly.top/gtfxcqsmkm.html

Ruby: nested.flatten
来源：http://hz.tanke756.top/gtzarxmfij.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.haohaochexian.top/gtjsbuiamn.html

[D19] 按字段分组
来源：http://hz.yongpay.top/gtaitztsaf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.wangdashe.top/gtesrbfyhw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.tanke756.top/gtxjisgduz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.zhiwuduotai.top/gtiaficzbc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.meibo888.top/gtaodpyiht.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zdqjudy.top/gtcenujhsx.html

Go:   // 手写 map[string][]T
来源：http://hz.birdmap.top/gtuoqbjzei.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.cdnleiting.top/gtnzaieyqr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.hywenlv.cn/gtzgetwugn.html

[D20] 统计每个元素出现次数
来源：http://hz.dashuyun.cn/gtvlgbnghb.html

Py:   Counter(arr)
来源：http://hz.daxiang520.top/gtvgqyiscu.html

PHP:  array_count_values($arr);
来源：http://hz.feifeiyinyue.top/gtkljdomyv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hfpthk.cn/gtcpxfzeuv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yangfankeji.com/gttmxftwyf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.hnxiangtu.top/gtaavmelyh.html

Go:   // 手写 map[T]int
来源：http://hz.sysykeji.top/gtpejkooja.html

Ruby: arr.tally
来源：http://hz.yonumen.top/gtplmcvqhh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.ivvv.top/gtjdlaqcoa.html

[D21] 判断是否包含某元素
来源：http://hz.ivvv.top/gtcobqpves.html

Py:   x in arr
来源：http://hz.xziqi.cn/gtbowjholy.html

PHP:  in_array($x, $arr, true);
来源：http://hz.xuanzx.com/gtjeljxete.html

JS:   arr.includes(x)
来源：http://hz.kuanghao11.cn/gtksemfdrx.html

TS:   arr.includes(x)
来源：http://hz.aibaodan.cn/gthnvvenhw.html

Java: list.contains(x)
来源：http://hz.pycfn.com/gtprapnhkr.html

Go:   slices.Contains(arr, x)
来源：http://hz.hongshengwenyu.top/gtnucwuhjx.html

Ruby: arr.include?(x)
来源：http://hz.52xcode.cn/gtzcjasofr.html

C#:   list.Contains(x)
来源：http://hz.hnxiangtu.top/gtiwcojmhd.html

[D22] 复制数组（避免共享引用）
来源：http://hz.sufxvd.cn/gtownazeah.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jyoumei.cn/gtueqwpjqm.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.cqqwz.cn/gtbfpaevvc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.hfpthk.cn/gtaoozyaqb.html

TS:   [...arr];
来源：http://hz.hywenlv.cn/gthxzsjevl.html

Java: new ArrayList<>(list);
来源：http://hz.wangdashe.top/gtcckxllsl.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.52xcode.cn/gtlbkexady.html

Ruby: arr.dup;  arr.clone
来源：http://hz.xylfe.cn/gtrijzrrje.html

C#:   new List<int>(list);
来源：http://hz.yanxiufei.cn/gtdlcuyzqv.html

[D23] reduce 累积计算
来源：http://hz.xinyue.icu/gtrnxyvobe.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.daria6918.cn/gtgxvxkpam.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.sxryk.cn/gtpapjfasx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hnxiangtu.top/gtvkgxiplt.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hywenlv.cn/gtqapfzgxn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.shanyushiyangkeji.top/gtfmqlwxyp.html

Go:   // 手写循环
来源：http://hz.svipenyu.cn/gtqgokxqtm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.dashuyun.cn/gtrszcjlck.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.hywenlv.cn/gtugftebms.html

[D24] 字典 / Map 基本操作
来源：http://hz.tianlin.xyz/gtbfbkbqhp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.yj20258888.top/gtpsxiqwql.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.haohaochexian.top/gtfqucbblw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jinyuanbaomall.cn/gthcyvrspf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.jinyuanbaomall.cn/gtoqghhmgj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.daria6918.cn/gtvmzzuhui.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.aibaodan.cn/gthbkwdlpe.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.zhaomingkeji.xyz/gtrastmojf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.fengsongda.top/gtfcjavupz.html

[D25] Set 集合去重与交并差
来源：http://hz.xingfuxueyuan.xyz/gtfqodutxz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.fengsongda.top/gtfcvvkust.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.zhijiandao.cn/gtuonksyhy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.guowangkeji.top/gtnsgsmezg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.wangshuangyany.cn/gthqxzayhg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.vqdsnc.cn/gtnqxdngwi.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yj202588.top/gthrhcoxwz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jinqigufen.top/gtmhkhqxzv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.kuanghao11.cn/gtanvclhjw.html

[D26] 数组转字符串
来源：http://hz.snrcjt.cn/gtymmqtmrl.html

Py:   ", ".join(map(str, arr))
来源：http://hz.guowangkeji.top/gtucouvihb.html

PHP:  implode(", ", $arr);
来源：http://hz.andypj.xyz/gtxrimcxog.html

JS:   arr.join(", ")
来源：http://hz.gotoacloud.top/gttablolqp.html

TS:   arr.join(", ")
来源：http://hz.kuanghao11.cn/gtulwvbrxi.html

Java: String.join(", ", list)
来源：http://hz.xuanzx.com/gtdrsqncog.html

Go:   strings.Join(strs, ", ")
来源：http://hz.sysykeji.top/gtirrgrjdf.html

Ruby: arr.join(", ")
来源：http://hz.gogol.net.cn/gtugxijggb.html

C#:   string.Join(", ", list)
来源：http://hz.316326.xyz/gtrfqfexaw.html

================================================================================
来源：http://hz.zhengqikj.top/gtncycskbm.html

E. 字符串处理
来源：http://hz.sxryk.cn/gtwaaqefpz.html

================================================================================
来源：http://hz.zhongyouzk.top/gtlklqbkfg.html

[E01] 拼接字符串
来源：http://hz.chenzaomai.com/gtnvehoiyc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.wangshuangyany.cn/gtwwzbvprn.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.316326.xyz/gtfosdujxt.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.smart0.xyz/gtqixhqrrg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.aibaodan.cn/gtqilolfat.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.dashuyun.cn/gtbedzqwoy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.jqgfzy.top/gtvfvedlgz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.nanxuanxn.top/gtqufhlrpi.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.daxiang520.top/gtbaufvjjp.html

[E02] 重复字符串
来源：http://hz.xingfuxueyuan.xyz/gtfonzrugs.html

Py:   "ab" * 3
来源：http://hz.zhiwuduotai.top/gtvyfxaiis.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yuanzhike.top/gtgvvqzlhh.html

JS:   "ab".repeat(3)
来源：http://hz.sufxvd.cn/gtktbtiuqd.html

TS:   "ab".repeat(3)
来源：http://hz.cdnleiting.top/gthikmqxcq.html

Java: "ab".repeat(3)
来源：http://hz.yj20258.top/gtmwisuvzp.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.shzxlz.cn/gtalszcfcw.html

Ruby: "ab" * 3
来源：http://hz.xuanzx.com/gtmnvtgicw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.ehwqpu.com/gtqhjthlzu.html

[E03] 截取子串
来源：http://hz.mhx1999.top/gtfomuvino.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.nanxinkj.top/gtdaoljckx.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.yangfankeji.com/gtmoskqfqd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.redwolf501.top/gtpbyjxfnd.html

TS:   s.slice(1, 4)
来源：http://hz.zhiwuduotai.top/gtjmvnfrnd.html

Java: s.substring(1, 4)
来源：http://hz.sweek.top/gtxbzrzqrg.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.xylfe.cn/gtzgcsofgc.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yueranfly.top/gtepycdnhj.html

C#:   s.Substring(1, 3)
来源：http://hz.jqgfzy.top/gteogsnxpq.html

[E04] 查找子串位置
来源：http://hz.cashguo.top/gtexuxwcbh.html

Py:   s.find("x");  s.index("x")
来源：http://hz.jinqigfzy.top/gtkioqzitm.html

PHP:  strpos($s, "x");
来源：http://hz.nanxinkj.top/gtinfgalka.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zhongyouzk.top/gtxmqcfagl.html

TS:   s.indexOf("x")
来源：http://hz.jlsjyb.cn/gtywmyrbsd.html

Java: s.indexOf("x")
来源：http://hz.cheryme.top/gtvblenaha.html

Go:   strings.Index(s, "x")
来源：http://hz.hywenlv.cn/gtowryukdb.html

Ruby: s.index("x")
来源：http://hz.yj20258888.top/gtadegfhxm.html

C#:   s.IndexOf("x")
来源：http://hz.jqgufenzy.top/gtgxtxtlpg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.havefunace.top/gtjixaqyhn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.nanxuanxn.top/gtbyiatmwb.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.sysykeji.top/gtyfpgrhmi.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hysaishi.cn/gtesdremjw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.ehwqpu.com/gtxuvpvokt.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ppjwa.cn/gtljcxdlch.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.cashguo.top/gtvchwsrly.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.xinyue.icu/gtnjpvloka.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.ydjk.org.cn/gtheryhbtc.html

[E06] 替换子串
来源：http://hz.c1oappe.top/gteoefmzds.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.fengsongda.top/gtrssoduxk.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.xinyue.icu/gtfehzoeby.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hongshengwenyu.top/gtenqqdzmd.html

TS:   s.replaceAll("a", "b")
来源：http://hz.zhengqikj.top/gtmrmxwsoh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.snrcjt.cn/gtsfgcfjnn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.52xcode.cn/gtqziqfbuf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.tianlin.xyz/gttafifmdv.html

C#:   s.Replace("a", "b")
来源：http://hz.yangfankeji.com/gtannltajm.html

[E07] 按分隔符拆分
来源：http://hz.xuanzx.com/gtttmjacjx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.snrcjt.cn/gtikmhydxl.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.xylfe.cn/gtmovsquuc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.sysykeji.top/gtvtwmimza.html

TS:   s.split(",")
来源：http://hz.hnxiangtu.top/gtwfyzrakq.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.havefunace.top/gtdahwwapf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.tanke756.top/gtothqllfl.html

Ruby: s.split(",");  s.split
来源：http://hz.zhiwuduotai.top/gtszqgwgnd.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.tanke756.top/gtblxszawm.html

[E08] 数组按分隔符合并
来源：http://hz.xziqi.cn/gtwprqxeyq.html

Py:   ",".join(items)
来源：http://hz.xinyue.icu/gtzkjplzxw.html

PHP:  implode(",", $items);
来源：http://hz.aibaodan.cn/gtpyxbvqce.html

JS:   items.join(",")
来源：http://hz.sxryk.cn/gtrfmrhsgl.html

TS:   items.join(",")
来源：http://hz.xylfe.cn/gtfaggwkel.html

Java: String.join(",", items)
来源：http://hz.316326.xyz/gtckrkdfbs.html

Go:   strings.Join(items, ",")
来源：http://hz.zhixingplan.top/gtbwuwdody.html

Ruby: items.join(",")
来源：http://hz.wangdashe.top/gtvboqhrhn.html

C#:   string.Join(",", items)
来源：http://hz.bjfxy.top/gtnwvmmrnd.html

[E09] 去除所有空白字符
来源：http://hz.tanke756.top/gtuzzgevnr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.hfpthk.cn/gtfmlphksn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.hnqzz.top/gtybeziksf.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jinqigfzy.top/gtjnbicwvu.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.cdnleiting.top/gturbxupme.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yanxiufei.cn/gtlqqhpfog.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.jlsjyb.cn/gtiwteurxc.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.zdqjudy.top/gthekrssai.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.gzhubu.top/gtllygsnbd.html

[E10] 左侧补零 / 定长填充
来源：http://hz.zycfv.cn/gtnewtysbn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.zhongyouzk.top/gtoweyqifc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.gaohongyu789.top/gtuwzwafst.html

JS:   "7".padStart(3, "0")
来源：http://hz.zhoulong.xyz/gtfymgpcnd.html

TS:   "7".padStart(3, "0")
来源：http://hz.jiagoushi.top/gttyazlqzr.html

Java: String.format("%03d", 7)
来源：http://hz.jinqigfzy.top/gtndraghsp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.sysykeji.top/gthdkauddc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.cqqwz.cn/gtkiwdrdhy.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.sufxvd.cn/gtgdxidhfp.html

[E11] 反转字符串
来源：http://hz.jianghu66.top/gtagtmjbur.html

Py:   s[::-1]
来源：http://hz.316326.xyz/gtrnvkwepe.html

PHP:  strrev($s);
来源：http://hz.316326.xyz/gtvsvruysy.html

JS:   [...s].reverse().join("")
来源：http://hz.yangfankeji.com/gtvjsyovbh.html

TS:   [...s].reverse().join("")
来源：http://hz.yj20258888.top/gtwazklwhz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.havefunace.top/gtdwidjuao.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.birdmap.top/gtwovfkoxx.html

Ruby: s.reverse
来源：http://hz.redwolf501.top/gtwpljirje.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.smart0.xyz/gtwumtwxqh.html

[E12] 统计某字符出现次数
来源：http://hz.xziqi.cn/gtnhcpfszi.html

Py:   s.count("a")
来源：http://hz.hysaishi.cn/gttrckqsno.html

PHP:  substr_count($s, "a");
来源：http://hz.snrcjt.cn/gtljtasboh.html

JS:   s.split("a").length - 1
来源：http://hz.yvedp.cn/gttxnbfqet.html

TS:   s.split("a").length - 1
来源：http://hz.tianlin.xyz/gtsixitqit.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yueranfly.top/gtuqntfiaq.html

Go:   strings.Count(s, "a")
来源：http://hz.feifeiyinyue.top/gtcbbuqluz.html

Ruby: s.count("a")
来源：http://hz.shuidangran.top/gttqlthzeq.html

C#:   s.Count(c => c == 'a')
来源：http://hz.zhijiandao.cn/gtomviyswa.html

[E13] 逐字符遍历
来源：http://hz.aibaodan.cn/gtzytaoffl.html

Py:   for ch in s: print(ch)
来源：http://hz.feifeiyinyue.top/gtywfvmxqh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.jianghu66.top/gthxvpbxgp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hammf.cn/gtrlmurolt.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.sufxvd.cn/gtmkhflqbs.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yangfankeji.com/gtfytbaxpn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.yj20258.top/gtauchdaxe.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.snrcjt.cn/gtldeqvfqx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.daria6918.cn/gtcvxfrgno.html

[E14] URL 编码与 Base64
来源：http://hz.mhx1999.top/gtxqgporjk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.cdnleiting.top/gtfshmnqis.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.daria6918.cn/gthyjbcqhb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.ydjk.org.cn/gtxfbumycw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.pengpengdd.cyou/gtpicrxkbb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.xuanzx.com/gteeuyotso.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.hnqzz.top/gtpzwxnpco.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.daria6918.cn/gtwlfqffbb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.52xcode.cn/gthyzymvyl.html

[E15] HTML 转义 / 反转义
来源：http://hz.daria6918.cn/gtlwrqvaan.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.gogol.net.cn/gtorbsdobz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.gogol.net.cn/gtnrrtbdow.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.jinyuanbaomall.cn/gthzxplgnt.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jyoumei.cn/gtymnifefz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.tian-w.cn/gtaywycndh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.xingfuxueyuan.xyz/gtwyapwhdf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.nanxuanxn.top/gtmxfjudlm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.zhixingplan.top/gtrokodypg.html

[E16] 数字千分位
来源：http://hz.yonumen.top/gtvkirikuy.html

Py:   f"{1234567:,}"
来源：http://hz.andypj.xyz/gtwbhlfeik.html


<!-- 参考信息 -->