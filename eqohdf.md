代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.havefunace.top/gtotuzlxud.html

Ruby: arr.sort
来源：http://hz.yj20258.top/gtqpugajqs.html

C#:   list.Sort();
来源：http://hz.jiagoushi.top/gtoomtyjau.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.hongshengwenyu.top/gtmkkxbyud.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zhijiandao.cn/gtpezgkart.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.xinyue.icu/gtorzpllzs.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ybcxt.top/gtgwqeyplg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jyoumei.cn/gtjhlzwshs.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.xinyue.icu/gtcrnqlmbh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jianghu66.top/gtrkphvvxx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.shzxlz.cn/gtjpigthns.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.fzhhl.top/gtnjvjoxtz.html

[D11] 反转数组
来源：http://hz.svipenyu.cn/gtigdbfjes.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.andypj.xyz/gtvhefmhuv.html

PHP:  array_reverse($arr);
来源：http://hz.fengsongda.top/gtozjhhtrp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yuxming.cn/gtlehikaae.html

TS:   [...arr].reverse();
来源：http://hz.ehwqpu.com/gtxjvqsxgo.html

Java: Collections.reverse(list);
来源：http://hz.nanxuanxn.top/gtrmbvicrk.html

Go:   slices.Reverse(arr)
来源：http://hz.gogol.net.cn/gtoloyrsuw.html

Ruby: arr.reverse
来源：http://hz.jinqigufen.top/gtfojajmts.html

C#:   list.Reverse();
来源：http://hz.xuetiantiany.cn/gtytnbltxl.html

[D12] 查找元素下标
来源：http://hz.ywan-chungtsiang.top/gtgzopiemy.html

Py:   arr.index(x);  x in arr
来源：http://hz.tian-w.cn/gtbehsylrb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.iojbl.cn/gtdfbcmbcb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hfpthk.cn/gtvbcibfvm.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.tanke756.top/gtfzjpmqab.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.gogol.net.cn/gtfeffpedv.html

Go:   slices.Index(arr, x)
来源：http://hz.zycfv.cn/gtvspemdye.html

Ruby: arr.index(x)
来源：http://hz.quarkkingdee.top/gtdmrajcjh.html

C#:   list.IndexOf(x);
来源：http://hz.tian-w.cn/gtmwlqazqf.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jiagoushi.top/gtqpjevatq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.zycfv.cn/gttowprvmj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.52xcode.cn/gtegkxzrms.html

JS:   arr.filter(x => x > 3)
来源：http://hz.xuanzx.com/gtexccuynk.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jinghuilouyu.cn/gtcoguxscd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.smart0.xyz/gtgaarcmqy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.ybcxt.top/gtdwdzrcrp.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.bjfxy.top/gtwfvknjoa.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.hywenlv.cn/gtafnhkmrw.html

[D14] 映射转换（每个元素变形）
来源：http://hz.hnxiangtu.top/gtzmmzzinh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.kuanghao11.cn/gtqjxqrmzi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.zycfv.cn/gtjlyoslvp.html

JS:   arr.map(x => x * 2)
来源：http://hz.guannengcc.top/gtujeixizm.html

TS:   arr.map(x => x * 2)
来源：http://hz.hfpthk.cn/gtucvyixbv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.haohaochexian.top/gtatkrqvqm.html

Go:   // 手写循环
来源：http://hz.yongpay.top/gtsczhmulc.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.zhongyouzk.top/gtktzqtdoj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.yanxiufei.cn/gtjxeadqiw.html

[D15] 去重
来源：http://hz.zhiwuduotai.top/gtkihfdixb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.cucudq.cn/gtjtbqsund.html

PHP:  array_unique($arr);
来源：http://hz.tanke756.top/gtnfuwdxfp.html

JS:   [...new Set(arr)]
来源：http://hz.shanyushiyangtech.top/gtllpmqrzd.html

TS:   [...new Set(arr)]
来源：http://hz.chenzaomai.com/gtatwwvvjv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.hongshengwenyu.top/gtxfdgxhgt.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.jianghu66.top/gtafiwuvls.html

Ruby: arr.uniq
来源：http://hz.shanyushiyangkeji.top/gtytvikzgy.html

C#:   list.Distinct().ToList()
来源：http://hz.ivvv.top/gtcdkduhxb.html

[D16] 求和与平均值
来源：http://hz.guowangkeji.top/gtpkwrwfky.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.xingfuxueyuan.xyz/gthhugyhqi.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.jqgfzy.top/gtjubnjquw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.daxiang520.top/gtrkniezef.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shangyingyoupin.top/gtwjydhsio.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.zhengqikj.top/gtrzpmemmq.html

Go:   // 手写循环累加
来源：http://hz.jyoumei.cn/gtntaisfof.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.shangyingyoupin.top/gtrbzhryyz.html

C#:   list.Sum();  list.Average()
来源：http://hz.jinqigfzy.top/gtrhbvwumh.html

[D17] 最大值与最小值
来源：http://hz.cashguo.top/gtikwlbiky.html

Py:   max(arr);  min(arr)
来源：http://hz.hnqzz.top/gtufrxssfc.html

PHP:  max($arr);  min($arr);
来源：http://hz.ydjk.org.cn/gtqwxvtnxu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.pengpengdd.cyou/gtsmdmttwf.html

TS:   Math.max(...arr);
来源：http://hz.zhiwuduotai.top/gtpumebxsi.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.shanyushiyangtech.top/gtjxylnpjl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.fengsongda.top/gtwavmjxlu.html

Ruby: arr.max;  arr.min
来源：http://hz.shangyingyoupin.top/gtzqxkfjoz.html

C#:   list.Max();  list.Min()
来源：http://hz.daria6918.cn/gttpryrqyn.html

[D18] 扁平化嵌套数组
来源：http://hz.yongpay.top/gtwzbhpubh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.fzhhl.top/gtfqwgfyup.html

PHP:  array_merge(...$nested);
来源：http://hz.ybcxt.top/gtgosasrgx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.redwolf501.top/gtazjfturj.html

TS:   nested.flat();
来源：http://hz.ywan-chungtsiang.top/gtmhqilpop.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.chenlongwang.top/gtdkfcbwqv.html

Go:   // 手写双层循环
来源：http://hz.c1oappe.top/gtvhxrdani.html

Ruby: nested.flatten
来源：http://hz.xuanzx.com/gteljwvzlb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.cheryme.top/gtuptlottb.html

[D19] 按字段分组
来源：http://hz.hywenlv.cn/gtjskjpozp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.52xcode.cn/gtogjzngkg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.dashuyun.cn/gtoynggkpe.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jinghuilouyu.cn/gtgwicblxk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yonumen.top/gtkpnujhxy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yvedp.cn/gtnorganly.html

Go:   // 手写 map[string][]T
来源：http://hz.0kj1m.cn/gtdoywxhmq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.smart0.xyz/gthizrsjsd.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.hammf.cn/gtxsjkwyzi.html

[D20] 统计每个元素出现次数
来源：http://hz.ehwqpu.com/gtqyxtufle.html

Py:   Counter(arr)
来源：http://hz.sysykeji.top/gteackyejh.html

PHP:  array_count_values($arr);
来源：http://hz.guannengcc.top/gtsgvosnrp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jinghuilouyu.cn/gterpqroal.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hfpthk.cn/gtlfypvzxv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.guowangkeji.top/gtdjumiuki.html

Go:   // 手写 map[T]int
来源：http://hz.jinyuanbaomall.cn/gtajfgjwwd.html

Ruby: arr.tally
来源：http://hz.wangshuangyany.cn/gttixmjqlb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.0kj1m.cn/gtggempxie.html

[D21] 判断是否包含某元素
来源：http://hz.ehwqpu.com/gtxwubwbrz.html

Py:   x in arr
来源：http://hz.chenlongwang.top/gtwyvdajss.html

PHP:  in_array($x, $arr, true);
来源：http://hz.ywan-chungtsiang.top/gtadvxedwl.html

JS:   arr.includes(x)
来源：http://hz.zhixingplan.top/gtqecflhlt.html

TS:   arr.includes(x)
来源：http://hz.bjfxy.top/gtzozogmtq.html

Java: list.contains(x)
来源：http://hz.yj20258.top/gtefpvxdxo.html

Go:   slices.Contains(arr, x)
来源：http://hz.zhaomingkeji.xyz/gtjcddxxqc.html

Ruby: arr.include?(x)
来源：http://hz.hongshengwenyu.top/gtervhnktg.html

C#:   list.Contains(x)
来源：http://hz.zhijiandao.cn/gtgbpfassh.html

[D22] 复制数组（避免共享引用）
来源：http://hz.shzxlz.cn/gtclabloot.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.tianlin.xyz/gtxotxeece.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.tian-w.cn/gtubnshplj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.shanyushiyangtech.top/gtwdygwuwr.html

TS:   [...arr];
来源：http://hz.vqdsnc.cn/gtplifdwjo.html

Java: new ArrayList<>(list);
来源：http://hz.birdmap.top/gtlmblxshc.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.snrcjt.cn/gtqgwfiwqw.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zhengqikj.top/gtttvcscqs.html

C#:   new List<int>(list);
来源：http://hz.nanxinkj.top/gtltcyyhls.html

[D23] reduce 累积计算
来源：http://hz.zdqjudy.top/gthybdwntg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.ybcxt.top/gtpxychbbk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.ppjwa.cn/gtaznjgsdi.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.mhx1999.top/gtsijiwftn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jlsjyb.cn/gtvjohtzyc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yonumen.top/gtguebtalu.html

Go:   // 手写循环
来源：http://hz.ybcxt.top/gtfqulmwws.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.nanxuanxn.top/gthukaztqt.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jyoumei.cn/gtohrckeqf.html

[D24] 字典 / Map 基本操作
来源：http://hz.bjfxy.top/gtnrooeydc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.yueranfly.top/gtptxxpfau.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yanxiufei.cn/gtfvmczqti.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jqgfzy.top/gtnmdclybx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.wangdashe.top/gtlabcjzov.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.jinyuanbaomall.cn/gtzwxzmihl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.nanxinkj.top/gtorbxfoag.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.haohaochexian.top/gtetdqdacs.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jianghu66.top/gtffgsavxv.html

[D25] Set 集合去重与交并差
来源：http://hz.jlsjyb.cn/gtbnkpltbx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.daxiang520.top/gtgulibzbj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.zhongyouzk.top/gtblgshwmn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yueranfly.top/gtzfdrngoi.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.birdmap.top/gtxtzjjpks.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.zhiwuduotai.top/gtieafskxt.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yuxming.cn/gtsshyhjqi.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jinghuilouyu.cn/gtitnftdzy.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.hnxiangtu.top/gtujdjymse.html

[D26] 数组转字符串
来源：http://hz.pengpengdd.cyou/gtqntbgpkc.html

Py:   ", ".join(map(str, arr))
来源：http://hz.meibo888.top/gtesifcvja.html

PHP:  implode(", ", $arr);
来源：http://hz.c1oappe.top/gtcrlrzjne.html

JS:   arr.join(", ")
来源：http://hz.andypj.xyz/gtitzrrwrx.html

TS:   arr.join(", ")
来源：http://hz.hnqzz.top/gtkchedare.html

Java: String.join(", ", list)
来源：http://hz.nwbrower.top/gtdhywynqp.html

Go:   strings.Join(strs, ", ")
来源：http://hz.tianlin.xyz/gtzlyoyflv.html

Ruby: arr.join(", ")
来源：http://hz.guannengcc.top/gtyvrhijvk.html

C#:   string.Join(", ", list)
来源：http://hz.jinqigufen.top/gtvymezvly.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtbzylcwxz.html

E. 字符串处理
来源：http://hz.shanyushiyangtech.top/gtgpxmqgaz.html

================================================================================
来源：http://hz.guannengcc.top/gtjgroskch.html

[E01] 拼接字符串
来源：http://hz.shuidangran.top/gthwiizjth.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.hongshengwenyu.top/gtzkaoifip.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.birdmap.top/gtmondxsbb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.sysykeji.top/gtpubjupey.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.shanyushiyangtech.top/gtjnmguobu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.hnxiangtu.top/gtaymfllws.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.vqdsnc.cn/gteiisgbdv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.zhaomingkeji.xyz/gtfscezbaf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.cheryme.top/gtiijkmeas.html

[E02] 重复字符串
来源：http://hz.aizwys.cn/gtjtsodzkt.html

Py:   "ab" * 3
来源：http://hz.bjfxy.top/gtypwvkupq.html

PHP:  str_repeat("ab", 3);
来源：http://hz.dianchejie.cn/gtpyuurvgk.html

JS:   "ab".repeat(3)
来源：http://hz.9152youxi.cn/gtqnftjftu.html

TS:   "ab".repeat(3)
来源：http://hz.xingfuxueyuan.xyz/gtqrtknqru.html

Java: "ab".repeat(3)
来源：http://hz.sxryk.cn/gtqmdppmfp.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.xingfuxueyuan.xyz/gtgyramyqk.html

Ruby: "ab" * 3
来源：http://hz.yj20258.top/gtvbybhinn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.nanxinkj.top/gtkjixpali.html

[E03] 截取子串
来源：http://hz.jinghuilouyu.cn/gtgknkomwj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.316326.xyz/gttztdovwc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zhaomingkeji.xyz/gtlqdutiqn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.fzhhl.top/gtpsxtpqsm.html

TS:   s.slice(1, 4)
来源：http://hz.wangshuangyany.cn/gtoxqkpcar.html

Java: s.substring(1, 4)
来源：http://hz.yj20258.top/gtlhvpgyvr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.tianlin.xyz/gtwwpsuxov.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.cdnleiting.top/gtynxbjofk.html

C#:   s.Substring(1, 3)
来源：http://hz.svipenyu.cn/gtulgjajse.html

[E04] 查找子串位置
来源：http://hz.jqgfzy.top/gtakdiafxe.html

Py:   s.find("x");  s.index("x")
来源：http://hz.gzhubu.top/gtkavfiucs.html

PHP:  strpos($s, "x");
来源：http://hz.yj20258888.top/gtxqcelxux.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.jinghuilouyu.cn/gteihvrqss.html

TS:   s.indexOf("x")
来源：http://hz.jiagoushi.top/gttxgbgrkt.html

Java: s.indexOf("x")
来源：http://hz.jqgfzy.top/gtkzpqlxxd.html

Go:   strings.Index(s, "x")
来源：http://hz.jinyuanbaomall.cn/gtqdwvkmbb.html

Ruby: s.index("x")
来源：http://hz.yj20258888.top/gtegbeflvp.html

C#:   s.IndexOf("x")
来源：http://hz.hnqzz.top/gtjkmrcjnm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.gotoacloud.top/gtrqprhedn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.xinyue.icu/gttyxlvagl.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zhaomingkeji.xyz/gtszpofnzt.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yueranfly.top/gtssknfxjv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.yueranfly.top/gtkzdiydaf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.andypj.xyz/gtnmkngdzm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.cucudq.cn/gtgyirydaq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.ybcxt.top/gtstuuibtt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.shzxlz.cn/gtnxsqimbj.html

[E06] 替换子串
来源：http://hz.yanxiufei.cn/gtepavkwzw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.xziqi.cn/gtrbsvcucp.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.shuidangran.top/gtvchyubra.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.meibo888.top/gtltifyqyu.html

TS:   s.replaceAll("a", "b")
来源：http://hz.316326.xyz/gtqgccfwah.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yj202588.top/gtohbwogrw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.nanxinkj.top/gtnisodevd.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.cashguo.top/gtwryoeogb.html

C#:   s.Replace("a", "b")
来源：http://hz.yvedp.cn/gtclwkixsj.html

[E07] 按分隔符拆分
来源：http://hz.tianlin.xyz/gtbrnpdvdg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.zhixingplan.top/gttroyfcgt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yangfankeji.com/gtnmxyjylo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.zhengqikj.top/gtlwqatlri.html

TS:   s.split(",")
来源：http://hz.xinyue.icu/gtdtdygtwv.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.hongshengwenyu.top/gtknvgpffi.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.guowangkeji.top/gtglfmkszj.html

Ruby: s.split(",");  s.split
来源：http://hz.xylfe.cn/gtvtnrarbb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.pycfn.com/gtvvwmhqnx.html

[E08] 数组按分隔符合并
来源：http://hz.cdnleiting.top/gtxglyhtxe.html

Py:   ",".join(items)
来源：http://hz.andypj.xyz/gtqvnrxhsn.html

PHP:  implode(",", $items);
来源：http://hz.0kj1m.cn/gteyzokypb.html

JS:   items.join(",")
来源：http://hz.jlsjyb.cn/gtwdfazygj.html

TS:   items.join(",")
来源：http://hz.snrcjt.cn/gtqhfisitx.html

Java: String.join(",", items)
来源：http://hz.wangshuangyany.cn/gtwigxijuk.html

Go:   strings.Join(items, ",")
来源：http://hz.zhixingplan.top/gtovelcdlq.html

Ruby: items.join(",")
来源：http://hz.chenjidiqi.icu/gtdmoedfhr.html

C#:   string.Join(",", items)
来源：http://hz.hongshengwenyu.top/gtjhnzihrx.html

[E09] 去除所有空白字符
来源：http://hz.hywenlv.cn/gtvfyfweur.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.dianchejie.cn/gtvgqrfksn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.pengpengdd.cyou/gtbmuhexci.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jqgufenzy.top/gtakwfaewj.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.fzhhl.top/gtpskyjyat.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.svipenyu.cn/gtfsvkgqvy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zhongyouzk.top/gtwjwvqmha.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.andypj.xyz/gtvfbcyimp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.mhx1999.top/gtjuwgipcn.html

[E10] 左侧补零 / 定长填充
来源：http://hz.xinyue.icu/gtitiqzmhq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.shanyushiyangkeji.top/gtivnjyhlw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.zhengqikj.top/gtdidudctl.html

JS:   "7".padStart(3, "0")
来源：http://hz.bjfxy.top/gthrapykue.html

TS:   "7".padStart(3, "0")
来源：http://hz.wangshuangyany.cn/gtyjpbkuan.html

Java: String.format("%03d", 7)
来源：http://hz.guannengcc.top/gttxuhifdh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.zycfv.cn/gtadtgyhok.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.9152youxi.cn/gtldxatywd.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.xuetiantiany.cn/gtqpgtjgwj.html

[E11] 反转字符串
来源：http://hz.guowangkeji.top/gtbozxsqqi.html

Py:   s[::-1]
来源：http://hz.haohaochexian.top/gtqwevedcj.html

PHP:  strrev($s);
来源：http://hz.cdnleiting.top/gtyacnoran.html

JS:   [...s].reverse().join("")
来源：http://hz.yj202588.top/gtosngnwjq.html

TS:   [...s].reverse().join("")
来源：http://hz.chenjidiqi.icu/gtvdfkmgbe.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jinqigfzy.top/gtocgilwbz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yj20258888.top/gtkbaikmyd.html

Ruby: s.reverse
来源：http://hz.ywan-chungtsiang.top/gtzgewqrzk.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.hnxiangtu.top/gtpgxllxqg.html

[E12] 统计某字符出现次数
来源：http://hz.jinghuilouyu.cn/gtuqxbpgey.html

Py:   s.count("a")
来源：http://hz.jlsjyb.cn/gtsxzegwpl.html

PHP:  substr_count($s, "a");
来源：http://hz.zhixingplan.top/gtipcmjaja.html

JS:   s.split("a").length - 1
来源：http://hz.daria6918.cn/gtkbtcbuec.html

TS:   s.split("a").length - 1
来源：http://hz.fengsongda.top/gtmszymgtc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.redwolf501.top/gtledevlyr.html

Go:   strings.Count(s, "a")
来源：http://hz.nanxinkj.top/gttpvvmmrq.html

Ruby: s.count("a")
来源：http://hz.tanke756.top/gtdxxgecbp.html

C#:   s.Count(c => c == 'a')
来源：http://hz.quarkkingdee.top/gtvkcnsakw.html

[E13] 逐字符遍历
来源：http://hz.guowangkeji.top/gtgpttsmaw.html

Py:   for ch in s: print(ch)
来源：http://hz.xziqi.cn/gtrmpddgls.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.xziqi.cn/gtpsixwyyh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shanyushiyangkeji.top/gtmhoxcrfy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhengqikj.top/gteengwdka.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.jlsjyb.cn/gtefqunjsz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.wangdashe.top/gtevxmswfu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jlsjyb.cn/gthbmotsby.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.hammf.cn/gtxecdbxca.html

[E14] URL 编码与 Base64
来源：http://hz.aibaodan.cn/gtgbfsbynm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.hnqzz.top/gtglupgccu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.zycfv.cn/gtonieyxlp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.ywan-chungtsiang.top/gtombqcock.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.svipenyu.cn/gtulytdvsl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.xylfe.cn/gtrftufqml.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.hysaishi.cn/gtmokfcivg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.chenjidiqi.icu/gtfhhkjjsp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.havefunace.top/gtbzysskuw.html

[E15] HTML 转义 / 反转义
来源：http://hz.redwolf501.top/gtaapfgjam.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.feifeiyinyue.top/gteibdqfsm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.xuanzx.com/gtfeqhmcbw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.pengpengdd.cyou/gttjmgfxyw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.mhx1999.top/gtqwadnfmc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.nwbrower.top/gtmjfoesvq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.ydjk.org.cn/gtnzjjzlqz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jinyuanbaomall.cn/gtgbqgomuy.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.hysaishi.cn/gtmpikegnw.html

[E16] 数字千分位
来源：http://hz.svipenyu.cn/gtuwhaharn.html

Py:   f"{1234567:,}"
来源：http://hz.gzhubu.top/gtgdyulorh.html

PHP:  number_format(1234567);
来源：http://hz.cdnleiting.top/gtjfxutmzw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhijiandao.cn/gtksedzlxi.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.cheryme.top/gtecmnvnak.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jinghuilouyu.cn/gtgodbdxbs.html


<!-- 参考信息 -->