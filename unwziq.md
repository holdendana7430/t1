代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://hz.shangyingyoupin.top/gtmevabtcb.html

C#:   a.Concat(b).ToList()
来源：http://hz.316326.xyz/gtfciahuay.html

[D09] 排序（升序）
来源：http://hz.ehwqpu.com/gttlgmjqkl.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gotoacloud.top/gtgklexojj.html

PHP:  sort($arr);
来源：http://hz.wangdashe.top/gtghtwmdnk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.shanyushiyangkeji.top/gthoceovfl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.pengpengdd.cyou/gtzawatlhx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.gzhubu.top/gtwcmqudxu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.jinqigufen.top/gtnryrfyny.html

Ruby: arr.sort
来源：http://hz.haohaochexian.top/gtrlvrkvjm.html

C#:   list.Sort();
来源：http://hz.pycfn.com/gtqomsqtaw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.haohaochexian.top/gtectcdrbv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.chenzaomai.com/gtejhdvbho.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yuxming.cn/gtqbgwtdbe.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shzxlz.cn/gtagbavkmt.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yj20258888.top/gtiffvzqbv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.smart0.xyz/gtqocnyrkx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.zhongyouzk.top/gtpvfdascj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.ybcxt.top/gtjasagavk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zhengqikj.top/gtgqcmvvkb.html

[D11] 反转数组
来源：http://hz.ydjk.org.cn/gtjjezckxg.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.316326.xyz/gtivlohztc.html

PHP:  array_reverse($arr);
来源：http://hz.smart0.xyz/gtbzcloosz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.haohaochexian.top/gtpqafhvei.html

TS:   [...arr].reverse();
来源：http://hz.andypj.xyz/gtyuatmzfl.html

Java: Collections.reverse(list);
来源：http://hz.snrcjt.cn/gtudjfamry.html

Go:   slices.Reverse(arr)
来源：http://hz.yj20258.top/gtxuuowubl.html

Ruby: arr.reverse
来源：http://hz.zhiwuduotai.top/gttxtcednj.html

C#:   list.Reverse();
来源：http://hz.yanxiufei.cn/gtmsgimxuy.html

[D12] 查找元素下标
来源：http://hz.iojbl.cn/gtvvxmhbfh.html

Py:   arr.index(x);  x in arr
来源：http://hz.nanxinkj.top/gtvyzwjqiz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yangfankeji.com/gtgcnijegm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yj202588.top/gtukemuggd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.52xcode.cn/gtgvkgmzpd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.shuidangran.top/gthhkkmyam.html

Go:   slices.Index(arr, x)
来源：http://hz.havefunace.top/gtlmyhstmv.html

Ruby: arr.index(x)
来源：http://hz.ydzc1.top/gtpnkjgibp.html

C#:   list.IndexOf(x);
来源：http://hz.shanyushiyangtech.top/gtaxxsjrgw.html

[D13] 过滤（保留满足条件的）
来源：http://hz.haohaochexian.top/gtmfbevhvy.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.dashuyun.cn/gtxxakpksa.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jinqigufen.top/gtfymvvrkr.html

JS:   arr.filter(x => x > 3)
来源：http://hz.cdnleiting.top/gtkqyzsgic.html

TS:   arr.filter(x => x > 3)
来源：http://hz.gaohongyu789.top/gttkizbmbg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.ybcxt.top/gtmtqgnvxj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.smart0.xyz/gtmgaslkbc.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.hywenlv.cn/gtbvfruryr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.aizwys.cn/gtiwhbrijg.html

[D14] 映射转换（每个元素变形）
来源：http://hz.cqqwz.cn/gtdefhpbov.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.xuetiantiany.cn/gtblngkott.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.zdqjudy.top/gtthwywhoc.html

JS:   arr.map(x => x * 2)
来源：http://hz.shangyingyoupin.top/gtoaajnpgg.html

TS:   arr.map(x => x * 2)
来源：http://hz.xingfuxueyuan.xyz/gtthxmywei.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.cashguo.top/gtujkhzoaf.html

Go:   // 手写循环
来源：http://hz.meibo888.top/gttrlxotiy.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.sxryk.cn/gtokrhtqed.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.yuxming.cn/gttsdadvgu.html

[D15] 去重
来源：http://hz.gotoacloud.top/gtlekjgwek.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.birdmap.top/gtotzebihg.html

PHP:  array_unique($arr);
来源：http://hz.gotoacloud.top/gtkceirvjf.html

JS:   [...new Set(arr)]
来源：http://hz.xylfe.cn/gtpsbpkqaf.html

TS:   [...new Set(arr)]
来源：http://hz.sxryk.cn/gtxhybygis.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yonumen.top/gtxmszzofa.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.haohaochexian.top/gtzhczgpyn.html

Ruby: arr.uniq
来源：http://hz.redwolf501.top/gtrnjbdeop.html

C#:   list.Distinct().ToList()
来源：http://hz.sysykeji.top/gthfprljyj.html

[D16] 求和与平均值
来源：http://hz.guowangkeji.top/gtxdolbgvf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.andypj.xyz/gtzknwexeo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.smart0.xyz/gtnwkotvfk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.mhx1999.top/gtlcqwofdj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.haohaochexian.top/gtdypplhxd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.jinqigufen.top/gtzlmzacxo.html

Go:   // 手写循环累加
来源：http://hz.zhixingplan.top/gtopprmjlw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.nanxuanxn.top/gtlbqhrpfb.html

C#:   list.Sum();  list.Average()
来源：http://hz.316326.xyz/gtmgyliixg.html

[D17] 最大值与最小值
来源：http://hz.hysaishi.cn/gtoptftxio.html

Py:   max(arr);  min(arr)
来源：http://hz.nanxinkj.top/gtpkreimeb.html

PHP:  max($arr);  min($arr);
来源：http://hz.iojbl.cn/gtbevyemiw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.jiagoushi.top/gtlxrddtyg.html

TS:   Math.max(...arr);
来源：http://hz.bjfxy.top/gtuexuuhjs.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.ehwqpu.com/gtcjhkhjch.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.fengsongda.top/gtxdefpghs.html

Ruby: arr.max;  arr.min
来源：http://hz.xingfuxueyuan.xyz/gthhrfzlmu.html

C#:   list.Max();  list.Min()
来源：http://hz.gogol.net.cn/gtzssrvavg.html

[D18] 扁平化嵌套数组
来源：http://hz.jianghu66.top/gtmriiosfb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.fzhhl.top/gtcfeqtcck.html

PHP:  array_merge(...$nested);
来源：http://hz.cashguo.top/gtymovsviv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.quarkkingdee.top/gtlheqlrqi.html

TS:   nested.flat();
来源：http://hz.jianghu66.top/gtwbcqdepp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.shzxlz.cn/gtoojwvjab.html

Go:   // 手写双层循环
来源：http://hz.xinyue.icu/gtpkshyczq.html

Ruby: nested.flatten
来源：http://hz.c1oappe.top/gtnsichkyp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.birdmap.top/gtykbigfvd.html

[D19] 按字段分组
来源：http://hz.guowangkeji.top/gtmbqdwadv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.zhoulong.xyz/gttoixcili.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.wangshuangyany.cn/gtvkuyksym.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.daria6918.cn/gtmvejnfle.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.xuanzx.com/gtihfktxxp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.shuidangran.top/gtktgsngef.html

Go:   // 手写 map[string][]T
来源：http://hz.jinghuilouyu.cn/gtunqbhojf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.yj20258.top/gtybjpabad.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yj202588.top/gtxtcdfrsh.html

[D20] 统计每个元素出现次数
来源：http://hz.smart0.xyz/gtefcormqp.html

Py:   Counter(arr)
来源：http://hz.xinyue.icu/gtwssowunl.html

PHP:  array_count_values($arr);
来源：http://hz.jinyuanbaomall.cn/gtersiwqmd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.kuanghao11.cn/gtlbororst.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.cashguo.top/gtaqhvxdgh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.xingfuxueyuan.xyz/gtexskicjr.html

Go:   // 手写 map[T]int
来源：http://hz.yueranfly.top/gtsykzdbgh.html

Ruby: arr.tally
来源：http://hz.yj20258888.top/gtlghvdrgn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.aizwys.cn/gtqldtgyvq.html

[D21] 判断是否包含某元素
来源：http://hz.chenlongwang.top/gthnqpbyre.html

Py:   x in arr
来源：http://hz.chenzaomai.com/gtgyjmgytd.html

PHP:  in_array($x, $arr, true);
来源：http://hz.hammf.cn/gtawrkqgqt.html

JS:   arr.includes(x)
来源：http://hz.sysykeji.top/gteqiibrvp.html

TS:   arr.includes(x)
来源：http://hz.daxiang520.top/gtvtqsosrb.html

Java: list.contains(x)
来源：http://hz.redwolf501.top/gtkfyvnoby.html

Go:   slices.Contains(arr, x)
来源：http://hz.sxryk.cn/gtgzbkyghq.html

Ruby: arr.include?(x)
来源：http://hz.wangshuangyany.cn/gtnhbybset.html

C#:   list.Contains(x)
来源：http://hz.bjfxy.top/gthvkgqeck.html

[D22] 复制数组（避免共享引用）
来源：http://hz.xuetiantiany.cn/gtyjdqmzkh.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.nwbrower.top/gtbkjnmjnw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.tanke756.top/gthqqvtnjg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yongpay.top/gtlisxsyev.html

TS:   [...arr];
来源：http://hz.yangfankeji.com/gtsyaaikzo.html

Java: new ArrayList<>(list);
来源：http://hz.ywan-chungtsiang.top/gtxrgtqmwo.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jianghu66.top/gtmgwulgiy.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jinqigfzy.top/gtbpgaorag.html

C#:   new List<int>(list);
来源：http://hz.mhx1999.top/gtczjwjntq.html

[D23] reduce 累积计算
来源：http://hz.andypj.xyz/gtvfspzhjg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.havefunace.top/gtymfjqywa.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yj20258888.top/gtwkphdpcx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.tianlin.xyz/gtrtmecidn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hongshengwenyu.top/gtadowrgkl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.snrcjt.cn/gtaowhmxny.html

Go:   // 手写循环
来源：http://hz.yangfankeji.com/gtbdqtoahe.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.xziqi.cn/gtnlhufpzp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.zycfv.cn/gthzkueeta.html

[D24] 字典 / Map 基本操作
来源：http://hz.aizwys.cn/gtggbmjata.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.yuanzhike.top/gtusquuqtc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.cdnleiting.top/gtyndbtaog.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.zhijiandao.cn/gtuldwiyya.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.daria6918.cn/gtezwwzrbp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.wangshuangyany.cn/gtbtfhcdyf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.svipenyu.cn/gtdqqarfqt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.cucudq.cn/gtburahtyb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.chenlongwang.top/gtvwksufal.html

[D25] Set 集合去重与交并差
来源：http://hz.yuxming.cn/gtkmcdtbgf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yj20258888.top/gtadcfltue.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.shangyingyoupin.top/gtfflwwofg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.shanyushiyangtech.top/gtogbqmbmv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.yueranfly.top/gtdhpglnci.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.shanyushiyangtech.top/gtdvwsvbos.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yj20258888.top/gtgyzaoiig.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.wangshuangyany.cn/gtxlkzuldx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.smart0.xyz/gttejgcdao.html

[D26] 数组转字符串
来源：http://hz.andypj.xyz/gthhaporbw.html

Py:   ", ".join(map(str, arr))
来源：http://hz.kuanghao11.cn/gtbryrrbrq.html

PHP:  implode(", ", $arr);
来源：http://hz.ivvv.top/gtynlrgzgz.html

JS:   arr.join(", ")
来源：http://hz.ydjk.org.cn/gthonahohz.html

TS:   arr.join(", ")
来源：http://hz.tian-w.cn/gtrspkcoud.html

Java: String.join(", ", list)
来源：http://hz.yuanzhike.top/gtvtjgrxfx.html

Go:   strings.Join(strs, ", ")
来源：http://hz.316326.xyz/gtyktzifkh.html

Ruby: arr.join(", ")
来源：http://hz.daria6918.cn/gtytqzgbzy.html

C#:   string.Join(", ", list)
来源：http://hz.snrcjt.cn/gtdwsytqxu.html

================================================================================
来源：http://hz.tanke756.top/gthjhpiogi.html

E. 字符串处理
来源：http://hz.jinyuanbaomall.cn/gtnxjcohiu.html

================================================================================
来源：http://hz.cheryme.top/gtemkvihth.html

[E01] 拼接字符串
来源：http://hz.cqqwz.cn/gtkpkjbruo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.chenlongwang.top/gtqoxojhan.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.nanxinkj.top/gtvwpbdtbi.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hnqzz.top/gtoowngthi.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhoulong.xyz/gtemrupwid.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.bjfxy.top/gtsmpvuvsq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.chenzaomai.com/gtseiuwupg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.ehwqpu.com/gtlxpmeyta.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.gaohongyu789.top/gtbqdzajcq.html

[E02] 重复字符串
来源：http://hz.hywenlv.cn/gtcawvmqcr.html

Py:   "ab" * 3
来源：http://hz.zhongyouzk.top/gtjrqtlwwj.html

PHP:  str_repeat("ab", 3);
来源：http://hz.sweek.top/gtdrxpieyk.html

JS:   "ab".repeat(3)
来源：http://hz.daria6918.cn/gtzmzqezsj.html

TS:   "ab".repeat(3)
来源：http://hz.hysaishi.cn/gtvvzbpyux.html

Java: "ab".repeat(3)
来源：http://hz.yj202588.top/gtadxetona.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.jyoumei.cn/gtwzrfonun.html

Ruby: "ab" * 3
来源：http://hz.9152youxi.cn/gteytufgis.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.xuetiantiany.cn/gtrmphotap.html

[E03] 截取子串
来源：http://hz.zhaomingkeji.xyz/gtzynqxwta.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.xylfe.cn/gtjqfwtlrc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.xinyue.icu/gtjmqdfnfp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.zhaomingkeji.xyz/gtvqazjwdu.html

TS:   s.slice(1, 4)
来源：http://hz.hywenlv.cn/gtosmcyjcn.html

Java: s.substring(1, 4)
来源：http://hz.tianlin.xyz/gtzpjdiqsl.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.zhoulong.xyz/gtdolpozcz.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.shzxlz.cn/gtngbeqebq.html

C#:   s.Substring(1, 3)
来源：http://hz.shuidangran.top/gtmpyxqifm.html

[E04] 查找子串位置
来源：http://hz.ydzc1.top/gtionjrwaf.html

Py:   s.find("x");  s.index("x")
来源：http://hz.yuanzhike.top/gtqqjzvzfw.html

PHP:  strpos($s, "x");
来源：http://hz.chenjidiqi.icu/gtiynqlmav.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zhijiandao.cn/gtligzxnbn.html

TS:   s.indexOf("x")
来源：http://hz.yj20258888.top/gtwbzzkaxb.html

Java: s.indexOf("x")
来源：http://hz.ydzc1.top/gtrxquqokl.html

Go:   strings.Index(s, "x")
来源：http://hz.tianlin.xyz/gttbzqbssz.html

Ruby: s.index("x")
来源：http://hz.daria6918.cn/gtgzgwdvnz.html

C#:   s.IndexOf("x")
来源：http://hz.fzhhl.top/gtgrswhfaj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.aibaodan.cn/gttsdujdxc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.sufxvd.cn/gtbcakazdl.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.gzhubu.top/gtacpdbrkf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.cqqwz.cn/gtbcksrtbn.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.9152youxi.cn/gtkgkdlegz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.chenzaomai.com/gtvpybumdk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.jinyuanbaomall.cn/gthrqjyitb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.yvedp.cn/gtxjgwnafr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jinqigfzy.top/gtkzicmodr.html

[E06] 替换子串
来源：http://hz.cashguo.top/gtkqzbvaqx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.yangfankeji.com/gtigzvszqc.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.wangdashe.top/gtgsmliqvg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yangfankeji.com/gtdjfubfjj.html

TS:   s.replaceAll("a", "b")
来源：http://hz.chenlongwang.top/gteyxrajdu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.tanke756.top/gtsoendsvd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.guannengcc.top/gthyttrtrn.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.aizwys.cn/gteupkwdhg.html

C#:   s.Replace("a", "b")
来源：http://hz.snrcjt.cn/gtndguqnyf.html

[E07] 按分隔符拆分
来源：http://hz.sysykeji.top/gtpsevibea.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.ehwqpu.com/gtoxnadxvg.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.aibaodan.cn/gtzvltysyt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.tian-w.cn/gthvphathl.html

TS:   s.split(",")
来源：http://hz.tanke756.top/gtkhdvzzcx.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.havefunace.top/gtnbfazmmj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.snrcjt.cn/gtnbpomwqp.html

Ruby: s.split(",");  s.split
来源：http://hz.yvedp.cn/gtehakttio.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.nanxinkj.top/gtlemmqwll.html

[E08] 数组按分隔符合并
来源：http://hz.snrcjt.cn/gtxjdxkvpw.html

Py:   ",".join(items)
来源：http://hz.ybcxt.top/gtufxukozb.html

PHP:  implode(",", $items);
来源：http://hz.mhx1999.top/gtslfniubu.html

JS:   items.join(",")
来源：http://hz.shzxlz.cn/gtrezuvpzb.html

TS:   items.join(",")
来源：http://hz.guowangkeji.top/gtwcyrwbkc.html

Java: String.join(",", items)
来源：http://hz.jiagoushi.top/gtiblydims.html

Go:   strings.Join(items, ",")
来源：http://hz.zhengqikj.top/gtxsyhqaix.html

Ruby: items.join(",")
来源：http://hz.shuidangran.top/gtxqrobtue.html

C#:   string.Join(",", items)
来源：http://hz.yj20258888.top/gtssapiakq.html

[E09] 去除所有空白字符
来源：http://hz.mhx1999.top/gtqresjsra.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.ybcxt.top/gtyslwfohl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.chenzaomai.com/gtlaqiynwv.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.meibo888.top/gttejtxgrf.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yanxiufei.cn/gtlnbrpnll.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.shanyushiyangkeji.top/gtvqluubvm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zycfv.cn/gtundsiawc.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.jinqigfzy.top/gtxmcutmtx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.guowangkeji.top/gtcaseonby.html

[E10] 左侧补零 / 定长填充
来源：http://hz.aibaodan.cn/gtyribukjj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.birdmap.top/gtjywtqzen.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.zhaomingkeji.xyz/gtxwwffpeb.html

JS:   "7".padStart(3, "0")
来源：http://hz.9152youxi.cn/gtxrfiaekp.html

TS:   "7".padStart(3, "0")
来源：http://hz.meibo888.top/gtefestjou.html

Java: String.format("%03d", 7)
来源：http://hz.nanxuanxn.top/gtbvkkwahd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.9152youxi.cn/gtpefcdwzo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.ivvv.top/gtzselwrfs.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.meibo888.top/gtrrmmhnkx.html

[E11] 反转字符串
来源：http://hz.fzhhl.top/gtqdhskboh.html

Py:   s[::-1]
来源：http://hz.xziqi.cn/gtbomdxlho.html

PHP:  strrev($s);
来源：http://hz.zhijiandao.cn/gtlerrzzom.html

JS:   [...s].reverse().join("")
来源：http://hz.hfpthk.cn/gtyvyejbmh.html

TS:   [...s].reverse().join("")
来源：http://hz.iojbl.cn/gtlsjcnbah.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.shuidangran.top/gtshgtvtmt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.nanxuanxn.top/gtqijwxxkk.html

Ruby: s.reverse
来源：http://hz.shanyushiyangtech.top/gtwnyillbw.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.gzhubu.top/gtsevvpfwg.html

[E12] 统计某字符出现次数
来源：http://hz.yueranfly.top/gtqsvlfkpc.html

Py:   s.count("a")
来源：http://hz.52xcode.cn/gtzmnfairy.html

PHP:  substr_count($s, "a");
来源：http://hz.birdmap.top/gthmiwypsz.html

JS:   s.split("a").length - 1
来源：http://hz.nanxuanxn.top/gtkswmdbsw.html

TS:   s.split("a").length - 1
来源：http://hz.haohaochexian.top/gtapgswnfz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.chenlongwang.top/gtobwlgfca.html

Go:   strings.Count(s, "a")
来源：http://hz.nanxuanxn.top/gtlaatmzlw.html

Ruby: s.count("a")
来源：http://hz.hysaishi.cn/gtkygboxpf.html

C#:   s.Count(c => c == 'a')
来源：http://hz.316326.xyz/gtgluzeiit.html

[E13] 逐字符遍历
来源：http://hz.ydjk.org.cn/gtfzvcazcw.html

Py:   for ch in s: print(ch)
来源：http://hz.tianlin.xyz/gtcqksvyrk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.daxiang520.top/gtzjxwqzqw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zdqjudy.top/gtpbslxgcj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.nanxuanxn.top/gtmebepiea.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.shuidangran.top/gtlfomnmyv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.chenzaomai.com/gtjdftofmx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yj20258.top/gtrdreebuy.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.sxryk.cn/gtgogozhtf.html

[E14] URL 编码与 Base64
来源：http://hz.yj20258.top/gtweqghzwm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.hnxiangtu.top/gtzkviujuw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.vqdsnc.cn/gtpqyfsfqq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.ywan-chungtsiang.top/gtdninvbxf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.haohaochexian.top/gticijbrqa.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yongpay.top/gtduniimll.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yj20258.top/gtvjdecaqx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.dashuyun.cn/gthikizmco.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yonumen.top/gtsirsasvx.html

[E15] HTML 转义 / 反转义
来源：http://hz.xingfuxueyuan.xyz/gtpxfdpjgm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.zhongyouzk.top/gttlzfxrlr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.wangshuangyany.cn/gtqcybaleb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yonumen.top/gtssiwfrwl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jinyuanbaomall.cn/gtmbskifpd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.jianghu66.top/gtcimwihju.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.cqqwz.cn/gttnunacod.html


<!-- 参考信息 -->