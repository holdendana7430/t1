代发 wailian999

PHP:  sort($arr);
来源：http://hz.zhixingplan.top/gtyckhyqyd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yj202588.top/gtahekmtly.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.xingfuxueyuan.xyz/gtarfihivz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.jlsjyb.cn/gtbyskghdn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.kuanghao11.cn/gtpazijigo.html

Ruby: arr.sort
来源：http://hz.52xcode.cn/gtqwiwrgpx.html

C#:   list.Sort();
来源：http://hz.birdmap.top/gtwctwftnj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.nanxinkj.top/gtawvtcdht.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.hongshengwenyu.top/gtozxhkfkl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.sysykeji.top/gtixekgjcf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.meibo888.top/gtobcrlgea.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xziqi.cn/gttpmbnblh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.bjfxy.top/gtrbtzseyi.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yuanzhike.top/gtoxhprogv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.jyoumei.cn/gtfjdqosbb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.snrcjt.cn/gtwafdrwqv.html

[D11] 反转数组
来源：http://hz.yvedp.cn/gtnpkbjsgn.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.tian-w.cn/gtflrqamdb.html

PHP:  array_reverse($arr);
来源：http://hz.wangdashe.top/gtppqfqzak.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.xuanzx.com/gthjdrhizq.html

TS:   [...arr].reverse();
来源：http://hz.jinqigufen.top/gtcuxzgcin.html

Java: Collections.reverse(list);
来源：http://hz.cdnleiting.top/gtthzhfjsj.html

Go:   slices.Reverse(arr)
来源：http://hz.jqgfzy.top/gtsvwragym.html

Ruby: arr.reverse
来源：http://hz.gogol.net.cn/gtacsqzdin.html

C#:   list.Reverse();
来源：http://hz.316326.xyz/gtwssexmln.html

[D12] 查找元素下标
来源：http://hz.jinqigfzy.top/gthwyjngmr.html

Py:   arr.index(x);  x in arr
来源：http://hz.hysaishi.cn/gtfpefjddp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.dianchejie.cn/gtikwajajl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yueranfly.top/gtcxbkjlzd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.xinyue.icu/gtqtqzsgno.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.xuetiantiany.cn/gtyctigxhq.html

Go:   slices.Index(arr, x)
来源：http://hz.yanxiufei.cn/gtbzqicnde.html

Ruby: arr.index(x)
来源：http://hz.cdnleiting.top/gtmaajiogb.html

C#:   list.IndexOf(x);
来源：http://hz.daria6918.cn/gtnafuizkj.html

[D13] 过滤（保留满足条件的）
来源：http://hz.meibo888.top/gtvrctstel.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.zdqjudy.top/gteeyqdckz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.guowangkeji.top/gteqmmulhp.html

JS:   arr.filter(x => x > 3)
来源：http://hz.fengsongda.top/gtwlekcogv.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jqgufenzy.top/gtxhllohuy.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.feifeiyinyue.top/gtuyyramyy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.feifeiyinyue.top/gteemtwlgj.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.cdnleiting.top/gtmtbwccit.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.aizwys.cn/gthdtpbznn.html

[D14] 映射转换（每个元素变形）
来源：http://hz.feifeiyinyue.top/gtvakrepgw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.sysykeji.top/gtpwuvfhtx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.xuetiantiany.cn/gtxpudgiwh.html

JS:   arr.map(x => x * 2)
来源：http://hz.svipenyu.cn/gtzdjodzer.html

TS:   arr.map(x => x * 2)
来源：http://hz.yangfankeji.com/gtxzzbsvem.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.hywenlv.cn/gtqbuuqxfm.html

Go:   // 手写循环
来源：http://hz.ydjk.org.cn/gtlmqphoil.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.cashguo.top/gtoxtfmuza.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.chenjidiqi.icu/gtojeouoeb.html

[D15] 去重
来源：http://hz.gotoacloud.top/gtxduxlsgu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.havefunace.top/gtonzdjisv.html

PHP:  array_unique($arr);
来源：http://hz.jqgfzy.top/gtrigiovpf.html

JS:   [...new Set(arr)]
来源：http://hz.zhoulong.xyz/gtlzbrynix.html

TS:   [...new Set(arr)]
来源：http://hz.ivvv.top/gtfpxtlqmo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.zhoulong.xyz/gtksqmpine.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.cucudq.cn/gtbwzplyux.html

Ruby: arr.uniq
来源：http://hz.bjfxy.top/gttujpasjc.html

C#:   list.Distinct().ToList()
来源：http://hz.c1oappe.top/gtumrzrktq.html

[D16] 求和与平均值
来源：http://hz.cashguo.top/gtkunkflqc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yuanzhike.top/gtauhblzpy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.nanxinkj.top/gtbxmtcicg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xingfuxueyuan.xyz/gtcuosyxsx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.chenlongwang.top/gtaygkzqkb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.zhoulong.xyz/gtznifqvld.html

Go:   // 手写循环累加
来源：http://hz.yanxiufei.cn/gtcnohdfqd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.jinqigufen.top/gtkyqixqum.html

C#:   list.Sum();  list.Average()
来源：http://hz.zhijiandao.cn/gtlbywhjow.html

[D17] 最大值与最小值
来源：http://hz.tanke756.top/gtzyfpkxts.html

Py:   max(arr);  min(arr)
来源：http://hz.zhiwuduotai.top/gtrbmfodbv.html

PHP:  max($arr);  min($arr);
来源：http://hz.yj20258.top/gtapjqnyer.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.shangyingyoupin.top/gtbxlednpa.html

TS:   Math.max(...arr);
来源：http://hz.iojbl.cn/gtzduebvqo.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zhiwuduotai.top/gtzuzzrazi.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.yuanzhike.top/gturrixmcb.html

Ruby: arr.max;  arr.min
来源：http://hz.xylfe.cn/gtlptpjmnq.html

C#:   list.Max();  list.Min()
来源：http://hz.aizwys.cn/gtsqbjgtug.html

[D18] 扁平化嵌套数组
来源：http://hz.ydzc1.top/gtwufcehhf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zhixingplan.top/gtkokzhunj.html

PHP:  array_merge(...$nested);
来源：http://hz.jiagoushi.top/gtwvcvaixn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.52xcode.cn/gtnbbudlew.html

TS:   nested.flat();
来源：http://hz.jqgufenzy.top/gtejgmjuiw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yvedp.cn/gtpkbbvsyy.html

Go:   // 手写双层循环
来源：http://hz.hnqzz.top/gtwglcmzno.html

Ruby: nested.flatten
来源：http://hz.xuetiantiany.cn/gtuieyvpwu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.wangshuangyany.cn/gtqocugyfg.html

[D19] 按字段分组
来源：http://hz.cucudq.cn/gtysweuwgh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.wangshuangyany.cn/gtaqldglqb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yuanzhike.top/gtqhpixcqw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.daria6918.cn/gtjtbuljrz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.fzhhl.top/gtmjsytezy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yj20258.top/gtxvogdpyf.html

Go:   // 手写 map[string][]T
来源：http://hz.fengsongda.top/gtxeidpayj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.yuanzhike.top/gtlztbhoau.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.gogol.net.cn/gtfezqunwe.html

[D20] 统计每个元素出现次数
来源：http://hz.feifeiyinyue.top/gtmwxpyrzx.html

Py:   Counter(arr)
来源：http://hz.ivvv.top/gtvkjfvroy.html

PHP:  array_count_values($arr);
来源：http://hz.c1oappe.top/gtgepsbnae.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhiwuduotai.top/gtjumhnlhw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.kuanghao11.cn/gtooswyvqv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.cqqwz.cn/gtumojkvxz.html

Go:   // 手写 map[T]int
来源：http://hz.meibo888.top/gttepnflhi.html

Ruby: arr.tally
来源：http://hz.nanxinkj.top/gtninanidc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.zhijiandao.cn/gthhqnbxcm.html

[D21] 判断是否包含某元素
来源：http://hz.jianghu66.top/gtlfekzbxa.html

Py:   x in arr
来源：http://hz.jinqigfzy.top/gtgnundtqp.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yanxiufei.cn/gtescvwttu.html

JS:   arr.includes(x)
来源：http://hz.xuetiantiany.cn/gtxtvtxhvp.html

TS:   arr.includes(x)
来源：http://hz.andypj.xyz/gthqyqzxay.html

Java: list.contains(x)
来源：http://hz.iojbl.cn/gtptjmrlsq.html

Go:   slices.Contains(arr, x)
来源：http://hz.gotoacloud.top/gtyhnsgajr.html

Ruby: arr.include?(x)
来源：http://hz.hnxiangtu.top/gtbaimlztg.html

C#:   list.Contains(x)
来源：http://hz.guowangkeji.top/gtcvwmyxri.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jiagoushi.top/gtyxbywpgp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.gogol.net.cn/gtqpqzzfax.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.gogol.net.cn/gtcpqvvddq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.52xcode.cn/gtzxeiuwat.html

TS:   [...arr];
来源：http://hz.guowangkeji.top/gtaxgrpcei.html

Java: new ArrayList<>(list);
来源：http://hz.sxryk.cn/gtjlphbynb.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.gotoacloud.top/gtnsygcfxu.html

Ruby: arr.dup;  arr.clone
来源：http://hz.gaohongyu789.top/gtymevckxx.html

C#:   new List<int>(list);
来源：http://hz.pycfn.com/gtivoigaom.html

[D23] reduce 累积计算
来源：http://hz.yj20258888.top/gtyrvszyao.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.xylfe.cn/gtuhzmjrok.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.feifeiyinyue.top/gtztzdcwyw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jinqigfzy.top/gtyhuwukho.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhiwuduotai.top/gtjfrgaulw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.xinyue.icu/gtftgrkmuc.html

Go:   // 手写循环
来源：http://hz.andypj.xyz/gtxcwkohqe.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.sufxvd.cn/gtlrkbmvqd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.zdqjudy.top/gtaxhfecay.html

[D24] 字典 / Map 基本操作
来源：http://hz.meibo888.top/gtosholceg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zhixingplan.top/gteyyrhibt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.cqqwz.cn/gtqlhiagat.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.smart0.xyz/gtitztrvva.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.hfpthk.cn/gtudodttbr.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.zhiwuduotai.top/gtsalshmaf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.shzxlz.cn/gtzpbxuiyp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.birdmap.top/gtvzfywpde.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.nanxinkj.top/gtdolhcdbj.html

[D25] Set 集合去重与交并差
来源：http://hz.yvedp.cn/gttptlfjqt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.jqgufenzy.top/gtjhnyvmqs.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.kuanghao11.cn/gtlqszvzvq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.daxiang520.top/gtljgocmbu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.0kj1m.cn/gtqxlvqufg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.jqgfzy.top/gtwecshohv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.meibo888.top/gtksnlzxkw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.snrcjt.cn/gtsbkueznw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.hnxiangtu.top/gtmjdansaf.html

[D26] 数组转字符串
来源：http://hz.bjfxy.top/gtsgepchph.html

Py:   ", ".join(map(str, arr))
来源：http://hz.bjfxy.top/gtisuxqaod.html

PHP:  implode(", ", $arr);
来源：http://hz.chenlongwang.top/gtqiunoqts.html

JS:   arr.join(", ")
来源：http://hz.hysaishi.cn/gttnvxufqu.html

TS:   arr.join(", ")
来源：http://hz.birdmap.top/gtgzuzeivu.html

Java: String.join(", ", list)
来源：http://hz.vqdsnc.cn/gtcrahsyvk.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yonumen.top/gtrdjriiue.html

Ruby: arr.join(", ")
来源：http://hz.havefunace.top/gttguxvmmw.html

C#:   string.Join(", ", list)
来源：http://hz.316326.xyz/gteodtgphz.html

================================================================================
来源：http://hz.ehwqpu.com/gtxstsmfjv.html

E. 字符串处理
来源：http://hz.yj20258888.top/gtocajvwdp.html

================================================================================
来源：http://hz.nwbrower.top/gttsxsfqjl.html

[E01] 拼接字符串
来源：http://hz.haohaochexian.top/gtpemnbori.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.gaohongyu789.top/gtepdhdfkf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.daria6918.cn/gtucaqfmdz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jiagoushi.top/gteeiddsri.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xuanzx.com/gtbfdeepeu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.haohaochexian.top/gtwxeitsme.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.nanxinkj.top/gtnxhfubsu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.meibo888.top/gtbzziwdma.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.nanxuanxn.top/gtefjydltv.html

[E02] 重复字符串
来源：http://hz.zhiwuduotai.top/gtcqjysfdg.html

Py:   "ab" * 3
来源：http://hz.c1oappe.top/gtvgvzfkhk.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yj20258888.top/gtlrihhmwp.html

JS:   "ab".repeat(3)
来源：http://hz.birdmap.top/gtfgxrjjcg.html

TS:   "ab".repeat(3)
来源：http://hz.quarkkingdee.top/gtmxvnkjkn.html

Java: "ab".repeat(3)
来源：http://hz.dianchejie.cn/gtzqqsvrhz.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.snrcjt.cn/gtcdeahsfe.html

Ruby: "ab" * 3
来源：http://hz.sufxvd.cn/gtqkakrcep.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.mhx1999.top/gtvwfgevdj.html

[E03] 截取子串
来源：http://hz.gogol.net.cn/gtyvvznsdx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.hongshengwenyu.top/gttsvruzkr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.redwolf501.top/gtdkomwntz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.aizwys.cn/gtdobjdwzn.html

TS:   s.slice(1, 4)
来源：http://hz.xylfe.cn/gtgldnopzb.html

Java: s.substring(1, 4)
来源：http://hz.yj20258888.top/gtwggzswwd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.cdnleiting.top/gtmzowltef.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yongpay.top/gtrlpjumrh.html

C#:   s.Substring(1, 3)
来源：http://hz.jinyuanbaomall.cn/gtkhrpalcb.html

[E04] 查找子串位置
来源：http://hz.zhijiandao.cn/gtsbrroiry.html

Py:   s.find("x");  s.index("x")
来源：http://hz.gaohongyu789.top/gtusgswtdw.html

PHP:  strpos($s, "x");
来源：http://hz.zhiwuduotai.top/gtubkkrrun.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.c1oappe.top/gtxeftphux.html

TS:   s.indexOf("x")
来源：http://hz.daxiang520.top/gtypzrajqt.html

Java: s.indexOf("x")
来源：http://hz.316326.xyz/gtosouzfby.html

Go:   strings.Index(s, "x")
来源：http://hz.zhengqikj.top/gtnainhrsx.html

Ruby: s.index("x")
来源：http://hz.xuetiantiany.cn/gtzsrmfcoo.html

C#:   s.IndexOf("x")
来源：http://hz.feifeiyinyue.top/gtxphooryf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.mhx1999.top/gtnmrhayzu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.zdqjudy.top/gtteccrjpb.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.yj20258888.top/gtershxapf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.xuanzx.com/gtiqfsxwib.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.xinyue.icu/gtygvvbpvi.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ybcxt.top/gtdnbzhyaj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.zhiwuduotai.top/gtdrxyrota.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.zhaomingkeji.xyz/gtneywzlxw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.ppjwa.cn/gtxsxdovmz.html

[E06] 替换子串
来源：http://hz.mhx1999.top/gthpcqmywx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.birdmap.top/gtsizvusrx.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.gogol.net.cn/gtldppndkm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhengqikj.top/gtggoirgrh.html

TS:   s.replaceAll("a", "b")
来源：http://hz.fengsongda.top/gtdgckskzo.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.gaohongyu789.top/gtvnhhvkku.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.meibo888.top/gtsnxossxt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.yanxiufei.cn/gtqlgunobt.html

C#:   s.Replace("a", "b")
来源：http://hz.andypj.xyz/gtvdmcirly.html

[E07] 按分隔符拆分
来源：http://hz.guannengcc.top/gtvlukhykz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.fengsongda.top/gtvdwhmphv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.guannengcc.top/gtxtyjkplh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.redwolf501.top/gtbpwtkymh.html

TS:   s.split(",")
来源：http://hz.vqdsnc.cn/gthrfjpesy.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.cqqwz.cn/gtfyvhbska.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.sysykeji.top/gtizzjfkir.html

Ruby: s.split(",");  s.split
来源：http://hz.nwbrower.top/gtevtzyioc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.svipenyu.cn/gthnfhleqw.html

[E08] 数组按分隔符合并
来源：http://hz.yj202588.top/gtpmqmkbjc.html

Py:   ",".join(items)
来源：http://hz.ywan-chungtsiang.top/gtgooxlgrl.html

PHP:  implode(",", $items);
来源：http://hz.hnxiangtu.top/gtmrvkflut.html

JS:   items.join(",")
来源：http://hz.jiagoushi.top/gtahdwbufe.html

TS:   items.join(",")
来源：http://hz.gotoacloud.top/gtqhturicb.html

Java: String.join(",", items)
来源：http://hz.nanxinkj.top/gtydxhlwfo.html

Go:   strings.Join(items, ",")
来源：http://hz.tian-w.cn/gtadflfhaf.html

Ruby: items.join(",")
来源：http://hz.ydzc1.top/gtpzqcwijs.html

C#:   string.Join(",", items)
来源：http://hz.quarkkingdee.top/gtoniyolrr.html

[E09] 去除所有空白字符
来源：http://hz.yonumen.top/gttlqeyvkt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.zhongyouzk.top/gtztkctcsh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.ydzc1.top/gtwjjxiexz.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.hnxiangtu.top/gtcthcnzdy.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.xylfe.cn/gtcvgeilxx.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yj20258888.top/gtczoosckw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yvedp.cn/gtytgocbll.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.hongshengwenyu.top/gtmwfrwexl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jyoumei.cn/gttnnqwibv.html

[E10] 左侧补零 / 定长填充
来源：http://hz.9152youxi.cn/gtrltkazvt.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.chenzaomai.com/gtnhjnlexi.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.jlsjyb.cn/gtoexebjmc.html

JS:   "7".padStart(3, "0")
来源：http://hz.zycfv.cn/gtdtnzowwp.html

TS:   "7".padStart(3, "0")
来源：http://hz.yueranfly.top/gtyftctimm.html

Java: String.format("%03d", 7)
来源：http://hz.chenjidiqi.icu/gtzyyrigtm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.ybcxt.top/gtnotlehzz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.dashuyun.cn/gtduscjpka.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.sufxvd.cn/gtnwmbrmtf.html

[E11] 反转字符串
来源：http://hz.jqgufenzy.top/gtxflyaafb.html

Py:   s[::-1]
来源：http://hz.redwolf501.top/gtngclxhxb.html

PHP:  strrev($s);
来源：http://hz.shuidangran.top/gtwaopasjn.html

JS:   [...s].reverse().join("")
来源：http://hz.pycfn.com/gtxbutusfs.html

TS:   [...s].reverse().join("")
来源：http://hz.ppjwa.cn/gtfwnxbske.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.hywenlv.cn/gtdgspltez.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.zycfv.cn/gttvevgfub.html

Ruby: s.reverse
来源：http://hz.wangdashe.top/gtthuwapqz.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.cqqwz.cn/gtjzxaxwrn.html

[E12] 统计某字符出现次数
来源：http://hz.hongshengwenyu.top/gtybrzhzve.html

Py:   s.count("a")
来源：http://hz.yj20258888.top/gtrhjsdysx.html

PHP:  substr_count($s, "a");
来源：http://hz.jianghu66.top/gtvfuedpus.html

JS:   s.split("a").length - 1
来源：http://hz.mhx1999.top/gthkcwmbry.html

TS:   s.split("a").length - 1
来源：http://hz.yueranfly.top/gtxaefpobc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yuanzhike.top/gtifgosccg.html

Go:   strings.Count(s, "a")
来源：http://hz.xuanzx.com/gtgkvpoptn.html

Ruby: s.count("a")
来源：http://hz.gotoacloud.top/gtabvsxrpg.html

C#:   s.Count(c => c == 'a')
来源：http://hz.xinyue.icu/gtcdfitnaa.html

[E13] 逐字符遍历
来源：http://hz.xziqi.cn/gtdjjbkzjg.html

Py:   for ch in s: print(ch)
来源：http://hz.zhengqikj.top/gtwyesdcap.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.zycfv.cn/gtofozcxqa.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.aibaodan.cn/gtlprdzivu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jinqigufen.top/gtzivqkvhu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.ywan-chungtsiang.top/gtrcesbcij.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.dashuyun.cn/gtctmvqxqi.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.ybcxt.top/gtlazekpie.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jinqigfzy.top/gtdolnwhmr.html

[E14] URL 编码与 Base64
来源：http://hz.jqgufenzy.top/gtdqifvttu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.xingfuxueyuan.xyz/gtrmqpvkwa.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.zhixingplan.top/gtvwgqepbt.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.shanyushiyangtech.top/gtlxmdtbnu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.fzhhl.top/gtcrxulewd.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.vqdsnc.cn/gtsgsqhiun.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.shzxlz.cn/gttzipfmgl.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.shanyushiyangtech.top/gtwdalvref.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.hfpthk.cn/gtsjiikzce.html

[E15] HTML 转义 / 反转义
来源：http://hz.daxiang520.top/gtvkapmbly.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.ydzc1.top/gtsjkksmep.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yangfankeji.com/gtllmsyidk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.jqgufenzy.top/gthczbxbsa.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.gzhubu.top/gtjtasqogf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.havefunace.top/gteknxkyzn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yj20258888.top/gtmxcvmpad.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.iojbl.cn/gtpjpumxjz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.iojbl.cn/gtmyumqyyq.html

[E16] 数字千分位
来源：http://hz.ppjwa.cn/gtfsaufbjc.html

Py:   f"{1234567:,}"
来源：http://hz.guowangkeji.top/gtpqnjumzd.html


<!-- 参考信息 -->